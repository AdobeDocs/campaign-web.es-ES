---
solution: Journey Optimizer
product: journey optimizer
title: Casos de uso de página de aterrizaje
description: Descubra los casos de uso más comunes con las páginas de aterrizaje en Journey Optimizer
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: aterrizaje, página de aterrizaje, caso de uso
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 0%

---

# Cómo utilizar una página de aterrizaje {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Copie la URL con precaución"
>abstract="Para probar o aprovechar al máximo la página de aterrizaje, no puede copiar y pegar este vínculo directamente en un explorador web o en las entregas. En su lugar, utilice el **Simular contenido** para probarla y siga los pasos descritos en la documentación para utilizar correctamente la página de aterrizaje."

Para utilizar correctamente la página de aterrizaje, debe hacer referencia a ella como un vínculo en una entrega con la opción dedicada.

>[!CAUTION]
>
>Para aprovechar al máximo la página de aterrizaje, no puede copiar y pegar el vínculo que se muestra en el panel de envío publicado directamente en las entregas o en una página web.

En el [!DNL Adobe Campaign Web] En primer lugar, cuatro plantillas predeterminadas le permiten implementar diferentes casos de uso. Sin embargo, los pasos principales siguen siendo los mismos y se detallan a continuación.

1. [Creación de una página de aterrizaje](create-lp.md#create-landing-page) y seleccione la plantilla que desee, según el caso de uso.

1. Defina las propiedades y la configuración de la página de aterrizaje.

   ![](assets/lp-uc-properties.png){zoomable=&quot;yes&quot;}

1. Según su caso, seleccione la opción **[!UICONTROL Adquisición]**, **[!UICONTROL Suscripción]**, **[!UICONTROL Baja]** o **[!UICONTROL Lista de bloqueados de]** página.

1. Se muestra el contenido de la página. Seleccione la parte correspondiente al formulario de página de aterrizaje.

   ![](assets/lp-uc-form.png){zoomable=&quot;yes&quot;}

1. Edite el contenido según la plantilla seleccionada:

   * [Adquisición](#lp-acquisition)
   * [Suscripción](#lp-subscription)
   * [Baja](#lp-unsubscription)
   * [Lista de bloqueados](#lp-denylist)

1. Modifique el resto del contenido según sea necesario, guarde los cambios y cierre.

1. Edite el **[!UICONTROL Confirmación]** según sea necesario, así como la **[!UICONTROL Error]** y **[!UICONTROL Caducidad]** páginas. El **[!UICONTROL Confirmación]** se mostrará a los destinatarios una vez que envíen el formulario.

   ![](assets/lp-uc-confirmation-page.png){zoomable=&quot;yes&quot;}

1. [Prueba](create-lp.md#test-landing-page) y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [email](../email/create-email.md) envío para dirigir el tráfico a la página de aterrizaje.

1. [Inserción de un vínculo](../email/message-tracking.md#insert-links) en el contenido del mensaje. Seleccionar **[!UICONTROL Página de aterrizaje]** como el **[!UICONTROL Tipo de vínculo]** y elija la página de aterrizaje que ha creado.

   ![](assets/lp-uc-email-link.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Para poder enviar el mensaje, asegúrese de que la página de aterrizaje seleccionada aún no haya caducado. [Más información](create-lp.md#create-landing-page)

Una vez recibido el correo electrónico, si los destinatarios hacen clic en el vínculo a la página de aterrizaje y envían el formulario:

* Se le redirigirá a la página de confirmación.

* Se aplicará cualquier otra acción definida en la página de aterrizaje. Por ejemplo: los usuarios se suscribirán a su servicio o no recibirán más comunicaciones de usted.

A continuación se muestran algunos ejemplos de cómo puede utilizar [!DNL Adobe Campaign] páginas de aterrizaje en los diferentes casos de uso posibles.

## Adquisición de perfil {#lp-acquisition}

La primera plantilla permite agregar o actualizar un perfil a la base de datos de Campaign.

1. Cuándo [creación de la página de aterrizaje](create-lp.md#create-landing-page), seleccione la **[!UICONTROL Adquisición]** plantilla.

1. En las propiedades de la página de aterrizaje, asegúrese de seleccionar la **[!UICONTROL Rellene previamente los datos a los que se hace referencia en el formulario]** para cargar previamente cualquier información existente del perfil y evitar la creación de duplicados.

1. Seleccione el **[!UICONTROL Adquisición]** para editar su contenido.

1. Edite los campos de texto según sea necesario según la información que desee recopilar en los perfiles.

1. Además, puede añadir una casilla de verificación para invitar a sus clientes a suscribirse al servicio de boletín informativo. [Obtenga información sobre cómo crear un servicio](../audience/manage-services.md)

   ![](assets/lp-uc-acquisition-page.png){zoomable=&quot;yes&quot;}

1. Ajuste el contenido según sea necesario y guarde los cambios.

1. Revisar y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [email](../email/create-email.md) y [añadir un vínculo](../email/message-tracking.md#insert-links) a la página de aterrizaje.

Una vez recibido el correo electrónico, si los destinatarios hacen clic en el vínculo a la página de aterrizaje y envían el formulario, su perfil se añade a la base de datos de Campaign o se actualiza con la información que han proporcionado.

![](assets/lp-uc-profile-updated.png){zoomable=&quot;yes&quot;}

Si optó por recibir su newsletter, se suscribirá al servicio correspondiente.

![](assets/lp-uc-newsletter-subscriber.png){zoomable=&quot;yes&quot;}

## Suscripción a un servicio {#lp-subscription}

Uno de los casos de uso más comunes consiste en invitar a sus clientes a [suscripción a un servicio](../audience/manage-services.md) (como un boletín informativo o un evento) a través de una página de aterrizaje. Siga los pasos a continuación.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Comience creando una plantilla de confirmación para los usuarios que se suscriban a su evento, de modo que pueda seleccionarla fácilmente al crear el servicio. [Más información](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png){zoomable=&quot;yes&quot;}

1. Cree un servicio de suscripción, que almacenará a los usuarios registrados en su evento. [Obtenga información sobre cómo crear un servicio](../audience/manage-services.md)

1. Seleccione la plantilla que creó como correo electrónico de confirmación que los usuarios recibirán tras la suscripción.

   ![](assets/lp-uc-subscription-service.png){zoomable=&quot;yes&quot;}

1. [Creación de una página de aterrizaje](create-lp.md#create-landing-page) para permitir que los destinatarios se registren en el evento. Seleccione el **[!UICONTROL Suscripción]** plantilla.

1. Seleccione el **[!UICONTROL Suscripción]** para editar su contenido.

1. Se muestra el contenido de la página. Seleccione la parte correspondiente al formulario de la página de aterrizaje y expanda **[!UICONTROL Casilla 1]** sección.

1. En el **[!UICONTROL Suscripciones y servicios]** , seleccione el servicio que creó para su evento. Deje el **[!UICONTROL Suscribirse si está marcado]** opción activada.

   ![](assets/lp-uc-subscription-checkbox-1.png){zoomable=&quot;yes&quot;}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. Ajuste el contenido según sea necesario y guarde los cambios.

1. Revisar y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [email](../email/create-email.md) y [añadir un vínculo](../email/message-tracking.md#insert-links) para dirigir el tráfico a la página de aterrizaje de registro.

1. Diseñe el correo electrónico para anunciar que el registro está abierto para su evento.

Una vez recibido el correo electrónico, si los destinatarios hacen clic en el vínculo a la página de aterrizaje y envían el formulario, se les dirige a la página de confirmación y se les añade a la lista de suscripción.

## Baja {#lp-unsubscription}

Puede permitir a sus clientes cancelar la suscripción a un servicio mediante una página de aterrizaje.

1. Asegúrese de haber creado una plantilla de confirmación para los usuarios que cancelan la suscripción al servicio, de modo que pueda seleccionarla fácilmente al crearlo. [Más información](../audience/manage-services.md#create-confirmation-message)

1. En su [servicio de suscripción](../audience/manage-services.md), seleccione la plantilla que creó como correo electrónico de confirmación que los usuarios recibirán al cancelar la suscripción.

1. [Creación de una página de aterrizaje](create-lp.md#create-landing-page). Seleccione el **[!UICONTROL Baja]** plantilla.

1. Seleccione el **[!UICONTROL Baja]** para editar su contenido.

1. Se muestra el contenido de la página. Seleccione la parte correspondiente al formulario de página de aterrizaje.

1. Puede añadir un **[!UICONTROL Casilla]** , seleccione el servicio y seleccione la **[!UICONTROL Cancelar suscripción si está marcado]** opción.

   ![](assets/lp-uc-unsubscription-checkbox-1.png){zoomable=&quot;yes&quot;}

1. También puede expandir la variable **[!UICONTROL Llamada a la acción]** y seleccione la sección **[!UICONTROL Actualizaciones adicionales]** opción. Seleccione el servicio y marque **[!UICONTROL Opción de exclusión]** opción.

   ![](assets/lp-uc-unsubscription-call-to-action.png){zoomable=&quot;yes&quot;}

1. Ajuste el contenido según sea necesario y guarde los cambios.

1. Revisar y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [email](../email/create-email.md) y [añadir un vínculo](../email/message-tracking.md#insert-links) a la página de aterrizaje.

Una vez recibido el correo electrónico, si los destinatarios hacen clic en el vínculo a la página de aterrizaje y envían el formulario, se les dirige a la página de confirmación de baja y se les elimina del servicio de suscripción correspondiente.

## Lista de bloqueados {#lp-denylist}

Proporcionar a los destinatarios la capacidad de cancelar su suscripción a la recepción de comunicaciones de una marca es un requisito legal. Por lo tanto, siempre debe incluir un **vínculo de cancelación de suscripción** en cada correo electrónico enviado a los destinatarios. Al hacer clic en este vínculo, los destinatarios se dirigen a una página de aterrizaje que incluye un botón para confirmar la exclusión.

Puede configurar un **[!UICONTROL Lista de bloqueados de]** página de aterrizaje que permite a los usuarios desactivar todas las entregas.

1. Cuándo [creación de la página de aterrizaje](create-lp.md#create-landing-page), seleccione la **[!UICONTROL Lista de bloqueados de]** plantilla.

1. Seleccione el **[!UICONTROL Lista de bloqueados de]** para editar su contenido.

1. Expanda el **[!UICONTROL Llamada a la acción]** y seleccione la sección **[!UICONTROL Actualizaciones adicionales]** opción.

1. En la lista desplegable correspondiente, seleccione **[!UICONTROL Canal (correo electrónico)]** para permitir que los destinatarios se excluyan únicamente de las comunicaciones por correo electrónico. También puede seleccionar **[!UICONTROL Por todos los canales]** para excluirlos a todos de todas las comunicaciones en todos los canales.

   ![](assets/lp-uc-denylist.png){zoomable=&quot;yes&quot;}

1. Ajuste el contenido según sea necesario y guarde los cambios.

1. Revisar y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [email](../email/create-email.md) y [añadir un vínculo](../email/message-tracking.md#insert-links) a la página de aterrizaje para permitir que los usuarios puedan excluirse de la recepción de comunicaciones.

Una vez recibido el correo electrónico, si los destinatarios hacen clic en el vínculo a la página de aterrizaje y envían el formulario, se les dirigirá a la página de confirmación de la lista de bloqueados de la aplicación y su perfil se actualizará con la información que proporcionaron.

Para comprobar que se ha actualizado la opción del perfil correspondiente, vaya a **[!UICONTROL Perfiles]** y seleccione ese perfil.

Por ejemplo, si elige actualizar el **[!UICONTROL Canal (correo electrónico)]** en la página de aterrizaje, la opción **[!UICONTROL Ya no se puede contactar por correo electrónico]** se marcará la opción.

![](assets/lp-uc-denylist-profile.png){zoomable=&quot;yes&quot;}

Este perfil no recibirá comunicaciones por correo electrónico de su marca a menos que se vuelva a suscribir.











