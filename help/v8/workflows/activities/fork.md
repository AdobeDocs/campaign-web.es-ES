---
audience: end-user
title: Uso de la actividad de flujo de trabajo Fork
description: Aprenda a utilizar la actividad del flujo de trabajo Bifurcación
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 5%

---


# Bifurcación {#fork}

El **Tenedor** la actividad es una **Control de flujo** actividad. Permite crear transiciones salientes para el inicio de varias actividades al mismo tiempo.

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

