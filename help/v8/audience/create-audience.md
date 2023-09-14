---
audience: end-user
title: Creación de audiencias
description: Obtenga información sobre cómo crear audiencias en Adobe Campaign Web
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 1%

---


# Creación de audiencias {#create-audiences}

Campaign Web le permite crear flujos de trabajo donde puede combinar audiencias existentes en un lienzo visual y aprovechar varias actividades (dividir, excluir...) para crear nuevas audiencias.

Una vez realizadas, las audiencias resultantes se guardan y se copian en la web de Campaign junto con las audiencias existentes, y se pueden aprovechar en envíos independientes o campañas dirigidas a particulares.

## Cree su primera audiencia {#create}

Para crear una audiencia, siga estos pasos:

1. Vaya a **[!UICONTROL Audiencias]** y haga clic en **[!UICONTROL Crear audiencia]** en la esquina superior derecha.
1. Proporcione una etiqueta para la audiencia.
1. Expanda la sección Opciones adicionales para configurar los parámetros de Advancer para la audiencia.

   >[!NOTE]
   >
   >De forma predeterminada, las audiencias se crean en el menú Explorador de perfiles y objetivos/listas. Puede cambiar la ubicación de almacenamiento predeterminada en la **[!UICONTROL Carpeta]** field.

1. Una vez establecida la configuración de la audiencia, haga clic en **[!UICONTROL Crear audiencia]** botón.

1. Se muestra un lienzo de flujo de trabajo con dos actividades predeterminadas:

   * **[!UICONTROL Crear audiencia]**: el punto de partida del flujo de trabajo. Esta actividad le permite seleccionar una o varias audiencias como base para el flujo de trabajo,
   * **[!UICONTROL Guardar audiencia]**: el último paso del flujo de trabajo. Esta actividad le permite guardar el resultado del flujo de trabajo en una nueva audiencia.

1. Configure el flujo de trabajo añadiendo tantas actividades como sea necesario. Para obtener más información sobre cómo configurar las distintas actividades, consulte la [documentación de flujos de trabajo](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Las actividades de canal no están disponibles para su uso en flujos de trabajo de audiencia.

   ![](assets/audience-creation-canvas.png)

1. Cuando el flujo de trabajo esté listo, haga clic en **[!UICONTROL Inicio]** para ejecutarlo.

1. El flujo de trabajo se guarda en **[!UICONTROL Flujos de trabajo]** y la audiencia o audiencias resultantes en la lista **[!UICONTROL Audiencias]** lista. [Obtenga información sobre cómo monitorizar y administrar audiencias](access-audiences.md)
