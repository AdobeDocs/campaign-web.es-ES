---
audience: end-user
title: Edición del contenido de correo electrónico
description: Obtenga información sobre cómo editar el contenido del correo electrónico en la interfaz de usuario web de Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 20%

---

# Configurar el contenido de correo electrónico {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Definición del contenido del correo electrónico"
>abstract="La pantalla **Editar contenido** le permite definir elementos básicos del mensaje, como la dirección del remitente y la línea de asunto, realizar acciones adicionales como agregar archivos adjuntos u ofertas y acceder al Designer de correo electrónico para darle un aspecto pulido al mensaje."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Establecer las propiedades del correo electrónico"
>abstract="La sección **Detalles básicos** le permite actualizar la dirección del remitente y la dirección de respuesta, así como definir la línea de asunto mediante el Editor de expresiones."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Adjuntar archivos a un correo electrónico"
>abstract="Seleccione uno o varios archivos para insertar en el mensaje. Para evitar problemas de rendimiento, se recomienda no incluir más de un archivo adjunto por correo electrónico."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Editar seguimiento"
>abstract="De forma predeterminada, el seguimiento está habilitado para el envío, lo que significa que se realiza el seguimiento de todos los vínculos incluidos en el contenido del mensaje. Puede desactivar esta opción desde aquí."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="Adición de vínculos y seguimiento de mensajes"

La pantalla del correo electrónico **[!UICONTROL Editar contenido]** le permite:

* Defina los elementos básicos del mensaje, como la dirección del remitente y la línea de asunto.
* Realice acciones adicionales, como agregar archivos adjuntos o configurar ofertas.
* Acceda a [Email Designer](get-started-email-designer.md#start-authoring) para comenzar a crear el contenido apropiado de su correo electrónico.

>[!NOTE]
>
>Todos los campos de texto editables de esta pantalla se pueden rellenar con campos de personalización. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

Para configurar o editar el contenido de un correo electrónico, siga los pasos a continuación.

1. Haga clic en el botón **[!UICONTROL Editar contenido]** de la pantalla [panel de envío de correo electrónico](../email/create-email.md).

   ![Captura de pantalla que muestra el botón Editar contenido en el panel de envío de correo electrónico.](assets/email-edit-content-button.png){zoomable="yes"}

1. Se abre la pantalla de edición de contenido de correo electrónico.

   ![Captura de pantalla que muestra el panel de edición de contenido de correo electrónico.](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si está configurando un correo electrónico nuevo, los campos **[!UICONTROL De nombre]** y **[!UICONTROL De correo electrónico]** ya se han rellenado.

1. El campo **[!UICONTROL Nombre desde]** se define en la plantilla de correo electrónico. Si desea modificarlo, utilice un nombre fácilmente identificable por los destinatarios, como el nombre de su marca, para aumentar la velocidad de apertura de sus envíos.

   >[!NOTE]
   >
   >Para mejorar aún más la experiencia del destinatario, puede agregar el nombre de una persona como, por ejemplo, &quot;Eva de Luma&quot;.

1. El campo de dirección **[!UICONTROL De correo electrónico]** también se define en la plantilla de correo electrónico. Asegúrese de que el dominio de dirección coincida con el subdominio que delegó en Adobe.

   >[!NOTE]
   >
   >Puede cambiar la parte que precede a &#39;@&#39;, pero no la dirección de dominio.

1. Expanda la sección **[!UICONTROL Campos de respuesta]**. El nombre y las direcciones del remitente se utilizan de forma predeterminada para las respuestas. Sin embargo, Adobe recomienda utilizar una dirección real existente, como el servicio de atención al cliente de su marca. En este caso, si un destinatario envía una respuesta, el equipo de atención al cliente podrá atenderla.

   ![Captura de pantalla que muestra la sección Campos de respuesta en el editor de contenido de correo electrónico.](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. Defina la **[!UICONTROL Línea de asunto]** del correo electrónico. Escriba el asunto directamente en el campo dedicado o abra el Editor de expresiones para agregar [personalización](../personalization/personalize.md) mediante varios atributos, fragmentos de expresiones u ofertas.

1. Si desea adjuntar un archivo al correo electrónico, haga clic en el botón **[!UICONTROL Agregar archivo adjunto]** y, a continuación, seleccione uno o varios archivos.

   >[!NOTE]
   >
   >Para evitar problemas de rendimiento, se recomienda no incluir más de un archivo adjunto por correo electrónico.

   <!--limitation on size + number of files?-->

1. Si desea enviar ofertas con su correo electrónico, selecciónelas con el botón **[!UICONTROL Configurar ofertas]**.

   A continuación, puede insertarlos en el correo electrónico mediante campos de personalización. [Aprenda a enviar ofertas](../msg/offers.md)

1. Haga clic en el botón **[!UICONTROL Editar cuerpo del correo electrónico]** para estructurar y diseñar el contenido del correo electrónico con [Email Designer](get-started-email-designer.md#start-authoring). Encontrará información adicional sobre cómo diseñar contenido de correo electrónico en estas secciones:

   * [Crear correos electrónicos desde cero](create-email-content.md)
   * [Estilos del contenido](get-started-email-style.md)

   >[!NOTE]
   >
   >También puede pasar el ratón sobre la vista previa del correo electrónico y seleccionar **[!UICONTROL Abrir diseñador de correo electrónico]**.

1. De forma predeterminada, el seguimiento está habilitado para el envío. Puede desactivar esta opción desde **[!UICONTROL Funciones opcionales]**. [Aprenda a agregar vínculos y administrar el seguimiento](message-tracking.md).

1. Una vez definido el contenido del correo electrónico, utilice el botón **[!UICONTROL Simular contenido]** para comprobar cómo se muestra antes de enviarlo. [Obtenga información sobre cómo obtener una vista previa y probar tu correo electrónico](../preview-test/preview-test.md).