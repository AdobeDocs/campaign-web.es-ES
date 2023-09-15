---
audience: end-user
title: Uso de la actividad de flujo de trabajo Tenedor
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
badge: label="Beta"
source-git-commit: 4b005f3feb70b8c5cf0f4cd9c5ba54547bd9261a
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 71%

---


# Bifurcación {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Bifurcación  actividad"
>abstract="El **Tenedor** la actividad es una **Control de flujo** actividad. Permite crear transiciones salientes para el inicio de varias actividades al mismo tiempo."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Bifurcación  actividad"
>abstract="La actividad Tenedor permite crear transiciones salientes para el inicio de varias actividades al mismo tiempo."

El **Tenedor** la actividad es una **Control de flujo** actividad. Permite crear transiciones salientes para el inicio de varias actividades al mismo tiempo.

## Configuración

Siga estos pasos para configurar la actividad **Tenedor**:

1. Añada una actividad **Tenedor** al flujo de trabajo.
1. Haga clic en **Agregar transición** para añadir una nueva transición saliente. De forma predeterminada, se definen dos transiciones.
1. Añada una etiqueta a cada una de las transiciones.

## Ejemplo

En el siguiente ejemplo, utilizamos dos actividades **Tenedor**:

* Una antes de las dos consultas, para ejecutarlas al mismo tiempo.
* Una después de la intersección, para enviar un correo electrónico y un SMS simultáneamente a la población objetivo.

![](../assets/workflow-fork-example.png)

