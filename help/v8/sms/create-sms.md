---
audience: end-user
title: Creación de un envío de SMS
description: Aprenda a crear y enviar SMS con la web de Adobe Campaign
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 29%

---

# Creación de un envío SMS {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Propiedades de envío de SMS"
>abstract="Las propiedades incluyen los parámetros de envío comunes que le ayudarán a nombrar y clasificar su envío. Si el envío utiliza un esquema ampliado, hay disponibles campos específicos de Opciones personalizadas."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Definición del público SMS"
>abstract="Crear una nueva audiencia o seleccione una existente haciendo clic en el **botón Seleccionar audiencia** . Si es necesario, añada un grupo de control para medir el impacto del envío."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=es" text="Establecer un grupo de control"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Selección de plantilla de SMS"
>abstract="Seleccione una plantilla predefinida para iniciar el envío del SMS. Las plantillas de envío permiten reutilizar contenido y configuraciones personalizadas en las campañas y envíos."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=es" text="Uso de plantillas de envío"

Puede crear una entrega de SMS independiente o crear un SMS en el contexto de un flujo de trabajo de la campaña. Los pasos siguientes explican el procedimiento para un envío de SMS independiente (único). Si está trabajando en el contexto de un flujo de trabajo de campaña, los pasos de creación se explican en [esta sección](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Para crear un nuevo envío SMS independiente, seguir estos pasos:

1. Examinar al **[!UICONTROL menú Entregas]** en el carril izquierdo y haga clic en la **[!UICONTROL Crear envío]** botón.

1. En la **[!UICONTROL sección Canal]** , elija SMS como canal y seleccione una plantilla. [Más información sobre las plantillas](../msg/delivery-template.md)

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.

   ![Captura de pantalla que muestra la selección de canal de botón y SMS envío Crear](assets/sms_create_1.png){zoomable="yes"}

1. Ingrese una **[!UICONTROL Etiquetar]** para el envío y acceda al **[!UICONTROL menú desplegable Opciones adicionales]** . Si el envío utiliza un esquema ampliado, están disponibles campos específicos **de Opciones** personalizadas.

   +++Configure la siguiente configuración según sus necesidades.
   * **[!UICONTROL Nombre interno]**: asignar un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene el envío en una carpeta específica.
   * **[!UICONTROL Código de envío]**: organice los envíos con su propia convención de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para el envío.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza del envío a efectos clasificación.

   +++

1. Haga clic en el botón **[!UICONTROL Seleccionar público]** para dirigirse a un público destinatario existente o crear el suyo propio. [Obtenga más información sobre las audiencias](../audience/about-recipients.md).

   ![Captura de pantalla que muestra el botón Select audiencia](assets/sms_create_2.png){zoomable="yes"}

   Aprenda a seleccionar un audiencia existente en [este Página](../audience/add-audience.md).

   Aprenda a crear una nueva audiencia en [este Página](../audience/one-time-audience.md).

1. Active la **[!UICONTROL opción Habilitar grupo de control]** para establecer un grupo de control que medir el impacto de su envío. Los mensajes no se envían a esa grupo de control, por lo que puede comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. [Más información](../audience/control-group.md)

1. Haz clic en **[!UICONTROL Editar contenido]** para empezar a diseñar el contenido de tu mensaje SMS. [Más información](content-sms.md)

   ![Captura de pantalla que muestra el botón de contenido de Editar](assets/sms_create_4.png){zoomable="yes"}

   Desde esta pantalla también [puede simular sus contenido](../preview-test/preview-test.md) y [configurar ofertas](../msg/offers.md).

1. Para programar su envío a una fecha y hora específicas, active la opción **[!UICONTROL Habilitar programación]**. Después de iniciar el envío, el mensaje se envía automáticamente en la fecha y hora exactas que defina para el destinatario. Obtenga más información sobre envío programación en [esta sección](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Cuando se envíe una envío en el contexto de una flujo de trabajo, utilice la actividad del **programador** . Obtenga más información en [esta página](../workflows/activities/scheduler.md).

1. Haga clic en **[!UICONTROL Configuración]** para acceder a las opciones avanzadas relacionadas con su plantilla de envíos. [Más información](../advanced-settings/delivery-settings.md)

   ![Captura de pantalla que muestra el botón Configuración](assets/sms_create_3.png){zoomable="yes"}