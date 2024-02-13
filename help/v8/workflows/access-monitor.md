---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 27%

---

# Acceso y administración de flujos de trabajo {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Flujos de trabajo"
>abstract="En esta pantalla, puede acceder a la lista completa de flujos de trabajo de la campaña e independientes, comprobar su estado actual, las fechas de última/siguiente ejecución y crear un nuevo flujo de trabajo. Vaya a la pestaña “Plantillas” para acceder a las plantillas de flujo de trabajo disponibles."

El **[!UICONTROL Flujos de trabajo]** permite acceder a la lista completa de flujos de trabajo. Esta lista incluye ambas **flujos de trabajo independientes** que se hayan creado a partir de esta pantalla, y **flujos de trabajo de campaña**, que se han creado dentro de una campaña.

![](assets/workflow-list.png){zoomable=&quot;yes&quot;}

Cada flujo de trabajo de la lista muestra información sobre su flujo de trabajo actual [status](#status), la última vez que se ejecutó o modificó y la siguiente fecha y hora de ejecución programadas.

Puede personalizar las columnas mostradas haciendo clic en el icono **[!UICONTROL Configurar la columna para un diseño personalizado]** situado en la esquina superior derecha de la lista. Esto permite agregar información adicional a la lista, como la última actividad con error para cada flujo de trabajo o la dimensión de segmentación aplicada.

Además, hay una barra de búsqueda y filtros disponibles para facilitar la búsqueda dentro de la lista. Por ejemplo, puede filtrar los flujos de trabajo para mostrar solo los que pertenecen a una campaña o los procesados durante un intervalo de fechas específico.

Para duplicar o eliminar un flujo de trabajo, haga clic en el botón de puntos suspensivos y seleccione **[!UICONTROL Duplicar]** o **[!UICONTROL Eliminar]**.

>[!NOTE]
>
>Puede duplicar un flujo de trabajo en curso, pero no puede eliminarlo.

## Estados de los flujos de trabajo {#status}

Los flujos de trabajo pueden tener varios estados:

* **[!UICONTROL Borrador]**: el flujo de trabajo se ha creado y guardado.
* **[!UICONTROL En curso]**: el flujo de trabajo se está ejecutando.
* **[!UICONTROL Finalizado]**: la ejecución del flujo de trabajo ha finalizado.
* **[!UICONTROL Pausado]**: el flujo de trabajo se ha pausado.
* **[!UICONTROL Erróneo]**: el flujo de trabajo ha encontrado un error. Abra el flujo de trabajo y acceda a los registros y tareas para identificar el error y resolverlo. [Obtenga información sobre cómo monitorizar registros y tareas](start-monitor-workflows.md#logs-tasks)

Encontrará información detallada sobre cómo iniciar y monitorizar la ejecución del flujo de trabajo en [esta página](start-monitor-workflows.md).

## Plantillas de flujo de trabajo {#templates}

El **[!UICONTROL Plantillas]** la pestaña enumera todas las plantillas de flujos de trabajo disponibles.

Las plantillas de flujo de trabajo contienen actividades preconfiguradas y configuraciones de propiedad generales que se pueden reutilizar para crear nuevos flujos de trabajo.

Puede crear plantillas de flujo de trabajo a partir de un flujo de trabajo existente o desde cero. [Obtenga información sobre cómo crear plantillas de flujo de trabajo](create-workflow.md#workflow-templates)
