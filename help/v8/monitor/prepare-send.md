---
audience: end-user
title: Preparación y envío de un correo electrónico
description: Obtenga información sobre cómo preparar y enviar un correo electrónico con la interfaz de usuario web de Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: 1a7ed05b974e72b76cf8a48e36ae86bd166db048
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 7%

---

# Prepare y envíe su correo electrónico {#prepare-send}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Prepare y envíe su correo electrónico"
>abstract="Descubra cómo preparar su correo electrónico y obtener más información sobre cómo enviar KPI."

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

Cuando haya definido el contenido, la audiencia y la programación, estará listo para preparar el mensaje. Durante la preparación, se calcula la población objetivo y el contenido del mensaje se genera para cada perfil incluido en el objetivo. Una vez finalizada la preparación, los mensajes están listos para enviarse, ya sea inmediatamente o en la fecha y hora programadas. Las reglas de validación utilizadas durante el análisis se describen en la sección [Documentación de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies){target="_blank"}.

Siga estos pasos:

1. En el panel de envío, haga clic en el botón **Preparación** situado en la esquina superior derecha y confirme.

   ![](assets/prepare.png)

   Se muestra el progreso de la preparación. En función del tamaño de la población de destino, esta operación puede tardar algún tiempo.

   >[!NOTE]
   >
   >Puede detener la preparación en cualquier momento utilizando la variable **Detener preparación** botón. Durante la fase de preparación, no se envían mensajes. Por lo tanto, puede iniciar o detener esto sin riesgo de afectar a nada.

1. Cuando finalice la preparación, compruebe los KPI. Si el número de mensajes que desea enviar no coincide con sus expectativas, modifique la audiencia y reinicie la preparación.

   ![](assets/prepare2.png)

   Estos son los diferentes KPI mostrados:

   * **Segmentado**: el número de destinatarios objetivo
   * **Para entregar**: el número de mensajes que se enviarán
   * **Para excluir**: el número de mensajes excluidos por una regla de tipología

1. Haga clic en el **Registros** y compruebe que no hay error. El último mensaje de “log” muestra los mensajes de error y el número de errores. Para obtener más información, consulte esta [sección](delivery-logs.md).

   ![](assets/prepare-logs.png)

Si la preparación detecta un error crítico que impide que se envíe la entrega, el estado de preparación aparece como fallido en el panel de envío.

![](assets/prepare-error.png)

Si necesita realizar cambios en el envío después de la preparación, debe reiniciar la preparación para que se tengan en cuenta esos cambios.

Una vez finalizada la preparación sin errores, el mensaje está listo para enviarse. Para obtener más información, consulte esta [sección](#send).

## Envío del mensaje{#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Entrega"
>abstract="Número de mensajes enviados correctamente. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado se basa en el número total de mensajes enviados."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Aperturas"
>abstract="Número de mensajes abiertos. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado es la relación entre el número de aperturas distintas comparado con el número de mensajes enviados."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Clics"
>abstract="El número de destinatarios que hicieron clic al menos una vez en el correo electrónico. Este indicador se actualiza cada 5 minutos. El porcentaje mostrado es la proporción del número de clics distintos comparados con el número de mensajes enviados."


Una vez finalizada la preparación, ahora puede enviar el mensaje. Este paso solo es necesario para los mensajes enviados inmediatamente. Si el mensaje está programado, se envía en la fecha definida.

Siga estos pasos:

1. En el panel de envío, haga clic en el botón **Enviar** en la esquina superior derecha y confirme.

   ![](assets/send.png)

1. Se muestra el progreso de envío. Compruebe los KPI mostrados. También puede comprobar los registros. Para obtener más información, consulte esta [sección](delivery-logs.md).

   ![](assets/send2.png)

   Estos son los diferentes KPI mostrados:

   * **Entrega**: el número de mensajes enviados correctamente. El porcentaje mostrado se basa en el número total de mensajes enviados.
   * **Aperturas**: el número de mensajes abiertos. El porcentaje mostrado es la relación entre el número de aperturas distintas comparado con el número de mensajes enviados.
   * **Clics**: el número de destinatarios que hicieron clic al menos una vez en el correo electrónico. El porcentaje mostrado es la proporción del número de clics distintos comparados con el número de mensajes enviados.

   >[!NOTE]
   >
   >Todos los indicadores se actualizan cada 5 minutos después del inicio del envío. Los indicadores de preparación de envíos son en tiempo real.

   Puede pausar el envío en cualquier momento y luego reanudarlo. Si detiene el envío mientras se está enviando, no puede reanudarlo.
