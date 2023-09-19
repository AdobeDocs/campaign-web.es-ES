---
audience: end-user
title: Creación de un envío de SMS
description: Aprenda a crear y enviar SMS con la web de Adobe Campaign
badge: label="Beta"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: 8139ec2f1e94bebacd89ea64af88d0b0babb8781
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 72%

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

Puede crear una entrega de SMS independiente o crear un SMS en el contexto de un flujo de trabajo de la campaña. Los pasos siguientes detallan el procedimiento para un envío de SMS independiente (único). Si está trabajando en el contexto de un flujo de trabajo de campaña, los pasos de creación se detallan en [esta sección](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


Para crear un nuevo envío de SMS independiente, siga estos pasos:

1. Vaya a la **[!UICONTROL Envíos]** en el carril izquierdo y haga clic en el botón  **[!UICONTROL Creación de envíos]** botón.

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

1. Haga clic en el botón **[!UICONTROL Seleccionar audiencia]** para dirigirse a un público destinatario existente o crear el suyo propio. [Más información](../audience/about-recipients.md).

   ![](assets/sms_create_2.png)

1. Encienda la opción del grupo **[!UICONTROL Habilitar control]** para establecer un grupo de control que mida el impacto de su envío, lo que le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. [Más información](../audience/control-group.md)

1. Haga clic en **[!UICONTROL Editar contenido]** para empezar a diseñar el contenido del mensaje SMS. [Más información](content-sms.md)

   ![](assets/sms_create_4.png)

   Desde esta pantalla, también puede [simular el contenido](../preview-test/preview-test.md) y [configuración de ofertas](../content/offers.md).

1. Para programar su envío a una fecha y hora específicas, active la opción **[!UICONTROL Habilitar programación]**. Después de iniciar el envío, el mensaje se envía automáticamente en la fecha y hora exactas definidas para el destinatario. Obtenga más información sobre la programación de entregas en [esta sección](../msg/gs-messages.md#gs-schedule).

1. Clic **[!UICONTROL Configuración de la entrega]** para acceder a las opciones avanzadas relacionadas con la plantilla de envíos. [Más información](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
