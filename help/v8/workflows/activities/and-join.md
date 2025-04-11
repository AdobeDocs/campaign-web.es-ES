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
>abstract="La actividad **AND-join** le permite sincronizar varias ramas de ejecución de un flujo de trabajo. Se activa una vez que han finalizado todas las actividades anteriores. Esto garantiza que determinadas actividades se completen antes de continuar ejecutando el flujo de trabajo."

La actividad **Combinación-Y** es una actividad de **Control de flujo**. Sincroniza varias ramas de ejecución de un flujo de trabajo.

Esta actividad almacena en déclencheur su transición saliente solo después de activar todas las transiciones entrantes. En otras palabras, se activa una vez completadas todas las actividades anteriores. Esto garantiza que determinadas actividades hayan finalizado antes de continuar ejecutando el flujo de trabajo.

## Configuración de la actividad And-join {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Combinación de opciones"
>abstract="Seleccione las actividades que desea unir. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante desea conservar."

Siga estos pasos para configurar la actividad **Combinación-Y**:

![Captura de pantalla que muestra la interfaz de configuración para la actividad AND-join.](../assets/workflow-andjoin.png)

1. Añada varias actividades, como actividades de canal, para formar, al menos, dos ramas de ejecución diferentes.
1. Añada una actividad **Combinación-Y** a cualquiera de las ramas.
1. En la sección **Combinar opciones**, compruebe todas las actividades anteriores a las que desee unirse.
1. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante se debe conservar. La transición saliente solo puede contener una de las poblaciones de transición entrantes.

## Ejemplo {#and-join-example}

El siguiente ejemplo muestra dos ramas de flujo de trabajo con un envío de correo electrónico y SMS. Los déclencheur AND-join cuando ambas transiciones de entrada están habilitadas. Las notificaciones push solo se envían una vez completados ambos envíos.

![Ejemplo de un flujo de trabajo con dos ramas, que muestra el envío de correo electrónico y SMS seguido de notificaciones push.](../assets/workflow-andjoin-example.png){zoomable="yes"}