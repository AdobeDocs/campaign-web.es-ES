---
audience: end-user
title: Diseño de una entrega de notificaciones push
description: Obtenga información sobre cómo diseñar una entrega de notificaciones push con Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: fbedfc5d1886b86932c156574037549270480f44
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 42%

---

# Diseño de una entrega push {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Contenido push para Android"
>abstract="Defina el contenido push de Android."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Contenido push para iOS"
>abstract="Defina el contenido push de iOS."

## Mensaje {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Con Firebase Cloud Messaging, puede elegir entre dos tipos de mensajes:

* El **Mensaje de datos**, gestionado por la aplicación del cliente. Los mensajes se envían directamente a la aplicación móvil, que generará y mostrará la notificación de Android al dispositivo. Los mensajes de datos solo contienen las variables de aplicación personalizadas.

   Haga clic en **[!UICONTROL Mensaje]** y utilice el Editor de expresiones para definir contenido, personalizar datos y añadir contenido dinámico.

* El mensaje de notificación, gestionado automáticamente por el SDK de FCM. FCM muestra automáticamente el mensaje en los dispositivos de los usuarios en nombre de la aplicación del cliente. Los mensajes de notificación contienen un conjunto predefinido de parámetros y opciones, pero pueden personalizarse aún más con las variables de aplicación personalizadas.

   Para redactar el mensaje, haga clic en el **[!UICONTROL Título]** y **[!UICONTROL Cuerpo]** campos. Utilice el Editor de expresiones para definir contenido, personalizar datos y agregar contenido dinámico.

   Para personalizar aún más la notificación push, puede elegir una imagen para añadirla a su notificación push, el icono de la notificación para mostrar en los dispositivos de sus perfiles y su color.

>[!TAB iOS]

![](assets/push_content_1.png)

Para redactar el mensaje, haga clic en el **[!UICONTROL Título]** y **[!UICONTROL Cuerpo]** campos. Utilice el Editor de expresiones para definir contenido, personalizar datos y agregar contenido dinámico.

Puede añadir un **[!UICONTROL Subtítulo]**, valor del parámetro subtitle de la carga útil de notificación de iOS. Consulte esta sección.

El modo Push silenciosa permite enviar una notificación &quot;silenciosa&quot; a una aplicación móvil. No se avisa al usuario de la llegada de la notificación. Esta se transfiere directamente a la aplicación.

>[!ENDTABS]

## Configuración avanzada {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

| Parámetro | Descripción |
|---------|---------|
| **[!UICONTROL Sonido]** | configure el sonido para que se reproduzca cuando el dispositivo reciba la notificación. |
| **[!UICONTROL Recuento de notificaciones]** | configure el número de información nueva sin leer para que se muestre directamente en el icono de la aplicación. |
| **[!UICONTROL ID de canal]** | Establezca el ID de canal de la notificación. La aplicación debe crear un canal con este ID de canal antes de recibir cualquier notificación. |
| **[!UICONTROL Acción de clic]** | configure en la notificación la acción asociada con el clic del usuario. |
| **[!UICONTROL Etiqueta]** | establezca el identificador utilizado para reemplazar las notificaciones existentes en el cajón de notificaciones. |
| **[!UICONTROL Prioridad]** | establezca los niveles de prioridad de la notificación en predeterminados, mínimos, bajos o altos. Para más información, consulte la documentación de FCM. |
| **[!UICONTROL Visibilidad]** | establezca los niveles de visibilidad de la notificación en pública, privada o secreta. Para más información, consulte la documentación de FCM. |
| **[!UICONTROL Adhesivo]** | Si se desactiva, la notificación se descarta automáticamente cuando el usuario hace clic en ella. Si está activada, la notificación se seguirá mostrando incluso cuando el usuario haga clic en ella. |

>[!TAB iOS]

![](assets/push_content_2.png)

| Parámetro | Descripción |
|---------|---------|
| **[!UICONTROL Modo de alerta crítica]** | Active esta opción para agregar sonido a la notificación, incluso si el teléfono del usuario está activado o si el iPhone está silenciado. |
| **[!UICONTROL Insignia limpia]** | Active estas opciones para actualizar el valor del distintivo. |
| **[!UICONTROL Recuento de notificaciones]** | Establezca un número que se utilizará para mostrar directamente en el icono de la aplicación la cantidad de información nueva no leída. |
| **[!UICONTROL Volumen]** | Volumen de su sonido de 0 a 100. |
| **[!UICONTROL Contenido modificable]** | Active esta opción para permitir que la aplicación móvil descargue contenido multimedia. Para obtener más información, consulte la [documentación para desarrolladores de Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Puntuación de relevancia]** | Establezca una puntuación de relevancia de 0 a 100. El sistema utiliza esto para ordenar las notificaciones en el resumen de notificaciones. |
| **[!UICONTROL Nivel de interrupción]** | <ul> <li>**[!UICONTROL Activo]**: de forma predeterminada, el sistema presenta la notificación inmediatamente, ilumina la pantalla y puede reproducir un sonido. Las notificaciones no rompen los modos de Enfoque.</li><li>**[!UICONTROL Pasivo]**: el sistema añade la notificación a la lista de notificaciones sin iluminar la pantalla ni reproducir un sonido. Las notificaciones no rompen los modos de Enfoque.</li><li>**[!UICONTROL Con distinción de tiempo]**: el sistema presenta la notificación inmediatamente, enciende la pantalla, puede reproducir un sonido y atravesar los modos de Enfoque. Este nivel no requiere un permiso especial de Apple.</li> <li>**[!UICONTROL Crítico]**: el sistema presenta la notificación inmediatamente, enciende la pantalla y evita el interruptor silencioso o los modos de enfoque. Tenga en cuenta que este nivel requiere un permiso especial de Apple.</ul> |
| **[!UICONTROL Thread-id]** | Identificador utilizado para agrupar las notificaciones relacionadas. |
| **[!UICONTROL Categoría]** | Nombre de su ID de categoría que mostrará botones de acción. Estas notificaciones proporcionan al usuario una forma más rápida de realizar distintas tareas en respuesta a una notificación sin necesidad de abrir ni navegar por la aplicación. |
| **[!UICONTROL ID de contenido del público destinatario]** | Identificador utilizado para destinar la ventana de aplicación que se reenvía cuando se abre la notificación. |
| **[!UICONTROL Iniciar imagen]** | Nombre del archivo de imagen de lanzamiento que se va a mostrar. Si el usuario decide iniciar la aplicación, se mostrará la imagen seleccionada en lugar de la pantalla de inicio de la aplicación. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



