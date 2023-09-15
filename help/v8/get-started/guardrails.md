---
title: Protecciones y limitaciones en la IU web de Campaign
description: Protecciones y limitaciones en la IU web de Campaign
badge: label="Beta"
source-git-commit: 86d87e9a3ac9028634a08c2c0969cd232dff15f5
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 4%

---


# Mecanismos de protección y limitaciones {#guardrails-limitations}

Al trabajar en la IU web de Campaign con componentes creados o modificados en la consola del cliente de Campaign, se aplican las protecciones y limitaciones que se enumeran a continuación.

## Flujos de trabajo {#wf-guardrails-limitations}

**Actividades**

* Las actividades de flujo de trabajo que aún no son compatibles con la interfaz de usuario web son de solo lectura. Aún puede ejecutar el flujo de trabajo, enviar mensajes, comprobar los registros, etc. Las actividades de flujo de trabajo disponibles tanto en la interfaz de usuario web como en la consola del cliente son editables.

| Console | IU web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="50%" align="left" zoomable="yes"} |

**Lienzo**

* Al crear un nuevo flujo de trabajo en la interfaz de usuario web, el lienzo solo admite un punto de entrada. Sin embargo, si ha creado un flujo de trabajo en la consola con varios puntos de entrada,

Sin embargo, aunque el flujo de trabajo se haya creado en el lienzo de la consola del cliente con varios puntos de entrada, también se podrá editar en la interfaz de usuario web. Aún puede abrir y editar



Para probar este escenario, cree un flujo de trabajo desde la consola del cliente con varios puntos de entrada y ábralo desde la interfaz de usuario web para ver el resultado.



Por supuesto, puede editar las actividades e iniciar y ejecutar el flujo de trabajo como de costumbre.



**Posicionamiento de actividades**

* La posición de los nodos se recalculará (por lo tanto, la posición inicial de las actividades se modificará) solo cuando se haya agregado o eliminado una actividad (no todo el tiempo).

**Opciones no expuestas**

* Las opciones no compatibles no se muestran en la interfaz de usuario web.

**Bucles**

* Los bucles aún no están disponibles en la interfaz de usuario web. Si ha creado un flujo de trabajo que incluye un bucle mediante la consola, no puede acceder a él desde la interfaz de usuario web. Se muestra un mensaje de error.

| Console | IU web |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="50%" align="left" zoomable="yes"} |

**Reconciliación y enriquecimiento**

En la consola del cliente de Campaign, la variable **Enriquecimiento** La actividad de puede realizar tanto la reconciliación como el enriquecimiento. En la IU web de Campaign, las funcionalidades de reconciliación aún no están disponibles. Si ha establecido la reconciliación en la actividad de la consola, se mostrará como una actividad no compatible en la interfaz de usuario web.

* Si la variable **Enriquecimiento** actividad en la consola solo realiza un enriquecimiento, la variable **Enriquecimiento** la actividad se muestra en la web.
* Si la variable **Enriquecimiento** la actividad de en la consola solo realiza una reconciliación, se muestra una actividad incompatible.

## Filtros predefinidos {#filters-guardrails-limitations}

En esa versión del producto, al seleccionar la audiencia de una entrega o al crear una audiencia en un flujo de trabajo, algunos filtros predefinidos no están disponibles en la interfaz de usuario.

Se muestra un mensaje de error específico. Aunque no pueda ver la representación gráfica de la consulta en el generador de reglas y no pueda editar el filtro, puede utilizarlo y ver las condiciones de filtrado y los resultados. También puede acceder a la consulta SQL para comprobar la configuración exacta.

![](assets/filter-unavailable.png){width="70%" align="left"}

Tenga en cuenta que si genera un filtro en la interfaz Web y lo modifica en la consola con atributos no admitidos, la representación gráfica ya no podrá estar disponible en la interfaz Web. En cualquier caso, puede seguir utilizando el filtro.

A continuación se enumeran los atributos no admitidos.

### Tipos de datos no compatibles {#unsupported-data-type}

Los siguientes tipos de datos disponibles en la consola del cliente no son compatibles al mostrar un filtro o una regla en la interfaz web:

* datetime
* tiempo
* intervalo de tiempo
* doble
* float

### Funciones de filtrado no admitidas {#unsupported-filtering-capabilities}

Cuando se crea un filtro con expresiones y funciones complejas en la consola del cliente, no se puede editar en la interfaz web.

Además, no se admiten los siguientes operadores:

* Tipo numérico
   * está incluido en
   * no en

* Tipo de cadena
   * mayor que
   * menos de
   * mayor o igual que
   * menor o igual que
   * gustar
   * no me gusta

* Tipo de fecha
   * el o después
   * el o antes
   * no es igual a
   * está vacío
   * no está vacío
   * está incluido en
   * no en
   * en última instancia

* Vínculos 1-N
   * COUNT, SUM, AVG, MIN, MAX