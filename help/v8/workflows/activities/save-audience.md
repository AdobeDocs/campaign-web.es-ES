---
audience: end-user
title: Uso de la actividad de flujo de trabajo Guardar audiencia
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
badge: label="Beta"
source-git-commit: 4924653e67f77a2108574e743c9016c6fc95a7e6
workflow-type: tm+mt
source-wordcount: '17'
ht-degree: 64%

---


# Guardado de audiencia {#save-audience}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_activity"
>title="Save an audience"
>abstract="Use this activity to save the workflow audience."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Outbound transition for save audience"
>abstract="tbc"

Mode
Audience label
Adobe Campaign is going to match this label against existing audiences. If it finds a match, it will update that audience, otherwise it will create a new audience.
Update method

Replace audience with new data

Complete audience with new data
Folder
Lists (/Profiles and Targets/Lists/)

Generate an outbound transition


The **Save audience** activity is a **Targeting** activity. This activity allows you to update an existing audience or create a new audience from the population computed upstream in a workflow. The audiences created are added to the list of application audiences, and are made available via the **Audiences** menu.

This activity is essentially used to keep population groups computed in the same workflow, by converting them into reusable audiences. Connect it to other targeting activities such as a **Build audience** or a **Combine** activity. 

## Configuration

Follow these steps to configure the **Save audience** activity:

1. Add a **Save audience** activity to your workflow.

   ![](../assets/workflow-save-audience.png)

1. In the **Mode** drop-down, select the action that you would like to carry out:

    * **Create or update an existing audience**: define an **Audience label**. If the audience already exists, it will be updated, otherwise a new audience will be created.

    * **Update an existing audience**: choose the **Audience** you wish to update among the list of existing audiences. 

1. Select the **Update mode** which will apply for existing audiences:

    * **Replace audience content with new data**: all audience content is replaced. The old data is lost. Only the data from the inbound transition of the save audience activity is kept. This option erases the audience type and the targeting dimension of the updated audience.

    * **Complete audience with new data**: the old audience content is kept and the data from the save audience activity's inbound transition is added to it.

1. Check the **Generate complement** option if you wish to exploit the remaining population. An additional transition will then be added to the activity.

The content of the saved audience is then available in the detail view of the audience, which can be accessed from the **Audiences** menu. The columns available from this view correspond to the columns of the inbound transition of the workflow's **SAve audience** activity. 


## Example



-->