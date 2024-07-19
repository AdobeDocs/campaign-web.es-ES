---
audience: end-user
title: Crear un envío de correo directo
description: Obtenga información sobre cómo crear una entrega de correo directo con Adobe Campaign Web
exl-id: 9b5172b2-1880-4768-a33b-8a20ec5a30ab
source-git-commit: 35de060a73c17b304d63000656ff86bb4a80ab15
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 26%

---

# Crear un envío de correo directo {#create-direct-mail}

Puede crear una entrega de correo postal independiente o crear una entrega de correo directo en el contexto de un flujo de trabajo de la campaña. Los pasos siguientes detallan el procedimiento para un envío de correo postal independiente (único). Si está trabajando en el contexto de un flujo de trabajo de campaña, los pasos de creación se detallan en [esta sección](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Para crear un nuevo envío de correo postal independiente, siga estos pasos:

1. Vaya al menú **[!UICONTROL Envíos]** en el carril izquierdo y haga clic en el botón **[!UICONTROL Crear envío]**.

1. En la sección **[!UICONTROL Canal]**, elija **[!UICONTROL Correo directo]** como canal y seleccione una plantilla. [Más información sobre las plantillas](../msg/delivery-template.md)

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.

   ![](assets/dm-create.png){zoomable="yes"}

1. Escriba una **[!UICONTROL Etiqueta]** para la entrega y acceda a la lista desplegable de **[!UICONTROL Opciones adicionales]**. Si su entrega se basa en un esquema ampliado, hay **campos de opciones personalizadas** específicos disponibles.

   ![](assets/dm-properties.png){zoomable="yes"}

   +++Configure la siguiente configuración según sus necesidades.
   * **[!UICONTROL Nombre interno]**: asignar un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene el envío en una carpeta específica.
   * **[!UICONTROL Código de envío]**: organice los envíos con su propia convención de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para el envío.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza de la entrega con fines de clasificación.
+++

1. Haga clic en el botón **[!UICONTROL Seleccionar audiencia]** para segmentar una audiencia existente o crear la suya propia.

   * [Obtenga información sobre cómo seleccionar una audiencia existente](../audience/add-audience.md)
   * [Obtenga información sobre cómo crear una audiencia nueva](../audience/one-time-audience.md)

   ![](assets/dm-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >Los destinatarios del correo postal deben contener al menos sus nombres y direcciones postales. Se considera que una dirección está completa si el nombre, el campo de código postal y el campo de municipio o ciudad no están vacíos. Los destinatarios con direcciones incompletas se excluirán de los envíos de correo directo.

1. Active la opción **[!UICONTROL Habilitar grupo de control]** para establecer un grupo de control y medir el impacto de su envío. Los mensajes no se envían a ese grupo de control, por lo que puede comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo recibieron. [Aprenda a trabajar con grupos de control](../audience/control-group.md)

1. Haga clic en **[!UICONTROL Editar contenido]** para definir la información (columnas) que se exportarán al archivo de extracción. [Más información](content-direct-mail.md)

   ![](assets/dm-content.png){zoomable="yes"}

1. Para programar su envío a una fecha y hora específicas, active la opción **[!UICONTROL Habilitar programación]**. Después de iniciar la entrega, el archivo de extracción se generará automáticamente en la fecha y hora exactas que haya definido. [Aprenda a programar envíos](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Cuando se realiza una entrega en el contexto de un flujo de trabajo, se debe utilizar la actividad **Planificador**. Obtenga más información en [esta página](../workflows/activities/scheduler.md).

1. Haga clic en **[!UICONTROL Configuración]** para acceder a las opciones avanzadas relacionadas con la plantilla de envíos. [Más información](../advanced-settings/delivery-settings.md)

   ![](assets/dm-settings.png){zoomable="yes"}

1. Una vez que tu entrega de correo postal esté lista, haz clic en el botón **[!UICONTROL Revisar y enviar]** para validar y realizar la entrega y generar el archivo de extracción. [Obtenga información sobre cómo obtener una vista previa y enviar una entrega de correo directo](send-direct-mail.md)
