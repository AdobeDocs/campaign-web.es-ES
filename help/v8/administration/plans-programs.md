---
audience: end-user
title: Planes y programas
description: Obtenga información sobre cómo crear y configurar planes y programas en Adobe Campaign
source-git-commit: f9b8c0805d816075c5ee9ea9443f50cfead371d1
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Planes y programas

Adobe Campaign permite configurar la jerarquía de carpetas para planes y programas de marketing.

Para organizarlos mejor, Adobe recomienda la siguiente jerarquía: Plan `>` Programas `>` Campañas

* A **plan** puede contener varios programas. Define objetivos estratégicos para un período de tiempo.
* A **programa** puede contener otros programas, así como campañas, flujos de trabajo y páginas de aterrizaje.
* A **campaña** puede contener envíos, flujos de trabajo y páginas de aterrizaje.

## Creación y configuración de un plan {#create-plan}

Para crear un plan, debe crear una carpeta con el tipo de carpeta **[!UICONTROL Plan]** [Más información sobre la creación de una carpeta](create-manage-folder.md).

![](assets/plan_create.png){zoomable="yes"}

Vaya a la **[!UICONTROL Configuración de carpeta]** de su plan para administrarlo.

![](assets/plan_settings.png){zoomable="yes"}

Puede definir **[!UICONTROL Opciones personalizadas]** y para establecer la fecha de programación del plan.

![](assets/plan_options.png){zoomable="yes"}

Para administrar el  **[!UICONTROL Opciones personalizadas]**:

1. Vaya a la **[!UICONTROL Esquemas]**
1. Elija la **[!UICONTROL Editable]** esquemas en los filtros
1. Haga clic en el icono de **[!UICONTROL Editar detalles personalizados]**

![](assets/plan_edit.png){zoomable="yes"}

Puede configurarlas:

![](assets/plan_customfields.png){zoomable="yes"}

## Creación y configuración de un programa

Para crear un programa en su plan ([Más información sobre la creación de un plan](#create-plan)), debe estar en su plan y crear una carpeta con el tipo de carpeta **[!UICONTROL Programa]** [Más información sobre la creación de una carpeta](create-manage-folder.md).

![](assets/program_create.png){zoomable="yes"}

Vaya a la **[!UICONTROL Configuración de carpeta]** de su programa para administrarlo.

![](assets/program_settings.png){zoomable="yes"}

Puede definir **[!UICONTROL Opciones personalizadas]** y para establecer la fecha de programación del programa.

![](assets/program_options.png){zoomable="yes"}

Para administrar el  **[!UICONTROL Opciones personalizadas]**:

1. Vaya a la **[!UICONTROL Esquemas]**
1. Elija la **[!UICONTROL Editable]** esquemas en los filtros
1. Haga clic en el icono de **[!UICONTROL Editar detalles personalizados]**

![](assets/program_edit.png){zoomable="yes"}

Puede configurarlos de la siguiente manera:

![](assets/program_customfields.png){zoomable="yes"}

## Vinculación de una campaña a un programa

Tiene dos formas de vincular una campaña a un programa:

### Forma #1 : Ya tiene un programa y desea crear una campaña vinculada a él

Para vincular una nueva campaña a su programa, cree directamente su campaña en el programa:

![](assets/program_campaign_create.png){zoomable="yes"}

El **[!UICONTROL Carpeta]** la configuración se rellenará automáticamente con la ruta del programa.

![](assets/program_campaign_folder.png){zoomable="yes"}

### Forma #2 : ya tiene una campaña y desea vincularla a un programa existente

Vaya a la **[!UICONTROL Configuración]** de la campaña que desea vincular a su programa:

![](assets/campaign_settings.png){zoomable="yes"}

En su **[!UICONTROL Propiedades]**, haga clic en **[!UICONTROL Carpeta]** en el menú **[!UICONTROL Carpeta]** , para poder elegir su **[!UICONTROL Programa]** carpeta.

![](assets/campaign_folder.png){zoomable="yes"}

Seleccione su **[!UICONTROL Programa]** y haga clic en **[!UICONTROL Confirmar]** botón y, a continuación, en **[!UICONTROL Guardar y cerrar]** botón.

![](assets/campaign_linked.png){zoomable="yes"}

La campaña ahora aparece en el programa:

![](assets/campaign_in_program.png){zoomable="yes"}