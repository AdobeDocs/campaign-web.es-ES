---
audience: end-user
title: Creación de un envío de SMS
description: Aprenda a crear y enviar SMS con la web de Adobe Campaign
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 37%

---

# Creación de una entrega de SMS {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Propiedades de envío de SMS"
>abstract="Las propiedades incluyen los parámetros de envío comunes que le ayudan a nombrar y clasificar su envío. Si el envío se basa en un esquema ampliado, hay disponibles campos de opciones personalizadas específicos."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Definición del público SMS"
>abstract="Puede crear un público nuevo o seleccionar uno existente haciendo clic en el botón **Seleccionar público**. Si es necesario, añada un grupo de control para medir el impacto del envío."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=es" text="Establecer un grupo de control"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Selección de plantilla de SMS"
>abstract="Seleccione una plantilla predefinida para iniciar el envío del SMS. Las plantillas de envío permiten reutilizar fácilmente el contenido y la configuración personalizados en sus campañas y envíos."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=es" text="Uso de plantillas de envíos"

Puede crear una entrega de SMS independiente o crear un SMS en el contexto de un flujo de trabajo de la campaña. Los pasos siguientes explican el procedimiento para un envío de SMS independiente (único). Si está trabajando en el contexto de un flujo de trabajo de campaña, los pasos de creación se explican en [esta sección](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Para crear un nuevo envío de SMS independiente, siga estos pasos:

1. Vaya al menú **[!UICONTROL Envíos]** en el carril izquierdo y haga clic en el botón **[!UICONTROL Crear envío]**.

1. En la sección **[!UICONTROL Canal]**, elija SMS como canal y seleccione una plantilla. [Más información sobre las plantillas](../msg/delivery-template.md)

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.

   ![Captura de pantalla que muestra el botón Crear envío y la selección del canal SMS](assets/sms_create_1.png){zoomable="yes"}

1. Escriba una **[!UICONTROL Etiqueta]** para la entrega y acceda a la lista desplegable de **[!UICONTROL Opciones adicionales]**. Si su entrega utiliza un esquema ampliado, hay **campos de opciones personalizadas** específicos disponibles.

   +++Configure las siguientes opciones según sus necesidades.
   * **[!UICONTROL Nombre interno]**: asignar un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene el envío en una carpeta específica.
   * **[!UICONTROL Código de envío]**: organice los envíos con su propia convención de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para el envío.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza de la entrega con fines de clasificación.
   +++

1. Haga clic en el botón **[!UICONTROL Seleccionar público]** para dirigirse a un público destinatario existente o crear el suyo propio. [Más información sobre las audiencias](../audience/about-recipients.md).

   ![Captura de pantalla que muestra el botón Seleccionar audiencia](assets/sms_create_2.png){zoomable="yes"}

   Aprenda a seleccionar una audiencia existente en [esta página](../audience/add-audience.md).

   Aprenda a crear una audiencia nueva en [esta página](../audience/one-time-audience.md).

1. Active la opción **[!UICONTROL Habilitar grupo de control]** para establecer un grupo de control y medir el impacto de su envío. Los mensajes no se envían a ese grupo de control, por lo que puede comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo recibieron. [Más información](../audience/control-group.md)

1. Puede configurar su envío de SMS como un envío multilingüe para enviar mensajes en función del idioma preferido de un perfil. [Más información](../msg/multilingual.md).

1. Haz clic en **[!UICONTROL Editar contenido]** para empezar a diseñar el contenido de tu mensaje SMS. [Más información](content-sms.md)

   ![Captura de pantalla que muestra el botón Editar contenido](assets/sms_create_4.png){zoomable="yes"}

   Desde esta pantalla, también puedes [simular tu contenido](../preview-test/preview-test.md) y [configurar ofertas](../msg/offers.md).

1. Para programar su envío a una fecha y hora específicas, active la opción **[!UICONTROL Habilitar programación]**. Después de iniciar la entrega, el mensaje se envía automáticamente en la fecha y hora exactas que defina para el destinatario. Obtenga más información acerca de la programación de entregas en [esta sección](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Cuando se realice una entrega en el contexto de un flujo de trabajo, use la actividad **Planificador**. Obtenga más información en [esta página](../workflows/activities/scheduler.md).

1. Haga clic en **[!UICONTROL Configuración]** para acceder a las opciones avanzadas relacionadas con la plantilla de envíos. [Más información](../advanced-settings/delivery-settings.md)

   ![Captura de pantalla que muestra el botón de configuración](assets/sms_create_3.png){zoomable="yes"}