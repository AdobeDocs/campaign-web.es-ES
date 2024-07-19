---
audience: end-user
title: Uso de la actividad de flujo de trabajo Change dimension
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Cambiar dimensión
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: 52b129be88e48dd70c0f55b404fd3bbe699dbebb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 26%

---

# Cambio de dimensión {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generación de un complemento"
>abstract="Puede generar una transición saliente adicional con la población restante, que se excluyó como duplicado. Para ello, active la opción **Generar complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Actividad cambiar dimensión"
>abstract="Esta actividad le permite cambiar la dimensión de segmentación a medida que genera un público. Desplace el eje en función de la plantilla de datos y la dimensión de entrada. Por ejemplo, puede cambiar de la dimensión “contratos” a la dimensión “clientes."

La actividad **Cambiar dimensión** es una actividad **Segmentación**. Esta actividad le permite cambiar la dimensión de segmentación a medida que crea el flujo de trabajo. Desplace el eje en función de la plantilla de datos y la dimensión de entrada. [Más información sobre las dimensiones de segmentación](../../audience/about-recipients.md#targeting-dimensions)

Por ejemplo, puede cambiar la dimensión objetivo de un flujo de trabajo de &quot;Destinatarios&quot; a &quot;Aplicación de suscriptores&quot; para enviar notificaciones push a los destinatarios objetivo.

>[!IMPORTANT]
>
>Tenga en cuenta que las actividades **[!UICONTROL Cambiar dimensión]** y **[!UICONTROL Cambiar fuente de datos]** no deben agregarse en una fila. Si necesita usar ambas actividades consecutivamente, asegúrese de incluir una actividad **[!UICONTROL Enrichement]** entre ellas. Esto garantiza una ejecución adecuada y evita posibles conflictos o errores.

## Configuración de la actividad Change dimension {#configure}

Siga estos pasos para configurar la actividad **Cambiar dimensión**:

1. Agregue una actividad **Cambiar dimensión** a su flujo de trabajo.

   ![](../assets/workflow-change-dimension.png)

1. Defina **Nueva dimensión de destino**. Durante el cambio de dimensión, se guardan todos los registros. Otras opciones aún no están disponibles.

1. Ejecute el flujo de trabajo para ver el resultado. Compare los datos de las tablas antes y después de la actividad de dimensión cambiante y compare la estructura de las tablas de flujo de trabajo.

## Ejemplo {#example}

En este ejemplo, deseamos enviar un envío SMS a todos los perfiles que han realizado una compra. Para ello, en primer lugar utilizamos una actividad **[!UICONTROL Generar audiencia]** vinculada a una dimensión de segmentación personalizada &quot;Compra&quot; para segmentar todas las compras que se produjeron.

Luego usamos una actividad **[!UICONTROL Change dimension]** para cambiar la dimensión de segmentación del flujo de trabajo a &quot;Recipients&quot;. Esto nos permite segmentar los destinatarios que coincidan con la consulta.

![](../assets/workflow-change-dimension-example.png)
