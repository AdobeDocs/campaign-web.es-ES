---
audience: end-user
title: Preparación y envío de un correo electrónico
description: Obtenga información sobre cómo preparar y enviar un correo electrónico con la interfaz de usuario web de Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 31%

---

# Preparación y envío de su correo electrónico {#prepare-send}

## Preparación del envío {#prepare}

Al definir el [contenido](../email/edit-content.md), la [audiencia](../audience/add-audience.md) y la [programación](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule), está listo para preparar su envío de correo electrónico.

Durante la preparación, se calcula la población objetivo y se genera el contenido del mensaje para cada perfil incluido en el objetivo. Una vez finalizada la preparación, los mensajes están listos para enviarse, ya sea inmediatamente o en la fecha y la hora programadas.

Las reglas de validación utilizadas durante la preparación de la entrega se describen en la [documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html){target="_blank"}.

A continuación se enumeran los pasos principales para preparar el envío.

1. En el panel de entregas, haga clic en **[!UICONTROL Revisar y enviar]**.

   ![Botón Revisar y enviar en el panel de envío](assets/email-review-and-send.png){zoomable="yes"}

1. Haga clic en el botón **[!UICONTROL Preparar]** situado en la esquina superior derecha y confirme la acción.

   ![Botón Preparar en el panel de envío](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si programas tu envío y deshabilitas la opción **[!UICONTROL Habilitar confirmación antes de enviar]**, los pasos de preparación y envío se agrupan bajo el botón **[!UICONTROL Preparar y enviar]**. [Más información sobre la programación](../msg/gs-deliveries.md#gs-schedule)

1. Se muestra el progreso de la preparación. En función del tamaño de la población de destinatarios, esta operación puede tardar algún tiempo.

   Puede detener la preparación en cualquier momento con el botón **[!UICONTROL Detener preparación]**.

   ![Botón Detener preparación en el panel de envío](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >Durante la fase de preparación, no se envían mensajes. Puede comenzar o detener esto sin riesgo de afectar a nada.

1. Cuando termine la preparación, compruebe los KPI. Si el número de mensajes que desea enviar no coincide con sus expectativas, modifique el público y reinicie la preparación.

   ![Pantalla de preparación completa que muestra los KPI](assets/email-preparation-complete.png){zoomable="yes"}

   Estos son los diferentes KPI mostrados:

   * **[!UICONTROL Objetivos]**: el número de destinatarios objetivo.
   * **[!UICONTROL Para entregar]**: el número de mensajes que se enviarán.
   * **[!UICONTROL Para excluir]**: el número de mensajes excluidos por una [regla de tipología](../advanced-settings/delivery-settings.md#typology).

1. Haga clic en el botón **[!UICONTROL Registros]** y compruebe que no haya errores. El último mensaje de registro muestra los mensajes de error y los errores. [Más información](delivery-logs.md)

   ![Botón Registros en el panel de envío](assets/email-prepare-logs.png){zoomable="yes"}

1. Si la preparación detecta un error crítico que impide que se realice el envío, el estado de preparación aparece como erróneo en el panel de control de envío.

   ![Estado de error en el panel de envío](assets/email-prepare-error.png){zoomable="yes"}

1. Si realiza cambios en la entrega después de la preparación, reinicie la preparación para que los cambios se tengan en cuenta.

Una vez completada la preparación sin errores, el mensaje está listo para enviarse.

## Envío del mensaje {#send}

Una vez completada la [preparación](#prepare), puedes enviar tu correo electrónico.

Si el mensaje está programado, se envía en la fecha y la hora definidas. [Más información sobre la programación](../msg/gs-deliveries.md#gs-schedule)

### Enviar inmediatamente {#send-immediately}

Para enviar un correo electrónico inmediatamente, siga los pasos a continuación.

1. En el panel de envío, haga clic en el botón **[!UICONTROL Enviar]** en la esquina superior derecha.

   ![Botón Enviar en el panel de envío](assets/email-send.png){zoomable="yes"}

1. Confirme esta acción para enviar inmediatamente el mensaje al destinatario principal.

1. Se muestra el progreso del envío.

### Programar el envío {#schedule-the-send}

Si programa el correo electrónico para enviarlo en una fecha y hora posteriores, siga los pasos a continuación.

1. Antes de hacer clic en el botón **[!UICONTROL Revisar y enviar]**, asegúrate de definir una programación para el correo electrónico. [Más información sobre la programación](../msg/gs-deliveries.md#gs-schedule)

1. En el panel de entregas, haga clic en el botón **[!UICONTROL Enviar como programado]** en la esquina superior derecha.

   ![Botón Enviar como programado en el panel de envío](assets/email-send-as-scheduled.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Confirmar envío]**. La entrega se realiza en la fecha programada al destinatario principal.

   >[!NOTE]
   >
   >Si deshabilita la opción **[!UICONTROL Habilitar confirmación antes de enviar]**, los pasos de preparación y envío se agrupan bajo el botón **[!UICONTROL Preparar y enviar]**. [Más información sobre la programación](../msg/gs-deliveries.md#gs-schedule)

## Pausar o detener el envío {#pause-stop-sending}

Independientemente de si la entrega está programada o no<!--TBC-->, se pueden realizar dos acciones en cualquier momento durante el proceso de entrega:

* Haga clic en **[!UICONTROL Pausar el envío]** para interrumpir el envío de los mensajes. Puede reanudar el envío en cualquier momento.

* Haga clic en **[!UICONTROL Detener envío]** para interrumpir el envío inmediatamente. Ni la preparación ni el envío se pueden reanudar una vez detenidos.

![Pausar o detener botones de envío en el panel de envío](assets/email-send-pause-or-stop.png){zoomable="yes"}

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

Una vez completado el envío, puede comprobar los KPI mostrados:

![KPI mostrados después de enviar](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL Enviado]**: el número de mensajes enviados. El porcentaje mostrado se basa en el número total de mensajes que se van a enviar.

* **[!UICONTROL Entregados]**: el número de mensajes entregados correctamente. El porcentaje mostrado se basa en el número total de mensajes enviados.

* **[!UICONTROL Abiertos]**: el número de mensajes abiertos. El porcentaje mostrado es el número de aperturas distintas en comparación con el número de mensajes enviados.

* **[!UICONTROL Clics]**: el número de destinatarios que hicieron clic al menos una vez en el correo electrónico. El porcentaje mostrado es el número de clics distintos comparado con el número de mensajes enviados.

* **[!UICONTROL Errores]**: número de correos electrónicos con el estado de error. El porcentaje mostrado se basa en el número total de mensajes enviados.

>[!NOTE]
>
>Todos los indicadores se actualizan cada 5 minutos después de iniciarse la entrega. Los indicadores de preparación de envíos son en tiempo real.

Obtenga más información acerca de los KPI en [esta página](../reporting/kpis.md).

También puede comprobar los registros. [Más información](delivery-logs.md)