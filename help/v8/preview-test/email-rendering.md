---
audience: end-user
title: Prueba del procesamiento de correo electrónico
description: Obtenga información sobre cómo probar el procesamiento de correo electrónico en la interfaz de usuario web de Campaign
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 3%

---


# Prueba del procesamiento de correo electrónico {#email-rendering}

Antes de enviar el correo electrónico, asegúrese de que el mensaje se muestra a los destinatarios de una forma óptima en una gran variedad de clientes y dispositivos web.

Para ello, puede aprovechar su cuenta de **Litmus** en [!DNL Adobe Campaign] para obtener una vista previa instantánea del procesamiento de correo electrónico en diferentes contextos y comprobar la compatibilidad en las aplicaciones y los escritorios principales (correo web, servicio de mensajes, móvil, etc.).

>[!CAUTION]
>
>El uso del procesamiento de correo electrónico en Campaign envía una prueba a un sistema de terceros. Al conectar su cuenta de Litmus con [!DNL Campaign], reconoce que Adobe no es responsable de ningún dato que pueda enviar a ese tercero. La política de correo electrónico para la retención de datos de Litmus se aplica a estos correos electrónicos, incluidos los datos de personalización que pueden incluirse en estas pruebas. Para acceder o eliminar dichos datos, deberá ponerse en contacto directamente con Litmus.

Para acceder a las funciones de procesamiento de correo electrónico, debe:

* Tener una cuenta de Litmus
* Seleccionar perfiles o perfiles de prueba: aprenda cómo en [esta sección](preview-content.md)

A continuación, siga los pasos a continuación.

1. En la pantalla [Editar contenido](../email/edit-content.md) o en el [Designer de correo electrónico](../email/get-started-email-designer.md), haga clic en el botón **[!UICONTROL Simular contenido]**.

1. Seleccione el botón **[!UICONTROL Procesar correo electrónico]**.

   ![](assets/simulate-rendering-button.png){zoomable="yes"}

1. Haga clic en **Conectar su cuenta de Litmus** en la sección superior derecha.

   ![](assets/simulate-rendering-litmus.png){zoomable="yes"}

1. Introduzca sus credenciales de e inicie sesión.

   ![](assets/simulate-rendering-credentials.png){zoomable="yes"}

1. Haga clic en el botón **Ejecutar prueba** para generar vistas previas de correo electrónico.

1. Compruebe el contenido de su correo electrónico en clientes populares de escritorio, móviles y web.

   ![](assets/simulate-rendering-previews.png){zoomable="yes"}

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png){zoomable="yes"}

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->
