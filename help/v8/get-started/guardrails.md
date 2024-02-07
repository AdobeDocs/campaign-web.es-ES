---
title: Protecciones y limitaciones en la interfaz de usuario web de Campaign
description: Protecciones y limitaciones en la interfaz de usuario web de Campaign
badge: label="Disponibilidad limitada"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: 5588adb52157370e265fbff803b25a8c1489d565
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 22%

---

# Mecanismos de protección y limitaciones {#guardrails-limitations}

Al trabajar en la interfaz de usuario web de Campaign con flujos de trabajo creados o modificados en la consola del cliente de Campaign, se aplican las protecciones y limitaciones enumeradas a continuación.

Tenga en cuenta que, aunque esta página identifica consideraciones clave al trabajar con flujos de trabajo en la consola y la interfaz de usuario web, no incluye todas las posibles incompatibilidades entre las dos interfaces.

## Actividades de flujo de trabajo {#wkf-activities}

Las actividades de flujo de trabajo que aún no se admiten en la web de Campaign son de solo lectura y se muestran como actividades incompatibles. Puede ejecutar de todos modos el flujo de trabajo, enviar mensajes, comprobar los registros, etc. Las actividades de flujo de trabajo disponibles tanto en la web de Campaign como en la consola del cliente son editables.

Las actividades de flujo de trabajo que aún no se admiten en la interfaz de usuario web de Campaign son de solo lectura y se muestran como actividades incompatibles. Puede ejecutar de todos modos el flujo de trabajo, enviar mensajes, comprobar los registros, etc. Las actividades de flujo de trabajo disponibles tanto en la interfaz de usuario web de Campaign como en la consola del cliente de Campaign son editables.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

Cuando un **Consulta** o un **Enriquecimiento** La actividad de se configura con datos adicionales en la consola; los datos de enriquecimiento se tienen en cuenta en Campaign Web y se pasan a la transición saliente, pero no se pueden editar.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

En la consola, la actividad **Enriquecimiento** puede realizar tanto la reconciliación como el enriquecimiento. Si ha definido, en la consola del cliente, la configuración de reconciliación en la variable **Enriquecimiento** actividad, se mostrará como una **Reconciliación** actividad en la interfaz de usuario web de Campaign.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){width="800px" align="left" zoomable="yes"} |

## Lienzo de flujo de trabajo {#wkf-canvas}

Al crear un nuevo flujo de trabajo en la interfaz de usuario web de Campaign, el lienzo solo admite un punto de entrada. Sin embargo, si ha creado un flujo de trabajo en la consola con varios puntos de entrada, puede abrirlo y editarlo en la interfaz de usuario web de Campaign.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

La posición de los nodos se actualiza cada vez que se añade o elimina una actividad. Si crea un flujo de trabajo en la consola, lo modifica mediante la interfaz de usuario web de Campaign y lo vuelve a abrir en la consola, puede que observe algunas imperfecciones de posición menores. Esto no afecta a los procesos y tareas del flujo de trabajo.

| Flujo de trabajo inicial | Cambio de posición |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |
