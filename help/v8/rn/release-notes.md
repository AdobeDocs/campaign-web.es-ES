---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e9022e53ff8733ecdfcca1aec2ba31ca6c79c3ad
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 52%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

## Notas de la versión de agosto {#24-8-release}

**Fecha de la versión**: 3 de septiembre de 2024

Las siguientes funciones y mejoras están disponibles a partir de la versión de agosto.

* **Distribución de valores**: al acceder a la lista de campos para personalización, ahora puede comprobar cómo se distribuyen los valores para cada campo. Una ventana emergente dedicada muestra el número y el porcentaje de cada valor. [Más información](../query/build-query.md#distribution-values-query)

* **Parámetros SMTP**: la configuración SMTP ahora está disponible en la configuración de envío de correo electrónico. [Más información](../advanced-settings/delivery-settings.md#smtp)

* **Variables globales**: ahora puede definir variables globales para definir valores para los envíos. [Más información](../advanced-settings/delivery-settings.md#variables-delivery)

### Nuevas funciones en disponibilidad limitada {#acs-24-8}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se pueden implementar en ningún otro entorno.
>
>Consulte las siguientes páginas de documentación: [Campaign Standard transition to Campaign v8](../rn/acs-migration.md) y [Características para usuarios Campaign Standards](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es){target="_blank"}.

* **Marca para correo postal**: los administradores técnicos ahora pueden definir una o varias marcas para centralizar los parámetros que afectan la identidad de una marca. Esto incluye el logotipo de la marca, el dominio de la URL de acceso de la página de aterrizaje o la configuración del seguimiento de mensajes. Ahora puede crear estas marcas y vincularlas a mensajes o páginas de aterrizaje. Esta configuración se administra en plantillas. [Más información](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **Suscripciones con páginas de aterrizaje**: ahora puede vincular una página de aterrizaje a un servicio y enviar un mensaje de confirmación cuando los usuarios lo validen. [Más información](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragmentos visuales**: ahora puede archivar fragmentos de contenido visual. [Más información](../content/create-fragment.md#archive)

* **Captcha en páginas de aterrizaje**: ahora puede agregar un captcha para proteger su página de aterrizaje del spam y los abusos causados por los bots. Esto no es intrusivo para los clientes, ya que no requiere ninguna interacción por parte de ellos y se basa en las interacciones con el sitio. [Más información](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
