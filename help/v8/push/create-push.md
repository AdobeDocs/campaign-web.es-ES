---
audience: end-user
title: Creación de un envío de notificación push
description: Obtenga información sobre cómo crear una entrega de notificaciones push con Adobe Campaign Web
badge: label="Disponibilidad limitada"
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 5ad8e402c330b192b00b8be36cb3e29403666c9e
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 16%

---

# Creación de un envío de notificación push {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Plantilla de notificaciones push"
>abstract="Seleccione una plantilla de notificación push para iniciar la entrega push. Las plantillas de envío permiten reutilizar fácilmente el contenido y la configuración personalizados en sus campañas y envíos."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="Uso de plantillas de envío"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Propiedades del envío push"
>abstract="Defina las propiedades de la entrega push. Introduzca la etiqueta de la notificación push y utilice el **Opciones adicionales** para configurar el nombre interno, la carpeta de entrega y el código. También puede escribir una descripción personalizada."

Puede crear una entrega de notificaciones push independiente o crear una notificación push en el contexto de un flujo de trabajo de la campaña. Los pasos siguientes detallan el procedimiento para una entrega push independiente (de una sola toma). Si está trabajando en el contexto de un flujo de trabajo de campaña, los pasos de creación se detallan en [esta sección](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Creación de una entrega push {#create-push-delivery}

Para crear un nuevo envío push independiente, siga estos pasos:

1. Vaya a la **[!UICONTROL Envíos]** en el carril izquierdo y haga clic en el botón  **[!UICONTROL Creación de envíos]** botón.

1. En el **[!UICONTROL Canal]** , elija **Notificación push** como canal y seleccione una plantilla, según el sistema operativo del dispositivo elegido: Android o iOS. [Más información sobre las plantillas](../msg/delivery-template.md)

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.

   ![](assets/push_create_1.png)

## Configuración de la entrega {#configure-push-settings}

Configure las entregas como se detalla a continuación:

1. Introduzca una **[!UICONTROL Etiqueta]** para la entrega. De forma predeterminada, la etiqueta se establece con la etiqueta de la plantilla seleccionada. Se debe actualizar.

1. Examine la **[!UICONTROL Opciones adicionales]** desplegable para personalizar las opciones, si es necesario. Si la entrega se basa en un esquema ampliado, especifique **Opciones personalizadas** Los campos de están disponibles.

   +++Configure la siguiente configuración según sus necesidades.
   * **[!UICONTROL Nombre interno]**: asignar un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene el envío en una carpeta específica.
   * **[!UICONTROL Código de envío]**: organice los envíos con su propia convención de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para el envío.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza del correo electrónico con fines de clasificación.
+++


## Seleccione la audiencia de envío push {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definición de la audiencia de notificaciones push"
>abstract="Para definir la audiencia del mensaje, primero debe seleccionar la aplicación asociada a la entrega push. De forma predeterminada, la notificación push se envía a todos los suscriptores de la aplicación. Puede ajustar a una audiencia específica haciendo clic en **Seleccionar audiencia** botón. Si es necesario, agregue un grupo de control para medir el impacto del envío."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=es" text="Establecer un grupo de control"


Primero debe seleccionar la aplicación y, a continuación, puede refinar la audiencia de notificaciones push como se detalla a continuación:

1. Desde el **[!UICONTROL Audiencia]** , seleccione la aplicación que desee utilizar para este envío. De forma predeterminada, la notificación push se envía a todos los suscriptores de la aplicación. Puede ajustar a una audiencia específica haciendo clic en **[!UICONTROL Seleccionar audiencia]** botón.

   ![](assets/push_create_2.png)

1. Seleccione una audiencia existente o cree su propia audiencia con el fin de restringir la población objetivo para la entrega push. Para las notificaciones push, la opción predeterminada [dimensión objetivo](../audience/about-recipients.md#targeting-dimensions) es **Aplicación de suscriptor** (nms:appSubscriptionRcp), que está vinculado a la tabla de destinatarios.

   Obtenga información sobre cómo seleccionar una audiencia existente en [esta página](../audience/add-audience.md)

   Obtenga información sobre cómo crear una nueva audiencia en [esta página](../audience/one-time-audience.md)

1. Encienda el **[!UICONTROL Habilitar grupo de control]** opción para establecer un grupo de control para medir el impacto del envío. Los mensajes no se envían a ese grupo de control, por lo que puede comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. [Más información](../audience/control-group.md)

## Definición del contenido de las notificaciones push {#create-content-push}

Para definir el contenido de la notificación, haga clic en **[!UICONTROL Editar contenido]**. [Más información](content-push.md)

![](assets/push_create_5.png)

Desde esta pantalla, también puede [simular el contenido](../preview-test/preview-test.md) y [configuración de ofertas](../msg/offers.md).

## Programe los envíos de entregas {#schedule-push}

Para programar su envío a una fecha y hora específicas, active la opción **[!UICONTROL Habilitar programación]**. Después de iniciar la entrega, el mensaje se envía automáticamente en la fecha y hora exactas definidas para el destinatario. Obtenga más información sobre la programación de entregas en [esta sección](../msg/gs-messages.md#gs-schedule)

![](assets/push_create_3.png)


## Configuración avanzada del envío {#adv-push}

Clic **[!UICONTROL Configuración de la entrega]** para acceder a las opciones avanzadas relacionadas con la plantilla de envíos. [Más información](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png)
