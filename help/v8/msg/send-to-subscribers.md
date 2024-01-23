---
audience: end-user
title: Envío de mensajes a los suscriptores de un servicio
description: Obtenga información sobre cómo enviar mensajes a los suscriptores de un servicio
badge: label="Disponibilidad limitada"
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: ad8d99ca73bebccae9ee7466bda566cdc465fb26
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Envío de mensajes a los suscriptores de un servicio {#send-to-subscribers}

Puede crear servicios de suscripción en Adobe Campaign y enviar mensajes a sus suscriptores. Obtenga información sobre cómo crear servicios de suscripciones en [esta página](../audience//manage-services.md#create-service).

Para enviar mensajes a los suscriptores, cree una audiencia específica para identificar a los suscriptores y luego cree la entrega como se detalla a continuación.

1. Cree una audiencia. Se crea automáticamente un nuevo flujo de trabajo. [Más información sobre las audiencias](../audience/create-audience.md)

1. Para mejorar la legibilidad, cambie el nombre del flujo de trabajo en la configuración del flujo de trabajo **Etiqueta** field. [Obtenga información sobre cómo configurar los ajustes del flujo de trabajo](../workflows/workflow-settings.md)

1. Abra el **[!UICONTROL Crear audiencia]** actividad y seleccione **[!UICONTROL Crear audiencia]**. [Obtenga información sobre cómo configurar una actividad Generar audiencia](../workflows/activities/build-audience.md)

   ![](assets/service-create-audience.png)

1. En el flujo de creación de audiencias, seleccione las siguientes condiciones personalizadas: **[!UICONTROL Suscripciones]** existen como **[!UICONTROL Servicio]** es igual al servicio que haya definido. En este ejemplo, seleccione su **Newsletter de yoga de Luma**.

   ![](assets/service-audience-subscribers.png)

1. Seleccionar **[!UICONTROL Confirmar]** y haga clic en **[!UICONTROL Inicio]** para ejecutar el flujo de trabajo.

1. Cree una entrega. Los pasos para crear una entrega se detallan en [esta página](../msg/gs-messages.md#create-delivery).
1. Vaya a la configuración de envío y cambie la asignación de destino predeterminada a **Suscripciones (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. En la sección del destinatario principal de la entrega, seleccione la audiencia que ha creado anteriormente.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Cree el contenido del mensaje, pruebe y realice la entrega tal como se detalla en [esta sección](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

Su entrega se realiza únicamente a los suscriptores de dicho servicio.
