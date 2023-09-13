---
audience: end-user
title: Uso de la actividad de flujo de trabajo Planificador
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Planificador
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 42%

---


# Planificador {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Actividad del planificador"
>abstract="La actividad Planificador le permite..."

La actividad Planificador le permite programar cuándo se inicia un flujo de trabajo o una actividad.

La actividad del Scheduler debe considerarse como un inicio programado. Esta actividad solo puede utilizarse como primera actividad del flujo de trabajo.

## Prácticas recomendadas

* No planifique un flujo de trabajo para que se ejecute durante más de 15 minutos, ya que podría limitar el rendimiento general del sistema y crear bloques en la base de datos.

## Configuración

Siga estos pasos para configurar el **Planificador** actividad:

1. Añadir un **Planificador** a su flujo de trabajo.

1. Configure las variables **Frecuencia de ejecución**:

   * Once: el flujo de trabajo se ejecuta una sola vez.

   * Diario: el flujo de trabajo se ejecuta a una hora específica una vez al día.

   * Varias veces al día: el flujo de trabajo se ejecuta regularmente varias veces al día. Puede configurar ejecuciones en momentos específicos o de forma periódica.

   * Semanal: el flujo de trabajo se ejecuta en un momento determinado una o varias veces a la semana.

   * Mensual: el flujo de trabajo se ejecuta en un momento determinado una o varias veces al mes. Puede seleccionar meses cuando necesite que se ejecute el flujo de trabajo. También puede configurar ejecuciones en un día de semana del mes específico, como el segundo martes de cada mes.
1. Defina los detalles de ejecución según la frecuencia seleccionada. Los campos de detalle pueden variar según la frecuencia utilizada (tiempo, frecuencia de repetición, días especificados, etc.).

1. Clic **Previsualizar tiempos de lanzamiento** para comprobar la programación de las siguientes diez ejecuciones del flujo de trabajo.

1. Defina el periodo de validez del planificador:

   * Permanente (nunca caduca): el flujo de trabajo se ejecutará según la frecuencia especificada, sin límites en el lapso de tiempo ni número de iteraciones.

   * Período de validez: el flujo de trabajo se ejecutará según la frecuencia especificada, hasta una fecha específica. Por lo tanto, se debe especificar el valor de la fecha límite de ejecución.

## Ejemplo


