---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 3b193cf7116859f31ce04ba89773ef388b7916c7
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 77%

---


# Principios clave de la creación de un flujo de trabajo {#gs-workflow-creation}

Con Campaign v8 Web, puede crear flujos de trabajo en un lienzo visual para diseñar procesos multicanal como segmentación, ejecución de campañas o procesamiento de archivos.

Los flujos de trabajo se pueden crear como flujos de trabajo independientes desde el menú Flujos de trabajo o directamente dentro de una campaña, en cuyo caso el flujo de trabajo se vincula a la campaña y se ejecuta junto con todos los flujos de trabajo de la otra campaña.

## ¿Qué hay dentro de un flujo de trabajo?

El diagrama de flujo de trabajo es una representación de lo que se supone que debe suceder. Describe las diversas tareas que se realizan y cómo se relacionan entre sí.

![](assets/workflow-example.png)

Cada flujo de trabajo contiene:

* **Actividades**: una Actividad es una tarea que se va a realizar. Las distintas actividades disponibles se representan en el diagrama mediante iconos. Cada actividad tiene propiedades específicas y otras propiedades que son comunes a todas las actividades.

   En un diagrama de flujo de trabajo, una actividad determinada puede producir varias tareas, en particular cuando hay un bucle o una acción recurrente.

* **Transiciones**: las transiciones vinculan una actividad de origen a una actividad de destino y definen su secuencia.

* **Tablas de trabajo**: la tabla de trabajo contiene toda la información que transmite la transición. Cada flujo de trabajo utiliza varias tablas de trabajo. Los datos transmitidos en estas tablas se pueden utilizar en todo el ciclo de vida del flujo de trabajo.

## Pasos principales para crear un flujo de trabajo

Los pasos principales para crear flujos de trabajo son los siguientes:

![](assets/workflow-creation-process.png)
