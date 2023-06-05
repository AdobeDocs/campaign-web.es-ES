---
audience: end-user
title: Uso de la actividad Flujo de trabajo Correo electrónico
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Correo electrónico
badge: label="Alpha" type="Positive"
source-git-commit: fc920737aa336bbb92b2d2ef03f997ca2eefa0bb
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 3%

---


# Correo electrónico, SMS, push {#email}

La web de Adobe Campaign le permite automatizar y ejecutar campañas de marketing en varios canales, como correo electrónico, SMS o push. Puede combinar actividades de canal en el lienzo para crear flujos de trabajo entre canales que puedan almacenar en déclencheur acciones basadas en el comportamiento del cliente.

Por ejemplo, puede crear una campaña de correo electrónico de bienvenida que incluya una serie de mensajes en diferentes canales, como correo electrónico, SMS y push. También puede enviar un correo electrónico de seguimiento después de que un cliente haya completado una compra o enviar un mensaje de cumpleaños personalizado a un cliente a través de SMS.

Mediante las actividades de canal, puede crear campañas completas y personalizadas que atraigan a los clientes en varios puntos de contacto e impulsen las conversiones.

Estos son los pasos para agregar una **Canal** actividad en un flujo de trabajo:

1. Asegúrese de haber agregado un **Crear audiencia** actividad. La audiencia es el destinatario principal de la entrega: los destinatarios que reciben los mensajes. Al enviar mensajes en el contexto de un flujo de trabajo de campaña, la audiencia del mensaje no se define en la actividad del canal, sino en el flujo de trabajo **Crear audiencia** actividad. Consulte [esta sección](build-audience.md).

   ![](../../msg/assets/add-delivery-in-wf.png)

1. Seleccione una actividad de entrega: **[!UICONTROL Correo electrónico]**, **[!UICONTROL SMS]**, **[!UICONTROL Notificación push (Android)]** o **[!UICONTROL Notificación push (iOS)]**.

1. Inicie el flujo de trabajo y compruebe los registros.






<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Los destinatarios del correo electrónico se definen antes de la actividad en el mismo flujo de trabajo, a través de una actividad de segmentación de audiencia.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
