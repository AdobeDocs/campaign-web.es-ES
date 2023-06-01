---
audience: end-user
title: Uso de la actividad de flujo de trabajo Espera
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Espera
badge: label="Alpha" type="Positive"
source-git-commit: 9be56c3c9c7a339e1f348ac9c74d425b501c317d
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 39%

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

El siguiente ejemplo ilustra el **Esperar** actividad en un caso de uso típico. Se envía una invitación por correo electrónico a un evento. 24 horas después de su envío, se realiza una entrega de SMS a la misma población.

![](../assets/workflow-wait-example.png)
