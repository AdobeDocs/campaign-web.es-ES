---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 748fef18a91a61f5ed956f65762a979e7dacabf3
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 35%

---


# Principios clave de la creación de un flujo de trabajo {#gs-workflow-creation}

Con Campaign v8 Web, puede crear flujos de trabajo en un lienzo visual para diseñar procesos multicanal como segmentación, ejecución de campañas o procesamiento de archivos.

Los flujos de trabajo se pueden crear como flujos de trabajo independientes desde el menú Flujos de trabajo o directamente dentro de una campaña, en cuyo caso el flujo de trabajo se vincula a la campaña y se ejecuta junto con todos los flujos de trabajo de la otra campaña.

## ¿Qué hay dentro de un flujo de trabajo?

El diagrama de flujo de trabajo es una representación de lo que se supone que debe suceder. Describe las diversas tareas que se deben realizar y cómo se vinculan entre sí.

![](assets/workflow-example.png)

Cada flujo de trabajo contiene:

* **Actividades**: una actividad es una tarea que se va a realizar. Las distintas actividades se representan en el diagrama mediante iconos. Cada actividad tiene propiedades específicas y otras propiedades que son comunes a todas las actividades.

   En un diagrama de flujo de trabajo, una actividad determinada puede producir varias tareas, en particular cuando hay un bucle o una acción recurrente.

* **Transiciones**: las transiciones vinculan una actividad de origen a una actividad de destino y definen su secuencia.

* **Tablas de trabajo**: la tabla de trabajo contiene toda la información que transmite la transición. Cada flujo de trabajo utiliza varias tablas de trabajo. Los datos transmitidos en estas tablas se pueden utilizar en todo el ciclo de vida del flujo de trabajo.

## Pasos principales para crear un flujo de trabajo

Los pasos principales para crear flujos de trabajo son los siguientes:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-workflow.md#create">
<img alt="Posible cliente" src="assets/do-not-localize/workflow-process-1 .jpeg">
</a>
<div><a href="create-workflow.md#create"><strong>Creación del flujo de trabajo</strong>
</div>
<p>
</td>
<td>
<a href="create-workflow.md#build">
<img alt="Poco frecuente" src="assets/do-not-localize/workflow-process-2.jpeg">
</a>
<div>
<a href="create-workflow.md#build"><strong>Organización de actividades</strong></a>
</div>
<p></td>
<td>
<a href="workflow-settings.md">
<img alt="Validación" src="assets/do-not-localize/workflow-process-3.jpeg">
</a>
<div>
<a href="workflow-settings.md"><strong>Configuración avanzada (opcional)</strong></a>
</div>
<p>
</td>
<td>
<a href="start-monitor-workflows.md">
<img alt="iniciar y monitorizar flujos de trabajo" src="assets/do-not-localize/workflow-process-4.jpeg">
</a>
<div>
<a href="start-monitor-workflows.md"><strong>Inicio y monitorización de la ejecución del flujo de trabajo</strong></a>
</div>
<p>
</td>
</tr></table>