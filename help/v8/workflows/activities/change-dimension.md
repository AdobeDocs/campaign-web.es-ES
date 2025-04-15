---
audience: end-user
title: Utilice el dimensión de cambio flujo de trabajo actividad
description: Aprenda a utilizar el actividad Change dimensión flujo de trabajo
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
>abstract="Esta actividad le permite cambiar la dimensión de segmentación a medida que genera un público. Desplace el eje en función de la plantilla de datos y la dimensión de entrada. Por ejemplo, puede cambiar del dimensión &quot;contratos&quot; al dimensión &quot;clientes&quot;."

La **actividad Cambiar dimensión** es un actividad de **Targeting** . Este actividad le permite cambiar el dimensión de segmentación a medida que va creando su flujo de trabajo. Desplace el eje en función de la plantilla de datos y la dimensión de entrada. [Obtenga más información sobre direccionamiento dimensiones](../../audience/about-recipients.md#targeting-dimensions).

Por ejemplo, puede cambiar el dimensión de segmentación de un flujo de trabajo de &quot;Destinatarios&quot; a &quot;Suscriptores aplicación&quot; para enviar notificaciones push a los destinatarios objetivo.

>[!IMPORTANT]
>
>Tenga en cuenta que las actividades Cambiar Dimension ]**y**[!UICONTROL  Cambiar fuente ]**de**[!UICONTROL  datos no deben agregarse en una fila. Si necesita utilizar ambas actividades consecutivamente, incluya una **[!UICONTROL actividad de enriquecimiento]** entre ellas. Esto garantiza una ejecución correcta y evita posibles conflictos o errores.

## Configurar el cambio dimensión actividad {#configure}

Siga estos pasos para configurar el **actividad Change dimensión** :

1. añadir un **cambio dimensión** actividad a su flujo de trabajo.

   ![Captura de pantalla que muestra el dimensión de cambio actividad agregado a un flujo de trabajo](../assets/workflow-change-dimension.png)

1. Definir el **Nuevo destino dimensión**. Durante dimensión cambio, se guardan todos los registros. Aún no hay otras opciones disponibles.

1. Ejecute los flujo de trabajo para vista el resultado. Comparar los datos de las tablas antes y después del actividad Change dimensión y comparar la estructura de las tablas flujo de trabajo.

## Ejemplo {#example}

En este ejemplo, envíe un SMS envío a todos los perfiles que hayan realizado una compra. Primero, use un **[!UICONTROL actividad de audiencia]** de compilación vinculado a un dimensión de segmentación personalizado de &quot;Compra&quot; para destino todas las compras que ocurrieron.

A continuación, utilice un **[!UICONTROL actividad Change dimensión]** para cambiar el dimensión de segmentación de flujo de trabajo a &quot;Destinatarios&quot;. Esto permite direccionamiento los destinatarios que coinciden con el consulta.

![Captura de pantalla que muestra un ejemplo de los actividad de cambio dimensión utilizados en una flujo de trabajo](../assets/workflow-change-dimension-example.png)