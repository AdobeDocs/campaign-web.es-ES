---
audience: end-user
title: Uso de la actividad de flujo de trabajo Esperar
description: Aprenda a utilizar la actividad de flujo de trabajo Esperar
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 39%

---

# Esperar {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Actividad de espera"
>abstract="La actividad **Wait** se usa para retrasar la transición de una actividad a otra."

La actividad **Esperar** es una actividad de **Control de flujo**. Permite que transcurra un cierto tiempo entre la ejecución de dos actividades. Por ejemplo, se puede utilizar para esperar varios días después de una actividad de entrega de correo electrónico y, a continuación, analizar las aperturas y los clics generados durante este periodo antes de realizar operaciones de seguimiento, como enviar un correo electrónico de recordatorio o crear una audiencia.

## Configuración {#wait-configuration}

Siga estos pasos para configurar la actividad **Esperar**:

1. Añadir una actividad **Esperar** en el flujo de trabajo.

1. Especifique la **Duración** de la espera entre las transiciones entrantes y salientes.

1. Seleccione la unidad de tiempo en el campo **Periodos**: segundos, minutos, horas o días.

## Ejemplo {#wait-example}

El siguiente ejemplo ilustra la actividad **Esperar** en un caso de uso típico. Se envía una invitación por correo electrónico a un evento. Después de 24 horas, se envía un SMS a la misma población.

![Ejemplo de un flujo de trabajo que utiliza la actividad Espera para enviar un SMS 24 horas después de una invitación por correo electrónico.](../assets/workflow-wait-example.png)