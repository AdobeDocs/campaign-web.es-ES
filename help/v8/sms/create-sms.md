---
audience: end-user
title: Creación de un envío de SMS
description: Aprenda a crear y enviar SMS con la web de Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: b18fb70aa498e3592f88f698bb6b526c9fb1439b
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 95%

---

# Creación de un envío SMS {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Propiedades de envío de SMS"
>abstract="Las propiedades engloban los parámetros de envío comunes que le ayudan a nombrar y clasificar el envío. Si el envío se basa en un esquema ampliado, hay disponibles campos de opciones personalizadas específicos."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Definición de la audiencia SMS"
>abstract="Seleccione la mejor audiencia para su mensaje de SMS."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Selección de plantilla de SMS"
>abstract="Seleccione una plantilla predefinida para iniciar el envío de SMS."

1. Desde la página de inicio **[!UICONTROL Envíos]**, haga clic en **[!UICONTROL Creación de envíos]**.

1. En la sección **[!UICONTROL Canal]**, elija SMS como el canal y seleccione una plantilla. [Más información sobre las plantillas](../msg/delivery-template.md)

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.

   ![](assets/sms_create_1.png)

1. Introduzca una **[!UICONTROL Etiqueta]** para el envío y acceda al menú desplegable **[!UICONTROL Opciones adicionales]**.

   +++Configure la siguiente configuración según sus necesidades.
   * **[!UICONTROL Nombre interno]**: asignar un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene el envío en una carpeta específica.
   * **[!UICONTROL Código de envío]**: organice los envíos con su propia convención de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para el envío.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza del correo electrónico con fines de clasificación.
+++

1. Haga clic en el botón **[!UICONTROL Seleccionar audiencia]** para dirigirse a un público destinatario existente o crear el suyo propio. [Más información](../audience/about-audiences.md).

   ![](assets/sms_create_2.png)

1. Encienda la opción del grupo **[!UICONTROL Habilitar control]** para establecer un grupo de control que mida el impacto de su envío, lo que le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. [Más información](../audience/control-group.md)

1. Haga clic en **[!UICONTROL Editar contenido]** para empezar a diseñar el contenido del mensaje SMS.

1. Para programar su envío a una fecha y hora específicas, active la opción **[!UICONTROL Habilitar programación]**. Después de iniciar el envío, el mensaje se envía automáticamente en la fecha y hora exactas definidas para el destinatario.

1. Clic **[!UICONTROL Configuración de la entrega]** para acceder a las opciones avanzadas relacionadas con la plantilla de envíos. [Más información](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
