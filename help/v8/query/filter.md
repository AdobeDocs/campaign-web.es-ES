---
audience: end-user
title: Filtrar listas
description: Obtenga información sobre cómo filtrar listas web de Adobe Campaign mediante filtros integrados y personalizados.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 485d8b4b715192cc5edb6442df0fa958e29d15ff
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Filtrar listas {#filter-lists}

Adobe Campaign Web proporciona filtros dentro de cada lista de objetos, lo que permite filtrar la información en función de criterios contextuales específicos. Por ejemplo, puede filtrar las entregas según su estado, canal, fecha de contacto o carpeta. También puede ocultar las pruebas.

>[!IMPORTANT]
>
>Hay disponible una interfaz completamente nueva para el modelador de consultas. El nuevo generador de reglas le permite crear la consulta con mayor facilidad gracias a su interfaz simplificada. Para cambiar a esta experiencia, pulse el botón de alternancia en la esquina superior derecha. Puede volver al modelador de consultas clásico en cualquier momento simplemente pulsando la tecla de retroceso para desactivar la nueva interfaz. Puede aplicar los mismos principios que el modelador de consultas en esta nueva interfaz.
>&#x200B;>![Imagen que muestra el conmutador para la nueva interfaz del generador de reglas](assets/query-modeler-toggle.png){zoomable="yes"}

## Aplicar filtros {#apply}

Para aplicar filtros a una lista, haga clic en el botón **[!UICONTROL Mostrar filtros]** situado en la esquina superior izquierda de la lista, junto a la barra de búsqueda.

Se abre el panel Filtros, que muestra los filtros disponibles para la lista seleccionada. Por ejemplo, puede filtrar las campañas en función de su estado, fechas de inicio y finalización o carpeta de almacenamiento, mientras que la lista de servicios de suscripción se puede filtrar según su canal y carpeta de almacenamiento.

![El panel Filtros muestra los filtros disponibles para las listas](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Para filtrar una lista según sus propios criterios, cree un filtro personalizado. Para ello, vaya a la parte inferior del panel de filtros y haga clic en el botón **Agregar reglas**. [Aprenda a crear filtros personalizados](#custom).

Una vez aplicados a una lista, los filtros son visibles debajo de la barra de búsqueda. Puede quitar un filtro individual en cualquier momento o quitar todos los filtros haciendo clic en el botón **Borrar todo**.

## Creación de filtros personalizados {#custom}

Los filtros personalizados le permiten refinar las listas según sus propios criterios específicos. Se diseñan utilizando el modelador de consultas de Campaign. Para crear un filtro personalizado, siga estos pasos:

1. Abra el panel de filtros y haga clic en el botón **Agregar reglas** situado en la parte inferior del panel.

1. Se abrirá el modelador de consultas. Defina y combine los criterios de filtro para adaptarlos a sus necesidades. Encontrará información detallada sobre cómo usar el modelador de consultas en [esta sección](../query/query-modeler-overview.md).

   El ejemplo siguiente muestra un filtro personalizado diseñado para mostrar en la lista de campañas las campañas SMS ejecutadas por operadores de los departamentos de Running o Yoga.

   ![Ejemplo de filtro personalizado que muestra campañas SMS filtradas por departamento](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Una vez configurado el filtro personalizado, haga clic en **[!UICONTROL Confirmar]** para aplicarlo a la lista.