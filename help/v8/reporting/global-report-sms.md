---
audience: end-user
title: Informes globales para el canal SMS
description: Comprensión de los informes globales del canal SMS
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 31%

---

# Informes globales para el canal SMS {#campaign-reports-sms}

Los informes globales proporcionan a los usuarios una visión general completa de las métricas de tráfico y participación a nivel de canal.

Vaya al menú **[!UICONTROL Informes]** dentro de la sección **[!UICONTROL Informes]**. Puede filtrar los datos según la fecha, la carpeta o las reglas del informe. [Más información](global-reports.md)

## Resumen de envíos {#delivery-summary-sms}

### Información general sobre el envío {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="Información general sobre el envío de SMS"
>abstract="Los indicadores clave de rendimiento (KPI) de la **Información general sobre el envío de SMS** ofrecen un resumen completo del envío de SMS, con información detallada y datos específicos. Proporciona información completa sobre el rendimiento, la eficacia y los resultados de su envío."

El informe **[!UICONTROL Información general de entrega]** ofrece indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre los patrones de interacción de los visitantes con cada envío de SMS. A continuación se describen las métricas siguientes.

![](assets/global_report_sms_delivery_overview.png){zoomable="yes"}

+++Más información sobre las Métricas de información general de entrega.

* **[!UICONTROL Mensajes para entregar]**: Número total de mensajes procesados durante la preparación de la entrega.

* **[!UICONTROL Entregado]**: porcentaje de mensajes enviados correctamente en relación con el número total de mensajes enviados.

* **[!UICONTROL Tasa de pulsaciones]**: Porcentaje de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

* **[!UICONTROL Errores]**: porcentaje de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

+++

### Público objetivo {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="Población de destino de SMS"
>abstract="El gráfico y la tabla de la **Población de destino** presentan datos relacionados con el público de sus SMS, incluida información sobre los mensajes que se enviarán y las exclusiones."

La tabla y el gráfico de la **[!UICONTROL audiencia de destino]** presentan datos relacionados con sus destinatarios para cada envío de SMS enviado. Las métricas se detallan a continuación.

![](assets/global_report_sms_targeted_audience.png){zoomable="yes"}

+++Más información sobre las Métricas de audiencia segmentadas.

* **[!UICONTROL Audiencia objetivo]**: Número total de destinatarios objetivo.

* **[!UICONTROL Mensaje para entregar]**: Número total de mensajes que se enviarán después de la preparación del envío.

* **[!UICONTROL Exclusión]**: número total de direcciones omitidas durante el análisis al aplicar reglas: dirección que falta, en cuarentena, en la lista de bloqueados de la, etc.

+++

### Estadísticas de envío {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="Estadísticas de envío de los SMS"
>abstract="El informe **Estadísticas de envío** proporciona información completa sobre el SMS enviado y ofrece un desglose de varias métricas, como tasas de éxito, ocurrencias de errores y público puesto en cuarentena. Esta presentación detallada ofrece un examen exhaustivo del rendimiento general y los resultados del proceso de envío de SMS."

La tabla **[!UICONTROL estadísticas de envío]** detalla el éxito de cada envío de SMS. Las métricas se detallan a continuación.

![](assets/global_report_sms_delivery_statistics.png){zoomable="yes"}

+++Más información sobre las Métricas de estadísticas de envío.

* **[!UICONTROL Mensajes totales]**: Número total de mensajes que se enviarán después de la preparación de la entrega.

* **[!UICONTROL Éxito]**: número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores / Devoluciones]**: Número total de errores acumulados durante las entregas y el procesamiento automático de los rechazos en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de una entrega fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

  Los tipos de error de SMS se enumeran en la [documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Causas de exclusión {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="Causas de exclusión de envíos de SMS"
>abstract="El gráfico y la tabla **Causas de exclusión** ilustran las diversas razones que impidieron que los perfiles de usuario recibieran los mensajes SMS."

El gráfico y la tabla **[!UICONTROL Causas de exclusión]** muestran las razones que impidieron que los perfiles de usuario, que se excluyeron de los perfiles de destino, recibieran sus envíos SMS.

Los tipos de error se enumeran en la [documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png){zoomable="yes"}

## Rendimiento del envío {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="Rendimiento del envío de SMS"
>abstract="El informe **Rendimiento del envío** proporciona una amplia perspectiva de la eficacia del sistema de entrega de mensajes SMS y presenta información general detallada de las tasas de éxito y error en un período de tiempo especificado."

![](assets/global_report_sms_delivery_throughput.png){zoomable="yes"}

El informe **[!UICONTROL Rendimiento de entrega]** ofrece una visión completa de la eficacia del sistema de entrega de mensajes SMS, con un resumen detallado de las tasas de éxito y error durante un periodo especificado.
