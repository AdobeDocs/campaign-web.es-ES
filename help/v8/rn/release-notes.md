---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: aea828da825a416dece6c4bee1da6d4e570e4e48
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 82%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

## Actualizaciones de septiembre {#9-2024}

<table>
<thead>
<tr>
<th><strong>Acelerador de contenido del asistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Una vez que haya creado y adaptado su mensaje, llévelo al siguiente nivel con el asistente de IA de Adobe Campaign Web para la aceleración de contenido. Esta potente herramienta le permite optimizar el impacto de su contenido mediante la generación de una amplia gama de atractivos textos, títulos principales e imágenes visualmente atractivas.</p>
<p>Sumérjase en una experiencia práctica con <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator">nuestra vista previa de características en vivo</a>, diseñada para que explore sus características de primera mano y comprenda plenamente sus capacidades.</a>.</p>
<p>Para obtener más información, consulte la <a href="../email/generative-gs.md">documentación detallada</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Fecha de disponibilidad: 12 de septiembre</p>
</td>
</tr>
</tbody>
</table>

## Notas de la versión de agosto {#24-8-release}

**Fecha de lanzamiento**: 3 de septiembre de 2024

Las siguientes funciones y mejoras están disponibles a partir de la versión de agosto.

* **Distribución de valores**: al acceder a la lista de campos para personalización, ahora puede comprobar cómo se distribuyen los valores para cada campo. Una ventana emergente dedicada muestra el número y el porcentaje de cada valor. [Más información](../query/build-query.md#distribution-values-query)

* **Parámetros SMTP**: la configuración de SMTP está ahora disponible en la configuración de envío de correo electrónico. [Más información](../advanced-settings/delivery-settings.md#smtp)

* **Variables globales**: ahora puede definir variables globales para los valores de los envíos. [Más información](../advanced-settings/delivery-settings.md#variables-delivery)

### Nuevas funciones en disponibilidad limitada {#acs-24-8}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se pueden implementar en ningún otro entorno.
>
>Consulte las siguientes páginas de documentación: [Transición de Campaign Standard a Campaign v8](../rn/acs-migration.md) y [Funciones para usuarios de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es){target="_blank"}.

* **Promoción de la marca para correo directo**: ahora los administradores técnicos pueden definir una o varias marcas para centralizar los parámetros que afectan a la identidad de una marca. Esto incluye el logotipo de la marca, el dominio de la URL de acceso de la página de aterrizaje o la configuración del seguimiento de mensajes. Ahora puede crear estas marcas y vincularlas a mensajes o páginas de aterrizaje. Esta configuración se administra en plantillas. [Más información](https://experienceleague.adobe.com/es/docs/experience-cloud/campaign/branding/branding-assign)

* **Suscripciones con páginas de aterrizaje**: ahora puede vincular una página de aterrizaje a un servicio y enviar un mensaje de confirmación cuando los usuarios la validen. [Más información](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragmentos visuales**: ahora puede archivar fragmentos de contenido visual. [Más información](../content/create-fragment.md#archive)

* **Captcha en páginas de aterrizaje**: ahora puede añadir captcha para proteger su página de aterrizaje contra spam y abusos causados por bots. Esto no es intrusivo para los clientes, ya que no requiere ninguna interacción por parte de ellos y se basa en las interacciones con el sitio. [Más información](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
