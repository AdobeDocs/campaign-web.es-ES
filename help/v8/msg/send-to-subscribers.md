---
audience: end-user
title: Envío de mensajes a los suscriptores de un servicio
description: Obtenga información sobre cómo enviar mensajes a los suscriptores de un servicio
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Envío de mensajes a los suscriptores de un servicio {#send-to-subscribers}

Puede crear servicios de suscripción en Adobe Campaign y enviar mensajes a sus suscriptores. Aprenda a crear servicios de suscripción en [esta página](../audience//manage-services.md#create-service).

Para enviar mensajes a los suscriptores, cree una audiencia específica para identificar a los suscriptores y luego cree la entrega como se detalla a continuación.

1. Cree una audiencia. Se crea automáticamente un nuevo flujo de trabajo. [Más información sobre las audiencias](../audience/create-audience.md).

1. Para facilitar la lectura, cambie el nombre del flujo de trabajo en el campo **Label** de la configuración del flujo de trabajo. [Aprenda a configurar las opciones del flujo de trabajo](../workflows/workflow-settings.md).

1. Abra la actividad **[!UICONTROL Generar audiencia]** y seleccione **[!UICONTROL Crear audiencia]**. [Aprenda a configurar una actividad Generar audiencia](../workflows/activities/build-audience.md).

   ![Captura de pantalla que muestra la configuración de actividad de audiencia de compilación en Adobe Campaign.](assets/service-create-audience.png){zoomable="yes"}

1. En el flujo de creación de audiencia, seleccione las siguientes condiciones personalizadas: existen **[!UICONTROL Suscripciones]**, como **[!UICONTROL Servicio]** que es igual al servicio que definió. En este ejemplo, selecciona tu **newsletter de yoga de Luma**.

   ![Captura de pantalla que muestra el flujo de creación de audiencias con condiciones personalizadas para suscripciones en Adobe Campaign.](assets/service-audience-subscribers.png){zoomable="yes"}

1. Seleccione **[!UICONTROL Confirmar]** y haga clic en **[!UICONTROL Iniciar]** para ejecutar el flujo de trabajo.

1. Cree una entrega. Los pasos para crear una entrega se detallan en [esta página](../msg/gs-messages.md#create-delivery).

1. Vaya a la configuración de envío y cambie la asignación de destino predeterminada a **Suscripciones (nms:subscriptions)**.

   ![Captura de pantalla que muestra la configuración de envío con la asignación de destino cambió a Suscripciones en Adobe Campaign.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. En la sección del destinatario principal de la entrega, seleccione la audiencia que ha creado anteriormente.

   ![Captura de pantalla que muestra la sección de destino principal del envío con la audiencia seleccionada en Adobe Campaign.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Cree el contenido del mensaje, pruébelo y realice la entrega tal como se detalla en [esta sección](../preview-test/preview-test.md).

   ![Captura de pantalla que muestra el envío listo para enviarse en Adobe Campaign.](assets/service-delivery-ready.png){zoomable="yes"}

Su entrega se realiza únicamente a los suscriptores de dicho servicio.