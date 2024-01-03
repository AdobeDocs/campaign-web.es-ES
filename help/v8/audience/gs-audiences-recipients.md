---
title: Trabajar con destinatarios y públicos
description: Aprenda a trabajar con destinatarios y audiencias en Campaign Web
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 18%

---

# Trabajar con destinatarios y públicos {#about-recipients}

## Destinatarios y audiencias {#about}

En Adobe Campaign, la población objetivo de una entrega es una audiencia. Una audiencia es un conjunto de personas que comparten comportamientos o características similares. Esta colección de personas se puede generar, seleccionar o cargar [como se detalla a continuación](#audiences).

En la mayoría de los casos, la audiencia está formada por perfiles, que se almacenan como [destinatarios](#recipients) en Adobe Campaign. También puede trabajar con otras asignaciones de destino cambiando la dimensión como se explica a continuación [en esta sección](#targeting-dimensions).

## Dimensiones de segmentación {#targeting-dimensions}

La dimensión de segmentación, también conocida como. asignación de destino, es el tipo de datos que administra una operación. Permite definir la población objetivo: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc.

La dimensión de segmentación de un flujo de trabajo se define mediante la primera **[!UICONTROL Crear audiencia]** y se utiliza en todas las demás actividades hasta el final del flujo de trabajo. Por ejemplo, si realiza una consulta en los destinatarios de la base de datos, la transición saliente contendrá datos del tipo destinatario y se transmitirá a la siguiente actividad.

Tenga en cuenta que puede cambiar la dimensión de segmentación en un flujo de trabajo mediante una [Cambiar actividad de dimensión](../workflows/activities/change-dimension.md). Esto le permite, por ejemplo, consultar la base de datos en una tabla específica, como compras o suscripciones, y luego cambiar la dimensión de segmentación a Destinatarios para realizar envíos a los destinatarios correspondientes.

De forma predeterminada, las plantillas de envío de correo electrónico y SMS están segmentadas **[!UICONTROL Destinatarios]**. Por lo tanto, su dimensión de destino utiliza los campos del **nms:destinatario** tabla. Para las notificaciones push, la dimensión de destino predeterminada es **Aplicaciones del suscriptor nms:appSubscriptionRcp**, que está vinculado a la tabla de destinatarios.

También puede utilizar otras asignaciones de destino integradas en los flujos de trabajo y envíos que se enumeran a continuación:

| Nombre | Usar para | Esquema |
|---|---|---|
| Destinatarios | Envío a destinatarios (tabla de destinatarios integrada) | nms:recipient |
| Visitantes | Envío a los visitantes cuyos perfiles se hayan recopilado mediante recomendación (marketing viral) por ejemplo. | mns:visitor |
| Suscripciones | Envío a destinatarios suscritos a un servicio de información como un boletín informativo | nms:subscription |
| Suscripciones de visitantes | Envío a los visitantes que están suscritos a un servicio de información | nms:visitorSub |
| Operadores | Envío a los operadores de Adobe Campaign | nms:operator |
| Archivo externo | Envío a través de un archivo que contiene toda la información necesaria para la entrega | No hay ningún esquema vinculado, no se ha introducido ningún destino |
| Aplicaciones del suscriptor | Envío a destinatarios suscritos a una aplicación | nms:appSubscriptionRcp |

Además, puede crear una nueva asignación de destino según sus necesidades. Esto se realiza desde la consola del cliente. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
