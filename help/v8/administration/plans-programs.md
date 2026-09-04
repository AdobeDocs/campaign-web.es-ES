---
audience: end-user
title: Planes y programas
description: Obtenga información sobre cómo crear y configurar planes y programas en Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
TQID: https://experienceleague.adobe.com/FSiHCjupRlS0zoI9HPdcU--Y2PZot5fQOzWICwmV-oQ
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: 640
ht-degree: 5%

---

# Planes y programas {#plan-and-programs}

Adobe Campaign permite configurar la jerarquía de carpetas para planes y programas de marketing.

Para organizar mejor estos componentes, Adobe recomienda la siguiente jerarquía: Planificar `>` Programas `>` Campañas.

* Un **plan** puede contener varios programas. Define objetivos estratégicos para un periodo específico.
* Un **programa** puede contener otros programas, así como campañas, flujos de trabajo y páginas de destino.
* Una **campaña** puede contener envíos, flujos de trabajo y páginas de aterrizaje.

## Creación y configuración de un plan {#create-plan}

Para crear un plan, cree una carpeta con el tipo de carpeta **[!UICONTROL Plan]**. [Más información sobre cómo crear una carpeta](../get-started/work-with-folders.md)

![Captura de pantalla que muestra la creación de una carpeta de plan](assets/plan_create.png){zoomable="yes"}

Vaya a la **[!UICONTROL configuración de la carpeta]** de su plan para administrarla.

![Captura de pantalla que muestra la configuración de la carpeta de un plan](assets/plan_settings.png){zoomable="yes"}

Defina **[!UICONTROL opciones personalizadas]** y establezca la fecha de horario de su plan.

![Captura de pantalla que muestra las opciones personalizadas de un plan](assets/plan_options.png){zoomable="yes"}

Para administrar **[!UICONTROL opciones personalizadas]**:

1. Vaya a **[!UICONTROL Esquemas]**.
1. Elija los **[!UICONTROL esquemas editables]** en los filtros.
1. Haga clic en el esquema.

![Captura de pantalla que muestra la edición de detalles personalizados para un plan](assets/plan_edit.png){zoomable="yes"}

1. Haga clic en el botón **[!UICONTROL Edición de pantalla]**.

   ![](assets/plan_edit2.png){zoomable="yes"}

Configure las opciones personalizadas:

![Captura de pantalla que muestra la configuración de campos personalizados para un plan](assets/plan_customfields.png){zoomable="yes"}

## Creación y configuración de un programa {#create-program}

Los programas están disponibles en el menú de navegación de la izquierda, de forma similar a las vistas de lista de campañas, envíos y flujos de trabajo. La entrada **[!UICONTROL Programas]** permite crear un programa dentro de un programa existente, no bajo un plan.

Para crear su primer programa de nivel superior en un plan, navegue hasta su plan en el Explorador (consulte esta [sección](#create-plan)) y cree una carpeta con el tipo de carpeta **[!UICONTROL Programa]**. [Más información sobre cómo crear una carpeta](../get-started/work-with-folders.md).

Para crear un programa dentro de uno existente, siga los pasos a continuación:

1. Vaya a la entrada **[!UICONTROL Programas]** en el menú de navegación de la izquierda. Esta vista enumera todos los programas y le permite buscar y filtrar. Al hacer clic en un programa, se abre en la vista del explorador.

   ![Captura de pantalla que muestra la vista de lista de programas](assets/program_view.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Crear programa]** y configure las siguientes opciones:

   ![Captura de pantalla que muestra la pantalla Crear programa](assets/program_create.png){zoomable="yes"}

   * Escriba una **[!UICONTROL etiqueta]**.
   * Seleccione el programa existente que se usará como **[!UICONTROL carpeta principal]**.
   * De manera opcional, establezca un **[!UICONTROL Intervalo de fechas]** en la sección **[!UICONTROL Programar]**.

   >[!TIP]
   >
   >Si crea un programa desde la vista del explorador, la carpeta principal se establece automáticamente en el programa actual.

1. Vuelva a hacer clic en **[!UICONTROL Crear programa]** para guardar los cambios y crear el programa. A continuación, el programa se muestra en la vista del explorador. Puede cambiarle el nombre, eliminarlo y acceder a su configuración, como cualquier otra carpeta. También puede crear programas secundarios dentro de este programa.

   ![Captura de pantalla que muestra el programa en la vista del explorador](assets/program_explorer.png){zoomable="yes"}

Las opciones personalizadas de un programa se configuran del mismo modo que para un plan. Ver [Crear y configurar un plan](#create-plan).

## Vinculación de una campaña a un programa

Tiene dos formas de vincular una campaña a un programa:

### Forma #1: ya tiene un programa y desea crear una campaña vinculada a él

Para vincular una nueva campaña al programa, cree la campaña directamente dentro del programa.

![Captura de pantalla que muestra la creación de una campaña dentro de un programa](assets/program_campaign_create.png){zoomable="yes"}

La configuración de **[!UICONTROL Carpeta]** se rellenará automáticamente con la ruta de acceso a su programa.

![Captura de pantalla que muestra la configuración de la carpeta para una campaña vinculada a un programa](assets/program_campaign_folder.png){zoomable="yes"}

### Forma #2: ya tiene una campaña y desea vincularla a un programa existente

Vaya al botón **[!UICONTROL Configuración]** de la campaña que desea vincular a su programa.

![Captura de pantalla que muestra el botón de configuración de una campaña](assets/campaign_settings.png){zoomable="yes"}

En sus **[!UICONTROL propiedades]**, haga clic en el icono **[!UICONTROL Carpeta]** en la configuración de **[!UICONTROL Carpeta]** para elegir la carpeta **[!UICONTROL Programa]**.

![Captura de pantalla que muestra la selección de carpetas para vincular una campaña a un programa](assets/campaign_folder.png){zoomable="yes"}

Seleccione la carpeta **[!UICONTROL Programa]**, haga clic en el botón **[!UICONTROL Confirmar]** y, a continuación, haga clic en el botón **[!UICONTROL Guardar y cerrar]**.

![Captura de pantalla que muestra una campaña vinculada a un programa](assets/campaign_linked.png){zoomable="yes"}

La campaña ahora aparece en el programa.

![Captura de pantalla que muestra una campaña en un programa](assets/campaign_in_program.png){zoomable="yes"}