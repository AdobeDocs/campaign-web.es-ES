---
audience: end-user
title: Uso de la actividad de flujo de trabajo Combinación-Y
description: Aprenda a utilizar la actividad de flujo de trabajo Combinación-Y
badge: label="Beta"
source-git-commit: 253889459de03cf4df72be5a5fbc223588e9b86c
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 84%

---


# Combinación-Y {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Actividad AND-join"
>abstract="La actividad **Combinación-Y** le permite sincronizar varias ramas de ejecución de un flujo de trabajo. Se activa una vez que han finalizado todas las actividades anteriores. Esto le permite asegurarse de que algunas actividades han finalizado antes de continuar ejecutándose el flujo de trabajo."

La actividad **Combinación-Y** es una actividad de **Control de flujo**. Le permite sincronizar varias ramas de ejecución de un flujo de trabajo.

Esta actividad solo activa su transición saliente una vez que se activan todas las transiciones entrantes; es decir, una vez que todas las actividades anteriores han finalizado. Esto le permite asegurarse de que ciertas actividades han finalizado antes de continuar con la ejecución del flujo de trabajo.

## Configuración

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Configuración de la actividad AND-join"
>abstract="Seleccione las actividades a las que desea unirse. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante desea conservar."

Siga estos pasos para configurar la actividad **Combinación-Y**:

1. Añada varias actividades, como actividades del canal, para formar al menos dos ramas de ejecución diferentes.
1. Añada una actividad **Combinación-Y** a cualquiera de las ramas.
1. En la sección **Opciones de combinación**, compruebe todas las actividades anteriores que desee combinar.
1. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante desea conservar. La transición saliente solo puede contener una de las poblaciones de transición entrantes.

## Ejemplo

El siguiente ejemplo muestra dos ramas de flujo de trabajo con un envío de correo electrónico y SMS. La actividad Combinación-Y se activará cuando ambas transiciones entrantes estén habilitadas. Las notificaciones push solo se envían una vez finalizados ambos envíos.

![](../assets/workflow-andjoin-example.png)