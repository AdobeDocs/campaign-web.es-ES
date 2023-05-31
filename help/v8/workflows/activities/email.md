---
audience: end-user
title: Uso de la actividad Flujo de trabajo Correo electrónico
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Correo electrónico
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 46%

---


# Correo electrónico {#email}

Descripción, qué caso de uso puede realizar (otras actividades comunes que puede vincular antes o después de la actividad)

Cómo añadir y configurar la actividad

Ejemplo de una actividad configurada dentro de un flujo de trabajo


La actividad Entrega de correo electrónico permite configurar la entrega de un correo electrónico en un flujo de trabajo.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Los destinatarios del correo electrónico se definen antes de la actividad en el mismo flujo de trabajo, a través de una actividad de segmentación de audiencia.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
