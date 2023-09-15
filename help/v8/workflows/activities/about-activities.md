---
audience: end-user
title: Trabajar con actividades de flujos de trabajo
description: Aprenda a trabajar con las actividades de flujo de trabajo
badge: label="Beta"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 100%

---


# Acerca de las actividades de flujo de trabajo {#workflow-activities}

Las actividades de flujo de trabajo se agrupan en tres categorías. Dependiendo del contexto, las actividades disponibles pueden diferir.

Todas las actividades se detallan en las secciones siguientes:

* [Actividades de segmentación](#targeting)
* [Actividades del canal](#channel)
* [Actividades de control de flujo](#flow-control)

![](../assets/workflow-activities.png)

## Actividades de segmentación {#targeting}

Estas actividades son específicas para la segmentación, manipulación y enriquecimiento de los datos de la población. Le permiten crear uno o más públicos destinatarios al definir públicos y dividirlos o combinarlos mediante operaciones de intersección, unión o exclusión.

* La actividad [Generar público destinatario](build-audience.md) le permite definir la población de público destinatario. Puede seleccionar un público destinatario existente o utilizar el generador de reglas para definir su propia consulta.
* La actividad [Combinar](combine.md) le permite realizar la segmentación de la población entrante. Puede utilizar una unión, una intersección o una exclusión.
* La actividad [Enriquecimiento](enrichment.md) le permite definir datos adicionales para procesarlos en el flujo de trabajo. Con esta actividad, puede aprovechar la transición entrante y configurar la actividad para completar la transición saliente con datos adicionales.
* La actividad [División](split.md) le permite segmentar la población entrante en varios subconjuntos.

## Actividades del canal {#channel}

Adobe Campaign Web le permite automatizar y ejecutar campañas de marketing en varios canales, como correo electrónico, SMS o push. Puede combinar actividades del canal en el lienzo para crear flujos de trabajo entre canales que puedan activar acciones basadas en el comportamiento del cliente.

Están disponibles las siguientes actividades del **Canal**:

* Correo electrónico
* Push
* SMS

Consulte esta [sección](channels.md).

## Actividades de control de flujo {#flow-control}


>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Actividad final"
>abstract="La actividad **Finalizar** le permite marcar de forma gráfica el final de un flujo de trabajo. Esta actividad no tiene impacto funcional y, por lo tanto, es opcional."

Las siguientes actividades son específicas para organizar y ejecutar flujos de trabajo. Su tarea principal es coordinar las otras actividades:

* La actividad [Combinación-Y](and-join.md) le permite sincronizar varias ramas de ejecución de un flujo de trabajo.
* La actividad **Finalizar** le permite marcar de forma gráfica el final de un flujo de trabajo. Esta actividad no tiene impacto funcional y, por lo tanto, es opcional.
* La actividad [Tenedor](fork.md) permite crear transiciones salientes para iniciar varias actividades al mismo tiempo.
* La actividad [Esperar](wait.md) suspende momentáneamente la ejecución de una parte de un flujo de trabajo.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

