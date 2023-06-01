---
audience: end-user
title: Uso de la actividad de flujo de trabajo Espera
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Espera
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 42%

---


# Espera {#wait}

El **Esperar** la actividad suspende momentáneamente la ejecución de una parte de un flujo de trabajo. Activa su transición saliente después de un retraso que puede oscilar entre unos segundos y varios meses, lo que ejecuta las actividades posteriores.

El **Esperar** se utiliza para permitir que transcurra un cierto tiempo entre dos actividades que se están ejecutando. Por ejemplo, para esperar varios días después de una actividad de envío de correo electrónico y, después, analizar las aperturas y los clics generados durante este período antes de realizar cualquier operación de seguimiento (correo electrónico de recordatorio, creación de una audiencia, etc.).

## Configuración

Siga estos pasos para configurar el **Esperar** actividad:

1. Añadir un **Esperar** en el flujo de trabajo.

1. Especifique el **Duración** de la espera entre la activación de las transiciones de entrada y salida de la actividad.

1. Seleccione la unidad de tiempo **Periodo**: segundos, minutos, horas.

## Ejemplo


