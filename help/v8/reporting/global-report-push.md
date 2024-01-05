---
audience: end-user
title: Informes globales del canal push
description: Comprensión de los informes globales del canal push
badge: label="Disponibilidad limitada"
source-git-commit: ac9a7918045e7ff02ef27c348b28a6ce09802caf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 4%

---

# Informes globales del canal push {#campaign-reports-push}

Los informes globales proporcionan a los usuarios una visión general completa de las métricas de tráfico y participación a nivel de canal.

Vaya a **[!UICONTROL Informes]** menú dentro de **[!UICONTROL Informes]** sección. Puede filtrar los datos según la fecha, la carpeta o las reglas del informe. [Más información](global-reports.md)

## Resumen de envíos {#delivery-summary-push}

### Resumen de envíos {#delivery-overview-push}

El **[!UICONTROL Resumen de entrega]** Este informe proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con cada envío de notificación push. Las métricas se detallan a continuación.

![](assets/global_report_push_delivery_overview.png)

+++Más información sobre las Métricas de información general de entrega.

* **[!UICONTROL Mensajes para enviar]**: Número total de mensajes procesados durante la preparación de la entrega.

* **[!UICONTROL Entregado]**: Número de mensajes enviados correctamente en relación con el número total de mensajes enviados.

* **[!UICONTROL Clics totales]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

* **[!UICONTROL Errores]**: Total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

+++

### Público objetivo {#delivery-summary-push-initial-target}

El **[!UICONTROL Audiencia objetivo]** La tabla y el gráfico presentan datos relacionados con los destinatarios para cada envío de notificación push enviado. Las métricas se detallan a continuación.

![](assets/global_report_push_targeted_audience.png)

+++Más información sobre las Métricas de audiencia segmentadas.

* **[!UICONTROL Audiencia objetivo]**: Número total de destinatarios objetivo.

* **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Exclusión]**: Número total de direcciones ignoradas durante el análisis al aplicar las reglas: direcciones faltantes, en cuarentena, en la lista de bloqueados, etc.

+++

### Estadísticas de envío {#delivery-summary-push-exec-stats}

El **[!UICONTROL Estadísticas de envío]** Esta tabla detalla el éxito de cada envío de notificaciones push. Las métricas se detallan a continuación.

![](assets/global_report_push_delivery_statistics.png)

+++Más información sobre las Métricas de estadísticas de envío.

* **[!UICONTROL Total de mensajes]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores/devoluciones]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de una entrega fallido (registro no válido, rechazo de mensaje, error de carga útil, por ejemplo). en relación con el número de mensajes que se van a enviar.

  Los tipos de error de notificaciones push se enumeran en [Documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Causas de exclusión {#causes-exclusion}

El **[!UICONTROL Causas de exclusión]** el gráfico y la tabla muestran los motivos que impidieron que los perfiles de usuario, que se excluyeron de los perfiles de destino, recibieran el mensaje.

Los tipos de error de notificaciones push se enumeran en [Documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## Rendimiento del envío {#delivery-throughput-sms}

![](assets/global_report_push_delivery_throughput.png)

Este informe proporciona detalles completos sobre el rendimiento del envío en un periodo de tiempo especificado.

