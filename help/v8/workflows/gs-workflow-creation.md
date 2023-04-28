---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: d7e19b2d8730cacbbff1ad42f1956b32c84a309a
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 32%

---


# Principios clave de la creación del flujo de trabajo {#gs-workflow-creation}

contenido TBD

Un flujo de trabajo es una definición de proceso: el diagrama de flujo de trabajo, que es una representación de lo que se supone que debe suceder. Un flujo de trabajo también es una instancia de este proceso: una instancia de flujo de trabajo, que es una representación de lo que realmente está ocurriendo.

La plantilla de flujo de trabajo describe las diversas tareas que se realizan y cómo se relacionan entre sí. Las plantillas de tareas se denominan actividades y se representan mediante iconos. Se vinculan entre sí mediante transiciones.

captura de pantalla del TBD

## ¿Qué hay dentro de un flujo de trabajo?

Cada flujo de trabajo contiene:

* **Actividades**: Una actividad describe una plantilla de tarea. Las distintas actividades disponibles se representan en el diagrama mediante iconos. Cada tipo tiene propiedades comunes y propiedades específicas.

   En un diagrama de flujo de trabajo, una actividad determinada puede producir varias tareas, en particular cuando hay un bucle o acciones recurrentes.

* **Transiciones**: Las transiciones permiten vincular actividades y definir su secuencia. Una transición vincula una actividad de origen a una actividad de destino.

* **Tablas de trabajo**: La tabla de trabajo contiene toda la información que transmite la transición. Cada flujo de trabajo utiliza varias tablas de trabajo. Los datos transmitidos en estas tablas se pueden acelerar y utilizar en todo el ciclo de vida del flujo de trabajo, siempre que no se depure. De hecho, las tablas innecesarias se depuran cada vez que se desactiva el flujo de trabajo y posiblemente durante la ejecución de los flujos de trabajo más grandes para evitar sobrecargar el servidor.

## Flujos de trabajo independientes y de campaña

Los flujos de trabajo se pueden crear como flujos de trabajo independientes o desde una campaña.

TBD: detalle las características específicas entre los flujos de trabajo independientes y los flujos de trabajo de campaña.

## Pasos principales para crear un flujo de trabajo

Los pasos principales para crear flujos de trabajo son los siguientes:

TBD: gráfico que muestra todo el proceso con explicación y referencia a páginas doc

cree y defina propiedades > orqueste actividades en el lienzo > configure la configuración si es necesario > inicie la ejecución y monitorice