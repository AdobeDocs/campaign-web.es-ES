---
audience: end-user
title: Uso de la actividad de flujo de trabajo Tenedor
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 83%

---

# Bifurcación {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Actividad de bifurcación"
>abstract="La actividad **Tenedor** permite crear transiciones salientes para iniciar varias actividades al mismo tiempo."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transiciones de la actividad de bifurcación"
>abstract="De forma predeterminada, se crean dos transiciones con una actividad de **bifurcación**. Haga clic en el botón **Añadir transición** para definir una transición de salida adicional e introducir su etiqueta."

La actividad **Fork** es una actividad de **control de flujo**. Permite crear transiciones salientes para el inicio de varias actividades al mismo tiempo.

## Configuración de la actividad Fork{#fork-configuration}

Siga estos pasos para configurar la actividad **Tenedor**:

![](../assets/workflow-fork.png)

1. Añada una actividad **Tenedor** al flujo de trabajo.
1. Haga clic en **Agregar transición** para añadir una nueva transición saliente. De forma predeterminada, se definen dos transiciones.
1. Añada una etiqueta a cada una de las transiciones.

## Ejemplo{#fork-example}

En el siguiente ejemplo, utilizamos dos actividades **Tenedor**:

* Una antes de las dos consultas, para ejecutarlas al mismo tiempo.
* Una después de la intersección, para enviar un correo electrónico y un SMS simultáneamente a la población objetivo.

![](../assets/workflow-fork-example.png)
