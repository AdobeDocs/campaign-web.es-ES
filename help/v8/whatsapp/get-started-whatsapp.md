---
audience: end-user
title: Introducción a los mensajes de WhatsApp
description: Aprenda a crear y enviar mensajes de WhatsApp con la interfaz de usuario web de Adobe Campaign
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
source-git-commit: f0c22710efcda2f59f75ea26cf239d549ff34f96
workflow-type: tm+mt
source-wordcount: '210'
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
* [Token de autorización de usuario con los permisos apropiados](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [Plantillas de Meta aprobadas](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

También debe reconocer lo siguiente antes de continuar:

* [Reglas de contenido de WhatsApp](https://www.whatsapp.com/legal/messaging-guidelines)
* [Cumplimiento de las directivas de Meta](https://www.whatsapp.com/legal)
* [Límites para las conversaciones de 24 horas](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


