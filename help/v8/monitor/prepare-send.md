---
audience: end-user
title: Preparación y envío de un correo electrónico
description: Documentación web de Campaign v8
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 13%

---

# Prepare y envíe su correo electrónico {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Prepare y envíe su correo electrónico"
>abstract="Descubra cómo preparar su correo electrónico y obtener más información sobre cómo enviar KPI."

>[!NOTE]
>
>Esta documentación está en construcción y se actualiza con frecuencia. La versión final de este contenido estará lista en enero de 2023.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Preparación del envío

Durante la preparación, se calcula la población objetivo y el contenido del mensaje generado para cada perfil incluido en el objetivo. Una vez finalizada la preparación, los mensajes están listos para enviarse, ya sea inmediatamente o en la fecha y hora programadas. Las reglas de validación utilizadas durante el análisis se describen en [sección](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. Haga clic en el **Preparación** situado en la esquina superior derecha.

1. Se muestra el progreso de la preparación. En función del tamaño de la población de destino, esta operación puede tardar algún tiempo.

   >[!NOTE]
   >
   >Puede detener la preparación en cualquier momento utilizando la variable **Detener preparación** botón. Durante la fase de preparación, no se envían mensajes. Por lo tanto, puede iniciar o detener esto sin riesgo de afectar a nada.

1. Cuando finalice la preparación, compruebe la **Segmentado**, **Para entregar** y **Para excluir** KPI. Si el número de mensajes que desea enviar no coincide con sus expectativas, modifique la audiencia y reinicie la preparación.

1. Haga clic en el **Registros** y compruebe que no hay error. Se muestran todos los pasos, advertencias y errores de validación. Los iconos de color muestran el tipo de mensaje:

   * El icono gris indica un mensaje informativo.
   * El icono amarillo indica un error de procesamiento no crítico.
   * El icono rojo indica un error crítico que impide realizar el envío.

1. Después de realizar los cambios, reinicie la preparación.

Una vez finalizada la preparación, el mensaje está listo para enviarse. Para obtener más información, consulte Confirmación de envío.


## Envío del mensaje

Una vez finalizada la preparación, siga los pasos a continuación para enviar el mensaje.

1. Haga clic en el **Botón Enviar** en la esquina superior derecha y confirme.

1. El progreso de envío se muestra junto con tres KPI: Entregado, Aperturas, Clics.

1. Finalice el envío haciendo clic en el botón OK .

REGISTROS

>[!NOTE]
>
>Si el mensaje está programado, se envía cuando se llega a la hora de envío. Para obtener más información sobre la programación de mensajes, consulte esta sección.

