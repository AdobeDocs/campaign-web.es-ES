---
audience: end-user
title: Uso de la actividad de flujo de trabajo Espera
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Espera
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 29%

---


# Espera {#wait}

El **Esperar** la actividad es una **Control de flujo** actividad. Se utiliza para permitir que transcurra un cierto tiempo entre dos actividades que se están ejecutando. Por ejemplo, para esperar varios días después de una actividad de envío de correo electrónico y, después, analizar las aperturas y los clics generados durante este período antes de realizar cualquier operación de seguimiento (correo electrónico de recordatorio, creación de una audiencia, etc.).

## Configuración

Siga estos pasos para configurar el **Esperar** actividad:

1. Añadir un **Esperar** en el flujo de trabajo.

1. Especifique el **Duración** de la espera entre las transiciones de entrada y salida.

1. Seleccione la unidad de tiempo en la **Períodos** campo: segundos, minutos, horas.

## Ejemplo

El siguiente ejemplo ilustra el **Esperar** actividad en un caso de uso típico. Se envía una invitación por correo electrónico a un evento. 24 horas después de su envío, se realiza una entrega de SMS a la misma población.

![](../assets/workflow-wait-example.png)
