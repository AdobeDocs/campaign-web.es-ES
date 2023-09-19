---
audience: end-user
title: Uso de la actividad de flujo de trabajo Change dimension
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Cambiar dimensión
badge: label="Beta"
source-git-commit: 8139ec2f1e94bebacd89ea64af88d0b0babb8781
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 6%

---


# Cambio de dimensión {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generar un complemento"
>abstract="Puede generar una transición saliente adicional con la población restante, que se excluyó como duplicado. Para ello, active la opción **Generar complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Cambiar actividad de dimensión"
>abstract="Esta actividad le permite cambiar la dimensión de segmentación a medida que crea una audiencia. Desplaza el eje en función de la plantilla de datos y la dimensión de entrada. Por ejemplo, puede cambiar de la dimensión &quot;contratos&quot; a la dimensión &quot;clientes&quot;."

El **Cambiar dimensión** la actividad es una **Segmentación** actividad. Esta actividad le permite cambiar la dimensión de segmentación a medida que crea una audiencia. Esta actividad desplaza el eje según la plantilla de datos y la dimensión de entrada. Por ejemplo, puede cambiar de la dimensión &quot;contratos&quot; a la dimensión &quot;clientes&quot;.

## Configuración de la actividad Change dimension {#configure}

Siga estos pasos para configurar el **Cambiar dimensión** actividad:

1. Añadir un **Cambiar dimensión** a su flujo de trabajo.

   ![](../assets/workflow-change-dimension.png)

1. Defina el **Nueva dimensión de destino**. Durante el cambio de dimensión, se guardan todos los registros. Otras opciones aún no están disponibles.

1. Ejecute el flujo de trabajo para ver el resultado. Compare los datos de las tablas antes y después de la actividad de dimensión cambiante y compare la estructura de las tablas de flujo de trabajo.

## Ejemplo {#example}


