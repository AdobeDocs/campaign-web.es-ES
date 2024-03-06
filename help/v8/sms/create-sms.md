---
audience: end-user
title: Creación de un envío de SMS
description: Aprenda a crear y enviar SMS con la web de Adobe Campaign
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 933cfcdfb9ff9a176f4942e349b882c404c4e2a8
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 44%

---

# Creación de un envío SMS {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Propiedades de envío de SMS"
>abstract="Las propiedades engloban los parámetros de envío comunes que le ayudan a nombrar y clasificar el envío. Si el envío se basa en un esquema ampliado, hay disponibles campos de opciones personalizadas específicos."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Definición del público SMS"
>abstract="Puede crear un público nuevo o seleccionar uno existente haciendo clic en el botón **Seleccionar público**. Si es necesario, añada un grupo de control para medir el impacto del envío."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=es" text="Establecer un grupo de control"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Selección de plantilla de SMS"
>abstract="Seleccione una plantilla predefinida para iniciar el envío del SMS. Las plantillas de envío permiten reutilizar fácilmente el contenido y la configuración personalizados en sus campañas y envíos."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=es" text="Uso de plantillas de envío"


Puede crear una entrega de SMS independiente o crear un SMS en el contexto de un flujo de trabajo de la campaña. Los pasos siguientes detallan el procedimiento para un envío de SMS independiente (único). Si está trabajando en el contexto de un flujo de trabajo de campaña, los pasos de creación se detallan en [esta sección](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


Para crear un nuevo envío de SMS independiente, siga estos pasos:

1. Vaya a la **[!UICONTROL Envíos]** en el carril izquierdo y haga clic en el botón  **[!UICONTROL Creación de envíos]** botón.

1. En el **[!UICONTROL Canal]** , elija SMS como canal y seleccione una plantilla. [Más información sobre las plantillas](../msg/delivery-template.md)

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.

   ![](assets/sms_create_1.png){zoomable=&quot;yes&quot;}

1. Introduzca una **[!UICONTROL Etiqueta]** para la entrega y acceda al **[!UICONTROL Opciones adicionales]** menú desplegable. Si la entrega se basa en un esquema ampliado, especifique **Opciones personalizadas** Los campos de están disponibles.

   +++Configure la siguiente configuración según sus necesidades.
   * **[!UICONTROL Nombre interno]**: asignar un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene el envío en una carpeta específica.
   * **[!UICONTROL Código de envío]**: organice los envíos con su propia convención de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para el envío.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza de la entrega con fines de clasificación.
+++

1. Haga clic en el botón **[!UICONTROL Seleccionar público]** para dirigirse a un público destinatario existente o crear el suyo propio. [Más información sobre las audiencias](../audience/about-recipients.md).

   ![](assets/sms_create_2.png){zoomable=&quot;yes&quot;}

   Obtenga información sobre cómo seleccionar una audiencia existente en [esta página](../audience/add-audience.md)

   Obtenga información sobre cómo crear una nueva audiencia en [esta página](../audience/one-time-audience.md)

1. Encienda el **[!UICONTROL Habilitar grupo de control]** opción para establecer un grupo de control para medir el impacto del envío. Los mensajes no se envían a ese grupo de control, por lo que puede comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. [Más información](../audience/control-group.md)

1. Clic **[!UICONTROL Editar contenido]** para empezar a diseñar el contenido del mensaje SMS. [Más información](content-sms.md)

   ![](assets/sms_create_4.png){zoomable=&quot;yes&quot;}

   Desde esta pantalla, también puede [simular el contenido](../preview-test/preview-test.md) y [configuración de ofertas](../msg/offers.md).

1. Para programar su envío a una fecha y hora específicas, active la opción **[!UICONTROL Habilitar programación]**. Después de iniciar la entrega, el mensaje se envía automáticamente en la fecha y hora exactas definidas para el destinatario. Obtenga más información sobre la programación de entregas en [esta sección](../msg/gs-messages.md#gs-schedule).

   >[!NOTE]
   >
   >Cuando se realiza una entrega en el contexto de un flujo de trabajo, se debe utilizar el **Planificador** actividad. Obtenga más información en [esta página](../workflows/activities/scheduler.md).

1. Clic **[!UICONTROL Configuración]** para acceder a las opciones avanzadas relacionadas con la plantilla de envíos. [Más información](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png){zoomable=&quot;yes&quot;}
