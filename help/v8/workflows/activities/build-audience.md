---
audience: end-user
title: Uso de la actividad de flujo de trabajo Generar público destinatario
description: Aprenda a utilizar la actividad de flujo de trabajo Generar público destinatario
badge: label="Beta"
source-git-commit: 2be8b4143edb720dea85dad352072028c36f0aca
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Generar público destinatario {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Crear actividad de audiencia"
>abstract="El **Crear audiencia** La actividad le permite definir la audiencia que entra en el flujo de trabajo. Al enviar mensajes en el contexto de un flujo de trabajo, la audiencia del mensaje no se define en la actividad del canal, sino en el **Crear audiencia** actividad."


La actividad **Generar público destinatario** es una actividad de **Segmentación**. Esta actividad le permite definir el público destinatario que entrará en el flujo de trabajo. Al enviar mensajes en el contexto de un flujo de trabajo, la audiencia del mensaje no se define en la actividad del canal, sino en el **Crear audiencia** actividad.

Para definir la población del público destinatario, puede hacer lo siguiente:

* Seleccione un público destinatario existente, creado como una lista en la consola del cliente.
* Seleccione un público destinatario de Adobe Experience Platform.
* Cree un nuevo público destinatario con el generador de reglas definiendo y combinando criterios de filtrado.

>[!NOTE]
>
>En este contexto, no se puede cargar un público destinatario desde un archivo. Para ello, debe crear un envío de correo electrónico independiente. [Más información](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuración de la actividad Generar audiencia

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Seleccione la dimensión de segmentación"
>abstract="La dimensión de segmentación permite definir la población a la que se dirige la operación: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. De forma predeterminada, el público destinatario se selecciona entre los destinatarios."


Siga estos pasos para configurar la actividad **Generar público destinatario**:

1. Añadir una actividad **Generar público destinatario**.
1. Defina una etiqueta.
1. Defina el tipo de público destinatario: **Crear la suya propia** o **Leer público destinatario**.

Para crear su propia consulta, siga estos pasos adicionales:

1. Seleccione **Crear su propia (consulta)**.
1. Elija la **Dimensión de segmentación**. La dimensión de segmentación permite definir la población a la que se dirige la operación: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. De forma predeterminada, el público destinatario se selecciona entre los destinatarios. Consulte la [documentación de la versión 8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=es#targeting-and-filtering-dimensions){target="_blank"}.
1. Haga clic en **Continuar**.
1. Utilice el generador de reglas para definir la consulta, del mismo modo que crea un público destinatario cuando diseña un nuevo correo electrónico. Consulte esta [sección](../../audience/segment-builder.md).

Para seleccionar un público destinatario existente, siga estos pasos:

1. Seleccione **Leer público destinatario**.
1. Haga clic en **Continuar**.
1. Seleccione el público destinatario, del mismo modo que utiliza un público destinatario cuando diseña un nuevo correo electrónico. Consulte esta [sección](../../audience/add-audience.md).

>[!IMPORTANT]
>
>Si desea combinar varias **[!UICONTROL Crear audiencia]** actividades en un flujo de trabajo que incluya una audiencia Experience Platform, debe añadir una **[!UICONTROL Cambiar dimensión]** actividad posterior, para garantizar que todas las audiencias pertenezcan a la dimensión de segmentación &quot;Destinatario&quot;. Hay un ejemplo de flujo de trabajo disponible en la parte inferior de esta página.

## Ejemplos

A continuación, se muestra un ejemplo de flujo de trabajo con dos actividades **Generar público destinatario**. El primero se dirige al público de jugadores de póquer, seguido de un envío por correo electrónico. El segundo se dirige al público de clientes VIP, seguido de un envío por SMS.

![](../assets/workflow-audience-example.png)

Este es otro ejemplo de flujo de trabajo en el que una audiencia de Adobe Experience Platform se combina con una audiencia de Adobe Campaign. Para permitir que se combinen estas audiencias, se debe usar un **[!UICONTROL Cambiar dimensión]** La actividad con la dimensión de segmentación &quot;Destinatario&quot; se agrega después de la audiencia de Adobe Experience Platform. [Obtenga información sobre cómo configurar una actividad de dimensión de cambio](change-dimension.md)

![](../assets/workflow-audience-aep.png)
