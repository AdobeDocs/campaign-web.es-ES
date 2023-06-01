---
audience: end-user
title: Uso de la actividad de flujo de trabajo AND-join
description: Aprenda a utilizar la actividad de flujo de trabajo AND-join
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 4%

---


# AND-join {#join}

El **And-join** Esta actividad permite sincronizar varias ramas de ejecución de un flujo de trabajo.

La actividad AND-join solo almacena en déclencheur su transición de salida una vez que se activan todas las transiciones de entrada; es decir, una vez que todas las actividades anteriores han finalizado.

Siga estos pasos para configurar el **AND-join** actividad:

1. Añada varias actividades, como **Combinar** actividades para formar al menos dos ramas de ejecución diferentes.
1. Añadir un **AND-join** actividad a cualquiera de las ramas.
1. En el **Combinación de opciones** , compruebe todas las actividades anteriores a las que desee unirse.
1. Seleccione el **Conjunto principal** para que se mantenga en la transición saliente.
