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
>abstract="La **actividad de espera** se utiliza para retrasar la transición de un actividad a otro."

La actividad **Esperar** es una actividad de **Control de flujo**. Permite que pase una cierta cantidad de tiempo entre la ejecución de dos actividades. Por ejemplo, se puede utilizar para esperar varios días después de una correo electrónico envío actividad, luego analizar las aperturas y los clics generados durante este período antes de realizar operaciones de seguir, como enviar un recordatorio correo electrónico o crear un audiencia.

## Configuración {#wait-configuration}

Siga estos pasos para configurar la actividad **Esperar**:

1. Añadir una actividad **Esperar** en el flujo de trabajo.

1. Especifique la **Duración** de la espera entre las transiciones entrantes y salientes.

1. Seleccione la unidad de tiempo en el **campo Períodos** : segundos, minutos, horas o días.

## Ejemplo {#wait-example}

El siguiente ejemplo ilustra la actividad **Esperar** en un caso de uso típico. Se envía una invitación por correo electrónico a un evento. Después de 24 horas, se envía un SMS envío a la misma población.

![Ejemplo de una flujo de trabajo que utiliza el actividad de espera para enviar un SMS 24 horas después de una invitación correo electrónico.](../assets/workflow-wait-example.png)