---
audience: end-user
title: Alertas de envío
description: Aprenda a trabajar con las alertas de entrega.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 9%

---

# Introducción a las alertas de envío {#gs-delivery-alerting}


Las alertas de envío son un sistema de administración de alertas que permite a grupos de usuarios recibir automáticamente notificaciones por correo electrónico con información sobre la ejecución de sus envíos. Los destinatarios pueden monitorizar los envíos en curso procesados por Adobe Campaign y tomar las medidas adecuadas si surgen problemas.

Las notificaciones se pueden personalizar según criterios de alerta específicos definidos a través de la interfaz de usuario web de Adobe Campaign.

Para obtener más información sobre cómo administrar los errores de entrega, consulte la [documentación de Adobe Campaign v8 (consola)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## Contenido de notificación por correo electrónico {#content}

Las notificaciones por correo electrónico incluyen las siguientes secciones:

* **Resumen**: muestra el número de envíos que cumplen los criterios definidos, con etiquetas y colores para cada criterio.
* **Detalles**: enumera todos los criterios de entrega definidos para el panel y los envíos correspondientes para cada criterio.

![](assets/alerting-email.png)

## Configuración de alertas de envío {#set-up}

Para ayudarle a configurar estas alertas, la interfaz de usuario web de Campaign le permite crear y administrar:

* **Paneles de alertas de entrega**: especifique destinatarios, establezca criterios de alerta para incluirlos en el panel y acceda a un historial de alertas enviadas. [Aprenda a trabajar con paneles](../msg/delivery-alerting-dashboards.md)
* **Criterios de alerta de entrega**: la interfaz de usuario web de Campaign proporciona criterios de alerta predefinidos (entregas con bajo rendimiento, entregas cuya preparación ha fallado...) que puede añadir a su panel. También puede crear sus propios criterios para adaptarlos a sus necesidades. [Aprenda a trabajar con criterios](../msg/delivery-alerting-criteria.md)

Supongamos que desea notificar a los usuarios con derechos de administración solo sobre los envíos fallidos y a los usuarios de marketing sobre los envíos con una proporción de errores de devoluciones en blanco alta. Para conseguirlo, cree dos paneles independientes con los criterios adecuados para cada grupo de destinatarios.

>[!NOTE]
>
>Para acceder y configurar paneles y criterios de alerta, debe tener **derechos de administración** o formar parte del grupo de seguridad **Supervisores de entrega**. Los usuarios estándar no pueden acceder a los paneles de la interfaz de Adobe Campaign, pero pueden recibir notificaciones de alerta. [Más información sobre acceso y permisos](../get-started/permissions.md)
