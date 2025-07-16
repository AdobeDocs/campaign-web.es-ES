---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 62294ce1809caee8af770b376aad97bac71c942c
workflow-type: ht
source-wordcount: '688'
ht-degree: 100%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

Los cambios y mejoras disponibles con las versiones anteriores se recogen en las versiones de [2024](release-notes-24.md) y [2025](release-notes-25.md).

## Actualizaciones del 25 de julio {#25-7-updates}

>[!AVAILABILITY]
>
>Para beneficiarse de estas actualizaciones, el servidor debe actualizarse a la versión 8.8.1 como mínimo. Consulte las [notas de la versión](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es){target="_blank"} de la consola del cliente.

Lanzadas anteriormente en disponibilidad limitada, las siguientes funciones ya están disponibles en todos los entornos (disponibilidad general):

* **Creación de envíos multilingües**: ahora puede mandar varios envíos de correo electrónico en diferentes idiomas en la interfaz de usuario de Adobe Campaign Web. La función Envío multilingüe le permite elegir el idioma predeterminado de su entrega, así como los diferentes idiomas en los que se puede realizar el envío. También puede previsualizar estos envíos en los idiomas que haya elegido. [Más información](../email/edit-content.md#multilingual-delivery).

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=es){target="_blank"}
-->

* **Alertas de envío**: la función de alertas de envío es un sistema de administración de alertas que permite a un grupo de usuarios recibir automáticamente notificaciones que contienen información sobre la ejecución de sus envíos. [Más información](../msg/delivery-alerting.md)

* **Mejoras en las páginas de aterrizaje**: ya están disponibles las siguientes mejoras en las páginas de aterrizaje.

   * Ahora puede hacer referencia a una página de destino de suscripción/baja predeterminada al configurar un servicio. Al diseñar un correo electrónico, si define un vínculo a esa página de destino, los usuarios que envíen el formulario de página de destino se suscriben o cancelan su suscripción automáticamente a este servicio. [Más información](../audience/manage-services.md#create-service)
   * Una nueva opción en la configuración de la página de destino permite a los visitantes anónimos acceder a la página de destino. Si anula la selección de esta opción, solo los usuarios identificados pueden acceder al formulario y enviarlo. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción en la configuración de la página de destino permite almacenar datos internos adicionales cuando se envía la página de destino. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción permite utilizar una página de destino para varios servicios, lo que la hace dinámica. Al añadir un vínculo a un correo electrónico, si selecciona una página de destino dinámica, puede seleccionar cualquier servicio. Si selecciona una página de destino que tiene un servicio específico asociado, este servicio se utilizará automáticamente (no puede seleccionar otro). [Más información](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Ahora se admite contenido condicional en las páginas de destino. [Más información](../landing-pages/lp-content.md)
   * Puede vincular una página de aterrizaje a un servicio y enviar un mensaje de confirmación cuando los usuarios la validen. [Más información](../landing-pages/lp-content.md#lp-message)
   * Ahora puede añadir captcha para proteger su página de aterrizaje contra el spam y los abusos causados por bots. Esto no es intrusivo para los clientes, ya que no requiere ninguna interacción por parte de ellos y se basa en las interacciones con el sitio. [Más información](../landing-pages/create-lp.md#captcha)

Las siguientes funcionalidades, anteriormente publicadas en disponibilidad limitada, ya están disponibles **bajo demanda**:

* **Sistema de informes dinámicos**: ahora puede acceder al sistema de informes dinámicos que proporciona informes totalmente personalizables y en tiempo real para medir el impacto de las actividades de marketing. Este añade acceso a los datos de perfil, lo que permite el análisis demográfico por dimensiones de perfil como sexo, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. El sistema de informes dinámicos también está disponible para envíos de correo electrónico multilingües y mensajes transaccionales. [Más información](../reporting/dynamic-reporting/get-started-reporting.md)

* **Promoción de la marca personalizada**: ahora los administradores técnicos pueden definir una o varias marcas para centralizar los parámetros que afectan a la identidad de una marca. Esto incluye el logotipo de la marca, el dominio de la URL de acceso de la página de destino o la configuración del seguimiento de mensajes. Con Adobe Campaign, puede crear estas marcas y vincularlas a mensajes o páginas de destino. Esta configuración se administra en plantillas. Las opciones de promoción de la marca ya están disponibles en todos los canales, incluidos SMS y correo directo. [Más información](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >Esta funcionalidad solo está disponible para nuevas implementaciones.

Además de las funciones enumeradas anteriormente, esta versión también incluye un conjunto de funcionalidades disponibles en la consola del cliente:

* [Nuevo conector de envío de SMS](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=es).
* [API de REST](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=es)

Consulte las [notas de la versión](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es){target="_blank"} de la consola del cliente.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=es){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/es/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->