---
audience: end-user
title: Campaign informes para el canal de inserción
description: Comprender campaña informes para el canal de inserción
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 15%

---

# Campaign informes para el canal de inserción {#campaign-reports-push-channel}

Cada informe campaña está dividido en diferentes widgets que detallan el éxito y los errores de su campaña. Para el canal de inserción, a continuación se describen los informes y métricas. Obtenga información sobre cómo acceder a sus informes de campaña en [este Página](campaign-reports.md).

## Resumen de envíos {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="Información general sobre el envío"
>abstract="El informe **Información general del envío** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de notificaciones push."

El **[!UICONTROL informe de información general]** de entrega proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo interactúan los visitantes con la envío de notificación de inserción. Las métricas se detallan a continuación.

![Métricas de resumen de entrega que se muestran en el informe Información general de entrega](assets/campaign-reporting-push-summary.png){zoomable="yes"}

+++Más información sobre las métricas de informes de campaña push.

* **[!UICONTROL Mensajes que se van a enviar]**: número total de mensajes procesados durante la preparación del envío.

* **[!UICONTROL Entregados: número de mensajes enviados correctamente, en relación con el número total de mensajes enviados]**.

* **[!UICONTROL Errores]**: número total de errores acumulados durante el procesamiento de envío y devolución automática, en relación con el número total de mensajes enviados.

* **[!UICONTROL Clics totales]**: número total de destinatarios distintos que hicieron clic en un envío al menos una vez.

+++

### Estadísticas de público destinatario inicial {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="Estadísticas de público destinatario inicial"
>abstract="La **destino inicial audiencia tabla de estadísticas** muestra los datos relativos a los destinatarios."

La **[!UICONTROL destino inicial audiencia tabla de estadísticas]** muestra los datos relativos a los destinatarios. Las métricas se detallan a continuación.

![Estadísticas iniciales de destino audiencia mostradas en el informe](assets/campaign-reporting-push-target.png){zoomable="yes"}

+++Más información sobre las métricas de informes de campaña push.

* **[!UICONTROL audiencia]** inicial: número total de destinatarios objetivo.

* **[!UICONTROL Enviar mensaje que se va a enviar]**: número total de mensajes que deben entregarse después de envío preparación.

* **[!UICONTROL rechazado por reglas]**: número total de direcciones ignoradas durante el análisis al aplicar reglas, como direcciones faltantes, en cuarentena o en lista de denegación.

+++

### Estadísticas de ejecución {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="Estadísticas de ejecución"
>abstract="La tabla **Estadísticas de ejecución** detalla el éxito de su envío: mensajes para entregar, éxitos, errores y nuevas cuarentenas."

La **[!UICONTROL tabla de estadísticas]** de ejecución detalla el éxito de su envío. Las métricas se detallan a continuación.

![Estadísticas de ejecución mostradas en el informe](assets/campaign-reporting-push-exec.png){zoomable="yes"}

+++Más información sobre las métricas de informes de campaña push.

* **[!UICONTROL Enviar mensaje que se va a enviar]**: número total de mensajes que deben entregarse después de envío preparación.

* **[!UICONTROL Éxito]**: número de mensajes procesados correctamente, en relación con el número de mensajes que desea enviar.

* **[!UICONTROL Errores]**: número total de errores acumulados durante los envíos y el procesamiento automático de rechazos, en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Nuevo cuarentenas]**: número total de direcciones en cuarentena después de un envío fallido (no válido registro, rechazo de mensaje o error de carga útil, por ejemplo), en relación con el número de mensajes que se van a enviar.

  Los tipos de error de notificaciones push se enumeran en la documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"} de Adobe Campaign v8 (consola de [cliente).

+++

### Flujos de clics generados {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="Flujos de clics generados"
>abstract="La tabla **Flujos de clics generados** muestra los datos disponibles en relación con la interacción de los destinatarios con el envío."

La **[!UICONTROL tabla Flujos de clics generados muestra datos relativos a la forma en que los destinatarios]** interactuaron con los envío. Las métricas se detallan a continuación.

![Las secuencias de clics generadas se muestran en el informe](assets/campaign-reporting-push-clicks.png){zoomable="yes"}

+++Más información sobre las métricas de informes de campaña push.

* **[!UICONTROL Clics únicos]**: número total de destinatarios distintos que hicieron clic en un envío al menos una vez.

* **[!UICONTROL Clics totales: número total de clics en los vínculos de los envíos]**.

* **[!UICONTROL Reactividad]**: proporción del número de destinatarios objetivo que hicieron clic en un envío, en relación con el número estimado de destinatarios objetivo que abrieron un envío.

+++