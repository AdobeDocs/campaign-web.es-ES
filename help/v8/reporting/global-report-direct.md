---
audience: end-user
title: Informes globales para la canal correo directo
description: Obtenga más información sobre los informes globales para el canal correo directo
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
source-git-commit: aa9ddb8841d8ef77c9f76e4d05cdffd4a1c87c66
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 27%

---

# Informes globales para la canal correo directo {#global-report-direct}

Los correo postal informes globales proporcionan a los usuarios una visión general completa de tráfico y métricas de participación a nivel canal.

Navegue hasta el **[!UICONTROL menú Informes]** dentro de la **[!UICONTROL sección Informes]** . Puede filtrar los datos en función de la fecha, la carpeta o las reglas del informe. [Más información](global-reports.md)

## Resumen de envíos {#delivery-summary-direct}

### Información general sobre el envío {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="Información general sobre el envío"
>abstract="La **Información general de entrega** presenta métricas clave de rendimiento (KPI) que ofrecen información exhaustiva sobre la interacción de los visitantes con cada envío de correo directo. Las métricas se describen a continuación."

La **[!UICONTROL descripción general]** de la entrega presenta métricas de rendimiento clave (KPI) que ofrecen información detallada sobre la interacción de los visitantes con cada correo directo envío. Las métricas se describen a continuación.

![Esta imagen muestra las métricas de resumen de envío para correo directo entregas.](assets/global_report_direct_mail_delivery_overview.png){zoomable="yes"}{align="center"}

+++Más información sobre métricas de información general de entrega.

* **[!UICONTROL Mensajes que se van a enviar]**: número total de mensajes procesados durante la preparación del envío.

* **[!UICONTROL Entregados: número de mensajes enviados correctamente, en relación con el número total de mensajes enviados]**.

* **[!UICONTROL Errores]**: errores totales acumulados durante el procesamiento de envío y devolución automática, en relación con el número total de mensajes enviados.

* **[!UICONTROL Cancelación de suscripción]**: número de destinatarios que han hecho clic en baja vínculos.

+++

### Público objetivo {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="Público objetivo"
>abstract="Los datos del destinatario y la información del mensaje se muestran en el gráfico **Público objetivo** que refleja el análisis de preparación de envíos."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="Público objetivo"
>abstract="La tabla **Público objetivo** proporciona un desglose detallado de los destinatarios y los mensajes correspondientes, en función de los resultados del proceso de preparación de la entrega."

La tabla y el gráfico de **[!UICONTROL la audiencia]** objetivo muestran datos relacionados con los destinatarios, con métricas detalladas a continuación.

![Esta imagen muestra las métricas de audiencia objetivo para correo directo entregas.](assets/global_report_direct_mail_targeted_audience.png){zoomable="yes"}{align="center"}

+++Más información sobre las métricas de audiencia objetivo.

* **[!UICONTROL audiencia]** objetivo: número total de destinatarios objetivo.

* **[!UICONTROL Enviar mensaje que se va a enviar]**: número total de mensajes que deben entregarse después de envío preparación.

* **[!UICONTROL Exclusión]**: número total de direcciones ignoradas durante el análisis al aplicar reglas, como direcciones ausentes, en cuarentena o en lista de denegación.

+++

### Estadísticas de envío {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="Estadísticas de envío"
>abstract="El gráfico **Estadísticas de envío** proporciona perspectivas sobre la eficacia de sus envíos de correo directo, incluidos los envíos correctos y los errores encontrados."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="Estadísticas de envío"
>abstract="La tabla **Estadísticas de envío** detalla el éxito de su envío de correo directo y los errores que se han producido."

El **[!UICONTROL gráfico y la tabla de estadísticas]** de entrega proporcionan una desglose del éxito de cada correo directo envío, con métricas detalladas que se describen a continuación.

+++Más información sobre las métricas de estadísticas de entrega.

* **[!UICONTROL Enviar mensaje que se va a enviar]**: número total de mensajes que deben entregarse después de envío preparación.

* **[!UICONTROL Éxito]**: número de mensajes procesados correctamente, en relación con el número de mensajes que desea enviar.

* **[!UICONTROL Errores / Devoluciones]**: Errores totales acumulados durante las entregas y el procesamiento automático de rebotes, en relación con el número de mensajes a entregar.

* **[!UICONTROL Nuevo cuarentenas]**: número total de direcciones en cuarentena después de un envío fallido (por ejemplo, usuario desconocido, dominio inválido), en relación con el número de mensajes que se van a enviar.

+++

### Causas de exclusión {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="Exclusiones"
>abstract="La tabla **Causas de exclusión** muestra un desglose detallado, por regla, de los mensajes rechazados durante el proceso de preparación del envío."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="Causas de exclusión"
>abstract="El gráfico **Causas de exclusión** ilustra la distribución de mensajes rechazados durante la preparación de la entrega, clasificados por cada regla."

![Esta imagen muestra las causas de las métricas de exclusión para correo directo entregas.](assets/global_report_direct_mail_exclusions.png){zoomable="yes"}{align="center"}

El gráfico y la tabla Exclusiones ilustran las razones que impidieron que usuario perfiles, excluidos de los perfiles objetivo, recibieran el mensaje.

+++Más información sobre Causas de las métricas de exclusión.

* **[!UICONTROL Dirección en cuarentena]**: Error tipo generado cuando se coloca una dirección en cuarentena.

* **[!UICONTROL Dirección no especificada]**: Error tipo generado al enviar un envío para indicar que la dirección no existe.

* **[!UICONTROL Dirección de mala calidad]**: Error tipo generado cuando la calificación de calidad de la dirección postal es demasiado baja.

* **[!UICONTROL Dirección denegada]**: Error tipo generado cuando el destinatario se incluyó en la lista de denegación cuando se realizó la envío.

* **[!UICONTROL Doble]**: Error tipo generado cuando se excluyó el destinatario porque sus valores clave no eran únicos.

* **[!UICONTROL Control grupo]**: la dirección del destinatario forma parte del grupo de control.

* **[!UICONTROL Target de tamaño]** limitado: se ha alcanzado el tamaño máximo de envío para el destinatario.

+++