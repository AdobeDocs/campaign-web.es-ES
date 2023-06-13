---
audience: end-user
title: Preparación y envío de un correo electrónico
description: Obtenga información sobre cómo preparar y enviar un correo electrónico con la IU de la web de Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 95%

---


# Preparación y envío de su correo electrónico {#prepare-send}


<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Preparación del envío{#prepare}

Cuando haya definido el contenido, la audiencia y la programación, estará listo para preparar el mensaje. Durante la preparación, se calcula la población de destinatarios y se genera el contenido del mensaje para cada perfil de los destinatarios. Una vez finalizada la preparación, los mensajes están listos para enviarse, ya sea inmediatamente o en la fecha y hora programadas.

Las reglas de validación utilizadas durante la preparación de la entrega se describen en la [Documentación de Campaign v8 (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/validate/delivery-analysis.html){target="_blank"}.

Siga estos pasos:

1. En el panel de envío, haga clic en el botón **Preparar**, situado en la esquina superior derecha, y pulse confirmar.

   ![](assets/prepare.png)

   Se muestra el progreso de la preparación. En función del tamaño de la población de destinatarios, esta operación puede tardar algún tiempo.

   >[!NOTE]
   >
   >Puede detener la preparación en cualquier momento con el botón **Detener preparación**. Durante la fase de preparación, no se envían mensajes. Por lo tanto, puede iniciarla o detenerla sin riesgo alguno.

1. Cuando finalice la preparación, compruebe los indicadores claves de rendimiento (KPI). Si el número de mensajes que desea enviar no coincide con sus expectativas, modifique la audiencia y reinicie la preparación.

   ![](assets/prepare2.png)

   Estos son los diferentes KPI mostrados:

   * **Objetivo**: el número de destinatarios segmentados.
   * **Pendiente de envío**: el número de mensajes que se enviarán.
   * **Para excluir**: el número de mensajes excluidos por las reglas de tipología.

1. Haga clic en el botón **Registros** y compruebe que no haya errores. El último mensaje de registro muestra los mensajes de error y los errores. Para obtener más información, consulte esta [sección](delivery-logs.md).

   ![](assets/prepare-logs.png)

Si la preparación detecta un error crítico que impide que se realice el envío, el estado de preparación aparece como erróneo en el panel de envío.

![](assets/prepare-error.png)

Si necesita realizar cambios en el envío después de la preparación, debe reiniciar la preparación para que se tengan en cuenta esos cambios.

Una vez finalizada la preparación sin errores, el mensaje está listo para enviarse. Para obtener más información, consulte esta [sección](#send).

## Envío del mensaje{#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Entregados"
>abstract="Número de mensajes entregados correctamente. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado se basa en el número total de mensajes enviados."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Aperturas"
>abstract="Número de mensajes abiertos. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado es la proporción del número de aperturas distintas comparado con el número de mensajes enviados."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Clics"
>abstract="El número de destinatarios que hicieron clic al menos una vez en el correo electrónico. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado es la proporción del número de clics distintos en comparación con el número de mensajes entregados."


Una vez finalizada la preparación, puede enviar el mensaje. Este paso solo es necesario para los mensajes que se envían en el momento. Si el mensaje está programado, se envía en la fecha definida.

Siga estos pasos:

1. En el panel de envío, haga clic en el botón **Enviar** en la esquina superior derecha y pulse confirmar.

   ![](assets/send.png)

1. Se muestra el progreso del envío. Compruebe los KPI mostrados. También puede comprobar los registros. Para obtener más información, consulte esta [sección](delivery-logs.md).

   ![](assets/send2.png)

   Estos son los diferentes KPI mostrados:

   * **Entregados**: el número de mensajes entregados correctamente. El porcentaje mostrado se basa en el número total de mensajes enviados.
   * **Abiertos**: el número de mensajes abiertos. El porcentaje mostrado es la proporción del número de aperturas distintas comparado con el número de mensajes enviados.
   * **Clics**: el número de destinatarios que hicieron clic al menos una vez en el correo electrónico. El porcentaje mostrado es la proporción del número de clics distintos en comparación con el número de mensajes entregados.

   >[!NOTE]
   >
   >Todos los indicadores se actualizan cada cinco minutos después del inicio del envío. Los indicadores de preparación del envío son en tiempo real.

   Puede pausar el envío en cualquier momento y luego reanudarlo. Si detiene el envío mientras lo ejecuta, no podrá reanudarlo.
