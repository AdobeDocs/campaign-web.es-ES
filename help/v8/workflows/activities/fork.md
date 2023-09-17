---
audience: end-user
title: Uso de la actividad de flujo de trabajo Tenedor
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
badge: label="Beta"
source-git-commit: 173141ec198b4d451a7b388f0e28a29230a11396
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 68%

---


# Bifurcación {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Bifurcación  actividad"
>abstract="La actividad **Tenedor** permite crear transiciones salientes para iniciar varias actividades al mismo tiempo."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transiciones de actividad de bifurcación"
>abstract="De forma predeterminada, se crean dos transiciones con una **Tenedor** actividad. Haga clic en **Añadir transición** para definir una transición saliente adicional e introducir su etiqueta."

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

