---
audience: end-user
title: Email Delivery Settings
description: Learn more about email delivery settings in Campaign Web UI
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
---
# Email delivery settings {#email-del-settings}

![Alpha version](../assets/do-not-localize/badge.png)

These settings are **technical delivery parameters** that are defined in the email template. They are available from the **Configure delivery settings** icon available when editing an email delivery.

## Email delivery settings {#email-delivery-settings}

>[!CAUTION]
>
> These settings are described for your information only. Some of them depend on your configuration and permissions. They must not be modified in this version of the product. 

## Typology {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typology"
>abstract="Typology lets you control, filter and monitor the sending of deliveries."

Typologies are sets of **typology rules**, that are executed during the message analysis phase. They allow you to make sure your emails always contain certain elements (such as an unsubscription link or a subject line) or filtering rules to exclude groups from your intended target (like unsubscribers, competitors, or non-loyalty customers).

When associating a typology with a message or message template, the typology rules included in the typology are executed to check the message validity during message preparation.

![](assets/delivery-settings-1.png)


### Pressure parameters {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Delivery weight"
>abstract="Delivery weights let you identify top-priority deliveries within the framework of pressure management. Messages with the highest weight have priority."

In this section, pressure parameters let you define a **threshold**. This is the maximum number of messages that can be sent to one profile over a given period. Once this threshold has been reached, no more deliveries can take place until the end of the period considered. This process lets you automatically exclude a profile from a delivery if a message exceeds the set threshold, thus avoiding over-solicitation.

Threshold values can be either constant or variable. This means that for a given period, thresholds can vary from one profile to another, or even for the same profile.

In the **Weight type** field, three options are available:

* **Constant**
* **Depends on the recipient**
* **Defined in each rule**

Use the **Delivery weight** field to define the delivery priority. Each delivery has a weight which represents its level of priority. By default, the weight of a delivery is set to 5. Pressure rules let you define the weight of the deliveries which they are applied to. Weights can be either set or calculated via a formula to suit recipients. For example, you can define the weight of a delivery based on recipient interests.


Use the **Delivery mode** field to select the target evaluation mode. Three modes are available:

* **Target estimation and message personalization**
* **Estimation and approval of the provisional target**
* **Target evaluation**

Fatigue management comes with the **Campaign Optimization** add-on. Learn more about pressure rules and how to configure fatigue management in [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}.

### Capacity settings {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importance of the recipient"
>abstract="The importance of the recipient is a formula used to determine which recipients are kept when the capacity typology rules are exceeded."

In this section, you can select a capacity rule defined in the Adobe Campaign v8 Console. This rule is associated to the email channel.

The **importance of the recipient** field is a formula used to determine which recipients are kept when the capacity typology rules are exceeded.

Learn more about consistency and capacity rules and how to configure them in [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## Audience {#audience}

In this section, you can select a **target mapping** among those available. Target mappings are defined in the Adobe Campaign v8 console. 

Learn more about target mappings in [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Delivery {#delivery}

Delivery parameters are technical settings which apply to your delivery. 

* **Routing**: the integrated email routing external account is provided by default. It contains the technical parameters that allow the application to send emails.

* **Test SMTP delivery**: this option is used to test sending via SMTP. The delivery is processed up to connection to the SMTP server but is not sent: for every recipient of the delivery, Campaign connects to the SMTP provider server, executes the SMTP RCPT TO command, and closes the connection before the SMTP DATA command.

* **Email BCC**: this option is used to store emails on an external system through BCC by simply adding a BCC email address to your message target. Learn more about Email BCC in [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### Retries {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Maximum number of retries"
>abstract="If a message fails due to a temporary error, retries are performed until the end of the delivery duration."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Learn more about retry management in [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Approval {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Approval mode"
>abstract="Each step of a delivery can be subject to approval in order to ensure full monitoring and control of the various processes."

If warnings are generated during the delivery preparation, you can configure the delivery to define whether or not it should still be executed. By default, the user must confirm the sending of messages at the end of the analysis phase: this is **manual** validation.

You can select another approval mode in the appropriate field. Available modes are: 

* **Manual**: At the end of the analysis phase, the user must confirm delivery to start sending. 

* **Semi-Automatic**: Sending begins automatically if the analysis phase generates no warning messages.

* **Automatic**: Sending begins automatically at the end of the analysis phase, irrespective of its result.


## Validity {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Delivery duration"
>abstract="The Delivery duration field lets you enter the limit for global delivery retries. This means that Adobe Campaign sends the messages beginning on the start date, and then, for messages returning an error only, regular, configurable retries are performed until the validity limit is reached."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, mainly for the mirror page and images. The resources on this page are valid for a limited time."


The **Delivery duration** field lets you enter the limit for global delivery retries. This means that Adobe Campaign sends the messages beginning on the start date, and then, for messages returning an error only, regular, configurable retries are performed until the validity limit is reached.

You can also choose to specify dates. To do this, select **Explicitly set validity dates**. In this case, the delivery and validity limit dates also let you specify the time. The current time is used by default, but you can modify this directly in the input field.

**Resources Validity limit** is used for uploaded resources, mainly for the mirror page and images. The resources on this page are valid for a limited time (to save disk space).

![](assets/delivery-settings-2.png)


Learn more about delivery validity period in [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Mirror page management {#mirror}

The mirror page is an HTML page accessible online via a web browser. Its content is identical to the email. By default, the mirror page is generated if the link is inserted in the content of the mail. 

In addition to the default mode, the following options are also available:

* **[!UICONTROL Force the generation of the mirror page]**: even if no link to the mirror page is inserted in the delivery, the mirror page is created.
* **[!UICONTROL Do not generate the mirror page]**: no mirror page is generated, even if the link is present in the delivery.
* **[!UICONTROL Generates a mirror page accessible using only the message identifier]**: this option lets you access the content of the mirror page, with personalization information, in the delivery log window. To do this, after the end of the delivery, click the **[!UICONTROL Delivery]** tab and select the line of the recipient whose mirror page you wish to view. Click the **[!UICONTROL Display the mirror page for this message...]** link.


### Tracking {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."

Tracking parameters are defined in the related section. Possible options are:

**Tracking validity limit**: use this option to change the duration for which the tracking is activated on the URLs.

**Substitution URL for expired URLs**: use this option to enter a URL to a fall-back web page: it is displayed once the tracking has expired.

## Test Settings {#test-setttings}

You can set the exclusion parameters in this section. Available options are:

* **Keep double** lets you authorize multiple deliveries to recipients who satisfy several targeting criteria.

* **Keep denylisted addresses** lets you keep from the target any profiles no longer being targeted by the delivery, such as after an unsubscription (opt-out).

* **Keep quarantined addresses** lets you keep from the target any profiles with an address that does not respond. 

You can also customize the name of the test emails.

Use the **Keep the delivery code for the proof** to associate to the test email the same delivery code as the one defined for the delivery to which it relates.

By default, the subject of the test email is prefixed by ‘PROOF #’, where # is the number of the test email. You can change this prefix in the **Label prefix** field.