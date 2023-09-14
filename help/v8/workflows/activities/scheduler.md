---
audience: end-user
title: Uso de la actividad de flujo de trabajo Planificador
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Planificador
badge: label="Beta"
source-git-commit: ea57053910aa98e79ceb7ef683f890a366a9001b
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 22%

---


# Planificador {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Actividad del planificador"
>abstract="La actividad Planificador le permite..."

El **Planificador** la actividad es una **Control de flujo** actividad. Permite programar cuándo se inicia el flujo de trabajo. Esta actividad debe considerarse como un inicio programado. Solo se puede utilizar como primera actividad del flujo de trabajo.

## Prácticas recomendadas

No planifique un flujo de trabajo para que se ejecute durante más de 15 minutos, ya que podría limitar el rendimiento general del sistema y crear bloques en la base de datos.

## Configuración

Siga estos pasos para configurar el **Planificador** actividad:

1. Añadir un **Planificador** a su flujo de trabajo.

   ![](../assets/workflow-scheduler.png)

1. Configure las variables **Frecuencia de ejecución**:

   * **Una**: el flujo de trabajo se ejecuta una sola vez.

   * **Diario**: el flujo de trabajo se ejecuta a una hora específica una vez al día.

   * **Varias veces al día:** el flujo de trabajo se ejecuta regularmente varias veces al día. Puede configurar ejecuciones en momentos específicos o de forma periódica.

   * **Semanalmente**: el flujo de trabajo se ejecuta en un momento determinado una o varias veces a la semana.

   * **Mensual**: el flujo de trabajo se ejecuta en un momento determinado una o varias veces al mes. Puede seleccionar meses cuando necesite que se ejecute el flujo de trabajo. También puede configurar ejecuciones en días de semana del mes específicos, como el segundo martes de mes.

1. Defina los detalles de ejecución según la frecuencia seleccionada. Los campos de detalle pueden variar según la frecuencia utilizada (tiempo, frecuencia de repetición, días especificados, etc.).

1. Clic **Previsualizar tiempos de lanzamiento** para comprobar la programación de las siguientes diez ejecuciones del flujo de trabajo.

1. Defina el periodo de validez del planificador:

   * **Permanente (nunca caduca)**: el flujo de trabajo se ejecuta según la frecuencia especificada, sin límites en el lapso de tiempo ni número de iteraciones.

   * **Período de validez**: el flujo de trabajo se ejecuta según la frecuencia especificada, hasta una fecha específica. Debe especificar las fechas de inicio y finalización.

## Ejemplo

En el siguiente ejemplo, la actividad se configura de modo que inicia el flujo de trabajo varias veces al día a las 9 y las 12 de la mañana, todos los días de la semana del 1 de octubre de 2023 al 1 de enero de 2024.

![](../assets/workflow-scheduler2.png)



