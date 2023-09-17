---
audience: end-user
title: Trabajo con servicios de suscripción
description: Obtenga información sobre cómo crear servicios en Adobe Campaign Web
badge: label="Beta"
source-git-commit: dd8e8acb37cf9a68768c5da48335275c09d67cc8
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 4%

---


# Trabajo con servicios de suscripción {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Crear y administrar sus servicios"
>abstract="Utilice Adobe Campaign para crear y supervisar sus servicios, como los boletines informativos, y para comprobar las suscripciones o bajas de suscripción a estos servicios. Las suscripciones solo se aplican al envío de correo electrónico y SMS."

Utilice la web de Adobe Campaign para administrar y crear sus servicios, como boletines informativos, y para comprobar las suscripciones o bajas de suscripción a estos servicios.

>[!NOTE]
>
>Las suscripciones solo se aplican al envío de correo electrónico y SMS.

Se pueden definir varios servicios en paralelo, por ejemplo: boletines para categorías de productos específicas, temas o áreas de un sitio web, suscripciones a varios tipos de mensajes de alerta y notificaciones en tiempo real.

Para obtener más información sobre la administración de suscripciones y bajas, consulte la [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Acceso a servicios de suscripción {#access-services}

Para acceder a los servicios de suscripción disponibles para su plataforma, vaya a la **[!UICONTROL Servicios de suscripción]** en el carril de navegación izquierdo.

![](assets/service-list.png)

Se muestra la lista de todos los servicios de suscripción existentes. Puede buscar en los servicios y filtrar por el canal, la carpeta o utilizar filtros avanzados.

![](assets/service-filters.png)

Para editar un servicio existente, haga clic en su nombre.

## Creación de su primer servicio de suscripción {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Propiedades del servicio de suscripciones"
>abstract="Introduzca la etiqueta del servicio de suscripción y defina opciones adicionales."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Mensajes de confirmación del servicio de suscripciones"
>abstract="Cuando un usuario se suscribe a un servicio o cancela su suscripción, puede enviar un mensaje de confirmación. Seleccione las plantillas que se utilizarán para estos mensajes."


Para crear un servicio de suscripción, siga estos pasos:

1. Seleccione el **[!UICONTROL Crear servicio de suscripción]** botón.

   ![](assets/service-create-button.png)

1. Seleccione un canal: **[!UICONTROL Correo electrónico]** o **[!UICONTROL SMS]**.

1. En las propiedades del servicio, introduzca una etiqueta y defina las opciones adicionales que desee.

   ![](assets/service-create-properties.png)

1. De forma predeterminada, las suscripciones son ilimitadas. Puede desactivar las **[!UICONTROL Período de validez ilimitado]** para definir una duración de validez del servicio. <!--The duration can be specified in days or months.TBC-->

   ![](assets/service-create-validity-period.png)

1. Cuando un usuario se suscribe o cancela la suscripción a un servicio, puede enviar un mensaje de confirmación. Seleccione las plantillas que desea utilizar para ese mensaje según el caso de uso.

   ![](assets/service-create-confirmation-msg.png)

1. Haga clic en **[!UICONTROL Save]**. El nuevo servicio se agrega al **[!UICONTROL Servicios de suscripción]** lista.

<!--
## Reporting

You can measure the effectiveness of your subscription services for SMS and email channels.

1. Select an existing service from the **[!UICONTROL Subscription services]** list.

1. From the service dashboard, click More > Reports?

1. Check the following indicators:

* Total numbers of subscribers

* Area graph with subscriptions and unsubscriptions. Use the dropwdown to change the time range. (24h, 48h, 1 week, 2 weeks, 1 month, 6 months)

* The breakdown by period. including subs, unsub, evolution in numbers and % and loyalty.
* Last updated / Next refresh time: these values are retrieved from the execution and schedule of the tracking workflow
-->


