---
audience: end-user
title: Envío de mensajes a los suscriptores de un servicio
description: Obtenga información sobre cómo enviar mensajes a los suscriptores de un servicio
badge: label="Beta"
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: cd7e2bb325b4e571018a8e04ffa0eaef74fe6768
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 2%

---

# Envío de mensajes a los suscriptores de un servicio

Puede crear servicios de suscripción en Adobe Campaign y enviar mensajes a sus suscriptores. Obtenga información sobre cómo crear servicios de suscripciones en [esta página](../audience//manage-services.md#create-service).

Para enviar mensajes a los suscriptores, cree una audiencia específica para identificar a los suscriptores y luego cree la entrega como se detalla a continuación.

1. Cree una audiencia. Obtenga más información sobre las audiencias en [esta página](../audience/create-audience.md).

1. En el **[!UICONTROL Crear audiencia]** actividad, muestre los atributos avanzados y seleccione **[!UICONTROL Destinatario]** > **[!UICONTROL Suscripciones]** > **[!UICONTROL Servicio]**.

   En este ejemplo, seleccione los usuarios suscritos al servicio que tiene el **Newsletter de Luma** etiqueta.

   ![](assets/service-audience-subscribers.png)

1. Guarde la audiencia.
1. Cree una entrega. Los pasos para crear una entrega se detallan en [esta página](../msg/gs-messages.md#create-delivery).
1. Vaya a la configuración de envío y cambie la asignación de destino predeterminada a **Suscripciones (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. En la sección del destinatario principal de la entrega, seleccione la audiencia que ha creado anteriormente.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Cree el contenido del mensaje, pruebe y realice la entrega tal como se detalla en [esta sección](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

Su entrega se realiza únicamente a los suscriptores de dicho servicio.
