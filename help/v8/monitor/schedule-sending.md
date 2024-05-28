---
audience: end-user
title: Programar el envío de una entrega
description: Obtenga información sobre cómo programar una entrega
source-git-commit: 7bee82ea7286fca3398bef9f84f3c5aa1e3d9959
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 6%

---

# Programar el envío de una entrega {#schedule-sending}

Puede programar el envío de una entrega. Los pasos dependerán de si se trata de una entrega independiente (única) o si está trabajando en el contexto de un flujo de trabajo de campaña.

## Envío independiente

Para las entregas independientes, puede programar directamente la fecha y la hora de la entrega.
Consulte los siguientes ejemplos para cada tipo de entrega: correo electrónico, SMS, notificación push.

### Correo electrónico {#schedule-email-standalone}

Para programar el envío de un envío de correo electrónico, siga los pasos a continuación:

1. En el **[!UICONTROL Programación]** de las propiedades de envío, active la variable **[!UICONTROL Habilitar programación]** alternar

1. Defina la fecha y la hora deseadas para el envío y haga clic en **[!UICONTROL Revisar y enviar]** botón.

   ![](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>De forma predeterminada, está activada la opción **[!UICONTROL Habilitar confirmación antes de enviar]**. Esta opción requiere que confirme el envío antes de que el correo electrónico se envíe en la fecha y hora programadas. Si es necesario **realizar la entrega automáticamente** en la fecha y la hora programadas, debe desactivar esta opción.
>

1. Compruebe que la programación es correcta y haga clic en **[!UICONTROL Preparar]** botón.

![](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. Una vez completada la preparación, los mensajes están listos para enviarse. Se muestran las métricas clave para la entrega: población objetivo total, número de mensajes que desea enviar, número de destinatarios excluidos. Haga clic en **[!UICONTROL Enviar como está programado]** para confirmar que permite que la entrega se envíe en la fecha y hora programadas al objetivo principal.

![](assets/schedule-email-standalone-send.png){zoomable="yes"}


### Sms

Para programar la entrega de SMS a una fecha y hora específicas, los pasos son los mismos que para las entregas por correo electrónico, [véase más arriba](#schedule-email-standalone).

![](assets/schedule-sms-standalone.png){zoomable="yes"}

También puede comprobar que el programa se tiene en cuenta:

![](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### Notificación push

Para programar una entrega push independiente a una fecha y hora específicas, los pasos son los mismos que para las entregas por correo electrónico. [véase más arriba](#schedule-email-standalone).

![](assets/schedule-push-standalone.png){zoomable="yes"}

También puede comprobar que el programa se tiene en cuenta:

![](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### Envío independiente en una campaña

Puede crear una entrega independiente dentro de una campaña sin utilizar un flujo de trabajo. Puede configurar la fecha y la hora programadas para este envío, tal como se explica más arriba.
La campaña puede tener su programación, con una fecha de inicio y una fecha de finalización. Esta programación no interferirá con su programación de entregas.

![](assets/schedule-delivery-standalone.png){zoomable="yes"}

## Programar una entrega en un flujo de trabajo de campaña

En el contexto de un flujo de trabajo de campaña, la variable **práctica recomendada** es utilizar el **[!UICONTROL Planificador]** actividad para aplicar una fecha y hora en la que se iniciará el flujo de trabajo, incluido el envío de la entrega. [Más información sobre el Planificador](../workflows/activities/scheduler.md)

![](assets/schedule-workflow.png){zoomable="yes"}


Debe configurar la fecha y la hora en la variable **[!UICONTROL Planificador]** actividad.

![](assets/schedule-workflow-scheduler.png){zoomable="yes"}


>[!NOTE]
>
>Cuando se usa la variable **[!UICONTROL Planificador]** actividad para programar el envío de su envío en un flujo de trabajo, **no activar** el **[!UICONTROL Habilitar programación]** alternar en **[!UICONTROL Envío]** configuración de actividades. Su envío se enviará automáticamente.
>

En caso de que active la variable **[!UICONTROL Habilitar programación]** alternar en **[!UICONTROL Envío]** configuración de actividad y establezca una fecha y hora allí, la entrega esperará a realizarse en esta fecha y hora. Esto significa que si hay un retraso entre la fecha de inicio del flujo de trabajo y la fecha de envío, es posible que la audiencia no esté actualizada.

