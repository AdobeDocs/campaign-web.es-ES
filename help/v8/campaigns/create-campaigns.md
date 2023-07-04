---
audience: end-user
title: Creación de campañas con la web de Adobe Campaign
description: Aprenda a crear campañas en canales múltiples con la web de Adobe Campaign
badge: label="Alpha"
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: c9954ce69e50e1c8db2532be3292f71ff20f9f74
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 25%

---


# Cree su primera campaña {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Propiedades de creación de campañas"
>abstract="Defina propiedades y metadatos para la campaña."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Propiedades de campaña"
>abstract="Defina la configuración de la campaña y los metadatos."

Para crear una nueva campaña, debe definir sus propiedades, programar e incluir flujos de trabajo y envíos.

## Creación de la campaña{#campaign-create}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="Programación de campañas"
>abstract="Defina la programación de campañas durante la creación de campañas."

Para crear una nueva campaña, siga estos pasos:

1. Haga clic en **[!UICONTROL Campañas]** y haga clic en el **[!UICONTROL Crear campaña]** botón.
1. Seleccione el **Plantilla** para utilizar y proporcionar una etiqueta para la campaña. Las plantillas de campaña están preconfiguradas para que se puedan reutilizar en la creación de nuevas campañas. Se crean desde la consola del cliente.
   [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=es).
1. Si es necesario, puede cambiar lo siguiente **Opciones adicionales**: nombre interno, carpeta, usuario asignado, descripción y naturaleza.
1. Defina el **Programación** de la campaña. La campaña comienza cuando se llega a la fecha de inicio. Las fechas de inicio y finalización se muestran en la lista de campañas y se pueden utilizar como filtro. Consulte esta [sección](manage-campaigns.md#access-campaigns).

   ![Definición de las propiedades de la campaña](assets/campaign-properties.png)

   >[!NOTE]
   >
   >Siempre puede modificar estas propiedades más adelante, desde el **Configuración de la campaña** , junto a la etiqueta de campaña. Consulte esta [sección](gs-campaigns.md#campaign-dashboard).

1. Haga clic en **Create**.
1. Añadir flujos de trabajo y envíos a la campaña:

   * Desde el **Flujos de trabajo** pestaña, haga clic en **Crear flujo de trabajo**. Al crear la campaña, se añade automáticamente un flujo de trabajo predeterminado. Obtenga más información sobre cómo [creación de un flujo de trabajo](../workflows/create-workflow.md).
   * Desde el **Envíos** pestaña, haga clic en **Creación de envíos**. [Más información](../msg/gs-messages.md)

1. Utilice el **Registros** y **Informes** para analizar el rendimiento de su campaña.

## Monitorización y seguimiento de la campaña{#campaign-monitoring}

La monitorización de campañas es un paso clave para analizar la eficacia de su campaña. Abra la campaña y haga clic en **Registros** botón.

También puede ver los informes dedicados haciendo clic en **Informes** botón. Consulte esta [sección](../reporting/campaign-reports.md).



<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Workflow list"
>abstract="List of workflows available for your campaign. Use the 'Create workflow' button to add a workflow in your campaign."

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.

-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header


About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and help you organize your marketing activities: you can separate them by country, by brand, by unit, etc.
A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.
To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

Timeline
About dynamic reports
Creating a campaign
In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card and access a program or sub-program.

Click on the Create button and select Campaign.

In the Creation mode screen, select a campaign type.



The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date to your campaign. These dates only apply to the campaign itself.



Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

NOTE
Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.


Programs and campaigns icons and statuses
Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

Gray: the program/campaign has not yet started - Editing status.
Blue: the program/campaign is in progress - In progress status.
Green: the program/campaign has finished - Finished status. By default, the current date is automatically shown as the validity start date and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.


Business.Adobe.com resources
-->
