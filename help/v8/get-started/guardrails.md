---
title: Mecanismos de protección y limitaciones en los flujos de trabajo de la interfaz de usuario web de Campaign
description: Mecanismos de protección y limitaciones al trabajar con flujos de trabajo en la interfaz de usuario web de Campaign
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 56%

---

# Mecanismos de protección y limitaciones de los flujos de trabajo {#guardrails-limitations}

Al trabajar en la interfaz de usuario web de Campaign con flujos de trabajo creados o modificados en la consola del cliente de Campaign, se aplican los mecanismos de protección y limitaciones que se enumeran a continuación.

Tenga en cuenta que, aunque esta página identifica las consideraciones clave a la hora de trabajar con flujos de trabajo en la consola y la interfaz de usuario web, no abarca todas las posibles incompatibilidades entre las dos interfaces.

## Actividades de flujo de trabajo {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Actividad no editable"
>abstract="Cuando una actividad de **Consulta** o **Enriquecimiento** se configura con datos adicionales en la consola, los datos de enriquecimiento se tienen en cuenta en la web de Campaign y pasan a la transición saliente, pero no se pueden editar."

Las actividades de flujo de trabajo que aún no se admiten en la interfaz de usuario web de Campaign son de solo lectura y se muestran como actividades incompatibles. Aún puede ejecutar el flujo de trabajo, enviar mensajes, comprobar los registros y realizar otras tareas. Las actividades de flujo de trabajo disponibles tanto en la interfaz de usuario web de Campaign como en la consola del cliente de Campaign se pueden editar.

| Consola | Web |
| --- | --- |
| ![Captura de pantalla que muestra limitaciones de actividades en la consola](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de pantalla que muestra limitaciones de actividades en la interfaz web](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Cuando una actividad de **Consulta** o **Enriquecimiento** se configura con datos adicionales en la consola, los datos de enriquecimiento se tienen en cuenta en la web de Campaign y pasan a la transición saliente, pero no se pueden editar.

| Consola | Web |
| --- | --- |
| ![Captura de pantalla que muestra las limitaciones de opciones en la consola](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de pantalla que muestra las limitaciones de las opciones en la interfaz web](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

En la consola, en la actividad **Enriquecimiento**, se puede realizar tanto la reconciliación como el enriquecimiento. Si ha definido la configuración de reconciliación en la actividad **Enrichment** de la consola del cliente, se mostrará como una actividad **Reconciliation** en la interfaz de usuario web de Campaign.

| Consola | Web |
| --- | --- |
| ![Captura de pantalla que muestra actividad de enriquecimiento en la consola](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de pantalla que muestra actividad de enriquecimiento en la interfaz web](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Lienzo de flujo de trabajo {#wkf-canvas}

Al crear un nuevo flujo de trabajo en la interfaz de usuario web de Campaign, el lienzo solo admite un punto de entrada. Sin embargo, si ha creado un flujo de trabajo en la consola con varios puntos de entrada, puede abrirlo y editarlo en la interfaz de usuario web de Campaign.

| Consola | Web |
| --- | --- |
| ![Captura de pantalla que muestra varios puntos de entrada en la consola](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de pantalla que muestra varios puntos de entrada en la interfaz web](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

La posición de los nodos se actualiza cada vez que se añade o elimina una actividad. Si crea un flujo de trabajo en la consola, lo modifica mediante la interfaz de usuario web de Campaign y lo vuelve a abrir en la consola, puede que observe algunas imperfecciones de posición menores. Esto no afecta a los procesos y tareas del flujo de trabajo.

| Flujo de trabajo inicial | Cambio de posición |
| --- | --- |
| ![Captura de pantalla que muestra el posicionamiento inicial del flujo de trabajo](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de pantalla que muestra cambios de posición después de modificaciones](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |