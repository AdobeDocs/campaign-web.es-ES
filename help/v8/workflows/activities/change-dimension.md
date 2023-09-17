---
audience: end-user
title: Uso de la actividad de flujo de trabajo Change dimension
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Cambiar dimensión
badge: label="Beta"
source-git-commit: 253889459de03cf4df72be5a5fbc223588e9b86c
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 4%

---


# Dimensión cambiante {#change-dimension}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generate Complement"
>abstract="TBD"
-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Dimensión cambiante actividad"
>abstract="Esta actividad le permite cambiar la dimensión de segmentación a medida que crea una audiencia. Desplaza el eje en función de la plantilla de datos y la dimensión de entrada. Por ejemplo, puede cambiar de la dimensión &quot;contratos&quot; a la dimensión &quot;clientes&quot;."


El **Cambiar dimensión** la actividad es una **Segmentación** actividad. Esta actividad le permite cambiar la dimensión de segmentación a medida que crea una audiencia. Esta actividad desplaza el eje según la plantilla de datos y la dimensión de entrada. Por ejemplo, puede cambiar de la dimensión &quot;contratos&quot; a la dimensión &quot;clientes&quot;.

También puede utilizar esta actividad para definir las columnas adicionales del nuevo destinatario y los criterios de anulación de duplicación de datos.

## Configuración

Siga estos pasos para configurar el **Cambiar dimensión** actividad:

1. Añadir un **Cambiar dimensión** a su flujo de trabajo.

   ![](../assets/workflow-change-dimension.png)

1. Defina el **Nueva dimensión de destino**.

Durante el cambio de dimensión, se guardan todos los registros.