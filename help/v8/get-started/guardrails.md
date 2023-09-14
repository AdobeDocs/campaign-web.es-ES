---
title: Protecciones y limitaciones en la IU web de Campaign
description: Protecciones y limitaciones en la IU web de Campaign
badge: label="Beta"
source-git-commit: ff95b563784ae507245e6690feedda33ea6a111b
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 2%

---


# Mecanismos de protección y limitaciones {#guardrails-limitations}

Al trabajar en la IU web de Campaign con componentes creados o modificados en la consola del cliente de Campaign, se aplican las protecciones y limitaciones que se enumeran a continuación.

## Flujos de trabajo {#wf-guardrails-limitations}

Se puede acceder al mismo flujo de trabajo tanto en la consola como en la interfaz de usuario web. Sin embargo, tenga en cuenta que se aplican ciertas limitaciones.

**Activity Edition**

* Al acceder a un flujo de trabajo de la consola en la interfaz de usuario web, solo puede modificar las actividades compatibles.

**Edición en lienzo**

* Si un flujo de trabajo de la consola tiene varios nodos/ramas de inicio o actividades flotantes, debe agregar una actividad de inicio y una ramificación para conectar los nodos de inicio al nodo principal. También debe eliminar las actividades flotantes.

**Posicionamiento de actividades**

* La posición de los nodos se recalculará (por lo tanto, la posición inicial de las actividades se modificará) solo cuando se haya agregado o eliminado una actividad (no todo el tiempo).

**Opciones no expuestas**

* Las opciones no compatibles no se muestran en la interfaz de usuario web.

**Bucles**

* Los flujos de trabajo, incluidos los bucles, no se muestran en la IU web. Se muestra un mensaje de error.

**Reconciliación y enriquecimiento**

En la consola del cliente de Campaign, la variable **Enriquecimiento** La actividad de puede realizar tanto la reconciliación como el enriquecimiento. En la IU web de Campaign, las funcionalidades de reconciliación aún no están disponibles. Si ha establecido la reconciliación en la actividad de la consola, se mostrará como una actividad no compatible en la interfaz de usuario web.

* Si la variable **Enriquecimiento** actividad en la consola solo realiza un enriquecimiento, la variable **Enriquecimiento** la actividad se muestra en la web.
* Si la variable **Enriquecimiento** la actividad de en la consola solo realiza una reconciliación, se muestra una actividad incompatible.

## Filtros predefinidos {#filters-guardrails-limitations}


Al seleccionar la audiencia de una entrega o al crear una audiencia en un flujo de trabajo, algunos filtros predefinidos no están disponibles. Se muestra un mensaje de error específico. Puede seguir utilizando la consulta y ver: la condición de filtrado y los resultados, pero no puede ver la consulta exacta en el generador de reglas y no puede editar el filtro.

![](assets/filter-unavailable.png)
