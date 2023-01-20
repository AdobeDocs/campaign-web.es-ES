---
audience: end-user
title: Set a control group
description: Learn how to set a control group for your messages in Campaign Web UI
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
---
# Set a control group {#control-group}

You can use control groups to avoid sending messages to a portion of your audience in order to measure the impact of your campaigns.

To do this, create a control group when defining the audience of your delivery. Profiles are added to the control group randomly, filtered or not, or based on criteria. You can then compare the behavior of the target population which did receive the message with the behavior of contacts which were not targeted. 

The control group can be extracted randomly from the main target and/or selected from a specific population. Consequently, there are two main ways you can define a control group:

* Extract a number of profiles from the main target.
* Exclude some profiles based on criteria defined in a query.

You can use both methods when defining a control group.

All profiles being part of the control group at the delivery preparation step are removed from the main target. They do not receive the message.

To create a control group, click the **[!UICONTROL Set Control Group]** button, from the **Audience** section of the delivery creation assistant.

![](assets/control-group1.png)

## Extract from target {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extract from target"
>abstract="TBC"

To define a control group, you can choose to extract, randomly or based on a sorting, a percentage or a fixed number of profiles from the target population.

First, define the way the profiles are e extracted from the target: randomly or based on a sorting.

Under the **Extract from target** section, choose an **Exclusion type**:

* **Random**: when preparing the delivery, Adobe Campaign  randomly extracts a number of profiles corresponding to the percentage or to the maximum number that is set as the size limit.

    ![](assets/control-group.png)

* **Ranked by attribute(s)**: this option enables you to exclude a set of profiles based on specific attribute(s) in a specific sorting order(s).

    ![](assets/control-group2.png)

Then define the **Size limit**: you must set how you are going to limit the number of profiles that you extract from the main target. 

**Example**

You can view the logs to check and identify the exluded profiles. Let's take the example of a random exclusion on five profiles.

![](assets/control-group4.png)

After the delivery preparation, you can view the exclusions on the following screens:

* The **To exclude** KPI in the delivery dashboard, before the sending.

    ![](assets/control-group5.png)

* The **Exclusion logs** display each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png)

* The **Exclusion causes** display the number of excluded profile for each typology rule.

    ![](assets/control-group7.png)

For more information on delivery logs, refer to this [section](../monitor/delivery-logs.md).

## Extra population {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Extra population"
>abstract="TBC"

Another way to define a control group is to exclude a specific population from the target using an existing audience or by defining a query.

From the **Extra population** section of the **Control Group** definition screen, click the **[!UICONTROL Select Audience]** button.

![](assets/control-group3.png)

* To use an existing audience, click **Select audience**. Refer to this [section](add-audience.md). 

* To define a new query, select **Create your own** and define the exclusion criteria using the rule builder. Refer to this [section](segment-builder.md). 

The profiles included in the audience or matching the result of the query are excluded from the target.