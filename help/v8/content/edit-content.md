---
audience: end-user
title: Edición del contenido de correo electrónico
description: Obtenga información sobre cómo editar el contenido del correo electrónico en la IU de la web de Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
source-git-commit: 666a1c2d4b31fed8e956f0b2984c1f39d74a2221
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 48%

---

# Configuración del contenido del correo electrónico {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Creación de contenido de correo electrónico"
>abstract="En esta sección, puede crear el contenido del correo electrónico y utilizar el diseñador de correo electrónico para darle un aspecto refinado."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Parámetros del correo electrónico"
>abstract="Los valores de nombre de remitente y de correo electrónico de origen se definen en la plantilla de correo electrónico. La línea Subject se puede personalizar mediante el Editor de expresiones."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Archivo adjunto de correo electrónico"
>abstract="Seleccione uno o varios archivos para insertar en el mensaje."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Opciones de seguimiento"
>abstract="De forma predeterminada, el seguimiento está habilitado para el envío. Puede desactivar esta opción desde aquí."

El correo electrónico **[!UICONTROL Editar contenido]** La pantalla de permite:
* Defina los elementos básicos del mensaje, como la dirección del remitente y la línea de asunto
* Realizar acciones adicionales, como agregar archivos adjuntos o configurar ofertas
* Acceda a la [Diseñador de correo electrónico](get-started-email-designer.md) para empezar a crear el contenido adecuado del correo electrónico

Para configurar o editar el contenido de un correo electrónico, siga los pasos a continuación.

1. Haga clic en **[!UICONTROL Editar contenido]** del menú contextual [panel de envío de correo electrónico](../email/create-email.md) pantalla.

   ![](assets/email-edit-content.png)

1. Se abre la pantalla de edición de contenido de correo electrónico. Si está configurando un nuevo correo electrónico, la variable **[!UICONTROL Nombre de remitente]** y **[!UICONTROL Desde correo electrónico]** Los campos de ya se han rellenado.

   ![](assets/email-edit-content-dashboard.png)

1. El **[!UICONTROL Nombre de remitente]** se define en la plantilla de correo electrónico. Si desea modificarlo, utilice un nombre fácilmente identificable por los destinatarios, como el nombre de su marca, para aumentar la velocidad de apertura de sus envíos.

   >[!NOTE]
   >
   >    Para mejorar aún más la experiencia del destinatario, puede agregar el nombre de una persona como, por ejemplo, &quot;Emma de Megastore&quot;.

1. El **[!UICONTROL Desde correo electrónico]** el campo de dirección también se define en la plantilla de correo electrónico. Asegúrese de que el dominio de dirección sea el mismo que el subdominio que delegó en Adobe.

   >[!NOTE]
   >
   >    Puede cambiar la parte que precede a &#39;@&#39;, pero no la dirección de dominio.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Defina la **[!UICONTROL Línea de asunto]** del correo electrónico. Escriba el asunto directamente en el campo dedicado o abra el Editor de expresiones para agregar personalización con varios atributos y bloques de contenido u ofertas. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

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

1. De forma predeterminada, el seguimiento está habilitado para el envío. Puede desactivar esta opción desde **[!UICONTROL Funciones opcionales]**. [Aprenda a añadir vínculos y a administrar el seguimiento](message-tracking.md)

1. Una vez definido el contenido del correo electrónico, utilice el botón **[!UICONTROL Simular contenido]** para comprobar cómo se muestra antes de enviarlo. [Obtenga información sobre cómo previsualizar y probar el correo electrónico](../preview-test/preview-test.md)

