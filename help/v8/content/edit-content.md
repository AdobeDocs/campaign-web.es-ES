---
audience: end-user
title: Edición del contenido de correo electrónico
description: Obtenga información sobre cómo editar el contenido del correo electrónico en la IU de la web de Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
source-git-commit: f04e8aa5ecb12fca02da640b0037441d4cd7d4d3
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 73%

---

# Edición del contenido de correo electrónico {#configure-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Creación de contenido de correo electrónico"
>abstract="En esta sección, puede crear el contenido del correo electrónico y utilizar el diseñador de correo electrónico para darle un aspecto refinado."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Parámetros del correo electrónico"
>abstract="Los valores Desde nombrey De correo electrónico se definen en la plantilla de correo electrónico. La línea de asunto se puede personalizar con el editor de expresiones."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Archivo adjunto de correo electrónico"
>abstract="Seleccione uno o varios archivos para insertarlos en el mensaje."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Opciones de seguimiento"
>abstract="De forma predeterminada, el seguimiento está habilitado para el envío. Puede desactivar esta opción desde aquí."

Para empezar a crear el contenido de un correo electrónico, haga clic en el botón **[!UICONTROL Editar contenido]** en la pantalla de creación del correo electrónico.[](../email/create-email.md)

![](assets/email-edit-content.png)

La pantalla que se abre le permite definir detalles básicos, realizar algunas acciones adicionales, como agregar archivos adjuntos o configurar ofertas, y acceder al Diseñador de correo electrónico para crear el contenido.

![](assets/email-edit-content-dashboard.png)

Los pasos para editar el contenido del correo electrónico son los siguientes:

1. En el **[!UICONTROL Nombre de remitente]** , utilice un nombre fácilmente identificable por los destinatarios, como el nombre de su marca, para aumentar la velocidad de apertura de sus envíos.

1. Defina la **[!UICONTROL Línea de asunto]** del correo electrónico. Para ello, escriba el asunto directamente en el campo correspondiente o abra el Editor de expresiones para definir y añadir una personalización mediante varios atributos y bloques de contenido u ofertas. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)
Para mejorar aún más la experiencia del destinatario, puede agregar el nombre de una persona como, por ejemplo, &quot;Emma de Megastore&quot;.

1. En el **[!UICONTROL Desde correo electrónico]** campo de dirección, asegúrese de que el dominio de dirección sea el mismo que el subdominio que delegó en Adobe.

   Puede cambiar la parte que precede a &#39;@&#39;, pero no la dirección de dominio.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Defina la **[!UICONTROL Línea de asunto]** del correo electrónico. Escriba el asunto directamente en el campo dedicado o abra el Editor de expresiones para agregar personalización con varios atributos y bloques de contenido u ofertas. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

1. Si desea adjuntar un archivo al correo electrónico, haga clic en el botón **[!UICONTROL Añadir adjunto]** y a continuación, seleccione uno o varios archivos.

   >[!NOTE]
   >
   >    Para evitar problemas de rendimiento, se recomienda no adjuntar más de un archivo en el correo electrónico.

   <!--limitation on size + number of files?-->

1. Si desea enviar ofertas con su correo electrónico, selecciónelas utilizando el botón **[!UICONTROL Configurar ofertas.]**

   A continuación, puede insertarlos en el correo electrónico mediante campos de personalización. [Aprenda a enviar ofertas](offers.md)

1. Haga clic en el botón **[!UICONTROL Editar cuerpo del correo electrónico]** para estructurar y diseñar el contenido del correo electrónico. En estas secciones encontrará información adicional sobre cómo diseñar el contenido del correo electrónico:

   * [Aprenda a diseñar correos electrónicos](create-email-content.md)
   * [Estilos del contenido](get-started-email-style.md)

1. De forma predeterminada, el seguimiento está habilitado para el envío. Puede desactivar esta opción desde **[!UICONTROL Funciones opcionales]**. [Aprenda a añadir vínculos y a administrar el seguimiento](message-tracking.md)

1. Una vez definido el contenido del correo electrónico, utilice el botón **[!UICONTROL Simular contenido]** para comprobar cómo se muestra antes de enviarlo. [Obtenga información sobre cómo previsualizar y probar el correo electrónico](../preview-test/preview-test.md)
