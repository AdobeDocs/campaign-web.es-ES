---
audience: end-user
title: Uso de la actividad de flujo de trabajo Combinación-Y
description: Aprenda a utilizar la actividad de flujo de trabajo Combinación-Y
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 100%

---

# Combinación-Y {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Actividad AND-join"
>abstract="La actividad **AND-join** le permite sincronizar varias ramas de ejecución de un flujo de trabajo. Se activa una vez que han finalizado todas las actividades anteriores. Esto le permite asegurarse de que ciertas actividades hayan finalizado antes de continuar con la ejecución del flujo de trabajo."

La actividad **Combinación-Y** es una actividad de **Control de flujo**. Le permite sincronizar varias ramas de ejecución de un flujo de trabajo.

Esta actividad solo activa su transición saliente una vez que se activan todas las transiciones entrantes; es decir, una vez que todas las actividades anteriores han finalizado. Esto le permite asegurarse de que ciertas actividades han finalizado antes de continuar con la ejecución del flujo de trabajo.

## Configuración de la actividad And-join{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Configurar la actividad de AND-join"
>abstract="Seleccione las actividades que desea unir. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante desea conservar."

Siga estos pasos para configurar la actividad **Combinación-Y**:

![](../assets/workflow-andjoin.png)

1. Añada varias actividades, como actividades del canal, para formar al menos dos ramas de ejecución diferentes.
1. Añada una actividad **Combinación-Y** a cualquiera de las ramas.
1. En la sección **Opciones de combinación**, compruebe todas las actividades anteriores que desee combinar.
1. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante desea conservar. La transición saliente solo puede contener una de las poblaciones de transición entrantes.

## Ejemplo{#and-join-example}

El siguiente ejemplo muestra dos ramas de flujo de trabajo con un envío de correo electrónico y SMS. La actividad Combinación-Y se activará cuando ambas transiciones entrantes estén habilitadas. Las notificaciones push solo se envían una vez finalizados ambos envíos.

![](../assets/workflow-andjoin-example.png){zoomable="yes"}
