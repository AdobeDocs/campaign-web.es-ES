---
audience: end-user
title: Uso de la actividad de flujo de trabajo Notificación push
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo de notificaciones push
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 4%

---


# Notificación push {#push-activity}

El **Notificación push** la actividad de entrega permite configurar el envío de una notificación push en un flujo de trabajo.

>[!BEGINTABS]

>[!TAB Notificación push (Android)]

1. Después de crear y configurar un nuevo flujo de trabajo, añada una actividad Generar audiencia para seleccionar una audiencia existente o utilice el generador de reglas para definir su propia consulta.

1. Añada una actividad de canal de notificaciones push (Android) al flujo de trabajo.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Seleccione su actividad. En el menú de envío, seleccione las plantillas que desee utilizar para este envío. Más información sobre las plantillas

1. Haga clic en Create delivery para configurar la entrega de las notificaciones push. Para obtener más información sobre la entrega de notificaciones push (Android), consulte esta página.

1. Una vez que la entrega esté lista para enviarse, vuelva al flujo de trabajo y haga clic en Start para iniciar el flujo de trabajo.

1. De forma predeterminada, el inicio de un flujo de trabajo de entrega déclencheur la fase de preparación del mensaje, sin enviarlo inmediatamente.

   Haga clic en Revisar y enviar en el menú avanzado de la actividad del canal de notificaciones push (Android) para confirmar el envío.

1. En el panel de envío de notificaciones push, haga clic en Enviar.

>[!TAB Notificación push (iOS)]

1. Después de crear y configurar un nuevo flujo de trabajo, añada una actividad Generar audiencia para seleccionar una audiencia existente o utilice el generador de reglas para definir su propia consulta.

1. Añada una actividad de canal de notificaciones push (iOS) al flujo de trabajo.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Seleccione su actividad. En el menú de envío, seleccione las plantillas que desee utilizar para este envío. Más información sobre las plantillas

1. Haga clic en Create delivery para configurar la entrega de las notificaciones push. Para obtener más información sobre la entrega de notificaciones push (iOS), consulte esta página.

1. Una vez que la entrega esté lista para enviarse, vuelva al flujo de trabajo y haga clic en Start para iniciar el flujo de trabajo.

1. De forma predeterminada, el inicio de un flujo de trabajo de entrega déclencheur la fase de preparación del mensaje, sin enviarlo inmediatamente.

   Haga clic en Revisar y enviar en el menú avanzado de la actividad del canal de notificaciones push (iOS) para confirmar el envío.

1. En el panel de envío de notificaciones push, haga clic en Enviar.

>[!ENDTABS]