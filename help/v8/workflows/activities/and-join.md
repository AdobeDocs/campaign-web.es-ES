---
audience: end-user
title: Uso de la actividad de flujo de trabajo AND-join
description: Aprenda a utilizar la actividad de flujo de trabajo AND-join
badge: label="Alpha" type="Positive"
source-git-commit: bdf569913dfcf9bee549c6ae3252f5a92a5f34e8
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 19%

---


# AND-join {#join}

El **And-join** la actividad es una **Control de flujo** actividad. Permite sincronizar varias ramas de ejecución de un flujo de trabajo.

Esta actividad solo almacena en déclencheur su transición de salida una vez que se activan todas las transiciones de entrada; es decir, una vez que todas las actividades anteriores han finalizado. Esto le permite asegurarse de que algunas actividades han finalizado antes de continuar ejecutándose el flujo de trabajo.

## Configuración

Siga estos pasos para configurar el **AND-join** actividad:

1. Agregue varias actividades, como actividades de canal, para formar al menos dos ramas de ejecución diferentes.
1. Añadir un **AND-join** actividad a cualquiera de las ramas.
1. En el **Combinación de opciones** , compruebe todas las actividades anteriores a las que desee unirse.
1. En el **Conjunto principal** , elija qué población de transición entrante desea conservar. La transición saliente solo puede contener una de las poblaciones de transición entrantes.

## Ejemplo

El siguiente ejemplo muestra dos ramas de flujo de trabajo con un envío de correo electrónico y SMS. La unión AND entrará en déclencheur cuando ambas transiciones de entrada estén habilitadas. Las notificaciones push solo se envían una vez finalizados ambos envíos.

![](../assets/workflow-andjoin-example.png)