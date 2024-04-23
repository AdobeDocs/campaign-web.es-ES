---
audience: end-user
title: Consentimiento
description: Obtenga información sobre el consentimiento en Adobe Campaign Web
badge: label="Disponibilidad limitada"
source-git-commit: 9a184d7558ca39be3afed4a7217a5e5687799c0d
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 13%

---

# Administración del consentimiento {#manage-consent}

## Recomendaciones generales {#general-recommendations}

Adobe Campaign le permite recopilar datos, incluida la información personal y confidencial. Por lo tanto, es esencial que obtenga y supervise el consentimiento de sus destinatarios en cumplimiento con las regulaciones de protección de datos como el RGPD (Reglamento General de Protección de Datos) y otras leyes de privacidad aplicables.

* En primer lugar, absténgase de enviar correos electrónicos no solicitados, notificaciones push y mensajes SMS (&quot;correo no deseado&quot;). Adobe cree firmemente en los principios del marketing autorizado para fomentar la lealtad y el valor de tiempo de vida del cliente; por lo tanto, prohíbe estrictamente el uso de Adobe Campaign para la entrega de mensajes no solicitados. [Más información](#denylisted-profiles)

* Los destinatarios siempre deben aceptar recibir comunicaciones proporcionándoles la capacidad de excluirse de las entregas<!-- and keep honoring opt-out requests as quickly as possible-->. [Más información](#opt-out)

* A través del proceso de administración de suscripciones, puede administrar las preferencias de sus destinatarios y rastrear qué destinatarios han elegido qué tipo de suscripciones. [Más información](../../delivery/using/about-services-and-subscriptions.md)

## Administración de la exclusión {#opt-out}

Proporcionar a los destinatarios la capacidad de cancelar la suscripción a la recepción de comunicaciones de una marca es un requisito legal, así como garantizar que se cumpla esta opción. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**¿Por qué es importante?**

* El incumplimiento de estas regulaciones conlleva riesgos legales para su marca.
* Le ayuda a evitar enviar comunicaciones no solicitadas a sus destinatarios, lo que podría hacer que marquen sus mensajes como correo no deseado y dañar su reputación.

Al realizar envíos a través de la web de Adobe Campaign, siempre debe asegurarse de que los clientes puedan cancelar la suscripción a comunicaciones futuras. Una vez cancelada la suscripción, los perfiles se eliminan automáticamente de la audiencia de futuros mensajes de marketing.

### Exclusión de correo electrónico {#email-opt-out}

Para proporcionar a los destinatarios la capacidad de cancelar la suscripción a la recepción de comunicaciones por correo electrónico, siempre debe incluir un **vínculo de cancelación de suscripción** en cada correo electrónico enviado a los destinatarios.

Para realizar esto, siga los pasos a continuación.

1. Cree una página de aterrizaje externa y aloje la página en el sistema de terceros que elija.

1. Creación de una entrega por correo electrónico. [Descubra cómo](../email/create-email.md)

1. Inserte un vínculo al contenido del correo electrónico. [Descubra cómo](../email/message-tracking.md#insert-links)

   ![](../email/assets/message-tracking-insert-link.png)

1. En el **[!UICONTROL Url]** , pegue el vínculo a la página de aterrizaje de terceros.

1. Haga clic en el icono **[!UICONTROL Vínculos]** del panel izquierdo para mostrar la lista de todas las direcciones URL del contenido que se va a rastrear.

1. Haga clic en el icono de lápiz situado junto al nuevo vínculo para editarlo.

1. Modifique la **[!UICONTROL Tipo de seguimiento]** y configúrelo en **[!UICONTROL Opción de exclusión]**.

   ![](../email/assets/message-tracking-edit-a-link.png)

1. Clic **[!UICONTROL Guardar]** y enviar el mensaje. [Más información](../monitor/prepare-send.md)

1. Una vez recibido el mensaje, si el destinatario hace clic en el vínculo para cancelar la suscripción, se muestra la página de aterrizaje.

1. Cuando el destinatario envía el formulario de página de aterrizaje, se actualizan los datos de perfil. [Más información](#denylisted-profiles)

<!--Any other option availabe such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Incluir en la lista de bloqueados perfiles de {#denylisted-profiles}

Después de una baja (exclusión), los perfiles se encuentran en la **lista de bloqueados de** para un canal determinado: esto implica que ya no se tienen en cuenta para las entregas.

>[!NOTE]
>
>Si un perfil de la lista de bloqueados de la para el canal de correo electrónico tiene dos direcciones de correo electrónico, ambas se excluirán de la entrega.

Puede comprobar si un perfil está en la lista de bloqueados de la para uno o más canales en la **[!UICONTROL Ya no se puede contactar]** de la sección del perfil **[!UICONTROL Detalles]** pestaña. [Más información](../audience/about-recipients.md#access)

![](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more on quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->



