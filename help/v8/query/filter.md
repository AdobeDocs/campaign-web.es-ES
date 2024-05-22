---
audience: end-user
title: Filtrar listas
description: Obtenga información sobre cómo filtrar listas web de Adobe Campaign mediante filtros integrados y personalizados.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 5%

---

# Filtrar listas {#filter-lists}

Adobe Campaign Web proporciona filtros dentro de cada lista de objetos, lo que permite filtrar la información en función de criterios contextuales específicos. Por ejemplo, puede filtrar los envíos según su estado, canal, fecha de contacto o carpeta. También puede ocultar las pruebas.

## Aplicar filtros{#apply}

Para aplicar filtros a una lista, haga clic en **[!UICONTROL Mostrar filtros]** situado en la esquina superior izquierda de la lista, junto a la barra de búsqueda.

Se abre el panel Filtros, que muestra los filtros disponibles para la lista seleccionada. Por ejemplo, puede filtrar las campañas por su estado, fechas de inicio y finalización o carpeta de almacenamiento, mientras que la lista de servicios de suscripción se puede filtrar por su canal y carpeta de almacenamiento.

![](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Para filtrar una lista según sus propios criterios, cree un filtro personalizado. Para ello, vaya a la parte inferior del panel de filtros y haga clic en **Agregar reglas** botón. [Obtenga información sobre cómo crear filtros personalizados](#custom)

Una vez aplicados a una lista, los filtros son visibles debajo de la barra de búsqueda. Puede quitar un filtro individual en cualquier momento o quitar todos los filtros haciendo clic en el icono **Borrar todo** botón.

## Creación de filtros personalizados {#custom}

Los filtros personalizados le permiten refinar las listas según sus propios criterios específicos. Se diseñan utilizando el modelador de consultas de Campaign. Para crear un filtro personalizado, siga estos pasos:

1. Abra el panel de filtros y haga clic en **Agregar reglas** situado en la parte inferior del panel.

1. Se abrirá el modelador de consultas. Defina y combine los criterios de filtro para adaptarlos a sus necesidades. Encontrará información detallada sobre cómo utilizar el modelador de consultas en [esta sección](../query/query-modeler-overview.md).

   El ejemplo siguiente muestra un filtro personalizado diseñado para mostrar en la lista de campañas las campañas SMS ejecutadas por operadores de los departamentos de Running o Yoga.

   ![](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Una vez configurado el filtro personalizado, haga clic en **[!UICONTROL Confirmar]** para aplicarlo a la lista.
