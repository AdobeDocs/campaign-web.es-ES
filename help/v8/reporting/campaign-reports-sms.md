---
audience: end-user
title: Informes de campaña para el canal SMS
description: Comprensión de los informes de campaña del canal SMS
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 17%

---

# Informes de campaña para el canal SMS {#campaign-reports-sms-channel}

Cada informe de campaña se divide en diferentes widgets que detallan el éxito y los errores de la campaña. A continuación se describen los informes y las métricas del canal SMS. Obtenga información sobre cómo acceder a los informes de campaña en [esta página](campaign-reports.md).

## Resumen de entregas {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Información general sobre el envío"
>abstract="El informe **Información general sobre el envío** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de los SMS."

El informe **[!UICONTROL Información general de entrega]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de SMS. Las métricas se detallan a continuación.

![Informe de descripción general de envío que muestra las métricas de SMS](assets/campaign_report_sms_1.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campaña de SMS.

* **[!UICONTROL Total de mensajes enviados]**: Número total de mensajes procesados durante la preparación de la entrega.

* **[!UICONTROL Entregado]**: número de mensajes enviados correctamente en relación con el número total de mensajes enviados.

* **[!UICONTROL Errores]**: Total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

* **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

+++

### Estadísticas de público destinatario inicial {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="Estadísticas de público destinatario inicial"
>abstract="La tabla **Estadísticas de público destinatario inicial** muestra datos relativos a los destinatarios."

La tabla **[!UICONTROL Estadísticas iniciales de audiencias de destino]** muestra datos relativos a sus destinatarios. Las métricas se detallan a continuación.

![Tabla de estadísticas de audiencias de destino inicial que muestra los datos del destinatario](assets/campaign_report_sms_2.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campaña de SMS.

* **[!UICONTROL Audiencia inicial]**: Número total de destinatarios objetivo.

* **[!UICONTROL Mensaje para entregar]**: Número total de mensajes que se enviarán después de la preparación del envío.

* **[!UICONTROL Rechazado por reglas]**: Número total de direcciones ignoradas durante el análisis al aplicar reglas, como direcciones que faltan, en cuarentena o en la lista de bloqueados de la.

+++

### Estadísticas de ejecución {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Estadísticas de ejecución"
>abstract="La tabla **Estadísticas de ejecución** detalla el éxito de su envío: mensajes para entregar, éxitos, errores y nuevas cuarentenas."

La tabla **[!UICONTROL Estadísticas de ejecución]** detalla el éxito de su envío. Las métricas se detallan a continuación.

![Tabla de estadísticas de ejecución que muestra las métricas de éxito de envío](assets/campaign_report_sms_3.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campaña de SMS.

* **[!UICONTROL Mensaje para entregar]**: Número total de mensajes que se enviarán después de la preparación del envío.

* **[!UICONTROL Éxito]**: número de mensajes procesados correctamente, en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores]**: Número total de errores acumulados durante las entregas y el procesamiento automático de los rechazos en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de una entrega fallido (usuario desconocido, dominio no válido), en relación con el número de mensajes que se van a enviar.

  Los tipos de error de SMS se enumeran en la [documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Flujos de clics generados {#delivery-summary-sms-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Flujos de clics generados"
>abstract="La tabla **Flujos de clics generados** muestra los datos disponibles en relación con la interacción de los destinatarios con el envío."

La tabla **[!UICONTROL Flujos de clics generados]** muestra datos relativos a cómo interactuaron los destinatarios con el envío. Las métricas se detallan a continuación.

![Tabla de flujos de clics generados que muestra los datos de interacción del destinatario](assets/campaign_report_sms_4.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campaña de SMS.

* **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

* **[!UICONTROL Clics]**: Número total de clics en los vínculos de los envíos.

* **[!UICONTROL Reactividad]**: la proporción del número de destinatarios objetivo que han hecho clic en una entrega en relación con el número estimado de destinatarios objetivo que han abierto una entrega.

+++
