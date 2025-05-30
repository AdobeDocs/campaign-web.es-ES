---
audience: end-user
title: Diseño de una entrega de notificaciones push
description: Obtenga información sobre cómo diseñar una entrega de notificaciones push con Adobe Campaign Web
exl-id: 031bc38a-2435-4468-8ee6-3bcf1132da55
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 43%

---


# Diseño de un envío push {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Contenido push para Android"
>abstract="Defina el contenido de la notificación push para dispositivos Android. Para empezar a componer el mensaje, haga clic en el botón **Editar contenido**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Contenido push para iOS"
>abstract="Defina el contenido de la notificación push para dispositivos iOS. Para empezar a componer el mensaje, haga clic en el botón **Editar contenido**."

## Definición del contenido de la notificación {#push-message}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_msg"
>title="Mensaje push de iOS"
>abstract="Defina el contenido de la notificación push para dispositivos iOS. Para componer el mensaje, haga clic en los campos **Título** y **Mensaje**. Utilice el editor de expresiones para personalizar datos y añadir contenido dinámico. Para ver más opciones de configuración personalizada, vaya a la sección **Configuración avanzada**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_msg"
>title="Mensaje push de Android"
>abstract="Defina el contenido de la notificación push para dispositivos Android. Para componer el mensaje, haga clic en los campos **Título** y **Mensaje**. Utilice el editor de expresiones para personalizar datos y añadir contenido dinámico. Para personalizar aún más la notificación push, puede elegir una imagen para añadirla, el icono de la notificación para mostrar en los dispositivos de los perfiles y su color. Para ver más opciones de configuración personalizada, vaya a la sección **Configuración avanzada**."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_silent"
>title="Notificación silenciosa para iOS"
>abstract="El modo Silent Push permite enviar una notificación “silenciosa” a una aplicación móvil. No se avisa al usuario de la llegada de la notificación. Esta se transfiere directamente a la aplicación."

Una vez creado el envío push, defina su contenido. Los parámetros y la configuración dependen del sistema operativo móvil: Android o iOS. Examine las pestañas siguientes para aprender a redactar el mensaje para cada sistema operativo.

>[!BEGINTABS]

>[!TAB Android]

Con Firebase Cloud Messaging, puede elegir entre dos tipos de mensajes:

* La aplicación cliente administra el **[!UICONTROL mensaje de datos]**. Estos mensajes se envían directamente a la aplicación móvil, que genera y muestra una notificación de Android en el dispositivo. Los mensajes de datos solo contienen las variables de aplicación personalizadas.

  Para definir el contenido, personalizar los datos y agregar contenido dinámico, haga clic en el campo **[!UICONTROL Mensaje]** y utilice el Editor de expresiones. Acceda a este editor para personalizar los mensajes.
En el menú **[!UICONTROL Variables de aplicación]**, las variables de su aplicación se agregan automáticamente. Estas variables permiten definir el comportamiento de las notificaciones. Por ejemplo, configure una pantalla específica de la aplicación que se mostrará cuando el usuario active la notificación.

  ![Descripción: ejemplo de definición de contenido para un mensaje de datos en notificaciones de Android](assets/push_content_4.png){zoomable="yes"}

* El **[!UICONTROL mensaje de notificación]**, gestionado automáticamente por FCM SDK. FCM muestra automáticamente el mensaje en los dispositivos de los usuarios en nombre de la aplicación del cliente. Los mensajes de notificación contienen un conjunto predefinido de parámetros y opciones, pero pueden personalizarse aún más con las variables de aplicación personalizadas.

  Para componer el mensaje, haga clic en los campos **[!UICONTROL Título]** y **[!UICONTROL Mensaje]**. Utilice el Editor de expresiones para definir contenido, personalizar datos y agregar contenido dinámico.

  Para personalizar aún más la notificación push, elija una imagen para añadirla a la notificación push, el icono de la notificación que se mostrará en los dispositivos de los perfiles y su color.

  ![Descripción: ejemplo de definición de contenido para un mensaje de notificación en notificaciones de Android](assets/push_content_3.png){zoomable="yes"}

>[!TAB iOS]

Para componer el mensaje, haga clic en los campos **[!UICONTROL Título]** y **[!UICONTROL Mensaje]**. Utilice el Editor de expresiones para definir contenido, personalizar datos y agregar contenido dinámico.

Puede agregar un **[!UICONTROL Subtítulo]**, que es el valor del parámetro subtitle de la carga útil de notificaciones de iOS. Consulte esta sección.

El modo push silencioso permite enviar una notificación “silenciosa” a una aplicación móvil. No se avisa al usuario de la llegada de la notificación. Esta se transfiere directamente a la aplicación.

![Descripción: ejemplo de definición de contenido para notificaciones de iOS](assets/push_content_1.png){zoomable="yes"}

>[!ENDTABS]

## Configuración avanzada de notificación push {#push-advanced}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings"
>title="Configuración avanzada de notificaciones push"
>abstract="Defina la configuración avanzada para la notificación push como su prioridad, el recuento de notificaciones asociado, las variables de aplicación y mucho más."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_critical"
>title="Modo de alerta crítica"
>abstract="Habilite esta opción para añadir sonido a la notificación, incluso si el teléfono del usuario está en modo de enfoque o si el dispositivo está silenciado. Esto garantiza que, en cualquier caso, se notifique a los usuarios de las alertas importantes."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_count"
>title="Recuento de notificaciones"
>abstract="Utilice esta opción para establecer el número de notificaciones sin leer que se mostrará directamente en el icono de la aplicación. Esto permite al usuario ver rápidamente el número de notificaciones pendientes."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_mutable"
>title="Contenido mutable"
>abstract="Utilice esta opción para permitir que la aplicación móvil descargue contenido multimedia asociado a la notificación."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_score"
>title="Puntuación de relevancia"
>abstract="Establezca una puntuación de relevancia de 0 a 100 para priorizar el orden de las notificaciones en el resumen de notificaciones. Las puntuaciones más altas indican notificaciones más importantes."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_app_variables"
>title="Variables de la aplicación"
>abstract="Utilice variables de aplicación para definir el comportamiento de las notificaciones. Estas variables son totalmente personalizables y se incluyen, ya que una parte de la carga útil de mensajes se envía al dispositivo móvil."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_advanced_settings_category"
>title="ID de categoría"
>abstract="Especifique el nombre del ID de categoría asociado a la notificación. Esto permite mostrar los botones de acción, lo que permite al usuario realizar varias tareas directamente desde la notificación sin abrir la aplicación."

Las opciones avanzadas dependen del sistema operativo móvil: Android o iOS. Examine las pestañas siguientes para aprender a definir las opciones del mensaje para cada sistema operativo.

>[!BEGINTABS]

>[!TAB Android]

![Descripción: ejemplo de configuración avanzada para notificaciones de Android](assets/push_content_5.png){zoomable="yes"}

| Parámetro | Descripción |
|---------|---------|
| **[!UICONTROL Sonido]** | Configure el sonido para que se reproduzca cuando el dispositivo reciba la notificación. |
| **[!UICONTROL Recuento de notificaciones]** | Configure el número de información nueva no leída que se mostrará directamente en el icono de la aplicación. Esto permite al usuario ver rápidamente el número de notificaciones pendientes. |
| **[!UICONTROL ID de canal]** | Establezca el ID de canal de la notificación. La aplicación debe crear un canal con este ID de canal antes de recibir cualquier notificación. |
| **[!UICONTROL Acción de clic]** | Defina la acción asociada con un clic del usuario en la notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación. |
| **[!UICONTROL Etiqueta]** | Establezca un identificador utilizado para reemplazar las notificaciones existentes en el cajón de notificaciones. Esto ayuda a evitar la acumulación de varias notificaciones y garantiza que solo se muestre la notificación relevante más reciente. |
| **[!UICONTROL Prioridad]** | Defina el nivel de prioridad de la notificación, que puede ser predeterminado, mínimo, bajo o alto. El nivel de prioridad determina la importancia y la urgencia de la notificación, lo que influye en cómo se muestra y si puede omitir determinada configuración del sistema. Para más información, consulte la [documentación de FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibilidad]** | Defina el nivel de visibilidad de la notificación, que puede ser pública, privada o secreta. El nivel de visibilidad determina la cantidad de contenido de la notificación que se muestra en la pantalla de bloqueo y en otras áreas confidenciales. Para obtener más información, consulte la [documentación de FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Adhesivo]** | Cuando se activa, la notificación permanece visible incluso después de que el usuario haga clic en ella. <br>Si está desactivada, la notificación se descarta automáticamente cuando el usuario interactúa con ella. El comportamiento adhesivo permite que las notificaciones importantes persistan en la pantalla durante períodos más largos. |
| **[!UICONTROL Variables de aplicación]** | Permite definir el comportamiento de las notificaciones. Estas variables son totalmente personalizables y se incluyen, ya que una parte de la carga útil de mensajes se envía al dispositivo móvil. |

>[!TAB iOS]

![Descripción: ejemplo de configuración avanzada para notificaciones de iOS](assets/push_content_2.png){zoomable="yes"}

| Parámetro | Descripción |
|---------|---------|
| **[!UICONTROL Modo de alerta crítica]** | Habilite esta opción para añadir sonido a la notificación, incluso si el teléfono del usuario está en modo de enfoque o si el dispositivo está silenciado. Esto garantiza que el usuario observe las alertas importantes. Cuando se selecciona, puede ajustar el volumen de la notificación mediante la barra de nivel de volumen. Un número entre 0 y 100 sobre la barra refleja su configuración. |
| **[!UICONTROL Limpiar insignia]** | Active esta opción para actualizar el valor del distintivo mostrado en el icono de la aplicación. Garantiza que el distintivo refleje con precisión la cantidad de información nueva no leída. |
| **[!UICONTROL Recuento de notificaciones]** | Establezca un número que se mostrará directamente en el icono de la aplicación, indicando la cantidad de información nueva no leída. Esto proporciona una referencia visual rápida para el usuario. |
| **[!UICONTROL Volumen]** | Volumen de su sonido de 0 a 100. |
| **[!UICONTROL Contenido mutable]** | Active esta opción para permitir que la aplicación móvil descargue contenido multimedia asociado a la notificación. Para obtener más información, consulte la [documentación para desarrolladores de Apple](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html). |
| **[!UICONTROL Puntuación de relevancia]** | Establezca una puntuación de relevancia de 0 a 100 para priorizar el orden de las notificaciones en el resumen de notificaciones. Las puntuaciones más altas indican notificaciones más importantes. |
| **[!UICONTROL Nivel de interrupción]** | <ul> <li>**[!UICONTROL Activo]**: de forma predeterminada, el sistema presenta la notificación inmediatamente, enciende la pantalla y puede reproducir un sonido. Las notificaciones no rompen los modos de Enfoque.</li><li>**[!UICONTROL Pasivo]**: el sistema agrega la notificación a la lista de notificaciones sin iluminar la pantalla ni reproducir un sonido. Las notificaciones no rompen los modos de Enfoque.</li><li>**[!UICONTROL Con distinción de tiempo]**: el sistema presenta la notificación inmediatamente, enciende la pantalla, puede reproducir un sonido y atravesar los modos de Enfoque. Este nivel no requiere permisos especiales de Apple.</li> <li>**[!UICONTROL Crítico]**: el sistema presenta la notificación inmediatamente, enciende la pantalla y evita el interruptor silencioso o los modos de enfoque. Tenga en cuenta que este nivel requiere un permiso especial de Apple.</ul> |
| **[!UICONTROL Id. de subproceso]** | Identificador utilizado para agrupar las notificaciones relacionadas. Las notificaciones con el mismo ID de hilo se organizan como una sola conversación o hilo en la lista de notificaciones. |
| **[!UICONTROL Categoría]** | Especifique el nombre del ID de categoría asociado a la notificación. Esto permite mostrar los botones de acción, lo que permite al usuario realizar varias tareas directamente desde la notificación sin abrir la aplicación. |
| **[!UICONTROL Id. de contenido de destino]** | Identificador utilizado para destinar la ventana de aplicación que se reenvía cuando se abre la notificación. |
| **[!UICONTROL Imagen de lanzamiento]** | Especifique el nombre del archivo de imagen de lanzamiento que se mostrará cuando el usuario decida iniciar la aplicación desde la notificación. Se mostrará la imagen seleccionada en lugar de la pantalla de inicio normal de la aplicación. |
| **[!UICONTROL Variables de aplicación]** | Permite definir el comportamiento de las notificaciones. Estas variables son totalmente personalizables y se incluyen, ya que una parte de la carga útil de mensajes se envía al dispositivo móvil. |

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->
