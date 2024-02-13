---
audience: end-user
title: Uso de la actividad de flujo de trabajo Esperar
description: Aprenda a utilizar la actividad de flujo de trabajo Esperar
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 92%

---

# Esperar {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Actividad de espera"
>abstract="La actividad **Espera** se utiliza para retrasar la transición de una actividad a otra."

La actividad **Esperar** es una actividad de **Control de flujo**. Se utiliza para permitir que transcurra un cierto tiempo entre dos actividades que se están ejecutando. Por ejemplo, para esperar varios días después de una actividad de envío de correo electrónico y, después, analizar las aperturas y los clics generados durante este período antes de realizar cualquier operación de seguimiento (correo electrónico recordatorio, creación de un público, etc.).

## Configuración{#wait-configuration}

Siga estos pasos para configurar la actividad **Esperar**:

1. Añadir una actividad **Esperar** en el flujo de trabajo.

1. Especifique la **Duración** de la espera entre las transiciones entrantes y salientes.

1. Seleccione la unidad de tiempo en la **Períodos** campo: segundos, minutos, horas, días.

## Ejemplo{#wait-example}

El siguiente ejemplo ilustra la actividad **Esperar** en un caso de uso típico. Se envía una invitación por correo electrónico a un evento. 24 horas después de su envío, se realiza un envío de SMS a la misma población.

![](../assets/workflow-wait-example.png)
