---
audience: end-user
title: Informes de campaña para el canal SMS
description: Comprensión de los informes de campaña del canal SMS
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 18%

---

# Informes de campaña para el canal SMS {#campaign-reports-sms-channel}

Cada informe de campaña se divide en diferentes widgets que detallan el éxito y los errores de la campaña. A continuación se describen los informes y las métricas del canal SMS. Obtenga información sobre cómo acceder a sus informes de campaña en [esta página](campaign-reports.md).

## Resumen de envíos {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Información general sobre el envío"
>abstract="El informe **Información general sobre el envío** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de los SMS."


El **[!UICONTROL Resumen de entrega]** Este informe proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de SMS. Las métricas se detallan a continuación.

![](assets/campaign_report_sms_1.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campañas de SMS.

* **[!UICONTROL Total enviado]**: Número total de mensajes procesados durante la preparación de la entrega.

* **[!UICONTROL Entregado]**: Número de mensajes enviados correctamente en relación con el número total de mensajes enviados.

* **[!UICONTROL Errores]**: Total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

* **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

+++


### Estadísticas de público destinatario inicial {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="Estadísticas de público destinatario inicial"
>abstract="La tabla **Estadísticas del público destinatario inicial** muestra datos relativos a los destinatarios"

El **[!UICONTROL Estadísticas de audiencia de destinatario inicial]** La tabla muestra datos relativos a los destinatarios. Las métricas se detallan a continuación.


![](assets/campaign_report_sms_2.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campañas de SMS.

* **[!UICONTROL Audiencia inicial]**: Número total de destinatarios objetivo.

* **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Rechazado por reglas]**: Número total de direcciones ignoradas durante el análisis al aplicar las reglas: direcciones faltantes, en cuarentena, en la lista de bloqueados, etc.

+++


### Estadísticas de ejecución {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Estadísticas de ejecución"
>abstract="La tabla **Estadísticas de ejecución** detalla el éxito de su envío: mensajes para entregar, éxitos, errores y nuevas cuarentenas."


El **[!UICONTROL Estadísticas de ejecución]** La tabla detalla el éxito de su envío. Las métricas se detallan a continuación.


![](assets/campaign_report_sms_3.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campañas de SMS.

* **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

  Los tipos de error de SMS se enumeran en la [Documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Flujos de clics generados {#delivery-summary-sms-click-streams}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Flujos de clics generados"
>abstract="La tabla **Flujos de clics generados** muestra los datos disponibles en relación con la interacción de los destinatarios con el envío."

El **[!UICONTROL Flujos de clics generados]** La tabla muestra datos relativos a la interacción de los destinatarios con el envío. Las métricas se detallan a continuación.

![](assets/campaign_report_sms_4.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campañas de SMS.

* **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

* **[!UICONTROL Clics]**: Número total de clics en los vínculos de los envíos.

* **[!UICONTROL Reactividad]**: la proporción del número de destinatarios objetivo que han hecho clic en una entrega en relación con el número estimado de destinatarios objetivo que han abierto una entrega.

+++
