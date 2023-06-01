---
audience: end-user
title: Uso de la actividad de flujo de trabajo Generar audiencia
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Crear audiencia
badge: label="Alpha" type="Positive"
source-git-commit: 9b639a533e75822570d6cc2b9752fc9380d069dd
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 12%

---


# Generar público destinatario {#build-audience}

Esta actividad le permite definir una audiencia. Puede seleccionar una audiencia existente o utilizar el generador de reglas para definir su propia consulta.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuración

Siga estos pasos para configurar el **Crear audiencia** actividad:

1. Añada una actividad Build audience.
1. Defina una etiqueta.
1. Defina el tipo de audiencia: **Cree su propio** o **Leer audiencia**.

Para crear su propia consulta, siga estos pasos adicionales:

1. Seleccionar **Cree su propio (consulta)**.
1. Elija la **Dimensión de segmentación**. La dimensión de segmentación permite definir la población objetivo de la operación: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. De forma predeterminada, el objetivo se selecciona en los destinatarios. Consulte la [Documentación de v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Haga clic en **Continue**.
1. Utilice el generador de reglas para definir la consulta, del mismo modo que crea una audiencia al diseñar un nuevo correo electrónico. Consulte esta [sección](../../audience/segment-builder.md).

Para seleccionar una audiencia existente, siga estos pasos:

1. Seleccionar **Leer audiencia**.
1. Haga clic en **Continue**.
1. Seleccione la audiencia, del mismo modo que utiliza una audiencia cuando diseña un nuevo correo electrónico. Consulte esta [sección](../../audience/add-audience.md).

## Ejemplo

Este es un ejemplo de flujo de trabajo con dos **Crear audiencia** actividades. El primero se dirige a la audiencia de jugadores de póquer, seguido de una entrega de correo electrónico. VIP El segundo se dirige a la audiencia de clientes de la red de distribución de correo electrónico, seguido de una entrega de SMS.

![](../assets/workflow-audience-example.png)