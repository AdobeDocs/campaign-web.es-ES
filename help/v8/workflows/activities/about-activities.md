---
audience: end-user
title: Trabajar con actividades de flujos de trabajo
description: Aprenda a trabajar con las actividades de flujo de trabajo
badge: label="Disponibilidad limitada"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 35%

---


# Acerca de las actividades de flujo de trabajo {#workflow-activities}

Las actividades de flujo de trabajo se agrupan en tres categorías. Dependiendo del contexto, las actividades disponibles pueden diferir.

Todas las actividades se detallan en las secciones siguientes:

* [Actividades de segmentación y administración de datos](#targeting)
* [Actividades del canal](#channel)
* [Actividades de control de flujo](#flow-control)

![](../assets/workflow-activities.png)

## Actividades de segmentación y administración de datos {#targeting}

Estas actividades son específicas para la segmentación, manipulación y enriquecimiento de los datos de la población. Le permiten crear uno o más públicos destinatarios al definir públicos y dividirlos o combinarlos mediante operaciones de intersección, unión o exclusión.

* Utilice el [Guardar audiencia](save-audience.md) actividad para actualizar una audiencia existente o crear una nueva a partir de la población calculada en sentido ascendente en un flujo de trabajo.
* Utilice el [Crear audiencia](build-audience.md) actividad para definir la población objetivo. Puede seleccionar una audiencia existente o utilizar el modelador de consultas para definir su propia consulta.
* Utilice el [Combinar](combine.md) actividad para realizar la segmentación en la población entrante. Puede utilizar una unión, una intersección o una exclusión.
* Utilice el [Split](split.md) actividad para segmentar la población entrante en varios subconjuntos.
* Utilice el [Reconciliación](reconciliation.md) actividad para definir el vínculo entre los datos de la base de datos de Adobe Campaign y los datos de una tabla de trabajo, por ejemplo, los datos cargados desde un archivo externo.
* Utilice el [Enriquecimiento](enrichment.md) actividad para definir datos adicionales que procesar en el flujo de trabajo. Con esta actividad, puede aprovechar la transición entrante y configurar la actividad para completar la transición saliente con datos adicionales.
* Utilice el [Deduplicación](deduplication.md) actividad para eliminar duplicados en los resultados de las actividades entrantes.
* Utilice el [Cambiar dimensión](change-dimension.md) actividad para cambiar la dimensión de segmentación mientras crea el flujo de trabajo.
* Utilice el [Cargar archivo](load-file.md) actividad para trabajar con perfiles y datos almacenados en un archivo externo.


## Actividades del canal {#channel}

Adobe Campaign Web le permite automatizar y ejecutar campañas de marketing en varios canales. Puede combinar actividades de canal en el lienzo para crear flujos de trabajo entre canales que puedan almacenar en déclencheur acciones basadas en el comportamiento del cliente. Lo siguiente **Canal** Hay actividades disponibles: notificaciones push por correo electrónico, SMS, Android y iOS. [Obtenga información sobre cómo configurar una entrega en el contexto de un flujo de trabajo](channels.md).

## Actividades de control de flujo {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Actividad final"
>abstract="La actividad **Finalizar** le permite marcar de forma gráfica el final de un flujo de trabajo. Esta actividad no tiene impacto funcional y, por lo tanto, es opcional."

Las siguientes actividades son específicas para organizar y ejecutar flujos de trabajo. Su tarea principal es coordinar las otras actividades:

* Utilice el [Planificador](scheduler.md) actividad para programar cuándo se inicia el flujo de trabajo.
* Utilice el [And-join](and-join.md) actividad para sincronizar varias ramas de ejecución de un flujo de trabajo.
* Añadir un **Fin** actividad para marcar de forma gráfica el final de un flujo de trabajo. Esta actividad no tiene impacto funcional y, por lo tanto, es opcional.
* Utilice el [Tenedor](fork.md) actividad para crear transiciones salientes e iniciar varias actividades al mismo tiempo.
* Añadir un [Esperar](wait.md) para pausar momentáneamente la ejecución de una parte de un flujo de trabajo.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

