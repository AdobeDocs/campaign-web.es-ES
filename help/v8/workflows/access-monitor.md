---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 17%

---

# Acceso y administración de flujos de trabajo {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Flujos de trabajo"
>abstract="En esta pantalla, puede acceder a la lista completa de flujos de trabajo de la campaña e independientes, comprobar su estado actual, las fechas de última/siguiente ejecución y crear un nuevo flujo de trabajo. Vaya a la pestaña “Plantillas” para acceder a las plantillas de flujo de trabajo disponibles."

El menú **[!UICONTROL Flujos de trabajo]** proporciona acceso a la lista completa de flujos de trabajo. Esta lista incluye **flujos de trabajo independientes**, creados a partir de esta pantalla, y **flujos de trabajo de campaña**, creados dentro de una campaña.

![Pantalla de lista de flujos de trabajo que muestra flujos de trabajo independientes y de campaña](assets/workflow-list.png){zoomable="yes"}

Cada flujo de trabajo de la lista muestra información sobre su [estado actual](#status), la última vez que se ejecutó o modificó, y la siguiente fecha y hora de ejecución programada.

Personalice las columnas mostradas haciendo clic en el icono **[!UICONTROL Configurar columna para un diseño personalizado]** ubicado en la esquina superior derecha de la lista. Esto le permite agregar información adicional a la lista, como la última actividad con error para cada flujo de trabajo o la dimensión de segmentación aplicada.

Además, hay disponible una barra de búsqueda y filtros para simplificar la búsqueda dentro de la lista. Por ejemplo, filtre los flujos de trabajo para mostrar solo los que pertenecen a una campaña o los procesados durante un intervalo de fechas específico.

Para duplicar o eliminar un flujo de trabajo, haga clic en el botón de puntos suspensivos y luego seleccione **[!UICONTROL Duplicar]** o **[!UICONTROL Eliminar]**.

>[!NOTE]
>
>Puede duplicar un flujo de trabajo en curso, pero no puede eliminarlo.

## Estados de los flujos de trabajo {#status}

Los flujos de trabajo pueden tener varios estados:

* **[!UICONTROL Borrador]**: el flujo de trabajo se ha creado y guardado.
* **[!UICONTROL En curso]**: el flujo de trabajo se está ejecutando.
* **[!UICONTROL Finalizado]**: la ejecución del flujo de trabajo ha finalizado.
* **[!UICONTROL En pausa]**: el flujo de trabajo se ha pausado.
* **[!UICONTROL Erróneo]**: el flujo de trabajo encontró un error. Abra el flujo de trabajo y acceda a los registros y tareas para identificar el error y resolverlo. [Obtenga información sobre cómo supervisar registros y tareas](start-monitor-workflows.md#logs-tasks)

Encontrará información detallada sobre cómo iniciar y supervisar la ejecución del flujo de trabajo en [esta página](start-monitor-workflows.md).

## Plantillas de flujo de trabajo {#templates}

La ficha **[!UICONTROL Plantillas]** enumera todas las plantillas de flujo de trabajo disponibles.

Las plantillas de flujo de trabajo contienen actividades preconfiguradas y configuraciones de propiedad generales que se pueden reutilizar para crear nuevos flujos de trabajo.

Cree plantillas de flujo de trabajo desde un flujo de trabajo existente o desde cero. [Aprenda a crear plantillas de flujo de trabajo](create-workflow.md#workflow-templates)