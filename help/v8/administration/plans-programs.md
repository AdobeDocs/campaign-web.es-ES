---
audience: end-user
title: Planes y programas
description: Obtenga información sobre cómo crear y configurar planes y programas en Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
TQID: https://experienceleague.adobe.com/FSiHCjupRlS0zoI9HPdcU--Y2PZot5fQOzWICwmV-oQ
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 522
ht-degree: 6%

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

## Creación y configuración de un programa

Para crear un programa en tu plan ([Más información sobre cómo crear un plan](#create-plan)), ve a tu plan y crea una carpeta con el tipo de carpeta **[!UICONTROL Programa]**. [Más información sobre cómo crear una carpeta](../get-started/work-with-folders.md).

![Captura de pantalla que muestra la creación de una carpeta de programa](assets/program_create.png){zoomable="yes"}

Vaya a la **[!UICONTROL configuración de carpeta]** de su programa para administrarla.

![Captura de pantalla que muestra la configuración de carpeta de un programa](assets/program_settings.png){zoomable="yes"}

Defina **[!UICONTROL opciones personalizadas]** y establezca la fecha de programación de su programa.

![Captura de pantalla que muestra las opciones personalizadas de un programa](assets/program_options.png){zoomable="yes"}

Para administrar **[!UICONTROL opciones personalizadas]**:

1. Vaya a **[!UICONTROL Esquemas]**.
1. Elija los **[!UICONTROL esquemas editables]** en los filtros.
1. Haga clic en el esquema.

![Captura de pantalla que muestra la edición de detalles personalizados para un programa](assets/program_edit.png){zoomable="yes"}

1. Haga clic en el botón **[!UICONTROL Edición de pantalla]**.

   ![](assets/program_edit2.png){zoomable="yes"}

Configure las opciones personalizadas:

![Captura de pantalla que muestra la configuración de campos personalizados para un programa](assets/program_customfields.png){zoomable="yes"}

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