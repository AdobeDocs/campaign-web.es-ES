---
audience: end-user
title: Uso de la actividad de flujo de trabajo Tenedor
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 51%

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

La actividad **Fork** es una actividad de **control de flujo**. Permite crear transiciones de salida para el inicio de varias actividades simultáneamente.

## Configuración de la actividad Fork {#fork-configuration}

Siga estos pasos para configurar la actividad **Tenedor**:

![Captura de pantalla de configuración de actividad de ramificación de flujo de trabajo](../assets/workflow-fork.png)

1. Añada una actividad **Tenedor** al flujo de trabajo.
1. Haga clic en **Agregar transición** para añadir una nueva transición saliente. De forma predeterminada, se definen dos transiciones.
1. Añada una etiqueta a cada transición.

## Ejemplo {#fork-example}

En el ejemplo siguiente, se usan dos actividades **Fork**:

* Uno antes de las dos consultas, para ejecutarlas simultáneamente.
* Uno después de la intersección, para enviar un correo electrónico y un SMS al mismo tiempo a la población de destino.

![Captura de pantalla de ejemplo de ramificación de flujo de trabajo](../assets/workflow-fork-example.png)
