---
audience: end-user
title: Edición del contenido de correo electrónico
description: Obtenga información sobre cómo editar el contenido del correo electrónico en la IU de la web de Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Beta"
source-git-commit: 26c1322a17e3659301982daadc7eadb45efdd2b0
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 37%

---

# Configurar el contenido de correo electrónico {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Definición del contenido del correo electrónico"
>abstract="El **Editar contenido** La pantalla de le permite definir elementos básicos del mensaje, como la dirección del remitente y la línea de asunto, realizar acciones adicionales como agregar archivos adjuntos u ofertas y acceder al Diseñador de correo electrónico para darle a su mensaje un aspecto pulido."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Definición de las propiedades de correo electrónico"
>abstract="El **Detalles básicos** Esta sección permite actualizar la dirección del remitente y la dirección de respuesta, así como definir la línea de asunto mediante el Editor de expresiones."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Adjuntar archivos al correo electrónico"
>abstract="Seleccione uno o varios archivos para insertar en el mensaje. Para evitar problemas de rendimiento, se recomienda no adjuntar más de un archivo en el correo electrónico."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Editar seguimiento"
>abstract="De forma predeterminada, el seguimiento está habilitado para la entrega, lo que significa que se realiza el seguimiento de todos los vínculos incluidos en el contenido del mensaje. Puede desactivar esta opción desde aquí."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/email/content/design-content/message-tracking.html" text="Adición de vínculos y seguimiento de mensajes"

El correo electrónico **[!UICONTROL Editar contenido]** La pantalla de permite:
* Defina los elementos básicos del mensaje, como la dirección del remitente y la línea de asunto
* Realizar acciones adicionales, como agregar archivos adjuntos o configurar ofertas
* Acceda a la [Diseñador de correo electrónico](get-started-email-designer.md#start-authoring) para empezar a crear el contenido adecuado del correo electrónico

>[!NOTE]
>
>Todos los campos de texto editables de esta pantalla se pueden rellenar con campos de personalización. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

Para configurar o editar el contenido de un correo electrónico, siga los pasos a continuación.

1. Haga clic en **[!UICONTROL Editar contenido]** del menú contextual [panel de envío de correo electrónico](../email/create-email.md) pantalla.

   ![](assets/email-edit-content-button.png)

1. Se abre la pantalla de edición de contenido de correo electrónico.

   ![](assets/email-edit-content-dashboard.png)

   >[!NOTE]
   >
   >Si está configurando un nuevo correo electrónico, la variable **[!UICONTROL Nombre de remitente]** y **[!UICONTROL Desde correo electrónico]** Los campos de ya se han rellenado.

1. El **[!UICONTROL Nombre de remitente]** se define en la plantilla de correo electrónico. Si desea modificarlo, utilice un nombre fácilmente identificable por los destinatarios, como el nombre de su marca, para aumentar la velocidad de apertura de sus envíos.

   >[!NOTE]
   >
   >Para mejorar aún más la experiencia del destinatario, puede agregar el nombre de una persona como, por ejemplo, &quot;Eva de Luma&quot;.

1. El **[!UICONTROL Desde correo electrónico]** el campo de dirección también se define en la plantilla de correo electrónico. Asegúrese de que el dominio de dirección sea el mismo que el subdominio que delegó en Adobe.

   >[!NOTE]
   >
   >Puede cambiar la parte que precede a &#39;@&#39;, pero no la dirección de dominio.

1. Expanda el **[!UICONTROL Campos de respuesta]** sección. El nombre y las direcciones del remitente se utilizan de forma predeterminada para las respuestas. Sin embargo, Adobe recomienda utilizar una dirección real existente, como el servicio de atención al cliente de su marca. En este caso, si un destinatario envía una respuesta, el servicio de atención al cliente podrá atenderla.

   ![](assets/email-edit-content-reply-to.png)

1. Defina la **[!UICONTROL Línea de asunto]** del correo electrónico. Escriba el asunto directamente en el campo dedicado o abra el Editor de expresiones para agregar [personalización](../personalization/personalize.md) uso de varios atributos y bloques de contenido, u ofertas.

1. Si desea adjuntar un archivo al correo electrónico, haga clic en el botón **[!UICONTROL Añadir adjunto]** y a continuación, seleccione uno o varios archivos.

   >[!NOTE]
   >
   >    Para evitar problemas de rendimiento, se recomienda no adjuntar más de un archivo en el correo electrónico.

   <!--limitation on size + number of files?-->

1. Si desea enviar ofertas con su correo electrónico, selecciónelas utilizando el botón **[!UICONTROL Configurar ofertas.]**

   A continuación, puede insertarlos en el correo electrónico mediante campos de personalización. [Aprenda a enviar ofertas](offers.md)

1. Haga clic en **[!UICONTROL Editar cuerpo del correo electrónico]** para estructurar y diseñar el contenido del correo electrónico utilizando [Diseñador de correo electrónico](#start-authoring). En estas secciones encontrará información adicional sobre cómo diseñar el contenido del correo electrónico:

   * [Crear correos electrónicos desde cero](create-email-content.md)
   * [Estilos del contenido](get-started-email-style.md)

   >[!NOTE]
   >
   >También puede pasar el ratón sobre la vista previa del correo electrónico y seleccionar **[!UICONTROL Abrir diseñador de correo electrónico]**.

1. De forma predeterminada, el seguimiento está habilitado para el envío. Puede desactivar esta opción desde **[!UICONTROL Funciones opcionales]**. [Aprenda a añadir vínculos y a administrar el seguimiento](message-tracking.md)

1. Una vez definido el contenido del correo electrónico, utilice el botón **[!UICONTROL Simular contenido]** para comprobar cómo se muestra antes de enviarlo. [Obtenga información sobre cómo previsualizar y probar el correo electrónico](../preview-test/preview-test.md)

