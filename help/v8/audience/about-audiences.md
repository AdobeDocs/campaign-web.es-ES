---
audience: end-user
title: Introducción a los públicos
description: Aprenda a utilizar audiencias en la IU de la web de Campaign
badge: label="Beta"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 100%

---


# Introducción a los públicos {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


El público destinatario es el destinatario principal de su envío: los destinatarios que reciben los mensajes. El tipo de público destinatario depende de la asignación de destino definida en la plantilla de envíos. Descubra qué es una plantilla de envíos [en esta sección](../msg/delivery-template.md).

Para definir la población de público destinatario, puede hacer lo siguiente:

* Seleccione un público destinatario existente, creado como una lista en la consola del cliente. [Más información](add-audience.md)
* Seleccionar un público destinatario de Adobe Experience Platform. [Más información](aep-audience.md)
* Cree un nuevo público destinatario con el generador de reglas definiendo y combinando criterios de filtrado. [Más información](segment-builder.md)
* Usar un público destinatario desde un archivo externo: esta opción solo está disponible para envíos de correo electrónico independientes y no se puede utilizar en entregas de campañas. [Más información](file-audience.md)

Al enviar mensajes en el contexto de un flujo de trabajo de campaña, el público destinatario se define en una actividad de flujo de trabajo **Leer público destinatario** específica. En este contexto, no se puede cargar un público destinatario de un archivo para un envío de correo electrónico, y el público destinatario se define solo en esta actividad dedicada. Obtenga información sobre cómo definir el público destinatario de su envío en un flujo de trabajo de campaña [en esta sección](../workflows/orchestrate-activities.md).

Además, puede utilizar grupos de control para evitar el envío de mensajes a una parte de la audiencia a fin de medir el impacto de sus campañas. [Más información](control-group.md)

![](assets/about-audience.png)

