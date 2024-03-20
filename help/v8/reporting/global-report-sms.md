---
audience: end-user
title: Informes globales para el canal SMS
description: Comprensión de los informes globales del canal SMS
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 32%

---

# Informes globales para el canal SMS {#campaign-reports-sms}

Los informes globales proporcionan a los usuarios una visión general completa de las métricas de tráfico y participación a nivel de canal.

Vaya a **[!UICONTROL Informes]** menú dentro de **[!UICONTROL Informes]** sección. Puede filtrar los datos según la fecha, la carpeta o las reglas del informe. [Más información](global-reports.md)

## Resumen de envíos {#delivery-summary-sms}

### Información general sobre el envío {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="Información general sobre el envío de SMS"
>abstract="Los indicadores clave de rendimiento (KPI) de la **Información general sobre el envío de SMS** ofrecen un resumen completo del envío de SMS, con información detallada y datos específicos. Proporciona información completa sobre el rendimiento, la eficacia y los resultados de su envío."

El **[!UICONTROL Resumen de entrega]** Este informe ofrece indicadores clave de rendimiento (KPI) completos que proporcionan una perspectiva exhaustiva de los patrones de interacción de los visitantes con cada envío de SMS. A continuación se describen las métricas siguientes.

![](assets/global_report_sms_delivery_overview.png){zoomable=&quot;yes&quot;}

+++Más información sobre las Métricas de información general de entrega.

* **[!UICONTROL Mensajes para enviar]**: Número total de mensajes procesados durante la preparación de la entrega.

* **[!UICONTROL Entregado]**: porcentaje de mensajes enviados correctamente en relación con el número total de mensajes enviados.

* **[!UICONTROL Tasa de pulsaciones]**: porcentaje de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

* **[!UICONTROL Errores]**: porcentaje de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

+++

### Público objetivo {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="Población de destino de SMS"
>abstract="El gráfico y la tabla de la **Población de destino** presentan datos relacionados con el público de sus SMS, incluida información sobre los mensajes que se enviarán y las exclusiones."

El **[!UICONTROL Audiencia objetivo]** La tabla y el gráfico presentan datos relacionados con los destinatarios para cada envío de SMS enviado. Las métricas se detallan a continuación.

![](assets/global_report_sms_targeted_audience.png){zoomable=&quot;yes&quot;}

+++Más información sobre las Métricas de audiencia segmentadas.

* **[!UICONTROL Audiencia objetivo]**: Número total de destinatarios objetivo.

* **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Exclusión]**: Número total de direcciones ignoradas durante el análisis al aplicar las reglas: direcciones faltantes, en cuarentena, en la lista de bloqueados, etc.

+++

### Estadísticas de envío {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="Estadísticas de envío de los SMS"
>abstract="El informe **Estadísticas de envío** proporciona información completa sobre el SMS enviado y ofrece un desglose de varias métricas, como tasas de éxito, ocurrencias de errores y público puesto en cuarentena. Esta presentación detallada ofrece un examen exhaustivo del rendimiento general y los resultados del proceso de envío de SMS."

El **[!UICONTROL Estadísticas de envío]** Esta tabla detalla el éxito de cada envío de SMS. Las métricas se detallan a continuación.

![](assets/global_report_sms_delivery_statistics.png){zoomable=&quot;yes&quot;}

+++Más información sobre las Métricas de estadísticas de envío.

* **[!UICONTROL Total de mensajes]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores/devoluciones]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

  Los tipos de error de SMS se enumeran en la [Documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Causas de exclusión {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="Causas de exclusión de envíos de SMS"
>abstract="El gráfico y la tabla **Causas de exclusión** ilustran las diversas razones que impidieron que los perfiles de usuario recibieran los mensajes SMS."

El **[!UICONTROL Causas de exclusión]** El gráfico y la tabla muestran los motivos que impidieron que los perfiles de usuario, que se excluyeron de los perfiles objetivo, recibieran sus envíos SMS.

Los tipos de error se enumeran en la [Documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png){zoomable=&quot;yes&quot;}

## Rendimiento del envío {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="Rendimiento del envío de SMS"
>abstract="El informe **Rendimiento del envío** proporciona una amplia perspectiva de la eficacia del sistema de entrega de mensajes SMS y presenta información general detallada de las tasas de éxito y error en un período de tiempo especificado."

![](assets/global_report_sms_delivery_throughput.png){zoomable=&quot;yes&quot;}

El **[!UICONTROL Rendimiento de entrega]** Este informe ofrece una visión completa de la eficacia del sistema de entrega de mensajes SMS, con un resumen detallado de las tasas de éxito y error durante un periodo especificado.
