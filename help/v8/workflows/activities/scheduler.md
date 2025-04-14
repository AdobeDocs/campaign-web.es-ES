---
audience: end-user
title: Uso de la actividad de flujo de trabajo Planificador
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Planificador
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 9%

---

# Planificador {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Scheduler activity"
>abstract="The **Scheduler** activity allows you to schedule when the workflow gets started. This activity should be considered as a scheduled start. It can only be used as the first activity of the workflow."

## Prácticas recomendadas {#scheduler-best-practices}

* No planifique un flujo de trabajo para que se ejecute durante más de 15 minutos, ya que podría limitar el rendimiento general del sistema y crear bloques en la base de datos.
* Para realizar una entrega de una sola vez en el flujo de trabajo, agregue una actividad de planificador y configúrela para que se ejecute **Una vez**. Defina **Schedule** en la configuración de la entrega.
* Para realizar una entrega recurrente en el flujo de trabajo, use la actividad **Scheduler** y establezca la frecuencia de ejecución. La actividad de entrega recurrente no permite definir una programación.

## Configure la actividad Planificador {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Scheduler validity"
>abstract="You can define a validity period for the scheduler. It can be permanent (default), or can be valid until a specific date."

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler options"
>abstract="Define the frequency of the scheduler. It can be executed at a specific moment, once or several times a day, week or month."

Siga estos pasos para configurar la actividad **Planificador**:

![Interfaz de configuración de actividades del planificador](../assets/workflow-scheduler.png)

1. Agregue una actividad **Scheduler** al flujo de trabajo.

1. Configure **Frecuencia de ejecución**:

   * **Una vez**: el flujo de trabajo se ejecuta una sola vez.
   * **Diario**: el flujo de trabajo se ejecuta a una hora específica una vez al día.
   * **Varias veces al día**: el flujo de trabajo se ejecuta regularmente varias veces al día. Configure las ejecuciones en momentos específicos o de forma periódica.
   * **Semanal**: el flujo de trabajo se ejecuta en un momento determinado una o varias veces a la semana.
   * **Mensual**: el flujo de trabajo se ejecuta en un momento determinado una o varias veces al mes. Seleccione los meses en los que debe ejecutarse el flujo de trabajo. También puede configurar ejecuciones en días de semana del mes específicos, como el segundo martes de cada mes.

1. Defina los detalles de ejecución según la frecuencia seleccionada. Los campos de detalle pueden variar según la frecuencia utilizada (tiempo, frecuencia de repetición, días especificados y opciones similares).

1. Haga clic en **Previsualizar horas de inicio** para comprobar la programación de las siguientes diez ejecuciones del flujo de trabajo.

1. Defina el periodo de validez del planificador:

   * **Permanente (nunca caduca)**: el flujo de trabajo se ejecuta según la frecuencia especificada, sin límites en el lapso de tiempo ni número de iteraciones.
   * **Período de validez**: el flujo de trabajo se ejecuta según la frecuencia especificada, hasta una fecha específica. Especifique las fechas de inicio y finalización.

>[!NOTE]\
Si desea iniciar el flujo de trabajo de inmediato, haga clic en **Ejecutar tarea pendiente** en la barra de acciones superior del programador. Este botón solo está disponible cuando se ha iniciado el flujo de trabajo.

## Ejemplo {#scheduler-example}

En el siguiente ejemplo, la actividad está configurada para que el flujo de trabajo se ejecute varias veces al día a las 9 y las 12 de la mañana, todos los días de la semana del 1 de octubre de 2023 al 1 de enero de 2024.

![Configuración de ejemplo de actividad del programador](../assets/workflow-scheduler2.png)