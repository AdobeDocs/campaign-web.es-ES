---
title: Notas de la versión anterior de la interfaz de usuario web de Campaign v8
description: Versiones de la interfaz de usuario web de Campaign de 2025
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '3052'
ht-degree: 100%

---

# Notas de la versión de 2025 {#2025-release}

Esta página enumera todos los cambios y mejoras disponibles con las **versiones de 2025**. Las notas de la versión más recientes están disponibles en [esta página](release-notes.md).

## Versión de octubre de 2025 {#25-10-updates}

_3 de noviembre de 2025_

<table>
<thead>
<tr>
<th><strong>Funciones multilingües para la mensajería transaccional, notificaciones push y SMS (LA-Disponibilidad limitada)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede enviar varios mensajes transaccionales, notificaciones push y mensajes SMS en diferentes idiomas en la interfaz de usuario web de Adobe Campaign. La función Envío multilingüe le permite elegir el idioma predeterminado de su entrega, así como los diferentes idiomas en los que se puede realizar el envío. También puede obtener una vista previa de estos envíos en los idiomas que haya elegido. </p>
<p>Nota: esta funcionalidad solo está disponible para un conjunto de organizaciones (disponibilidad limitada) y se implementará globalmente en una versión futura.</p>
<p>Para obtener más información, consulte la <a href="../msg/multilingual.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>Enriquecimiento del perfil en mensajes transaccionales (LA-Disponibilidad limitada)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Esta funcionalidad le permite personalizar mensajes transaccionales vinculando campos de base de datos de Adobe Campaign al contenido del mensaje. Puede seleccionar asignaciones de destinatario, columnas de enriquecimiento y una clave de reconciliación para garantizar una personalización precisa y en tiempo real mientras mantiene los umbrales de rendimiento.</p>
<p>Nota: Esta funcionalidad solo está disponible para un conjunto de organizaciones (disponibilidad limitada) y se implementará a nivel global en una versión futura. Esta función solo está disponible actualmente en los correos electrónicos.</p>
<p>Para obtener más información, consulte la <a href="../transactional-messaging/profile-enrichment.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integración con Adobe GenStudio</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Para mejorar la eficacia del marketing y mantener la uniformidad de la marca, ahora puede integrar sin problemas las experiencias de GenStudio for Performance Marketing con Campaign. Esto le permite aprovechar la creación de contenido con tecnología IA de GenStudio junto con las funcionalidades de orquestación avanzadas de Campaign.<p>
<p>Para obtener más información, consulte la <a href="../integrations/genstudio.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Compatibilidad con el modo oscuro en el Diseñador de correo electrónico</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El Diseñador de correo electrónico ahora permite cambiar a la vista de modo oscuro, donde también puede definir ajustes personalizados específicos. Tenga en cuenta que la representación final depende del cliente de correo electrónico del destinatario y no todos los clientes de correo electrónico son compatibles con el modo oscuro.</p>
<p>Para obtener más información, consulte la <a href="../email/dark-mode.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### Mejoras {#25-10-improvements}

* En los envíos creados en la consola del cliente, la sección **Público** ahora indica si se ha definido una condición dinámica para los destinos de prueba. <!-- [Learn more](../msg/gs-deliveries.md#access)-->

* Ahora puede conmutar entre el generador de reglas nuevo y el heredado cuando vaya a configurar una condición mediante la funcionalidad de contenido condicional del Diseñador de correo electrónico. <!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* Ahora puede seleccionar vínculos de colección, como compras, en la definición de pantalla del esquema Destinatarios. Se muestran los datos relacionados en las pantallas de perfil a través de una pestaña específica. <!-- [Learn more](../administration/schemas.md#collection-lists)-->

* Como administrador de Campaign, ahora puede configurar conexiones a Salesforce CRM y Microsoft Dynamics.
  [Más información](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

## Versión de septiembre de 2025 {#25-9-release}

_23 de septiembre de 2025_

Las siguientes funciones están disponibles a partir de la versión de septiembre.

<table>
<thead>
<tr>
<th><strong>Canal personalizado para envíos de API</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora, directamente desde la interfaz de usuario de Adobe Campaign web, puede organizar y ejecutar envíos basados en canales de API personalizados. Estos envíos pueden ser independientes o formar parte de un flujo de trabajo. La configuración del canal de API personalizado se realiza en la consola.</p>
<p>Para obtener más información, consulte la <a href="../call-center/gs-custom-channel.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Creación de cuentas externas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Como administrador de Campaign, ahora puede configurar nuevas conexiones con sistemas externos desde la interfaz de usuario web de Campaign. También puede ver, actualizar y administrar cuentas externas existentes.</p>
<p>Para obtener más información, consulte la <a href="../administration/create-external-account.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Bloqueo de contenido de correo electrónico</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora Campaign le permite bloquear contenido en las plantillas de correo electrónico, ya sea bloqueando toda la plantilla o estructuras y componentes específicos. Esto le permite evitar ediciones o eliminaciones no intencionadas, lo que le proporciona un mayor control sobre la personalización de las plantillas y mejora la eficacia y fiabilidad de sus campañas de correo electrónico.</p>
<p>Para obtener más información, consulte la <a href="../content/content-locking.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### Mejoras {#25-9-improvements}

* Se ha añadido un conjunto de operadores nuevos al configurar una condición mediante la capacidad de contenido condicional del diseñador de correo electrónico.
* La dimensión de filtrado ya está disponible en la actividad de flujo de trabajo **Generar público**. Para verla o cambiarla, haga clic en el icono situado junto a la dimensión de segmentación. [Más información](../workflows/activities/build-audience.md#build-audience-configuration).
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

## Versión de agosto de 2025 {#25-8-release}

Esta versión incluye una serie de correcciones de errores, que incluyen:

* El proceso de duplicación de perfiles se ha mejorado para que coincida con el comportamiento de la consola del cliente, lo que garantiza una experiencia coherente en ambas interfaces. Esto corrige un problema que podría evitar la creación de perfiles duplicados.

* La opción **[!UICONTROL CCO del correo electrónico]**, en la pantalla de configuración de envío, ahora funciona con Momentum (MTA mejorado). Antes, esta funcionalidad solo estaba disponible en la consola del cliente.  

## Versión de julio de 2025 {#25-7-release}

### Nuevas funciones {#25-7-features}

Las siguientes funciones están disponibles a partir de la versión de julio.

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>Compatibilidad con CSS personalizado en el Diseñador de correo electrónico</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Al diseñar los correos electrónicos, ahora puede añadir su propio CSS personalizado directamente en el Diseñador de correo electrónico. Esta capacidad le permite aplicar estilos avanzados y específicos para obtener una mayor flexibilidad y control sobre el aspecto del contenido.</p>
<p>Para obtener más información, consulte la <a href="../email/custom-css.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Marcas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear y personalizar sus propias marcas para definir claramente su identidad visual y verbal en todas las comunicaciones. Con la puntuación de alineación de marca, puede recibir comentarios en tiempo real sobre cómo el contenido refleja el tono, el estilo y las directrices de su marca, lo que le ayuda a mantenerse constantemente al día con la marca con cada mensaje que envía.
</p>
<p>Para obtener más información, consulte la <a href="../content/brands.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Alertas de envío</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La función de alertas de envío es un sistema de administración de alertas que permite a un grupo de usuarios recibir automáticamente notificaciones que contienen información sobre la ejecución de sus envíos.</p>
<p>Para obtener más información, consulte la <a href="../msg/delivery-alerting.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>Sistema de informes dinámicos</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede acceder al sistema de informes dinámicos que proporciona informes totalmente personalizables y en tiempo real para medir el impacto de las actividades de marketing. Este añade acceso a los datos de perfil, lo que permite el análisis demográfico por dimensiones de perfil como sexo, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. El sistema de informes dinámicos también está disponible para envíos de correo electrónico multilingües y mensajes transaccionales.</p>
<p>Esta funcionalidad solo está disponible bajo demanda. Para obtener acceso, póngase en contacto con su representante de Adobe. El servidor debe actualizarse a la versión 8.8.1 como mínimo. Consulte las <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es" target="_blank">notas de la versión</a> de la consola del cliente.
<p>Para obtener más información, consulte la <a href="../reporting/dynamic-reporting/get-started-reporting.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Promoción de la marca centralizada</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora los administradores técnicos pueden definir una o varias marcas para centralizar los parámetros que afectan a la identidad de una marca. Esto incluye el logotipo de la marca, el dominio de la URL de acceso de la página de destino o la configuración del seguimiento de mensajes. Con Adobe Campaign, puede crear estas marcas y vincularlas a mensajes o páginas de destino. Esta configuración se administra en plantillas. Las opciones de promoción de la marca ya están disponibles en todos los canales, incluidos SMS y correo directo.</p>
<p>Esta funcionalidad solo está disponible bajo demanda para nuevas implementaciones. Para obtener acceso, póngase en contacto con su representante de Adobe. El servidor debe actualizarse a la versión 8.8.1 como mínimo. Consulte las <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es" target="_blank">notas de la versión</a> de la consola del cliente.
<p>Para obtener más información, consulte la <a href="../administration/branding/branding-gs.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

Además de las funciones enumeradas anteriormente, esta versión también incluye el siguiente conjunto de funcionalidades, disponibles en la consola del cliente:

* [Nuevo conector de envío de SMS](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=es) (entornos de FDA)
* [API de REST](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=es) (bajo demanda, entornos de FDA)

Consulte las [notas de la versión](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es){target="_blank"} de la consola del cliente.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

-->

### Mejoras {#25-7-improvements}

* Ahora puede calcular la población objetivo directamente en cada condición y grupo del generador de reglas. Haga clic en el número de resultado para ver la lista detallada de registros. [Más información](../query/build-query.md#validate-query)

* Ahora puede editar o eliminar un filtro predefinido directamente desde el generador de reglas. [Más información](../get-started/predefined-filters.md#manage-predefined-filter)

* Al configurar un envío de SMS, en la sección **SMS**, ahora tiene acceso a los **parámetros SMPP opcionales (TLV)**. Este parámetro es el mismo que en la Consola de cliente. [Más información](../advanced-settings/delivery-settings.md#sms-tab)

* Ahora puede habilitar las notificaciones en segundo plano en iOS mediante la nueva opción **Contenido disponible**, disponible en la sección **Ajustes avanzados** de la pantalla de edición de contenido de iOS. Esto añade el indicador `content-available:1` en la carga útil `aps`. Obtenga más información [en esta página](../push/content-push.md). Consulte [esta página](../push/rich-push-ios.md)

* Ya están disponibles las siguientes mejoras en la página de aterrizaje:

   * Ahora puede hacer referencia a una página de destino de suscripción/baja predeterminada al configurar un servicio. Al diseñar un correo electrónico, si define un vínculo a esa página de destino, los usuarios que envíen el formulario de página de destino se suscriben o cancelan su suscripción automáticamente a este servicio. [Más información](../audience/manage-services.md#create-service)
   * Una nueva opción en la configuración de la página de destino permite a los visitantes anónimos acceder a la página de destino. Si anula la selección de esta opción, solo los usuarios identificados pueden acceder al formulario y enviarlo. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción en la configuración de la página de destino permite almacenar datos internos adicionales cuando se envía la página de destino. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción permite utilizar una página de destino para varios servicios, lo que la hace dinámica. Al añadir un vínculo a un correo electrónico, si selecciona una página de destino dinámica, puede seleccionar cualquier servicio. Si selecciona una página de destino que tiene un servicio específico asociado, este servicio se utilizará automáticamente (no puede seleccionar otro). [Más información](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Ahora se admite contenido condicional en las páginas de destino. [Más información](../landing-pages/lp-content.md)
   * Puede vincular una página de aterrizaje a un servicio y enviar un mensaje de confirmación cuando los usuarios la validen. [Más información](../landing-pages/lp-content.md#lp-message)
   * Ahora puede añadir captcha para proteger su página de aterrizaje contra el spam y los abusos causados por bots. Esto no es intrusivo para los clientes, ya que no requiere ninguna interacción por parte de ellos y se basa en las interacciones con el sitio. [Más información](../landing-pages/create-lp.md#captcha)

## Versión de junio de 2025 {#25-6-release}

### Mejoras {#25-6-improvements}

* El informe Resumen del envío ya está disponible, tanto para el centro de llamadas como para los canales personalizados. [Más información](../reporting/direct-mail.md)

* Al configurar un envío por SMS, ahora tiene acceso a los parámetros específicos del SMS. Son los mismos parámetros que están disponibles en la consola del cliente. [Más información](../advanced-settings/delivery-settings.md#sms-tab)

* Sus carpetas favoritas ahora aparecen en la parte superior del panel izquierdo en la página del explorador, lo que facilita su acceso. [Más información](../get-started/work-with-folders.md#favorite-folders)

* El Generador de reglas ahora admite la función de arrastrar y soltar, lo que le permite reorganizar los componentes de la consulta de forma más eficaz. [Más información](../query/build-query.md#drag-and-drop)

* Se ha mejorado la &quot;condición humana&quot; en el Generador de reglas. Esta es la versión escrita en lenguaje simple de sus reglas, que se muestra en la parte inferior de la pantalla:

   * Ahora los atributos se resaltan y se muestra el esquema asociado.
   * Puede hacer clic en estos elementos para ver información más detallada.
   * Ahora puede copiar la condición humana con el botón correspondiente.

* El acceso y la visualización de las carpetas &quot;Flujos de trabajo técnicos&quot; y &quot;Objetos creados automáticamente&quot; está ahora restringido. [Más información](../get-started/work-with-folders.md#about-folders)

## Versión de mayo de 2025 {#25-5-release}

Las siguientes funciones están disponibles para todos los usuarios a partir de la versión de mayo.

<table>
<thead>
<tr>
<th><strong>Puntuación de alineación con la marca (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La función de puntuación de alineación con la marca proporciona comentarios claros directamente en el diseñador de correo electrónico, lo que le ayuda a ver si el contenido se ajusta al tono, el estilo y las directrices de la marca. Esta función está disponible en Beta.</p>
<p>Para obtener más información, consulte la <a href="../content/brands-score.md">documentación detallada</a>.</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Canal personalizado para envíos externos</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora, directamente desde la interfaz de usuario de Adobe Campaign Web, puede organizar y ejecutar envíos basados en canales externos personalizados. Estos envíos pueden ser independientes o formar parte de un flujo de trabajo. La creación del canal externo personalizado integrado con un tercero se realiza en la consola.</p>
<p>Nota: La creación de informes no está disponible en la interfaz de usuario web para el canal personalizado. Debe navegar a la consola del cliente para acceder a los informes.</p>
<p>Para obtener más información, consulte la <a href="../call-center/gs-custom-channel.md">documentación detallada</a>.</p>
<img src="assets/do-not-localize/custom-channel.gif">
</td>
</tr>
</tbody>
</table>

### Mejoras {#25-5-improvements}

La pantalla de creación de reglas de tipología se ha actualizado para facilitar la selección del tipo de regla.

## Versión de abril de 2025 {#25-4-release}

**Fecha de lanzamiento**: 29 de abril de 2025

### Nuevas funciones {#25-4-features}

Las siguientes funciones están disponibles para todos los usuarios a partir de la versión de abril.

<table>
<thead>
<tr>
<th><strong>Canal de centro de llamadas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El canal del centro de llamadas ahora está disponible en la interfaz de usuario de Campaign Web. Este canal se refiere a un método de comunicación utilizado para administrar y rastrear comunicaciones o interacciones que se gestionan a través de un centro de llamadas, generalmente llamadas telefónicas realizadas por agentes a clientes o clientes potenciales.</p>
<p>Nota: La creación de informes no está disponible en la interfaz de usuario web para el canal del centro de llamadas. Debe navegar a la consola del cliente para acceder a los informes.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Para obtener más información, consulte la <a href="../call-center/gs-call-center.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Nuevo generador de reglas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora hay disponible un nuevo generador de reglas para definir condiciones complejas en una interfaz de usuario mejorada. Puede cambiar del generador de reglas antiguo al nuevo según sea necesario.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Para obtener más información, consulte la <a href="../query/query-modeler-overview.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Creación de cuentas externas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Como administrador de Campaign, ahora puede configurar nuevas conexiones con sistemas externos desde la interfaz de usuario de Campaign Web.
También puede ver, actualizar y administrar cuentas externas existentes.</p>
<p>Para obtener más información, consulte la <a href="../administration/external-account.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#25-4-improvements}

**Mejoras generales en la interfaz**

* Las opciones Descripción del campo, Añadir a favoritos y Distribución de valores para los atributos del esquema ahora son más visibles en la interfaz de usuario. Para obtener más información, consulte la [documentación detallada](../get-started/attributes.md).
* En la interfaz, la fecha y la hora ahora se muestran según el idioma principal establecido en las preferencias de Experience League. Esta mejora solo está disponible para varios idiomas. Para ver la lista completa de idiomas admitidos, consulte la [documentación detallada](https://experienceleague.adobe.com/es/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Editor de correo electrónico**: para mejorar la accesibilidad en la interfaz de usuario de Campaign Web, hay dos campos nuevos disponibles en el Diseñador de correo electrónico. Estos se corresponden con el elemento `title` y el atributo lang en el elemento `html` del contenido del correo electrónico. Puede definir esta configuración además del campo preencabezado, en la sección cuerpo del correo electrónico. Para obtener más información, consulte la [documentación detallada](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Esquemas**

* Ahora puede editar el esquema temporal de una lista desde la interfaz de usuario de Campaign Web. Para obtener más información, consulte la [documentación detallada](../audience/manage-audience.md).
* Ahora puede obtener una vista previa de los campos personalizados de un esquema en una pantalla de ejemplo. Para obtener más información, consulte la [documentación detallada](../administration/custom-fields.md#add).
* Ahora puede mover campos personalizados a la lista arrastrando y soltando. Para obtener más información, consulte la [documentación detallada](../administration/custom-fields.md#add).


### Nuevas funciones en disponibilidad limitada {#25-4-features-la}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se pueden implementar en ningún otro entorno. Estos requieren actualizar el servidor de Campaign a la versión 8.7.4.
>
>Consulte las siguientes páginas de documentación: [transición de Campaign Standard a la versión 8 de Campaign](../rn/acs-migration.md) y las [Funciones para usuarios de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es).

* **Creación de envíos multilingües**: ahora puede mandar varios envíos de correo electrónico en diferentes idiomas en la interfaz de usuario de Adobe Campaign Web. La función Envío multilingüe le permite elegir el idioma predeterminado de su entrega, así como los diferentes idiomas en los que se puede realizar el envío. También puede previsualizar estos envíos en los idiomas que haya elegido. Para obtener más información, consulte la [documentación detallada](../email/edit-content.md).

* **Informes dinámicos para envíos multilingües**: ahora los informes dinámicos están disponibles para los envíos de correo electrónico multilingües. Para obtener más información, consulte la [documentación detallada](../reporting/global-reports.md).

* **Compatibilidad con la API REST de SMS (LA)**: la API REST de mensajería transaccional ya está disponible para el canal de SMS. Cuando el correo electrónico como el teléfono móvil están presentes en la carga útil, puede utilizar el campo &quot;wishedChannel&quot; para especificar el canal. Si no se proporciona, el correo electrónico se utilizará de forma predeterminada a menos que wishedChannel solicite explícitamente un SMS. Para obtener más información, consulte la [documentación detallada](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=es){target=_blank}.

## Versión de febrero de 2025 {#25-2-release}

**Fecha de lanzamiento**: 18 de febrero de 2025

Las siguientes funciones y mejoras están disponibles a partir de la versión de febrero.

### Funciones {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Creación de reglas empresariales (reglas de tipología)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear tipologías y reglas de tipología en la interfaz de usuario de Adobe Campaign Web. Las tipologías permiten controlar, filtrar y priorizar la entrega de envíos. Le permiten asegurarse de que los envíos siempre contengan componentes obligatorios (como un vínculo de cancelación de suscripción o una línea de asunto) o reglas de filtrado para excluir grupos de su público (como suscriptores que han cancelado la suscripción, competidores o clientes que no sean fieles).</p>
<img src="assets/do-not-localize/typology.gif">
<p>Para obtener más información, consulte la <a href="../administration/typologies.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Asignaciones de destino</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear asignaciones de público destinatario en la interfaz de usuario de Campaign Web. Las asignaciones de público destinatario definen cómo los distintos canales de envío (correo electrónico, SMS o notificaciones push) se vinculan a los campos de datos de un esquema. La asignación de público destinatario permite definir el público: perfiles, beneficiarios de contratos, operadores, suscriptores, clientes potenciales, etc.</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>Para obtener más información, consulte la <a href="../administration/target-mappings.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Detalles del esquema</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede acceder a los detalles de un esquema seleccionando su nombre en la lista. Ahora se puede acceder a la edición de campos personalizados desde el botón <b>Editar campos personalizados</b> disponible en los detalles del esquema.</p>
<img src="assets/do-not-localize/schemas.gif">
<p>Para obtener más información, consulte la <a href="../administration/schemas.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

## Versión de enero de 2025 {#25-1-release}

**Fecha de lanzamiento**: 5 de febrero de 2025

Las siguientes funciones y mejoras están disponibles a partir de la versión de enero.

### Funciones {#25-1-features}


<table>
<thead>
<tr>
<th><strong>Crear y utilizar fragmentos visuales</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Los fragmentos visuales son bloques visuales predefinidos que se pueden reutilizar en varios envíos de correo electrónico o en plantillas de contenido. Esta función ya está disponible para todos los clientes que ejecuten la versión 8.6.4 o superior del servidor.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>Para obtener más información, consulte la <a href="../content/use-visual-fragments.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Uso de un sistema de terceros para remitir envíos</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede definir envíos externos y plantillas de envío externo en la interfaz de Campaign Web. En este modo, los mensajes se compilan en un archivo de salida que se puede compartir con su proveedor externo. De forma predeterminada, el modo de envío externo es el que se utiliza para el canal de correo directo.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>Para obtener más información, consulte la <a href="../msg/send-external-deliveries.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Administrar las enumeraciones</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear enumeraciones directamente mediante la interfaz de usuario de Adobe Campaign Web. Una enumeración es una lista de valores sugeridos por el sistema para rellenar los campos. Utilice las enumeraciones para estandarizar los valores de estos campos, facilitar la introducción de datos o utilizarlas en las consultas.</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>Para obtener más información, consulte la <a href="../administration/enumerations.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Crear opciones personalizadas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede acceder a las opciones técnicas de la interfaz de usuario de Adobe Campaign Web y crear sus propias opciones personalizadas para adaptarlas a sus necesidades. Esto resulta particularmente útil cuando se trabaja con actividades de flujo de trabajo de código JavaScript para almacenar datos intermedios.</p>
<img src="assets/do-not-localize/options.gif">
<p>Para obtener más información, consulte la <a href="../administration/options.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Definir y llamar códigos JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear códigos JavaScript en la interfaz de usuario de Adobe Campaign Web. Esto le permite crear funciones reutilizables que se pueden utilizar en distintos flujos de trabajo, de forma similar a una biblioteca.</p>
<img src="assets/do-not-localize/javascript.gif">
<p>Para obtener más información, consulte la <a href="../administration/javascript-codes.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Generación de la página de destino con el Asistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El Asistente de IA ya está disponible con los envíos de la página de destino, lo que le permite generar texto, imágenes o diseños de página completos.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>Para obtener más información sobre el Asistente de IA, consulte la <a href="../content/generative-full-content.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>


### Mejoras {#25-1-improvements}

* Personalice la visualización de los campos personalizados en la interfaz:

   * Ahora puede seleccionar campos personalizados adicionales para mostrarlos en la interfaz
   * Ahora puede establecer reglas para mostrar campos personalizados de tipo vínculo, como restringir valores de lista basados en la entrada de otro campo
   * Ahora puede organizar los campos en la interfaz con más flexibilidad: los campos pueden abarcar una sola columna o agruparse en subsecciones para una mejor organización
   * Ahora puede establecer campos específicos como de solo lectura

* Filtros recientes y favoritos: para reutilizar rápidamente atributos que se utilizan con frecuencia, ahora puede añadirlos a favoritos. Esto garantiza que sean fácilmente accesibles para tareas futuras. Además de los favoritos, también puede ver y utilizar los atributos seleccionados más recientemente.

* Cuentas externas: el nuevo tipo de **[!UICONTROL Enrutamiento]** está disponible para su selección al crear una nueva cuenta externa. Le permite configurar una cuenta externa específica para utilizarla en los envíos externos. [Más información](../administration/external-account.md#routing)
