---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: ht
source-wordcount: '900'
ht-degree: 100%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

Los cambios y mejoras disponibles con las versiones anteriores se listan en las páginas de [2024](release-notes-24.md) y [2025](release-notes-25.md).

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
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es" target="_blank">release notes</a>.
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
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=es){target="_blank"}

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

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=es) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=es) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es){target="_blank"}.

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
