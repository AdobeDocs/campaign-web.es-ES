---
audience: end-user
title: Acerca de la cuarentena
description: Comprensión de la administración de direcciones en cuarentena
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: 3e99bf1453ef38ec915dc82828f44c7d7ffb2acd
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 13%

---

# Administración de cuarentena {#quarantines}

Adobe Campaign administra las direcciones en cuarentena de los canales de correo electrónico, push y SMS.

La cuarentena solo se aplica a una **dirección de correo electrónico**, un **número de teléfono** o un **token de dispositivo**, pero no al propio perfil. Del mismo modo, un perfil cuya dirección de correo electrónico se haya puesto en cuarentena puede actualizar su perfil e introducir una nueva, y luego puede volver a recibir entregas. Del mismo modo, si dos perfiles tienen el mismo número de teléfono, ambos se verán afectados si el número está en cuarentena.

>[!CAUTION]
>
>La cuarentena en Adobe Campaign distingue entre mayúsculas y minúsculas.

## Qué es la cuarentena {#quarantines-what}

La cuarentena es la forma de **administrar las direcciones no válidas en las entregas**.

Si una entrega tiene una alta tasa de direcciones no válidas, puede considerarse como correo no deseado. Incluir en la lista de bloqueados Al administrar esas direcciones con cuarentena, se evitará que los proveedores de Internet le. Esto es importante para su reputación.

Cuando una dirección se pone en cuarentena en Adobe Campaign, el perfil se excluye automáticamente del destinatario durante el análisis de la entrega.

La cuarentena le ayudará a reducir el coste de envío de SMS mediante la exclusión de los números de teléfono incorrectos de las entregas.

Obtenga más información acerca de las cuarentenas en la [documentación de Campaign v8 (consola)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"}.


## Por qué se envía una dirección a cuarentena {#quarantines-why}

Muchas razones pueden enviar una dirección a la cuarentena:

* Para SMS, números de teléfono erróneos
* En el caso de los SMS, cuando el perfil responde a un mensaje SMS con una palabra clave como &quot;STOP&quot;
* En el caso del correo electrónico, cuando el mensaje se clasifica como correo no deseado. El mensaje se redirige automáticamente a un buzón de correo técnico administrado por el Adobe. Incluir en la lista de bloqueados A continuación, la dirección de correo electrónico del usuario se envía automáticamente a la cuarentena con el estado.
* Una dirección de correo electrónico se puede poner en cuarentena, por ejemplo, cuando el buzón está lleno, si la dirección no existe o si el servidor de correo electrónico no está disponible.

Obtenga más información acerca de los errores de entrega en la [documentación de Campaign v8 (consola)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"}.

## Dónde encontrar las direcciones en cuarentena {#quarantines-where}

Puede ver todas las direcciones en cuarentena de su instancia en **[!UICONTROL Explorador]** > **[!UICONTROL Administración]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Administración de no entregables]** > **[!UICONTROL No entregables y direcciones]**. Esta sección enumera los elementos en cuarentena para los canales de correo electrónico, SMS y notificaciones push.

![](assets/quarantine_location.png){zoomable="yes"}

También puede tener el informe sobre la cuarentena en su instancia:

![](assets/quarantine_reports.png){zoomable="yes"}

Para cada entrega, también puede comprobar el Delivery summary report: muestra la cantidad de direcciones en cuarentena en el destino de la entrega

![](assets/quarantine_delivery.png){zoomable="yes"}

Puede tener más posibilidades para administrar las direcciones en cuarentena en la consola de Adobe Campaign. [Más información](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)
