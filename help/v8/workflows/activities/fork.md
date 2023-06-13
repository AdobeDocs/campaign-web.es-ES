---
audience: end-user
title: Uso de la actividad de flujo de trabajo Fork
description: Aprenda a utilizar la actividad del flujo de trabajo Bifurcación
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 19%

---


# Bifurcación (Fork) {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Bifurcación (Fork) Actividad"
>abstract="La actividad Bifurcación permite crear transiciones de salida para el inicio de varias actividades al mismo tiempo."

## Configuración

Siga estos pasos para configurar el **Tenedor** actividad:

1. Añadir un **Tenedor** a su flujo de trabajo.
1. Clic **Añadir transición** para añadir una nueva transición saliente. De forma predeterminada, se definen dos transiciones.
1. Añada una etiqueta a cada una de las transiciones.

## Ejemplo

En el siguiente ejemplo, utilizamos dos **Tenedor** actividades:

* Uno antes de las dos consultas, para ejecutarlas al mismo tiempo.
* Uno después de la intersección, para enviar un correo electrónico y un SMS simultáneamente a la población de destino.

![](../assets/workflow-fork-example.png)

