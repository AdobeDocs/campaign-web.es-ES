---
audience: end-user
title: Consent
description: Learn about consent in Adobe Campaign Web
badge: label="Limited Availability"
---
# Manage consent {#manage-consent}

## General recommendations {#general-recommendations}

Adobe Campaign enables you to collect data, including personal and sensitive information. It is essential to obtain and monitor consent from recipients in compliance with data protection regulations such as GDPR (General Data Protection Regulation) and other applicable privacy laws.

* First, refrain from sending unsolicited email, push notifications, and SMS messages ("spam"). Adobe strongly supports the principles of permission marketing to foster customer lifetime value and loyalty. Adobe strictly forbids the use of Adobe Campaign for sending unsolicited messages. [Learn more](#denylisted-profiles)

* Always ensure recipients agree to receive communications by providing them the ability to opt out from your deliveries<!-- and keep honoring opt-out requests as quickly as possible-->. [Learn more](#opt-out)

* Use the subscription management process to manage recipients' preferences and track which recipients have opted in to specific types of subscriptions. [Learn more](../../delivery/using/about-services-and-subscriptions.md)

## Manage opt-out {#opt-out}

Providing recipients the ability to unsubscribe from receiving communications from a brand is a legal requirement. It is also necessary to ensure this choice is honored. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**Why is it important?**

* Failing to comply with these regulations introduces regulatory legal risks for your brand.
* It helps avoid sending unsolicited communications to recipients, which could lead them to mark your messages as spam and harm your reputation.

When sending deliveries using Adobe Campaign Web, ensure customers can unsubscribe from future communications. Once unsubscribed, profiles are automatically removed from the audience of future marketing messages.

### Email opt-out {#email-opt-out}

To allow recipients to unsubscribe from receiving email communications, include an **unsubscribe link** in every email sent to recipients.

Follow these steps:

1. Create an external landing page and host it on the third-party system of your choice.

1. Create an email delivery. [Learn how](../email/create-email.md)

1. Insert a link into your email content. [Learn how](../email/message-tracking.md#insert-links)

    ![Insert link into email content](../email/assets/message-tracking-insert-link.png)

1. In the **[!UICONTROL Url]** field, paste the link to your third-party landing page.

1. Click the **[!UICONTROL Links]** icon from the left pane to display the list of all URLs in your content to be tracked.

1. Click the pencil icon next to the new link to edit it.

1. Modify the **[!UICONTROL Tracking Type]** and set it to **[!UICONTROL Opt out]**.

   ![Edit tracking type for opt-out](../email/assets/message-tracking-edit-a-link.png)

1. Click **[!UICONTROL Save]** and send the message. [Learn more](../monitor/prepare-send.md)

1. Once the message is received, if the recipient clicks the unsubscribe link, your landing page is displayed.

1. When the recipient submits the landing page form, the profile data is updated. [Learn more](#denylisted-profiles)

<!--Any other option available such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Denylisted profiles {#denylisted-profiles}

After an unsubscription (opt-out), profiles are added to the **denylist** for a given channel. This means they are no longer targeted by any delivery.

>[!NOTE]
>
>If a profile on the denylist for the email channel has two email addresses, both addresses are excluded from delivery.

You can check if a profile is on the denylist for one or more channels in the **[!UICONTROL No longer contact]** section of the profile's **[!UICONTROL Details]** tab. [Learn more](../audience/about-recipients.md#access)

![Check denylist status in profile details](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more about quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->