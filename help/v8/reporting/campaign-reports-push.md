---
audience: end-user
title: Informes de campaña para el canal push
description: Comprender los informes de campaña del canal push
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 17%

---

# Informes de campaña para el canal push {#campaign-reports-push-channel}

Cada informe de campaña se divide en diferentes widgets que detallan el éxito y los errores de la campaña. A continuación se describen los informes y las métricas del canal push. Obtenga información sobre cómo acceder a los informes de campaña en [esta página](campaign-reports.md).

## Resumen de envíos {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="Información general sobre el envío"
>abstract="El informe **Información general del envío** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de notificaciones push."

El informe **[!UICONTROL Información general de entrega]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de notificaciones push. Las métricas se detallan a continuación.

![Métricas de resumen de envío mostradas en el informe Información general de envío](assets/campaign-reporting-push-summary.png){zoomable="yes"}

+++Obtenga más información acerca de las métricas de informes de campañas push.

* **[!UICONTROL Mensajes para entregar]**: Número total de mensajes procesados durante la preparación de la entrega.

* **[!UICONTROL Entregado]**: número de mensajes enviados correctamente en relación con el número total de mensajes enviados.

* **[!UICONTROL Errores]**: Número total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

* **[!UICONTROL Clics totales]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

+++

### Estadísticas de público destinatario inicial {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="Estadísticas de público destinatario inicial"
>abstract="La tabla **Estadísticas de público destinatario inicial** muestra datos relativos a los destinatarios."

La tabla **[!UICONTROL Estadísticas iniciales de audiencias de destino]** muestra datos relativos a sus destinatarios. Las métricas se detallan a continuación.

![Estadísticas de audiencia de destinatario iniciales mostradas en el informe](assets/campaign-reporting-push-target.png){zoomable="yes"}

+++Obtenga más información acerca de las métricas de informes de campañas push.

* **[!UICONTROL Audiencia inicial]**: Número total de destinatarios objetivo.

* **[!UICONTROL Mensaje para entregar]**: Número total de mensajes que se enviarán después de la preparación del envío.

* **[!UICONTROL Rechazado por reglas]**: Número total de direcciones ignoradas durante el análisis al aplicar reglas, como direcciones que faltan, en cuarentena o en la lista de bloqueados de la.

+++

### Estadísticas de ejecución {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="Estadísticas de ejecución"
>abstract="La tabla **Estadísticas de ejecución** detalla el éxito de su envío: mensajes para entregar, éxitos, errores y nuevas cuarentenas."

La tabla **[!UICONTROL Estadísticas de ejecución]** detalla el éxito de su envío. Las métricas se detallan a continuación.

![Estadísticas de ejecución mostradas en el informe](assets/campaign-reporting-push-exec.png){zoomable="yes"}

+++Obtenga más información acerca de las métricas de informes de campañas push.

* **[!UICONTROL Mensaje para entregar]**: Número total de mensajes que se enviarán después de la preparación del envío.

* **[!UICONTROL Éxito]**: número de mensajes procesados correctamente, en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores]**: Número total de errores acumulados durante las entregas y el procesamiento automático de los rechazos en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (registro no válido, rechazo de mensaje o error de carga útil, por ejemplo) en relación con el número de mensajes que se van a enviar.

  Los tipos de error de notificaciones push se enumeran en [Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=es#push-error-types){target="_blank"}.

+++

### Flujos de clics generados {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="Flujos de clics generados"
>abstract="La tabla **Flujos de clics generados** muestra los datos disponibles en relación con la interacción de los destinatarios con el envío."

La tabla **[!UICONTROL Flujos de clics generados]** muestra datos relativos a cómo interactuaron los destinatarios con el envío. Las métricas se detallan a continuación.

![Flujos de clics generados mostrados en el informe](assets/campaign-reporting-push-clicks.png){zoomable="yes"}

+++Obtenga más información acerca de las métricas de informes de campañas push.

* **[!UICONTROL Clics únicos]**: Número total de destinatarios diferentes que hicieron clic en un envío al menos una vez.

* **[!UICONTROL Clics totales]**: Número total de clics en los vínculos de los envíos.

* **[!UICONTROL Reactividad]**: la proporción del número de destinatarios objetivo que hicieron clic en una entrega en relación con el número estimado de destinatarios objetivo que abrieron una entrega.

+++