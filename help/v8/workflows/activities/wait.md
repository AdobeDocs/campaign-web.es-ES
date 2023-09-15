---
audience: end-user
title: Uso de la actividad de flujo de trabajo Esperar
description: Aprenda a utilizar la actividad de flujo de trabajo Esperar
badge: label="Beta"
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 100%

---


# Espera {#wait}


>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Esperar"
>abstract="La actividad **Esperar** es una actividad de **Control de flujo**. Se utiliza para permitir que transcurra un cierto tiempo entre dos actividades que se están ejecutando."


La actividad **Esperar** es una actividad de **Control de flujo**. Se utiliza para permitir que transcurra un cierto tiempo entre dos actividades que se están ejecutando. Por ejemplo, para esperar varios días después de una actividad de envío de correo electrónico y, después, analizar las aperturas y los clics generados durante este período antes de realizar cualquier operación de seguimiento (correo electrónico recordatorio, creación de un público, etc.).

## Configuración

Siga estos pasos para configurar la actividad **Esperar**:

1. Añadir una actividad **Esperar** en el flujo de trabajo.

1. Especifique la **Duración** de la espera entre las transiciones entrantes y salientes.

1. Seleccione la unidad de tiempo en el campo **Períodos**: segundos, minutos u horas.

## Ejemplo

El siguiente ejemplo ilustra la actividad **Esperar** en un caso de uso típico. Se envía una invitación por correo electrónico a un evento. 24 horas después de su envío, se realiza un envío de SMS a la misma población.

![](../assets/workflow-wait-example.png)
