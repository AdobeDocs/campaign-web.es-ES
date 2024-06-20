---
audience: end-user
title: Acerca de la cuarentena
description: Comprensión de la administración de direcciones en cuarentena
source-git-commit: 9abf58c35fcf396e3003f9ecba728cd77df844a1
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 13%

---

# Cuarentena

Adobe Campaign administra las direcciones en cuarentena (correo electrónico, SMS, notificación push).

La cuarentena solo se aplica a un **dirección de email**, a **número de teléfono**, o a **token de dispositivo**, pero no al propio perfil. Del mismo modo, un perfil cuya dirección de correo electrónico se haya puesto en cuarentena puede actualizar su perfil e introducir una nueva, y luego puede volver a recibir entregas. Del mismo modo, si dos perfiles tienen el mismo número de teléfono, ambos se verán afectados si el número está en cuarentena.


>[!CAUTION]
>
>La cuarentena en Adobe Campaign distingue entre mayúsculas y minúsculas.

## ¿Qué es la cuarentena?

La cuarentena es la forma de **administración de direcciones no válidas en envíos**.

Si una entrega tiene una alta tasa de direcciones no válidas, puede considerarse como correo no deseado. Incluir en la lista de bloqueados Al administrar esas direcciones con cuarentena, se evitará que los proveedores de Internet le. Esto es importante para su reputación.

Cuando una dirección se pone en cuarentena en Adobe Campaign, el perfil se excluye automáticamente del destinatario durante el análisis de la entrega.

La cuarentena le ayudará a reducir el coste de envío de SMS mediante la exclusión de los números de teléfono incorrectos de las entregas.

## Por qué se envía una dirección a cuarentena

Muchas razones pueden enviar una dirección a cuarentena:

- Para SMS, números de teléfono erróneos
- En el caso de los SMS, cuando el perfil responde a un mensaje SMS con una palabra clave como &quot;STOP&quot;
- En el caso del correo electrónico, cuando el mensaje se clasifica como correo no deseado. El mensaje se redirige automáticamente a un buzón de correo técnico administrado por el Adobe. Incluir en la lista de bloqueados A continuación, la dirección de correo electrónico del usuario se envía automáticamente a la cuarentena con el estado.
- Una dirección de correo electrónico se puede poner en cuarentena, por ejemplo, cuando el buzón está lleno, si la dirección no existe o si el servidor de correo electrónico no está disponible.

[Más información sobre los errores de entrega](https://experienceleague.adobe.com/en/docs/campaign-classic/using/sending-messages/monitoring-deliveries/understanding-delivery-failures)

## Dónde encontrar las direcciones en cuarentena

Puede ver todas las direcciones en cuarentena de la instancia en **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Gestión de no entregables]** > **[!UICONTROL No entregables y direcciones]**. Esta sección enumera los elementos en cuarentena para los canales de correo electrónico, SMS y notificaciones push.

![](assets/quarantine_location.png){zoomable="yes"}

También puede tener el informe sobre la cuarentena en su instancia:

![](assets/quarantine_reports.png){zoomable="yes"}

Para cada entrega, también puede comprobar el Delivery summary report: muestra la cantidad de direcciones en cuarentena en el destino de la entrega

![](assets/quarantine_delivery.png){zoomable="yes"}

Puede tener más posibilidades para administrar las direcciones en cuarentena en la consola de Adobe Campaign. [Más información](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)
