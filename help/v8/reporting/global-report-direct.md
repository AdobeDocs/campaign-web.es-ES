---
audience: end-user
title: Informes globales para el canal de correo postal
description: Más información sobre los Informes globales para el canal de correo postal
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 33%

---

# Informes globales para el canal de correo postal {#global-report-direct}

Los informes globales de correo directo proporcionan a los usuarios una visión general completa de las métricas de tráfico y participación a nivel de canal.

Vaya a **[!UICONTROL Informes]** menú dentro de **[!UICONTROL Informes]** sección. Puede filtrar los datos según la fecha, la carpeta o las reglas del informe. [Más información](global-reports.md)

## Resumen de envíos {#delivery-summary-direct}

### Información general sobre el envío {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="Información general sobre el envío"
>abstract="La **Información general de entrega** presenta métricas clave de rendimiento (KPI) que ofrecen información exhaustiva sobre la interacción de los visitantes con cada envío de correo directo. Las métricas se describen a continuación."

La **[!UICONTROL Información general de entrega]** presenta métricas clave de rendimiento (KPI) que ofrecen información exhaustiva sobre la interacción de los visitantes con cada envío de correo directo. Las métricas se describen a continuación.

![](assets/global_report_direct_mail_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++Más información sobre las Métricas de información general de entrega.

* **[!UICONTROL Mensajes para enviar]**: Número total de mensajes procesados durante la preparación de la entrega.

* **[!UICONTROL Entregado]**: Número de mensajes enviados correctamente en relación con el número total de mensajes enviados.

* **[!UICONTROL Errores]**: Total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

* **[!UICONTROL Cancela la suscripción]**: Número de destinatarios que hicieron clic en las bajas de suscripción.
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

La tabla y el gráfico de **[!UICONTROL Audiencia objetivo]** Muestre datos relacionados con sus destinatarios, con las métricas detalladas que se proporcionan a continuación.

![](assets/global_report_direct_mail_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++Más información sobre las Métricas de audiencia segmentadas.

* **[!UICONTROL Audiencia objetivo]**: Número total de destinatarios objetivo.

* **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Exclusión]**: Número total de direcciones ignoradas durante el análisis al aplicar las reglas: direcciones faltantes, en cuarentena, en la lista de bloqueados, etc.

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

El **[!UICONTROL Estadísticas de envío]** el gráfico y la tabla proporcionan un desglose del éxito de cada envío de correo postal, con métricas detalladas que se describen a continuación.

+++Más información sobre las Métricas de estadísticas de envío.

* **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores/devoluciones]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

+++

### Causas de exclusión {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="Exclusiones"
>abstract="La tabla **Causas de exclusión** muestra un desglose detallado, por regla, de los mensajes rechazados durante el proceso de preparación del envío."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="Causas de exclusión de entrega"
>abstract="El gráfico **Causas de exclusión** ilustra la distribución de mensajes rechazados durante la preparación de la entrega, clasificados por cada regla."

![](assets/global_report_direct_mail_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

El gráfico y la tabla Exclusiones ilustran los motivos que impidieron que los perfiles de usuario, excluidos de los perfiles de destino, recibieran el mensaje.

+++Más información sobre las Causas de las métricas de exclusión.

* **[!UICONTROL Dirección en cuarentena]**: Tipo de error generado cuando la dirección se envía a cuarentena.

* **[!UICONTROL Dirección no especificada]**: Tipo de error generado al realizar un envío para indicar que la dirección no existe.

* **[!UICONTROL Dirección de mala calidad]**: Tipo de error generado cuando la clasificación de calidad de la dirección postal es demasiado baja.

* **[!UICONTROL Incluir en la lista de bloqueados dirección de]** incluir en la lista de bloqueados : Tipo de error generado cuando se el destinatario cuando se realizó la entrega.

* **[!UICONTROL Doble]**: Tipo de error generado cuando se excluyó al destinatario porque sus valores de claves no eran únicos.

* **[!UICONTROL Grupo de control]**: la dirección del destinatario forma parte del grupo de control.

* **[!UICONTROL Destinatario de tamaño limitado]**: se ha alcanzado el tamaño máximo de entrega para el destinatario.

+++
