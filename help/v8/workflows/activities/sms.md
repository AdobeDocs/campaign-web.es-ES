---
audience: end-user
title: Uso de la actividad SMS workflow
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo SMS
badge: label="Alpha" type="Positive"
source-git-commit: c0e5902d3ee504aa5aa4e55f18416facfe4020b1
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 3%

---


# SMS {#sms}

El **SMS** proporciona la funcionalidad para enviar mensajes SMS dentro de un flujo de trabajo. Permite la automatización de la entrega de SMS a un destinatario específico determinado dentro del mismo flujo de trabajo.

Para definir los destinatarios del SMS, puede configurarlos antes de la actividad de envío de SMS en el flujo de trabajo mediante la actividad de creación de audiencia. Más información.

1. Después de crear y configurar un nuevo flujo de trabajo, añada una actividad Generar audiencia para seleccionar una audiencia existente o utilice el generador de reglas para definir su propia consulta.

1. Añada una actividad del canal SMS al flujo de trabajo.

   ![](../assets/activity-sms-1.png)
<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the SMS to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the SMS to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the SMS to be sent at regular intervals.
-->

1. Seleccione su actividad. En el menú de envío, seleccione las plantillas que desee utilizar para este envío. Más información sobre las plantillas

1. Haga clic en Crear envío para configurar el envío de SMS. Para obtener más información sobre la entrega de SMS, consulte esta página.

1. Una vez que la entrega esté lista para enviarse, vuelva al flujo de trabajo y haga clic en Start para iniciar el flujo de trabajo.

1. De forma predeterminada, el inicio de un flujo de trabajo de entrega déclencheur la fase de preparación del mensaje, sin enviarlo inmediatamente.

   Haga clic en Revisar y enviar en el menú avanzado de la actividad de SMS para confirmar el envío.

1. En el panel de entregas de SMS, haga clic en Send.
