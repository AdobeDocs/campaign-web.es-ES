---
audience: end-user
title: Creación de campañas con la web de Adobe Campaign
description: Aprenda a crear campañas en canales múltiples con la web de Adobe Campaign
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 35%

---

# Cree su primera campaña {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Propiedades de creación de campañas"
>abstract="En esta pantalla, defina la configuración de la campaña: seleccione una plantilla e introduzca una etiqueta para la campaña. Vaya a la configuración adicional para cambiar el nombre interno predeterminado, la carpeta, añadir una descripción y seleccionar la persona asignada."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Propiedades de campaña"
>abstract="En esta pantalla, puede comprobar y actualizar la configuración de la campaña: su etiqueta, nombre interno, carpeta y descripción. También puede ver a qué usuario está asignado."

Para crear una nueva campaña, defina su configuración, programe e incluya flujos de trabajo y envíos.

## Crear el campaña {#campaign-create}

Para crear una nueva campaña, seguir estos pasos:

1. Haga clic en el **[!UICONTROL menú Campañas]** y haga clic en el **[!UICONTROL Crear campaña]** botón.

   ![Captura de pantalla que muestra el botón &quot;Crear campaña&quot; en el menú Campañas](assets/create-campaign-button.png)

1. Seleccione la **plantilla** que desea utilizar y proporcione una etiqueta para el campaña. [Más información](manage-campaigns.md#manage-campaign-templates).
1. Si es necesario, cambie las siguientes **opciones** adicionales: nombre interno, carpeta, usuario asignado, descripción y naturaleza.
1. Defina el **horario** de su campaña. Obtén información sobre cómo configurar tu horario de campaña en [esta sección](#campaign-schedule).
1. Haga clic en **Crear**.

   ![Captura de pantalla que muestra la pantalla de propiedades de campaña, incluidos los campos de nombre interno, carpeta, usuario asignado, descripción y naturaleza.](assets/create-a-campaign-properties.png)

1. añadir flujos de trabajo y entregas a su campaña:

   * En la **pestaña Flujos de** trabajo, haga clic en **Crear flujo de trabajo**. Al crear el campaña, se añade automáticamente un flujo de trabajo predeterminado. Obtén más información sobre cómo [crear una flujo de trabajo](../workflows/create-workflow.md).

   * En la **pestaña Envíos** , haga clic en **Crear envío**. [Más información](../msg/gs-messages.md)

## Monitoree y rastree su campaña {#campaign-monitoring}

Campaign monitoreo es un paso clave para analizar la efectividad de su campaña. Abra el campaña y haga clic en el **botón Registros** .

También puede vista los informes dedicados haciendo clic en el **botón Informes** . Consulte esta [sección](../reporting/campaign-reports.md).

## Definición de la programación de la campaña {#campaign-schedule}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="Programación de campañas"
>abstract="Seleccione la programación de la campaña. Puede crear la campaña que comienza cuando se llega a la fecha de inicio. De forma predeterminada, la fecha de inicio de la campaña es la fecha de creación y dura 5 días. Las fechas de inicio y finalización se muestran en la lista de campañas y se pueden utilizar como filtro."

El campaña comienza cuando se llega a la fecha inicio. Mientras no se alcance la fecha inicio, el campaña tiene el estado de **[!UICONTROL borrador]** . Cuando se llega a **[!UICONTROL la fecha inicio, se convierte en En progreso]**. Una vez que se alcanza la fecha de finalización, el campaña se establece en **[!UICONTROL Completado]**.

Las fechas Inicio y final se muestran en el lista campaña y se pueden utilizar como filtro. Consulte esta [sección](manage-campaigns.md#access-campaigns).

>[!NOTE]
>
>Puede modificar estas propiedades más adelante desde el **icono Configurar campaña junto** a la etiqueta campaña. Consulte esta [sección](gs-campaigns.md#campaign-dashboard).

Una vez que se alcanza la fecha, las entregas creadas en ese campaña en el contexto de un flujo de trabajo, que están listas para ser enviadas, se envían realmente. Para ello, la flujo de trabajo debe haberse iniciado.

<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.
-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header

About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and helps you organize your marketing activities: you can separate them by country, by brand, by unit, and similar criteria.

A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.

To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

* Timeline
* About dynamic reports
* Creating a campaign

In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card, and access a program or sub-program.

Click on the Create button, and select Campaign.

In the Creation mode screen, select a campaign type.

The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date for your campaign. These dates only apply to the campaign itself.

Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

>[!NOTE]
>
>Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.

Programs and campaigns icons and statuses:

Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

* Gray: the program/campaign has not yet started - Editing status.
* Blue: the program/campaign is in progress - In progress status.
* Green: the program/campaign has finished - Finished status.

By default, the current date is automatically shown as the validity start date, and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.

Business.Adobe.com resources
-->