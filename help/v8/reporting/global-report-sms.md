---
audience: end-user
title: Informes globales para el canal SMS
description: Comprensión de los informes globales del canal SMS
badge: label="Disponibilidad limitada"
source-git-commit: 6fbc6d477aac54e8cb7a1eeba40f7c32903c261f
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 3%

---

# Informes globales para el canal SMS {#campaign-reports-sms}

Los informes globales proporcionan a los usuarios una visión general completa de las métricas de tráfico y participación a nivel de canal.

Vaya a **[!UICONTROL Informes]** menú dentro de **[!UICONTROL Informes]** sección. Puede filtrar los datos según la fecha, la carpeta o las reglas del informe. [Más información](global-reports.md)

## Resumen de envíos {#delivery-summary-sms}

### Información general sobre el envío {#delivery-overview-sms}

El **[!UICONTROL Resumen de entrega]** Este informe ofrece indicadores clave de rendimiento (KPI) completos que proporcionan una perspectiva exhaustiva de los patrones de interacción de los visitantes con cada envío de SMS. A continuación se describen las métricas siguientes.

![](assets/global_report_sms_delivery_overview.png)

+++Más información sobre las Métricas de información general de entrega.

* **[!UICONTROL Mensajes para enviar]**: Número total de mensajes procesados durante la preparación de la entrega.

* **[!UICONTROL Entregado]**: porcentaje de mensajes enviados correctamente en relación con el número total de mensajes enviados.

* **[!UICONTROL Tasa de pulsaciones]**: porcentaje de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

* **[!UICONTROL Errores]**: porcentaje de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

+++

### Público objetivo {#delivery-summary-sms-initial-target}

El **[!UICONTROL Audiencia objetivo]** La tabla y el gráfico presentan datos relacionados con los destinatarios para cada envío de SMS enviado. Las métricas se detallan a continuación.

![](assets/global_report_sms_targeted_audience.png)

+++Más información sobre las Métricas de audiencia segmentadas.

* **[!UICONTROL Audiencia objetivo]**: Número total de destinatarios objetivo.

* **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Exclusión]**: Número total de direcciones ignoradas durante el análisis al aplicar las reglas: direcciones faltantes, en cuarentena, en la lista de bloqueados, etc.

+++

### Estadísticas de envío {#delivery-summary-sms-exec-stats}

El **[!UICONTROL Estadísticas de envío]** Esta tabla detalla el éxito de cada envío de SMS. Las métricas se detallan a continuación.

![](assets/global_report_sms_delivery_statistics.png)

+++Más información sobre las Métricas de estadísticas de envío.

* **[!UICONTROL Total de mensajes]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores/devoluciones]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

  Los tipos de error de SMS se enumeran en la [Documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Causas de exclusión {#causes-exclusion}

El **[!UICONTROL Causas de exclusión]** El gráfico y la tabla muestran los motivos que impidieron que los perfiles de usuario, que se excluyeron de los perfiles objetivo, recibieran sus envíos SMS.

Los tipos de error se enumeran en la [Documentación de Adobe Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Rendimiento del envío {#delivery-throughput-sms}

![](assets/global_report_sms_delivery_throughput.png)

Este informe proporciona detalles completos sobre el rendimiento del envío en un periodo de tiempo especificado.
