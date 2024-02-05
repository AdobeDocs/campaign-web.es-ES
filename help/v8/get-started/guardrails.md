---
title: Protecciones y limitaciones en la interfaz de usuario web de Campaign
description: Protecciones y limitaciones en la interfaz de usuario web de Campaign
badge: label="Beta"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: db06e0f54984991e1d6b1056932a9974e340546e
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 65%

---

# Mecanismos de protección y limitaciones {#guardrails-limitations}

Al trabajar en la interfaz de usuario web de Campaign con componentes creados o modificados en la consola del cliente de Campaign, se aplican las protecciones y limitaciones que se enumeran a continuación.

## Flujos de trabajo {#wf-guardrails-limitations}

### Actividades

Las actividades de flujo de trabajo que aún no se admiten en la interfaz de usuario web de Campaign son de solo lectura y se muestran como actividades incompatibles. Puede ejecutar de todos modos el flujo de trabajo, enviar mensajes, comprobar los registros, etc. Las actividades de flujo de trabajo disponibles tanto en la interfaz de usuario web de Campaign como en la consola del cliente de Campaign son editables.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

No se muestran los ajustes de actividad de flujo de trabajo que aún no son compatibles con la interfaz de usuario web. Sin embargo, cuando se ejecuta el flujo de trabajo, se aplica esta configuración.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

En la consola, la actividad **Enriquecimiento** puede realizar tanto la reconciliación como el enriquecimiento. En la interfaz de usuario web de Campaign, las funcionalidades de reconciliación aún no están disponibles. Si ha definido, en la consola del cliente, la configuración de reconciliación en la variable **Enriquecimiento** actividad, se muestra como una actividad de solo lectura no compatible en la interfaz de usuario web de Campaign.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

### Lienzo

Al crear un nuevo flujo de trabajo en la interfaz de usuario web de Campaign, el lienzo solo admite un punto de entrada. Sin embargo, si ha creado un flujo de trabajo en la consola con varios puntos de entrada, puede abrirlo y editarlo en la interfaz de usuario web de Campaign.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

Los bucles aún no están disponibles en la interfaz de usuario web de Campaign. Si ha creado un flujo de trabajo que incluye un bucle mediante la consola, no puede acceder a él desde la interfaz de usuario web de Campaign. Se muestra un mensaje de error.

| Consola | Web |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="800px" align="left" zoomable="yes"} |

La posición de los nodos se actualiza cada vez que se añade o elimina una actividad. Si crea un flujo de trabajo en la consola, lo modifica mediante la interfaz de usuario web de Campaign y lo vuelve a abrir en la consola, puede que observe algunas imperfecciones de posición menores. Esto no afecta a los procesos y tareas del flujo de trabajo.

| Flujo de trabajo inicial | Cambio de posición |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |

## Filtros predefinidos {#filters-guardrails-limitations}

>[!CONTEXTUALHELP]
>id="acw_predefined_filter_read_only"
>title="Este filtro es de solo lectura"
>abstract="Algunos filtros predefinidos no están disponibles en la interfaz de usuario en esa versión del producto. Estos filtros están marcados como de solo lectura. Aunque no pueda ver la representación gráfica de la consulta en el modelador de consultas y no pueda editar el filtro, puede utilizarlo y ver las condiciones de filtrado en la sección **Atributos** de la pantalla."

Al seleccionar el público de un envío o al crear un público en un flujo de trabajo, algunos filtros predefinidos no están disponibles en la interfaz de usuario en esa versión del producto. Estos filtros están marcados como de solo lectura.

Se muestra un mensaje de error específico.

![](assets/filter-unavailable.png){width="70%" align="left"}

Aunque no pueda ver la representación gráfica de la consulta en el modelador de consultas y no pueda editar el filtro, puede utilizarlo y ver las condiciones de filtrado en la sección **Atributos** de la pantalla.

![](assets/rule-edit.png){width="70%" align="left"}

También puede acceder a la consulta SQL para comprobar la configuración exacta. Para ello, haga clic en el botón **Vista de código**.

![](assets/rule-code-view.png){width="70%" align="left"}

Haga clic en el botón **Calcular** para comprobar cuántos elementos cumplen los criterios del filtro.

![](assets/rule-calculate.png){width="70%" align="left"}

Use el botón **Ver resultados** para mostrar esos elementos.

![](assets/rule-view-results.png){width="70%" align="left"}

Tenga en cuenta que si genera un filtro en la interfaz web y lo modifica en la consola con atributos no admitidos, la representación gráfica ya no estará disponible en la interfaz web. En cualquier caso, podrá utilizar el filtro.

A continuación se enumeran los atributos no admitidos.

### Tipos de datos no compatibles {#unsupported-data-type}

Los siguientes tipos de datos disponibles en la consola del cliente no son compatibles al mostrar un filtro o una regla en la interfaz web:

* datetime
* tiempo
* intervalo de tiempo
* doble
* flotante

### Funcionalidades de filtrado no admitidas {#unsupported-filtering-capabilities}

Cuando se crea un filtro con expresiones y funciones complejas en la consola del cliente, no se puede editar en la interfaz web.

Además, no se admiten los siguientes operadores:

* Tipo numérico
   * Se incluye en
   * no en

* Tipo de cadena
   * mayor que
   * menos de
   * mayor que o igual a
   * menor que o igual a
   * like
   * not like

* Tipo de fecha
   * el o después
   * el o antes
   * no es igual a
   * está vacío
   * no está vacío
   * Se incluye en
   * no en
   * en el último

* 1-N links
   * COUNT, SUM, AVG, MIN, MAX
