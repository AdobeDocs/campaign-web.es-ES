---
audience: end-user
title: Uso de la actividad de flujo de trabajo Combinación-Y
description: Aprenda a utilizar la actividad de flujo de trabajo Combinación-Y
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '187'
ht-degree: 100%

---


# Combinación-Y {#join}

La actividad **Combinación-Y** es una actividad de **Control de flujo**. Le permite sincronizar varias ramas de ejecución de un flujo de trabajo.

Esta actividad solo activa su transición saliente una vez que se activan todas las transiciones entrantes; es decir, una vez que todas las actividades anteriores han finalizado. Esto le permite asegurarse de que ciertas actividades han finalizado antes de continuar con la ejecución del flujo de trabajo.

## Configuración

Siga estos pasos para configurar la actividad **Combinación-Y**:

1. Añada varias actividades, como actividades del canal, para formar al menos dos ramas de ejecución diferentes.
1. Añada una actividad **Combinación-Y** a cualquiera de las ramas.
1. En la sección **Opciones de combinación**, compruebe todas las actividades anteriores que desee combinar.
1. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante desea conservar. La transición saliente solo puede contener una de las poblaciones de transición entrantes.

## Ejemplo

El siguiente ejemplo muestra dos ramas de flujo de trabajo con un envío de correo electrónico y SMS. La actividad Combinación-Y se activará cuando ambas transiciones entrantes estén habilitadas. Las notificaciones push solo se envían una vez finalizados ambos envíos.

![](../assets/workflow-andjoin-example.png)