---
solution: Campaign, Campaign v8 Web User Interface
title: Casos de uso del Página de aterrizaje
description: Discover los casos de uso más comunes con páginas de aterrizaje en Campaign interfaz web de usuario
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: aterrizaje, página de aterrizaje, caso de uso
exl-id: e51cf54c-9db1-4704-bc5b-0df098d67c7d
source-git-commit: a9ce4fd103c4af8f47ba887031e8d6d53e8d5f0b
workflow-type: tm+mt
source-wordcount: '1419'
ht-degree: 9%

---

# Cómo utilizar una página de aterrizaje {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Copie la URL con cuidado"
>abstract="Para probar o aprovechar al máximo la página de aterrizaje, no puede copiar y pegar este vínculo directamente en un explorador web o en los envíos. En su lugar, utilice la función **Simular contenido** para probarla y siga los pasos que se describen en la documentación para utilizar correctamente la página de aterrizaje."

>[!CONTEXTUALHELP]
>id="acw_landingpages_templates"
>title="Copie la URL con cuidado"
>abstract="Al crear una página de aterrizaje, cuatro plantillas predeterminadas le permiten implementar diferentes casos de uso: añadir o actualizar un perfil en la base de datos de Campaign, suscribir a los clientes a un servicio, cancelar su suscripción a un servicio o excluir usuarios."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/landing-pages/create-lp.html?lang=es#create-landing-page" text="Creación de una página de aterrizaje"

Para hacer un uso adecuado de su página de aterrizaje, haga referencia a ella como un vincular en un mensaje utilizando la opción dedicada. No puede copiar y pegar los vincular que se muestran en el panel de envío publicados directamente en los envíos o en un Página web. En su lugar, utilice la capacidad Simular **contenido** para prueba ella.

En la [!DNL Adobe Campaign Web] interfaz, cuatro plantillas listas para usar le permiten implementar diferentes casos de uso. Sin embargo, los pasos principales siguen siendo los mismos y se detallan a continuación.

1. [Crear un página de aterrizaje](create-lp.md#create-landing-page) y seleccione el plantilla que desee, según su caso de uso.

1. Defina la página de aterrizaje propiedades y la configuración.

   ![Captura de pantalla que muestra la interfaz de configuración y propiedades de página de aterrizaje.](assets/lp-uc-properties.png){zoomable="yes"}

1. Según su caso, seleccione la **[!UICONTROL lista]** de adquisición **,**&#x200B;[!UICONTROL &#x200B; suscripción &#x200B;]&#x200B;**,**&#x200B;[!UICONTROL &#x200B; baja &#x200B;]&#x200B;**o** denegación Página.

1. Se muestra el contenido del Página. Seleccione la parte correspondiente al formulario página de aterrizaje.

   ![Captura de pantalla que muestra la interfaz de formulario página de aterrizaje.](assets/lp-uc-form.png){zoomable="yes"}

1. Editar los contenido según el plantilla seleccionado:

   * [Adquisición](#lp-acquisition)
   * [Suscripción](#lp-subscription)
   * [Baja](#lp-unsubscription)
   * [Lista de bloqueados](#lp-denylist)

1. Modifique el resto de la contenido según sea necesario, guarde los cambios y cierre.

1. Editar el Página de **[!UICONTROL confirmación]** según sea necesario, así como las **[!UICONTROL páginas Error]** y **[!UICONTROL Caducidad]** . El **[!UICONTROL Página de confirmación]** se mostrará a los destinatarios una vez que envíen el formulario.

   ![Captura de pantalla que muestra la interfaz del Página de confirmación.](assets/lp-uc-confirmation-page.png){zoomable="yes"}

1. [Pruebe](create-lp.md#test-landing-page) y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [envío correo electrónico](../email/create-email.md) para dirigir tráfico al página de aterrizaje.

1. [Inserte un vincular](../email/message-tracking.md#insert-links) en el contenido de mensajes. Seleccione **[!UICONTROL Página]** de destino como Tipo **de** vínculo y elija el página de aterrizaje que ha creado.

   ![Captura de pantalla que muestra la correo electrónico vincular la interfaz de inserción.](assets/lp-uc-email-link.png){zoomable="yes"}

   >[!NOTE]
   >
   >Para poder enviar el mensaje, asegúrese de que el página de aterrizaje que seleccione aún no haya caducado. [Más información](create-lp.md#create-landing-page)

Una vez que reciban el correo electrónico, si los destinatarios hacen clic en la vincular de la página de aterrizaje y envían el formulario:

* Se les dirigirá al Página de confirmación.
* Se aplicará cualquier otra acción definida en su página de aterrizaje. Por ejemplo, los usuarios se suscribirán a su servicio o no recibirán más comunicaciones de usted.

A continuación encontrará algunos ejemplos de cómo puede utilizar [!DNL Adobe Campaign] las páginas de aterrizaje en los distintos casos de uso posibles.

## Adquisición perfil {#lp-acquisition}

El primer plantilla permite agregar o actualizar un perfil a la base de datos Campaign.

1. Al [crear el página de aterrizaje](create-lp.md#create-landing-page), seleccione el **[!UICONTROL plantilla adquisición]** .

1. En las propiedades página de aterrizaje, seleccione la **[!UICONTROL opción Rellenar previamente con los datos a los que se hace referencia en el formulario]** para precargar cualquier información existente del perfil y evitar la creación de duplicados.

1. Seleccione el **[!UICONTROL Página de adquisición]** para editar su contenido.

1. Editar los campos de texto según sea necesario, de acuerdo con la información que desea recopilar en sus perfiles.

1. añadir una casilla de verificación para invitar a los clientes a suscribirse al servicio de boletín informativo. [Aprenda a crear un servicio](../audience/manage-services.md)

   ![Captura de pantalla que muestra la interfaz del Página Adquisición con una casilla de verificación de suscripción a newsletter.](assets/lp-uc-acquisition-page.png){zoomable="yes"}

1. Ajuste los contenido según sea necesario y guarde los cambios.

1. Revise y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [correo electrónico](../email/create-email.md) y [añada un vincular](../email/message-tracking.md#insert-links) a la página de aterrizaje.

Una vez que reciban el correo electrónico, si sus destinatarios hacen clic en el vincular de la página de aterrizaje y envían el formulario, sus perfil se agregarán a la base de datos de Campaign o se actualizarán con la información que proporcionaron.

![Captura de pantalla que muestra un perfil actualizado en la base de datos Campaign.](assets/lp-uc-profile-updated.png){zoomable="yes"}

Si optaron por recibir su boletín informativo, se suscribirán al servicio correspondiente.

![Captura de pantalla que muestra la confirmación de suscripción a la newsletter.](assets/lp-uc-newsletter-subscriber.png){zoomable="yes"}

## Suscripción a un servicio {#lp-subscription}

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Establecimiento de la página de aterrizaje de la suscripción"
>abstract="Una página de suscripción permite a los clientes suscribirse a un servicio."

Uno de los casos de uso más comunes consiste en invitar a sus clientes a [suscribirse a un servicio](../audience/manage-services.md) (como un boletín informativo o un evento) a través de un página de aterrizaje. Siga los pasos a continuación.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Crear un plantilla de confirmación para los usuarios que se suscriban a su evento, de modo que pueda seleccionarlo fácilmente al crear el servicio. [Más información](../audience/manage-services.md#create-confirmation-message)

   ![Captura de pantalla que muestra el correo electrónico de confirmación plantilla interfaz.](assets/lp-uc-confirmation-email.png){zoomable="yes"}

1. Crear un servicio de suscripción, que tienda los usuarios registrados para su evento. [Aprenda a crear un servicio](../audience/manage-services.md)

1. Seleccione el plantilla que creó como confirmación correo electrónico recibirán los usuarios al suscribirse.

   ![Captura de pantalla que muestra la interfaz servicio de suscripción.](assets/lp-uc-subscription-service.png){zoomable="yes"}

1. [Crear un página de aterrizaje](create-lp.md#create-landing-page) para permitir que los destinatarios se registren en el evento. Seleccione el plantilla de **[!UICONTROL suscripción]** .

1. Seleccione el Página de suscripción **para editar su** contenido.

1. Se muestra el contenido del Página. Seleccione la parte correspondiente al formulario de página de aterrizaje y amplíe la **[!UICONTROL sección Casilla de verificación 1]** .

1. En el **[!UICONTROL campo Suscripciones y servicios]** , seleccione el servicio que ha creado para su evento. Deje activada la **[!UICONTROL opción Suscribirse si está activada]** .

   ![Captura de pantalla que muestra la interfaz de la casilla de verificación de suscripción.](assets/lp-uc-subscription-checkbox-1.png){zoomable="yes"}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. Ajuste los contenido según sea necesario y guarde los cambios.

1. Revise y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [correo electrónico](../email/create-email.md) y [agregue un vincular](../email/message-tracking.md#insert-links) a dirigir tráfico al registro página de aterrizaje.

1. Diseñe el correo electrónico para anunciar que el registro ya está abierto para su evento.

Una vez que reciban el correo electrónico, si sus destinatarios hacen clic en el vincular de la página de aterrizaje y envían el formulario, se les dirigirá al Página de confirmación y se agregarán al lista de suscripción.

## Baja {#lp-unsubscription}

Puede permitir a sus clientes cancelar la suscripción desde un servicio mediante un página de aterrizaje.

1. Crear un plantilla de confirmación para los usuarios que cancelan la suscripción a su servicio, de modo que pueda seleccionarlo fácilmente al crear el servicio. [Más información](../audience/manage-services.md#create-confirmation-message)

1. En su [servicio de suscripción](../audience/manage-services.md), seleccione el plantilla que creó como confirmación correo electrónico recibirán los usuarios al cancelar la suscripción.

1. [Crear un página de aterrizaje](create-lp.md#create-landing-page). Seleccione el plantilla Cancelación de **[!UICONTROL suscripción]** .

1. Seleccione el Página Cancelar suscripción **&#x200B;**&#x200B;para editar su contenido.

1. Se muestra el contenido del Página. Seleccione la parte correspondiente al formulario página de aterrizaje.

1. añadir una **[!UICONTROL sección de casilla de verificación]** , seleccione el servicio y seleccione la **[!UICONTROL opción Cancelar suscripción si está marcada]** .

   ![Captura de pantalla que muestra la interfaz de casilla de verificación baja.](assets/lp-uc-unsubscription-checkbox-1.png){zoomable="yes"}

1. Expanda la **[!UICONTROL sección Llamada a acción]** y seleccione la **[!UICONTROL opción Actualizaciones]** adicionales. Seleccione el servicio y marque la **[!UICONTROL opción Opt out]** .

   ![Captura de pantalla que muestra la interfaz de llamada a acción para baja.](assets/lp-uc-unsubscription-call-to-action.png){zoomable="yes"}

1. Ajuste los contenido según sea necesario y guarde los cambios.

1. Revise y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [correo electrónico](../email/create-email.md) y [agregar un vincular](../email/message-tracking.md#insert-links) al página de aterrizaje.

Una vez recibido el correo electrónico, si tus destinatarios hacen clic en el vincular al página de aterrizaje y envían el formulario, serán dirigidos al baja Página de confirmación y eliminados del servicio de suscripción correspondiente.

## Lista de bloqueados {#lp-denylist}

Proporcionar a los destinatarios la capacidad de cancelar la suscripción de recibir comunicaciones de una marca es un requisito legal. Por lo tanto, siempre debe incluir un **vincular cancelar la suscripción** en cada correo electrónico enviado a los destinatarios. Al hacer clic en este vincular, los destinatarios serán dirigidos a una página de aterrizaje que incluye un botón para confirmar la exclusión.

Puede configurar una **[!UICONTROL lista]** de denegación página de aterrizaje que permita a los usuarios exclusión de todas las entregas.

1. Al [crear su página de aterrizaje](create-lp.md#create-landing-page), seleccione el plantilla Lista **[!UICONTROL de]** denegación.

1. Seleccione el **[!UICONTROL Página de la lista]** de denegación para editar su contenido.

1. Expanda la **[!UICONTROL sección Llamada a acción]** y seleccione la **[!UICONTROL opción Actualizaciones]** adicionales.

1. En el lista desplegable correspondiente, seleccione **[!UICONTROL Canal (correo electrónico)]** para permitir que los destinatarios exclusión solo desde correo electrónico comunicaciones. También puede seleccionar **[!UICONTROL Por todos los canal]** para excluirlos de todas las comunicaciones en todos los canales.

   ![Captura de pantalla que muestra la interfaz de llamada a la acción denylist.](assets/lp-uc-denylist.png){zoomable="yes"}

1. Ajuste los contenido según sea necesario y guarde los cambios.

1. Revise y [publicar](create-lp.md#publish-landing-page) su página de aterrizaje.

1. Crear un [correo electrónico](../email/create-email.md) y [agregue un vincular](../email/message-tracking.md#insert-links) a su página de aterrizaje para permitir a los usuarios exclusión recibir comunicaciones.

Una vez que reciban el correo electrónico, si sus destinatarios hacen clic en el vincular de la página de aterrizaje y envían el formulario, serán dirigidos al Página de confirmación de la lista de denegación y sus perfil se actualizarán con la información que proporcionaron.

Para comprobar que se ha actualizado la opción del perfil correspondiente, vaya al **[!UICONTROL menú Perfiles]** y seleccione ese perfil.

Por ejemplo, si elige actualizar la **[!UICONTROL opción Canal (correo electrónico)]** en su página de aterrizaje, se marcará la **[!UICONTROL opción Ya no contactar por correo electrónico]** .

![Captura de pantalla que muestra un perfil actualizado con preferencias de lista de negación.](assets/lp-uc-denylist-profile.png){zoomable="yes"}

Este perfil no recibirá correo electrónico comunicaciones de su marca a menos que se suscriba de nuevo.