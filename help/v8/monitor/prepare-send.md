---
audience: end-user
title: Preparación y envío de un correo electrónico
description: Aprenda a preparar y enviar una correo electrónico con Campaign interfaz de Web usuario
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 29%

---

# Preparación y envío de su correo electrónico {#prepare-send}

## Preparación del envío {#prepare}

Cuando defina su [contenido](../email/edit-content.md), [audiencia](../audience/add-audience.md) y [programación](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule), estará listo para preparar su correo electrónico envío.

Durante la preparación del envío, se calcula la población destino y se genera el contenido del mensaje para cada perfil incluido en el destino. Una vez finalizada la preparación, los mensajes están listos para ser enviados, ya sea inmediatamente o en la fecha y hora programadas.

Las reglas validación utilizadas durante la preparación envío se describen en la documentación[&#128279;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html?lang=es){target="_blank"} de Campaign v8 (consola de cliente).

A continuación se detallan los pasos principales para preparar el envío.

1. En la panel envío, haga clic en **[!UICONTROL Revisar y enviar]**.

   ![Revise y envíe botón en el panel de envío](assets/email-review-and-send.png){zoomable="yes"}

1. Haga clic en el **[!UICONTROL botón Preparar]** situado en la esquina superior derecha y confirme.

   ![Preparar botón en la envío panel](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si programa su envío y deshabilita la opción Habilitar confirmación **[!UICONTROL antes de enviar]** , los pasos de preparación y envío se agrupan en Preparar **[!UICONTROL y enviar]** botón. [Más información sobre la programación](../msg/gs-deliveries.md#gs-schedule)

1. Se muestra el progreso de la preparación. En función del tamaño de la población de destinatarios, esta operación puede tardar algún tiempo.

   Puede detener la preparación en cualquier momento usando el **[!UICONTROL Parada botón de preparación]** .

   ![Parada preparación botón en el envío panel](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >Durante la fase de preparación, no se envían mensajes. Puede inicio o detener esto sin riesgo de afectar nada.

1. Cuando finalice la preparación, compruebe los KPI. Si el número de mensajes que desea enviar no coincide con sus expectativas, modifique el público y reinicie la preparación.

   ![Pantalla de preparación completa que muestra los KPI](assets/email-preparation-complete.png){zoomable="yes"}

   Estos son los diferentes KPI mostrados:

   * **[!UICONTROL Segmentado]**: número de destinatarios objetivo.
   * **[!UICONTROL Para entregar]**: el número de mensajes que se enviarán.
   * **[!UICONTROL Para excluir]**: número de mensajes excluidos por una [reglas de tipología](../advanced-settings/delivery-settings.md#typology).

1. Haga clic en el **[!UICONTROL botón Registros]** y compruebe que no haya errores. El último mensaje de registro muestra los mensajes de error y los errores. [Más información](delivery-logs.md)

   ![Los registros botón en la panel de envío](assets/email-prepare-logs.png){zoomable="yes"}

1. Si la preparación detecta un error crítico que impide que se realice el envío, el estado de preparación aparece como erróneo en el panel de envío.

   ![Error estado en la panel envío](assets/email-prepare-error.png){zoomable="yes"}

1. Si realiza algún cambio en el envío después de la preparación, reinicie la preparación para que esos cambios se tengan en cuenta.

Una vez que la preparación se completa sin errores, su mensaje está listo para ser enviado.

## Envío del mensaje {#send}

Una vez finalizada la [preparación](#prepare) , puedes enviar tu correo electrónico.

Si el mensaje está programado, se envía en la fecha y hora definidas. [Más información sobre la programación](../msg/gs-deliveries.md#gs-schedule)

### Enviar inmediatamente {#send-immediately}

Para enviar una correo electrónico inmediatamente, seguir los pasos a continuación.

1. En el panel envío, haz clic en el **[!UICONTROL botón Enviar]** situado en la esquina superior derecha.

   ![Enviar botón en el panel envío](assets/email-send.png){zoomable="yes"}

1. Confirme esta acción para enviar inmediatamente el mensaje a la destino principal.

1. Se muestra el progreso de envío.

### Programación del envío {#schedule-the-send}

Si programa su correo electrónico para enviarlo en una fecha y hora posteriores, seguir los pasos que se indican a continuación.

1. Antes de hacer clic en Revisar **[!UICONTROL y enviar]** botón, asegúrese de definir una programación para su correo electrónico. [Más información sobre la programación](../msg/gs-deliveries.md#gs-schedule)

1. En el envío panel, haga clic en el **[!UICONTROL botón]** Enviar según lo programado en la esquina superior derecha.

   ![Enviar según lo programado botón en la envío panel](assets/email-send-as-scheduled.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Confirmar envío]**. El envío se envía en la fecha programada al destino principal.

   >[!NOTE]
   >
   >Si deshabilita la opción Habilitar confirmación **[!UICONTROL antes de enviar]** , los pasos de preparación y envío se agrupan en Preparar **[!UICONTROL y enviar]** botón. [Más información sobre la programación](../msg/gs-deliveries.md#gs-schedule)

## Detener o detener el envío {#pause-stop-sending}

Tanto si su envío está programada como si no<!--TBC-->, se pueden realizar dos acciones en cualquier momento durante el proceso de envío:

* Haga clic en **[!UICONTROL Pausar envío]** para interrumpir el envío de los mensajes. Puede reanudar el envío en cualquier momento.

* Haga clic en **[!UICONTROL Parada envío]** para interrumpir inmediatamente el envío. Ni la preparación ni el envío se pueden reanudar una vez detenidos.

![Poner en pausa o detener el envío de botones en el panel envío](assets/email-send-pause-or-stop.png){zoomable="yes"}

## Compruebe los KPI mostrados {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Entregados"
>abstract="Número de mensajes entregados correctamente. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado se basa en el número total de mensajes enviados."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/reports/kpis" text="Comprender los indicadores clave de rendimiento (KPI)"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Aperturas"
>abstract="Número de mensajes abiertos. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado es la proporción del número de aperturas distintas comparado con el número de mensajes enviados."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/reports/kpis" text="Comprender los indicadores clave de rendimiento (KPI)"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Clics"
>abstract="El número de destinatarios que hicieron clic al menos una vez en el correo electrónico. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado es la proporción del número de clics distintos en comparación con el número de mensajes entregados."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/reports/kpis" text="Comprender los indicadores clave de rendimiento (KPI)"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Enviado"
>abstract="Número total de mensajes procesados durante el análisis de entregas."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/reports/kpis" text="Comprender los indicadores clave de rendimiento (KPI)"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Errores"
>abstract="Total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/reports/kpis" text="Comprender los indicadores clave de rendimiento (KPI)"

Una vez finalizado el envío, puede comprobar los KPI mostrados:

![KPI mostrados después de enviar](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL Enviados]**: número de mensajes enviados. El porcentaje mostrado se basa en el número total de mensajes que se van a enviar.

* **[!UICONTROL Entregados]**: el número de mensajes entregados correctamente. El porcentaje mostrado se basa en el número total de mensajes enviados.

* **[!UICONTROL Abiertos]**: el número de mensajes abiertos. El porcentaje mostrado es el número de aperturas distintas en comparación con el número de mensajes enviados.

* **[!UICONTROL Clics]**: número de destinatarios que hicieron clic al menos una vez en la correo electrónico. El porcentaje mostrado es el número de clics distintos comparado con el número de mensajes enviados.

* **[!UICONTROL Errores]**: el número de correos electrónicos con el estado de error. El porcentaje mostrado se basa en el número total de mensajes enviados.

>[!NOTE]
>
>Todos los indicadores se actualizan cada 5 minutos después de que comience la envío. Los indicadores de preparación del envío son en tiempo real.

Obtenga más información sobre los KPI en [este Página](../reporting/kpis.md).

También puede comprobar los registros. [Más información](delivery-logs.md)