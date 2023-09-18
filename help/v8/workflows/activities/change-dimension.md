---
audience: end-user
title: Uso de la actividad de flujo de trabajo Change dimension
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Cambiar dimensión
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '191'
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

También puede utilizar esta actividad para definir las columnas adicionales del nuevo destinatario y los criterios de anulación de duplicación de datos.

## Configuración

Siga estos pasos para configurar el **Cambiar dimensión** actividad:

1. Añadir un **Cambiar dimensión** a su flujo de trabajo.

   ![](../assets/workflow-change-dimension.png)

1. Defina el **Nueva dimensión de destino**.

Durante el cambio de dimensión, se guardan todos los registros.