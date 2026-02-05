---
audience: end-user
title: Creación de un envío de notificación push
description: Obtenga información sobre cómo crear una entrega de notificaciones push con Adobe Campaign Web
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 28%

---

# Creación de un envío de notificación push {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Plantilla de notificaciones push"
>abstract="Seleccione una plantilla de notificación push para iniciar el envío push. Las plantillas de envío permiten reutilizar fácilmente el contenido y la configuración personalizados en sus campañas y envíos."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/start/delivery-template" text="Uso de plantillas de envíos"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Propiedades del envío push"
>abstract="Definición de las propiedades de los envíos push. Introduzca la etiqueta de la notificación push y utilice las **Opciones adicionales** para configurar el nombre interno, la carpeta de envío y el código. También puede escribir una descripción personalizada."

Puede crear una entrega de notificaciones push independiente o crear una notificación push en el contexto de un flujo de trabajo de la campaña. Los pasos siguientes detallan el procedimiento para una entrega push independiente (de una sola toma). Si está trabajando en el contexto de un flujo de trabajo de campaña, los pasos de creación se detallan en [esta sección](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Creación de un envío push {#create-push-delivery}

Para crear un nuevo envío push independiente, siga estos pasos:

1. Vaya al menú **[!UICONTROL Envíos]** en el carril izquierdo y haga clic en el botón **[!UICONTROL Crear envío]**.

1. En la sección **[!UICONTROL Canal]**, elija **Notificación push** como canal y seleccione una plantilla, según el sistema operativo del dispositivo elegido: Android o iOS. [Más información sobre las plantillas](../msg/delivery-template.md)

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.

   ![Captura de pantalla que muestra la creación de una entrega push](assets/push_create_1.png){zoomable="yes"}

## Configuración de la entrega {#configure-push-settings}

Configure las entregas como se detalla a continuación:

1. Escriba una **[!UICONTROL Etiqueta]** para la entrega. De forma predeterminada, la etiqueta se establece con la etiqueta de la plantilla seleccionada. Se debe actualizar.

1. Examine la lista desplegable **[!UICONTROL Opciones adicionales]** para personalizar las opciones, si es necesario. Si su entrega se basa en un esquema ampliado, hay **campos de opciones personalizadas** específicos disponibles.

   +++Configure las siguientes opciones según sus necesidades.
   * **[!UICONTROL Nombre interno]**: asignar un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene el envío en una carpeta específica.
   * **[!UICONTROL Código de envío]**: organice los envíos con su propia convención de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para el envío.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza de la entrega con fines de clasificación.
   +++

1. Puede configurar la notificación push como un envío multilingüe para enviar mensajes en función del idioma preferido de un perfil. [Más información](../msg/multilingual.md).

## Seleccione el público del envío push {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definición del público de la notificación push"
>abstract="Para definir el público del mensaje, primero debe seleccionar la aplicación asociada al envío Push. De forma predeterminada, la notificación push se envía a todos los suscriptores de la aplicación. Puede restringirla a un público específico haciendo clic en el botón **Seleccionar público**. Si es necesario, añada un grupo de control para medir el impacto del envío."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=es" text="Establecer un grupo de control"

Primero debe seleccionar la aplicación y, a continuación, puede refinar la audiencia de notificaciones push como se detalla a continuación:

1. En la sección **[!UICONTROL Audience]**, seleccione la aplicación que desee utilizar para este envío. De forma predeterminada, la notificación push se envía a todos los suscriptores de la aplicación. Puede ajustar la audiencia a una audiencia específica haciendo clic en el botón **[!UICONTROL Seleccionar audiencia]**.

   ![Captura de pantalla que muestra la selección de audiencias para la entrega push](assets/push_create_2.png){zoomable="yes"}

1. Seleccione una audiencia existente o cree su propia audiencia con el fin de restringir la población objetivo para la entrega push. Para las notificaciones push, la [dimensión de destino](../audience/about-recipients.md#targeting-dimensions) predeterminada es **Aplicación de suscriptor** (nms:appSubscriptionRcp), que está vinculada a la tabla de destinatarios.

   Aprenda a seleccionar una audiencia existente en [esta página](../audience/add-audience.md).

   Aprenda a crear una audiencia nueva en [esta página](../audience/one-time-audience.md).

1. Active la opción **[!UICONTROL Habilitar grupo de control]** para establecer un grupo de control y medir el impacto de su envío. Los mensajes no se envían a ese grupo de control, por lo que puede comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo recibieron. [Más información](../audience/control-group.md).

## Definición del contenido de las notificaciones push {#create-content-push}

Para definir el contenido de la notificación, haga clic en **[!UICONTROL Editar contenido]**. [Más información](content-push.md).

![Captura de pantalla que muestra la edición de contenido para la entrega push](assets/push_create_5.png){zoomable="yes"}

Desde esta pantalla, también puedes [simular tu contenido](../preview-test/preview-test.md) y [configurar ofertas](../msg/offers.md).

## Programe los envíos de entregas {#schedule-push}

Cuando se realiza una entrega en el contexto de un flujo de trabajo, se debe utilizar la actividad **Planificador**. Obtenga más información en [esta página](../workflows/activities/scheduler.md). Los pasos siguientes solo se aplican a envíos independientes.

Para programar una entrega push independiente a una fecha y hora específicas, siga estos pasos:

1. Vaya a la sección **[!UICONTROL Programar]** de las propiedades de entrega.

1. Utilice la opción **[!UICONTROL Habilitar programación]** para activarla.

1. Establezca la fecha y la hora deseadas para el envío.

Después de iniciar la entrega, el mensaje se envía automáticamente en la fecha y hora exactas que haya definido para el destinatario.

![Captura de pantalla que muestra las opciones de programación de la entrega push](assets/push_create_3.png){zoomable="yes"}

Obtenga más información acerca de la programación de entregas en [esta sección](../msg/gs-deliveries.md#gs-schedule).

## Configuración avanzada del envío {#adv-push}

Haga clic en **[!UICONTROL Configurar opciones de envío]** para acceder a las opciones avanzadas relacionadas con su plantilla de envíos. [Más información](../advanced-settings/delivery-settings.md).

![Captura de pantalla que muestra la configuración avanzada de la entrega push](assets/push_create_4.png){zoomable="yes"}