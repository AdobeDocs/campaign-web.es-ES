---
audience: end-user
title: Uso de la actividad de flujo de trabajo Change dimension
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Cambiar dimensión
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 21%

---

# Cambio de dimensión {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Generación de un complemento"
>abstract="Puede generar una transición saliente adicional con la población restante, que se excluyó como duplicado. Para ello, active la opción **Generar complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Actividad cambiar dimensión"
>abstract="Esta actividad le permite cambiar la dimensión de segmentación a medida que genera un público. Desplace el eje en función de la plantilla de datos y la dimensión de entrada. Por ejemplo, puede cambiar de la dimensión &quot;contratos&quot; a la dimensión &quot;clientes&quot;."

La actividad **Cambiar dimensión** es una actividad **Segmentación**. Esta actividad le permite cambiar la dimensión de segmentación a medida que crea el flujo de trabajo. Desplace el eje en función de la plantilla de datos y la dimensión de entrada. [Más información sobre las dimensiones de segmentación](../../audience/about-recipients.md#targeting-dimensions).

Por ejemplo, puede cambiar la dimensión objetivo de un flujo de trabajo de &quot;Destinatarios&quot; a &quot;Aplicación de suscriptores&quot; para enviar notificaciones push a los destinatarios objetivo.

>[!IMPORTANT]
>
>Tenga en cuenta que las actividades **[!UICONTROL Cambiar dimensión]** y **[!UICONTROL Cambiar fuente de datos]** no deben agregarse en una fila. Si necesita usar ambas actividades consecutivamente, incluya una actividad **[!UICONTROL Enrichment]** entre ellas. Esto garantiza una ejecución adecuada y evita posibles conflictos o errores.

## Configuración de la actividad Change dimension {#configure}

Siga estos pasos para configurar la actividad **Cambiar dimensión**:

1. Agregue una actividad **Cambiar dimensión** a su flujo de trabajo.

   ![Captura de pantalla que muestra la actividad Cambiar dimensión agregada a un flujo de trabajo](../assets/workflow-change-dimension.png)

1. Defina **Nueva dimensión de destino**. Durante el cambio de dimensión, se guardan todos los registros. Otras opciones aún no están disponibles.

1. Ejecute el flujo de trabajo para ver el resultado. Compare los datos de las tablas antes y después de la actividad Change dimension y compare la estructura de las tablas de flujo de trabajo.

## Ejemplo {#example}

En este ejemplo, envíe un SMS a todos los perfiles que han realizado una compra. En primer lugar, use una actividad **[!UICONTROL Generar audiencia]** vinculada a una dimensión de segmentación personalizada &quot;Compra&quot; para segmentar todas las compras que se hayan producido.

A continuación, use una actividad **[!UICONTROL Change dimension]** para cambiar la dimensión de segmentación del flujo de trabajo a &quot;Destinatarios&quot;. Esto permite dirigirse a los destinatarios que coincidan con la consulta.

![Captura de pantalla que muestra un ejemplo de la actividad de dimensión Change utilizada en un flujo de trabajo](../assets/workflow-change-dimension-example.png)