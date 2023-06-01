---
audience: end-user
title: Uso de la actividad de flujo de trabajo AND-join
description: Aprenda a utilizar la actividad de flujo de trabajo AND-join
badge: label="Alpha" type="Positive"
source-git-commit: 6ed2c73a5348871348ec4cbdd89fc8119fdbc718
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 4%

---


# AND-join {#join}

El **And-join** Esta actividad permite sincronizar varias ramas de ejecución de un flujo de trabajo.

La actividad AND-join solo almacena en déclencheur su transición de salida una vez que se activan todas las transiciones de entrada; es decir, una vez que todas las actividades anteriores han finalizado.

## Configuración

Siga estos pasos para configurar el **AND-join** actividad:

1. Añada varias actividades, como **Combinar** actividades para formar al menos dos ramas de ejecución diferentes.
1. Añadir un **AND-join** actividad a cualquiera de las ramas.
1. En el **Combinación de opciones** , compruebe todas las actividades anteriores a las que desee unirse.
1. Seleccione el **Conjunto principal** para que se mantenga en la transición saliente.

## Ejemplo

El siguiente ejemplo muestra dos ramas de flujo de trabajo con un envío de correo electrónico y SMS. La unión AND entrará en déclencheur cuando ambas transiciones de entrada estén habilitadas. Las notificaciones push solo se envían una vez finalizados ambos envíos.

![](../assets/workflow-andjoin-example.png)