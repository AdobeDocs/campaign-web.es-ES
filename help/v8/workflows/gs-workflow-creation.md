---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 59%

---


# Principios clave de la creación de un flujo de trabajo {#gs-workflow-creation}

Con Campaign v8 Web, puede crear flujos de trabajo en un lienzo visual para diseñar procesos multicanal como segmentación, ejecución de campañas o procesamiento de archivos.

Los flujos de trabajo se pueden crear como flujos de trabajo independientes, desde el menú Flujos de trabajo o desde una campaña, desde el menú Campañas.

Por determinar: detallar las características específicas entre los flujos de trabajo de la campaña independientes.

## ¿Qué hay dentro de un flujo de trabajo?

El diagrama de flujo de trabajo es una representación de lo que se supone que debe suceder. Describe las diversas tareas que se deben realizar y cómo se vinculan entre sí.

Cada flujo de trabajo contiene:

* **Actividades**: una actividad es una tarea que se va a realizar. Las distintas actividades se representan en el diagrama mediante iconos. Cada actividad tiene propiedades específicas y otras propiedades que son comunes a todas las actividades.

   En un diagrama de flujo de trabajo, una actividad determinada puede producir varias tareas, en particular cuando hay un bucle o una acción recurrente.

* **Transiciones**: las transiciones vinculan una actividad de origen a una actividad de destino y definen su secuencia.

* **Tablas de trabajo**: la tabla de trabajo contiene toda la información que transmite la transición. Cada flujo de trabajo utiliza varias tablas de trabajo. Los datos transmitidos en estas tablas pueden acelerarse y utilizarse en todo el ciclo de vida del flujo de trabajo, siempre y cuando no se depure. De hecho, las tablas innecesarias se depuran cada vez que se desactiva el flujo de trabajo y posiblemente durante la ejecución de los flujos de trabajo más grandes para evitar sobrecargar el servidor.

## Pasos principales para crear un flujo de trabajo

Los pasos principales para crear flujos de trabajo son los siguientes:

Por determinar: gráfico que muestra todo el proceso con explicación y referencia a páginas de documentos.

Cree y defina propiedades > orqueste actividades en el lienzo > configure los ajustes si es necesario > inicie la ejecución y monitorice