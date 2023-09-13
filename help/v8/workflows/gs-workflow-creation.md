---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
badge: label="Beta"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 5c4ace1fc8d299048c398fcce14900c797ef6207
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 62%

---


# Principios clave de la creación de un flujo de trabajo {#gs-workflow-creation}

Con Campaign v8 Web, puede crear flujos de trabajo en un lienzo visual para diseñar procesos multicanal como segmentación, ejecución de campañas o procesamiento de archivos.

Los flujos de trabajo se pueden crear como flujos de trabajo independientes desde el **Flujos de trabajo** o directamente dentro de una campaña, en cuyo caso el flujo de trabajo se vincula a la campaña y se ejecuta junto con todos los flujos de trabajo de la otra campaña.

## ¿Qué hay dentro de un flujo de trabajo? {#gs-workflow-inside}

El diagrama de flujo de trabajo es una representación de lo que se supone que debe suceder. Describe las diversas tareas que se realizan y cómo se relacionan entre sí.

![](assets/workflow-example.png)

Cada flujo de trabajo contiene:

* **Actividades**: una Actividad es una tarea que se va a realizar. Las distintas actividades disponibles se representan en el diagrama mediante iconos. Cada actividad tiene propiedades específicas y otras propiedades que son comunes a todas las actividades.

  En un diagrama de flujo de trabajo, una actividad determinada puede producir varias tareas, en particular cuando hay un bucle o una acción recurrente.

* **Transiciones**: las transiciones vinculan una actividad de origen a una actividad de destino y definen su secuencia.

* **Tablas de trabajo**: la tabla de trabajo contiene toda la información que transmite la transición. Cada flujo de trabajo utiliza varias tablas de trabajo. Los datos transmitidos en estas tablas se pueden utilizar en todo el ciclo de vida del flujo de trabajo.

## Pasos clave para crear un flujo de trabajo {#gs-workflow-steps}

Los pasos clave para crear flujos de trabajo son los siguientes:

![](assets/workflow-creation-process.png)

Estos pasos se detallan en la siguiente sección:

1. [Cree el flujo de trabajo y defina sus propiedades](create-workflow.md)
1. [Organización y configuración de actividades](orchestrate-activities.md)
1. [Configuración avanzada del flujo de trabajo](workflow-settings.md)
1. [Inicie el flujo de trabajo y monitorice su ejecución](start-monitor-workflows.md)

