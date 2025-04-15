---
audience: end-user
title: Uso de la actividad de flujo de trabajo Combinación-Y
description: Aprenda a utilizar la actividad de flujo de trabajo Combinación-Y
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 45%

---

# Combinación-Y {#join}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Actividad AND-join"
>abstract="La actividad **AND-join** le permite sincronizar varias ramas de ejecución de un flujo de trabajo. Se activa una vez que han finalizado todas las actividades anteriores. Esto garantiza que ciertas actividades se completen antes de continuar con la ejecución del flujo de trabajo."

La actividad **Combinación-Y** es una actividad de **Control de flujo**. Sincroniza varias ramas de ejecución de una flujo de trabajo.

Este actividad desencadena su transición saliente solo después de que se hayan activado todas las transiciones entrantes. En otras palabras, se activa una vez que se completan todas las actividades anteriores. Esto garantiza que ciertas actividades finalicen antes de continuar con la ejecución del flujo de trabajo.

## Configuración de la actividad And-join {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Combinación de opciones"
>abstract="Seleccione las actividades que desea unir. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante desea conservar."

Siga estos pasos para configurar la actividad **Combinación-Y**:

![Captura de pantalla que muestra la interfaz de configuración para el actividad AND-join.](../assets/workflow-andjoin.png)

1. añadir varias actividades, como canal actividades, para formar al menos dos ramas de ejecución diferentes.
1. Añada una actividad **Combinación-Y** a cualquiera de las ramas.
1. En la **sección Opciones** de combinación, marque todas las actividades anteriores a las que desea unirse.
1. En el **menú desplegable Conjunto** principal, elija qué población de transición entrante desea conservar. La transición saliente solo puede contener una de las poblaciones de transición entrantes.

## Ejemplo {#and-join-example}

El siguiente ejemplo muestra dos ramas de flujo de trabajo con un envío de correo electrónico y SMS. La unión AND se activa cuando ambas transiciones entrantes están habilitadas. Las notificaciones push solo se envían después de que se hayan completado ambos envíos.

![Ejemplo de una flujo de trabajo con dos ramas que muestra envío correo electrónico y SMS seguidas de notificaciones push.](../assets/workflow-andjoin-example.png){zoomable="yes"}