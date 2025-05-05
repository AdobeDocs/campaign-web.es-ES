---
audience: end-user
title: Diseño de una entrega de notificaciones push enriquecidas
description: Aprenda a diseñar una entrega de notificaciones push enriquecidas con Android con Adobe Campaign Web
exl-id: a87cb933-b564-4fa4-b173-6a94d7e27da5
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '3379'
ht-degree: 5%

---

# Diseño de un envío push enriquecido para Android {#rich-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_remind_later"
>title="Botón Recordar más tarde"
>abstract="El botón **Recordar más tarde** proporciona la opción de programar un recordatorio. El campo Marca de tiempo requiere un valor que represente la época en segundos."

>[!IMPORTANT]
>
>* Esta capacidad requiere una actualización a la versión 8.6.3 de Campaign<!--or v8.7.2-->. Obtenga más información en las [Notas de la versión](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/releases/release-notes){target="_blank"} de la consola del cliente de la versión 8 de Campaign.
>
>* Antes de diseñar una notificación push enriquecida, primero debe configurar el conector V2. Consulte este [Página](https://experienceleague.adobe.com/en/docs/campaign-classic/using/sending-messages/sending-push-notifications/configure-the-mobile-app/configuring-the-mobile-application-android#configuring-external-account-android){target="_blank"} para conocer los detalles del procedimiento.


Con Firebase Cloud Messaging, puede elegir entre dos tipos de mensajes:

* La aplicación cliente gestiona los **[!UICONTROL mensajes]** de datos. Estos mensajes se envían directamente al aplicación móvil, que genera y muestra un notificación de Android en el dispositivos. Los mensajes de datos solo contienen las variables de aplicación personalizadas.

* El **[!UICONTROL mensaje]** de notificación, gestionado automáticamente por el SDK de FCM. FCM muestra automáticamente el mensaje en el dispositivos de los usuarios en nombre de la aplicación cliente. Los mensajes de notificación contienen un conjunto predefinido de parámetros y opciones, pero pueden personalizarse aún más con las variables de aplicación personalizadas.

![Captura de pantalla de la página Entregar en Android](assets/rich_push.png){zoomable="yes"}

## Definición del contenido de la notificación {#push-message}

Una vez creada la envío de inserción, puede definir su contenido mediante una de las siguientes plantillas:

* **Predeterminado** le permite enviar notificaciones con un icono simple y una imagen adjunta.

* **Basic** puede incluir texto, imágenes y botones en las notificaciones.

* **Carrusel** le permite enviar notificaciones con texto y varias imágenes que los usuarios pueden deslizar rápidamente.

* **Los botones de** icono le permiten enviar notificaciones con un icono y una imagen correspondiente.

* **Cuadro de entrada** recopila datos proporcionados por el usuario y comentarios directamente a través de la notificación.

* **El catálogo de productos** muestra una variedad de imágenes de productos.

* **Clasificación del producto** permite que los usuarios proporcionen comentarios y valoren los productos.

* **Timer** incluye un temporizador de cuenta atrás activo en tus notificaciones.

* **Bisel cero** usa toda la superficie de fondo para una imagen, con texto superpuesto sin problemas.

Desplácese por las pestañas siguientes para obtener más información sobre cómo personalizar estas plantillas.

>[!BEGINTABS]

>[!TAB Predeterminado]

1. En la lista desplegable **[!UICONTROL Plantilla]**, seleccione **[!UICONTROL Predeterminada]**.

   ![](assets/rich_push_default.png)

1. Para redactar el mensaje, escribe el texto en los campos **[!UICONTROL Título]** y **[!UICONTROL Mensaje]**.

   ![](assets/rich_push_default_2.png)

1. Utilice el Editor de expresiones para definir contenido, personalizar datos y agregar contenido dinámico. [Más información](../personalization/personalize.md)

1. Defina la **[!UICONTROL acción de clic]** asociada con un clic del usuario en su notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Para personalizar aún más la notificación push, puede elegir una URL de **[!UICONTROL Image]** para agregarla a la notificación push y el **[!UICONTROL icono]** de la notificación para mostrarla en los dispositivos de sus perfiles.

   ![](assets/rich_push_default_3.png)

1. Configure **[!UICONTROL Advanced settings]** de su notificación push. [Más información](#push-advanced)

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje.

>[!TAB Básico]

1. En la lista desplegable **[!UICONTROL Plantilla]**, seleccione **[!UICONTROL Básico]**.

   ![](assets/rich_push_basic.png)

1. Para redactar el mensaje, escribe el texto en los campos **[!UICONTROL Título]**, **[!UICONTROL Mensaje]** y **[!UICONTROL Mensaje ampliado]**.

   El texto **[!UICONTROL Message]** aparece en la vista contraída mientras que el **[!UICONTROL mensaje expandido]** se muestra cuando se expande la notificación.

   ![](assets/rich_push_basic_2.png)

1. Utilice el Editor de expresiones para definir contenido, personalizar datos y agregar contenido dinámico. [Más información](../personalization/personalize.md)

1. Agregue la URL que define la **[!UICONTROL acción de clic]** asociada con un clic del usuario en su notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Seleccione el **[!UICONTROL tipo de vínculo]** de la dirección URL que agregó al campo **[!UICONTROL Acción de clic]**:

   * **[!UICONTROL URL web]**: Las URL web dirigen a los usuarios al contenido en línea. Al hacer clic en, se solicita al explorador web predeterminado del dispositivo que abra y navegue hasta la dirección URL designada.

   * **[!UICONTROL Vínculo profundo]**: Los vínculos profundos son direcciones URL que guían a los usuarios a secciones específicas de una aplicación, incluso si esta está cerrada. Al hacer clic en él, puede aparecer un cuadro de diálogo que permite a los usuarios elegir entre varias aplicaciones capaces de gestionar el vínculo.

   * **[!UICONTROL Abrir aplicación]**: Las direcciones URL de Abrir aplicación permiten conectarse directamente al contenido de una aplicación. Permite a la aplicación establecerse como controlador predeterminado para un tipo específico de vínculo, omitiendo el cuadro de diálogo de desambiguación.

   Para obtener más información sobre cómo administrar los vínculos de la aplicación de Android, consulte [Documentación para desarrolladores de Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_basic_3.png)

1. Para personalizar aún más su notificación push, puede elegir un **[!UICONTROL URL Imagen]** para agregar a su notificación push y el icono del **[!UICONTROL notificación]** para mostrar en el dispositivos de sus perfiles.

1. Haga clic en **[!UICONTROL añadir botón]** y rellene los siguientes campos:

   * **[!UICONTROL Etiquetar]**: texto mostrado en el botón.
   * **[!UICONTROL URI de enlace:]** especifique el URI que se ejecutará al hacer clic en el botón.
   * **[!UICONTROL Tipo de vínculo]**: el tipo de vínculo es **[!UICONTROL URL web]**, **[!UICONTROL Vínculo profundo]** o **[!UICONTROL Abrir aplicación]**.

   Tiene la opción de incluir hasta tres botones en la notificación push. Si opta por el botón **[!UICONTROL Recordar más tarde]**, solo puede incluir un máximo de dos botones.

   ![](assets/rich_push_basic_4.png)

1. Haga clic en **[!UICONTROL Agregar recordatorio más tarde]** para agregar una opción Recordármelo más tarde a la notificación de inserción. Escriba una **[!UICONTROL Etiqueta]** y **[!UICONTROL Marca de tiempo]**.

   El campo Marca de tiempo espera un valor que represente la época en segundos.

   ![](assets/rich_push_basic_5.png)

1. Configure **[!UICONTROL Advanced settings]** de su notificación push. [Más información](#push-advanced)

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje.

>[!TAB Carrusel]

1. En la lista desplegable **[!UICONTROL Plantilla]**, seleccione **[!UICONTROL Carrusel]**.

   ![](assets/rich_push_carousel.png)

1. Para redactar el mensaje, escribe el texto en los campos **[!UICONTROL Título]**, **[!UICONTROL Mensaje]** y **[!UICONTROL Mensaje ampliado]**.

   El **[!UICONTROL texto Enviar mensaje]** aparece en el vista contraído, mientras que el **[!UICONTROL mensaje]** ampliado se muestra cuando se expande el notificación.

   ![](assets/rich_push_carousel_1.png)

1. Utilice el editor de expresión para definir contenido, personalizar datos y agregar contenido dinámico. [Más información](../personalization/personalize.md)

1. añadir la URL que define la acción **Haga** clic asociada a un clic usuario en su notificación. Esto determina el comportamiento cuando el usuario interactúa con el notificación, como al abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Seleccione el **[!UICONTROL tipo de vínculo]** de la dirección URL que agregó al campo **[!UICONTROL Acción de clic]**:

   * **[!UICONTROL URL web]**&#x200B;L: Las URL web dirigen a los usuarios al contenido en línea. Al hacer clic, solicitan al explorador web predeterminado del dispositivos que se abra y navegue hasta el URL designado.

   * **[!UICONTROL Enlace]** profundo: los vínculos profundos son URL que guían a los usuarios a secciones específicas dentro de una aplicación igualado si la aplicación está cerrada. Al hacer clic, puede aparecer un cuadro de diálogo que permite a los usuarios elegir entre varias aplicaciones capaces de manejar el vincular.

   * **[!UICONTROL Abrir aplicación]**: Las URL de aplicación abiertas le permiten conectarse directamente a contenido dentro de un aplicación. Permite que su aplicación se establezca como el controlador predeterminado para un tipo específico de vincular, evitando el cuadro de diálogo de desambiguación.

   Para obtener más información sobre cómo gestionar vínculos de aplicación Android, consulte la [documentación](https://developer.android.com/training/app-links) de Android Developers.

   ![](assets/rich_push_carousel_2.png)

1. Para personalizar aún más la notificación push, puede elegir el **[!UICONTROL icono]** de la notificación para que se muestre en los dispositivos de sus perfiles.

1. Elija cómo funciona el **[!UICONTROL Carrusel]** :

   * **[!UICONTROL Automático]**: alterna automáticamente las imágenes como diapositivas, realizando la transición a intervalos predefinidos.
   * **[!UICONTROL Manual]**: permite a los usuarios deslizar manualmente entre diapositivas para navegar por las imágenes.

     Active la **[!UICONTROL opción tira de película]** para incluir vistas previas de las imágenes anteriores y siguientes junto con el diapositiva principal.

1. Haga clic en **[!UICONTROL añadir imagen]** e introduzca su URL y texto de imagen.

   Asegúrese de incluir un mínimo de tres imágenes y un máximo de cinco.

   ![](assets/rich_push_carousel_3.png)

1. Controle el orden de las imágenes con las flechas Abajo y Arriba.

1. Configure **[!UICONTROL Advanced settings]** de su notificación push. [Más información](#push-advanced)

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje.

>[!TAB Botones de icono]

1. En la lista desplegable **[!UICONTROL Plantilla]**, seleccione **[!UICONTROL botones de icono]**.

   ![](assets/rich_push_icon_1.png)

1. Agregue la URL que define la **[!UICONTROL acción de clic]** asociada con un clic del usuario en su notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Seleccione el **[!UICONTROL tipo de vínculo]** de la dirección URL que agregó al campo **[!UICONTROL Acción de clic]**:

   * **[!UICONTROL URL web]**: Las URL web dirigen a los usuarios al contenido en línea. Al hacer clic en, se solicita al explorador web predeterminado del dispositivo que abra y navegue hasta la dirección URL designada.

   * **[!UICONTROL Vínculo profundo]**: Los vínculos profundos son direcciones URL que guían a los usuarios a secciones específicas de una aplicación, incluso si esta está cerrada. Al hacer clic en él, puede aparecer un cuadro de diálogo que permite a los usuarios elegir entre varias aplicaciones capaces de gestionar el vínculo.

   * **[!UICONTROL Abrir aplicación]**: Las direcciones URL de Abrir aplicación permiten conectarse directamente al contenido de una aplicación. Permite a la aplicación establecerse como controlador predeterminado para un tipo específico de vínculo, omitiendo el cuadro de diálogo de desambiguación.

   Para obtener más información sobre cómo administrar los vínculos de la aplicación de Android, consulte [Documentación para desarrolladores de Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_icon_2.png)

1. Para personalizar aún más la notificación push, puede elegir el **[!UICONTROL icono]** de la notificación para que se muestre en los dispositivos de sus perfiles.

1. Agrega la URL de tu **[!UICONTROL imagen del botón Cancelar]**.

1. Haga clic en **[!UICONTROL Agregar icono]** e introduzca su **URL de imagen**, **[!UICONTROL URI de vínculo]** y elija su **[!UICONTROL tipo de vínculo]**.

   Asegúrese de incluir un mínimo de tres iconos y un máximo de cinco.

   ![](assets/rich_push_icon_3.png)

1. Controle el orden de las imágenes con las flechas Abajo y Arriba.

1. Configure **[!UICONTROL Advanced settings]** de su notificación push. [Más información](#push-advanced)

   ![](assets/rich_push_icon_4.png)

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje.

>[!TAB Cuadro de entrada]

1. En la lista desplegable **[!UICONTROL Tipo de notificación]**, seleccione **[!UICONTROL Cuadro de entrada]**.

   ![](assets/rich_push_input_1.png)

1. Para redactar el mensaje, escribe el texto en los campos **[!UICONTROL Título]**, **[!UICONTROL Mensaje]** y **[!UICONTROL Mensaje ampliado]**.

   El texto **[!UICONTROL Message]** aparece en la vista contraída mientras que el **[!UICONTROL mensaje expandido]** se muestra cuando se expande la notificación.

   ![](assets/rich_push_input_2.png)

1. Utilice campos de personalización dinámicos para definir contenido, personalizar datos y agregar contenido dinámico. [Más información](../personalization/personalize.md)

1. Agregue la URL que define la **[!UICONTROL acción de clic]** asociada con un clic del usuario en su notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Seleccione el **[!UICONTROL tipo de vínculo]** de la dirección URL que agregó al campo **[!UICONTROL Acción de clic]**:

   * **[!UICONTROL URL web]**: Las URL web dirigen a los usuarios al contenido en línea. Al hacer clic, solicitan al explorador web predeterminado del dispositivos que se abra y navegue hasta el URL designado.

   * **[!UICONTROL Enlace]** profundo: los vínculos profundos son URL que guían a los usuarios a secciones específicas dentro de una aplicación igualado si la aplicación está cerrada. Al hacer clic, puede aparecer un cuadro de diálogo que permite a los usuarios elegir entre varias aplicaciones capaces de manejar el vincular.

   * **[!UICONTROL Abrir aplicación]**: Las direcciones URL de Abrir aplicación permiten conectarse directamente al contenido de una aplicación. Permite a la aplicación establecerse como controlador predeterminado para un tipo específico de vínculo, omitiendo el cuadro de diálogo de desambiguación.

   Para obtener más información sobre cómo administrar los vínculos de la aplicación de Android, consulte [Documentación para desarrolladores de Android](https://developer.android.com/training/app-links).

1. Para personalizar aún más la notificación push, puede elegir una URL de **[!UICONTROL Image]** para agregarla a la notificación push y el **[!UICONTROL icono]** de la notificación para mostrarla en los dispositivos de sus perfiles.

1. Complete las siguientes opciones para su **cuadro de entrada**:

   * **[!UICONTROL Nombre del receptor de entrada]**: escriba el nombre o identificador del receptor de la entrada.
   * **[!UICONTROL Texto de entrada]**: escriba el texto para el **cuadro de entrada**.
   * **[!UICONTROL Texto de comentarios]**: escriba el texto que se mostrará tras la respuesta.
   * **[!UICONTROL Imagen de comentarios]**: agrega la dirección URL de la imagen mostrada después de una respuesta.

   ![](assets/rich_push_input_3.png)

1. Configure **[!UICONTROL Advanced settings]** de su notificación push. [Más información](#push-advanced)

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje.

>[!TAB Catálogo de productos]

1. En el menú desplegable Tipo de **[!UICONTROL notificación, seleccione**&#x200B;[!UICONTROL &#x200B; Catálogo &#x200B;]&#x200B;**]** de productos.

   ![](assets/rich_push_catalog_1.png)

1. Para redactar el mensaje, introduzca el texto en los **[!UICONTROL campos Título]** y **[!UICONTROL Enviar mensaje]** .

   ![](assets/rich_push_catalog_2.png)

1. Utilice campos de personalización dinámicas para definir contenido, personalizar los datos y añadir contenido dinámico. [Más información](../personalization/personalize.md)

1. Agregue la URL que define la **[!UICONTROL acción de clic]** asociada con un clic del usuario en su notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Seleccione el **[!UICONTROL tipo]** de vínculo de la URL agregó al campo Acción de **[!UICONTROL clic]** :

   * **[!UICONTROL URL]** web: las direcciones URL web dirigen a los usuarios hacia en línea contenido. Al hacer clic, solicitan al explorador web predeterminado del dispositivos que se abra y navegue hasta el URL designado.

   * **[!UICONTROL Enlace]** profundo: los vínculos profundos son URL que guían a los usuarios a secciones específicas dentro de una aplicación igualado si la aplicación está cerrada. Al hacer clic en él, puede aparecer un cuadro de diálogo que permite a los usuarios elegir entre varias aplicaciones capaces de gestionar el vínculo.

   * **[!UICONTROL Abrir aplicación]**: Las direcciones URL de Abrir aplicación permiten conectarse directamente al contenido de una aplicación. Permite a la aplicación establecerse como controlador predeterminado para un tipo específico de vínculo, omitiendo el cuadro de diálogo de desambiguación.

   Para obtener más información sobre cómo gestionar vínculos de aplicación Android, consulte la [documentación](https://developer.android.com/training/app-links) de Android Developers.

1. Para personalizar aún más su notificación, puede elegir el icono del **[!UICONTROL notificación]** para mostrar en el dispositivos de sus perfiles.

1. Introduzca el texto y la **imagen de hacer clic para la acción**.**&#x200B;**

1. Elija el **[!UICONTROL tipo de]** visualización entre horizontal o vertical.

1. Rellene la **[!UICONTROL información de los elementos del catálogo]** .

   Asegúrese de incluir un mínimo de tres elementos y un máximo de cinco elementos.

   ![](assets/rich_push_catalog_3.png)

1. Controle el orden de las imágenes con las flechas Abajo y Arriba.

1. Configure **[!UICONTROL Advanced settings]** de su notificación push. [Más información](#push-advanced)

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje.

>[!TAB Clasificación del producto]

1. En el menú desplegable Tipo **de notificación, seleccione**&#x200B;[!UICONTROL &#x200B; Clasificación &#x200B;]&#x200B;**del** producto.

   ![](assets/rich_push_rating_1.png)

1. Para redactar el mensaje, escribe el texto en los campos **[!UICONTROL Título]**, **[!UICONTROL Mensaje]** y **[!UICONTROL Mensaje ampliado]**.

   El texto **[!UICONTROL Message]** aparece en la vista contraída mientras que el **[!UICONTROL mensaje expandido]** se muestra cuando se expande la notificación.

   ![](assets/rich_push_rating_2.png)

1. Agregue la URL que define la **[!UICONTROL acción de clic]** asociada con un clic del usuario en su notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Seleccione el **[!UICONTROL tipo de vínculo]** de la dirección URL que agregó al campo **[!UICONTROL Acción de clic]**:

   * **[!UICONTROL URL web]**: Las URL web dirigen a los usuarios al contenido en línea. Al hacer clic en, se solicita al explorador web predeterminado del dispositivo que abra y navegue hasta la dirección URL designada.

   * **[!UICONTROL Vínculo profundo]**: Los vínculos profundos son direcciones URL que guían a los usuarios a secciones específicas de una aplicación, incluso si esta está cerrada. Al hacer clic en él, puede aparecer un cuadro de diálogo que permite a los usuarios elegir entre varias aplicaciones capaces de gestionar el vínculo.

   * **[!UICONTROL Abrir aplicación]**: Las direcciones URL de Abrir aplicación permiten conectarse directamente al contenido de una aplicación. Permite a la aplicación establecerse como controlador predeterminado para un tipo específico de vínculo, omitiendo el cuadro de diálogo de desambiguación.

   Para obtener más información sobre cómo administrar los vínculos de la aplicación de Android, consulte [Documentación para desarrolladores de Android](https://developer.android.com/training/app-links).

1. Para personalizar aún más la notificación push, puede elegir una URL de **[!UICONTROL Image]** para agregarla a la notificación push y el **[!UICONTROL icono]** de la notificación para mostrarla en los dispositivos de sus perfiles.

1. Agregue su **[!UICONTROL icono de clasificación en estado no seleccionado]** y el **[!UICONTROL icono de clasificación en estado seleccionado]** direcciones URL.

   ![](assets/rich_push_rating_3.png)

1. Haga clic en **[!UICONTROL Agregar clasificación]** e introduzca su **[!UICONTROL URI de vínculo]** y **[!UICONTROL tipo de vínculo]**.

   Asegúrese de incluir un mínimo de tres clasificaciones y un máximo de cinco clasificaciones.

   ![](assets/rich_push_rating_4.png)

1. Controle el orden de las imágenes con las flechas Abajo y Arriba.

1. Configure **[!UICONTROL Advanced settings]** de su notificación push. [Más información](#push-advanced)

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje.

>[!TAB Temporizador]

1. En el menú desplegable **[!UICONTROL Tipo de notificación]**, seleccione **[!UICONTROL Temporizador]**.

   ![](assets/rich_push_timer_1.png)

1. Para redactar el mensaje, escribe el texto en los campos **[!UICONTROL Título]** y **[!UICONTROL Mensaje]**.

   Utilice campos de personalización dinámicos para definir contenido, personalizar datos y agregar contenido dinámico. [Más información](../personalization/personalize.md)

   ![](assets/rich_push_timer_2.png)

1. Agregue la URL que define la **[!UICONTROL acción de clic]** asociada con un clic del usuario en su notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Seleccione el **[!UICONTROL tipo de vínculo]** de la dirección URL que agregó al campo **[!UICONTROL Acción de clic]**:

   * **[!UICONTROL URL]** web: las direcciones URL web dirigen a los usuarios hacia en línea contenido. Al hacer clic, solicitan al explorador web predeterminado del dispositivos que se abra y navegue hasta el URL designado.

   * **[!UICONTROL Enlace]** profundo: los vínculos profundos son URL que guían a los usuarios a secciones específicas dentro de una aplicación igualado si la aplicación está cerrada. Al hacer clic en él, puede aparecer un cuadro de diálogo que permite a los usuarios elegir entre varias aplicaciones capaces de gestionar el vínculo.

   * **[!UICONTROL Abrir aplicación]**: Las direcciones URL de Abrir aplicación permiten conectarse directamente al contenido de una aplicación. Permite a la aplicación establecerse como controlador predeterminado para un tipo específico de vínculo, omitiendo el cuadro de diálogo de desambiguación.

   Para obtener más información sobre cómo administrar los vínculos de la aplicación de Android, consulte [Documentación para desarrolladores de Android](https://developer.android.com/training/app-links).

   ![](assets/rich_push_timer_3.png)

1. Para personalizar aún más la notificación push, puede elegir una URL de **[!UICONTROL Image]** para agregarla a la notificación push y el **[!UICONTROL icono]** de la notificación para mostrarla en los dispositivos de sus perfiles.

1. Establezca su **[!UICONTROL Duración del temporizador]** en segundos o la **[!UICONTROL Marca de tiempo de fin del temporizador]** en una marca de tiempo de época específica.

   ![](assets/rich_push_timer_4.png)

1. Escriba el texto y la imagen que se mostrarán después de que caduque el temporizador en los campos **[!UICONTROL Título alternativo]**, **[!UICONTROL Mensaje alternativo]**, **[!UICONTROL Mensaje expandido alternativo]** y **[!UICONTROL Imagen de lanzamiento alternativa]**.

   ![](assets/rich_push_timer_5.png)

1. Configure **[!UICONTROL Advanced settings]** de su notificación push. [Más información](#push-advanced)

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje.

>[!TAB Sin bisel]

1. En la lista desplegable **[!UICONTROL Tipo de notificación]**, seleccione **[!UICONTROL Cero carcasa]**.

   ![](assets/rich_push_bezel_1.png)

1. Para redactar el mensaje, introduzca el texto en los **[!UICONTROL campos Título]**, **[!UICONTROL Enviar mensaje]** y **[!UICONTROL Mensaje]** ampliado.

   El **[!UICONTROL texto Enviar mensaje]** aparece en el vista contraído, mientras que el **[!UICONTROL mensaje]** ampliado se muestra cuando se expande el notificación.

   ![](assets/rich_push_bezel_2.png)

1. Utilice campos de personalización dinámicos para definir contenido, personalizar datos y agregar contenido dinámico. [Más información](../personalization/personalize.md)

1. Agregue la URL que define la **[!UICONTROL acción de clic]** asociada con un clic del usuario en su notificación. Determina el comportamiento cuando el usuario interactúa con la notificación, como abrir una pantalla específica o realizar una acción específica en la aplicación.

1. Seleccione el **[!UICONTROL tipo de vínculo]** de la dirección URL que agregó al campo **[!UICONTROL Acción de clic]**:

   * **[!UICONTROL URL web]**: Las URL web dirigen a los usuarios al contenido en línea. Al hacer clic en, se solicita al explorador web predeterminado del dispositivo que abra y navegue hasta la dirección URL designada.

   * **[!UICONTROL Vínculo profundo]**: Los vínculos profundos son direcciones URL que guían a los usuarios a secciones específicas de una aplicación, incluso si esta está cerrada. Al hacer clic en él, puede aparecer un cuadro de diálogo que permite a los usuarios elegir entre varias aplicaciones capaces de gestionar el vínculo.

   * **[!UICONTROL Abrir aplicación]**: Las direcciones URL de Abrir aplicación permiten conectarse directamente al contenido de una aplicación. Permite a la aplicación establecerse como controlador predeterminado para un tipo específico de vínculo, omitiendo el cuadro de diálogo de desambiguación.

   Para obtener más información sobre cómo administrar los vínculos de la aplicación de Android, consulte [Documentación para desarrolladores de Android](https://developer.android.com/training/app-links).

1. Para personalizar aún más la notificación push, puede elegir una URL de **[!UICONTROL Image]** para agregarla a la notificación push y el **[!UICONTROL icono]** de la notificación para mostrarla en los dispositivos de sus perfiles.

   ![](assets/rich_push_bezel_3.png)

1. Elija el **[!UICONTROL estilo]** de notificación contraído para su notificación si el notificación muestra principalmente una imagen o un texto.

1. Configure los **[!UICONTROL ajustes]** de Avanzadas de su notificación push. [Más información](#push-advanced)

Una vez que haya definido su contenido de mensaje, puede usar prueba suscriptores para previsualización y prueba el mensaje.

>[!ENDTABS]

## Configuración avanzada de notificación push {#push-advanced}

![](assets/push_content_5.png){zoomable="yes"}

| Parámetro | Descripción |
|---------|---------|
| **[!UICONTROL Color del icono]** | Establece el color de tu icono con tus códigos de color hexadecimales. |
| **[!UICONTROL Título color]** | Establece el color de tu Título con tus códigos de color hexadecimales. |
| **[!UICONTROL Color del texto del mensaje]** | Defina el color del texto del mensaje con sus códigos de color hexadecimales. |
| **[!UICONTROL Color del temporizador]** | Configure el color de su Timer con sus códigos de color hexadecimales. |
| **[!UICONTROL Color de fondo de notificación]** | Establece el color de tu fondo de notificación con tus códigos de color hexadecimales. |
| **[!UICONTROL Sonido]** | Configure el sonido para que se reproduzca cuando el dispositivo reciba la notificación. |
| **[!UICONTROL Recuento de notificaciones]** | Configure el número de información nueva no leída que se mostrará directamente en el icono de la aplicación. Esto permite al usuario ver rápidamente el número de notificaciones pendientes. |
| **[!UICONTROL ID de canal]** | Establezca el ID de canal de la notificación. La aplicación debe crear un canal con este ID de canal antes de recibir cualquier notificación. |
| **[!UICONTROL Etiqueta]** | Establezca un identificador utilizado para reemplazar las notificaciones existentes en el cajón de notificaciones. Esto ayuda a evitar la acumulación de varias notificaciones y garantiza que solo se muestre la notificación relevante más reciente. |
| **[!UICONTROL Prioridad]** | Defina el nivel de prioridad de la notificación, que puede ser predeterminado, mínimo, bajo o alto. El nivel de prioridad determina la importancia y la urgencia de la notificación, lo que influye en cómo se muestra y si puede omitir determinada configuración del sistema. Para más información, consulte la [documentación de FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibilidad]** | Defina el nivel de visibilidad de la notificación, que puede ser pública, privada o secreta. El nivel de visibilidad determina la cantidad de contenido de la notificación que se muestra en la pantalla de bloqueo y en otras áreas confidenciales. Para obtener más información, consulte la [documentación de FCM](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Notificación fija]** | Cuando se activa, la notificación permanece visible incluso después de que el usuario haga clic en ella. <br>Si se desactiva, la notificación se descarta automáticamente cuando el usuario interactúa con ella. El comportamiento pegajoso permite que notificaciones importantes permanezcan en la pantalla durante períodos más largos. |
| **[!UICONTROL Variables de aplicación]** | permiten definir notificación comportamiento. Estas variables son totalmente personalizables y se incluyen, ya que una parte de la carga útil de mensajes se envía al dispositivo móvil. |