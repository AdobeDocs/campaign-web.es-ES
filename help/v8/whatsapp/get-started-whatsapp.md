---
audience: end-user
title: Introducción a los mensajes de WhatsApp
description: Aprenda a crear y enviar mensajes de WhatsApp con la interfaz de usuario web de Adobe Campaign
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%
---
# Introducción a los mensajes de WhatsApp {#get-started-whatsapp}

Puede enviar mensajes de WhatsApp desde la **interfaz de usuario web de Adobe Campaign** mediante la [API en la nube](https://developers.facebook.com/docs/whatsapp/cloud-api/) de Meta. Utiliza WhatsApp en envíos independientes, en flujos de trabajo de campañas o dentro de campañas de marketing, junto con tus otros canales.

* **[!UICONTROL Envíos]**: en la interfaz de usuario web de Adobe Campaign, cree un envío independiente de WhatsApp desde el menú de **[!UICONTROL Envíos]** en el carril izquierdo, similar a SMS o push. [Más información](create-whatsapp.md).

* **[!UICONTROL Campañas]**: en la interfaz de usuario web de Adobe Campaign, abra una campaña y agregue una entrega de WhatsApp desde la pestaña **[!UICONTROL Envíos]**, o bien organice los envíos con un flujo de trabajo adjunto a la campaña. [Más información](../campaigns/create-campaigns.md).

* **[!UICONTROL Flujos de trabajo]**: en el lienzo de flujo de trabajo de la interfaz de usuario web de Adobe Campaign, agregue una actividad de canal **[!UICONTROL WhatsApp]**, elija una plantilla de envío y, a continuación, defina el contenido y la configuración en el panel de envío. Obtenga más información acerca de las actividades de canal en [esta sección](../workflows/activities/channels.md).

## Requisitos previos {#prereq}

La integración de WhatsApp requiere lo siguiente:

* Cuenta de Meta Business Manager
* [Cuenta comercial de WhatsApp con nombre de remitente y número de teléfono verificados](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [Token de autorización de usuario con los permisos adecuados](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [Plantillas de Meta aprobadas](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

También debe reconocer lo siguiente antes de continuar:

* [Reglas de contenido de WhatsApp](https://www.whatsapp.com/legal/messaging-guidelines)
* [Cumplimiento de las políticas de Meta](https://www.whatsapp.com/legal)
* [Límites de conversación de 24 horas](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


