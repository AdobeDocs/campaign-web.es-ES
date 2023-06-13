---
audience: end-user
title: Introducción a las audiencias
description: Aprenda a utilizar audiencias en la IU de la web de Campaign
badge: label="Alfa"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 30%

---


# Introducción a las audiencias {#about-audiences}

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


La audiencia es el destinatario principal de la entrega: los destinatarios que reciben los mensajes. El tipo de audiencia depende de la asignación de destino definida en la plantilla de envíos. Descubra qué es una plantilla de envíos [en esta sección](../msg/delivery-template.md).

Para definir la población de audiencias, puede:

* Seleccione una audiencia existente, creada como lista en la consola del cliente. [Más información](add-audience.md)
* Seleccione una audiencia de Adobe Experience Platform. [Más información](aep-audience.md)
* Cree una nueva audiencia con el generador de reglas definiendo y combinando criterios de filtrado. [Más información](segment-builder.md)
* Use an audience from an external file: esta opción solo está disponible para envíos de correo electrónico independientes y no se puede utilizar en envíos de campañas. [Más información](file-audience.md)

Al enviar mensajes en el contexto de un flujo de trabajo de campaña, la audiencia se define en una **Leer audiencia** actividad de flujo de trabajo. En este contexto, no se puede cargar una audiencia de un archivo para una entrega de correo electrónico, y la audiencia se define solo en esta actividad dedicada. Obtenga información sobre cómo definir la audiencia de su envío en un flujo de trabajo de la campaña [en esta sección](../workflows/orchestrate-activities.md).

Además, puede utilizar grupos de control para evitar el envío de mensajes a una parte de la audiencia a fin de medir el impacto de sus campañas. [Más información](control-group.md)

![](assets/about-audience.png)

