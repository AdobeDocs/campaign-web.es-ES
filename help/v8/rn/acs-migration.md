---
audience: end-user
title: Transición de Campaign Standard a la web de Adobe Campaign
description: Interfaz de usuario web de Discover Campaign
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: fede3e616d45c78db9d0613409254f3c8cc93bba
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 80%

---

# Transición de Campaign Standard a Campaign v8 {#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

¡Bienvenido a Adobe Campaign Managed Cloud Services v8!

Nos complace anunciar que los usuarios de Adobe Campaign Standard ahora pueden realizar la transición a Adobe Campaign Managed Cloud Services v8. Esta transición ofrece muchos beneficios:

* Infraestructura de TI sólida: con los Cloud Services administrados v8, los clientes pueden aprovechar una infraestructura de TI más sólida para garantizar un rendimiento, una fiabilidad y una escalabilidad mejorados para sus campañas.
* Soporte mejorado: nuestro equipo de Cloud Services administrados está comprometido a proporcionar asistencia de primera categoría para garantizar una transición sin problemas y una monitorización continua de su plataforma. Desde la solución de problemas hasta el mantenimiento proactivo, le ofrecemos todo lo que necesita.
* Integración con Adobe Experience Platform: la versión 8 de los Cloud Services administrados se conecta perfectamente con Adobe Experience Platform, lo que permite a los clientes aprovechar todo el potencial de sus datos y ofrecer campañas personalizadas e impactantes en todos los canales.
* Interfaz de usuario y experiencia coherentes: puede estar seguro de que la transición a la versión 8 de Cloud Services administrados no interrumpirá el flujo de trabajo. Seguirá disfrutando de la interfaz de usuario y la experiencia del usuario, lo que garantiza una curva de aprendizaje mínima para su equipo.

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Funcionalidades clave {#key-features}

Vamos a profundizar en las funcionalidades clave que le ofrecerá Campaign v8:

* Experiencia moderna, descriptiva y unificada. [Más información](../get-started/connect-to-campaign.md).
* Nuevas y potentes funcionalidades y procesos sin problemas. [Más información](../get-started/user-interface.md)
* Nuevo modelador de consultas simplificado e intuitivo. [Más información](../query/query-modeler-overview.md)
* Funcionalidades integradas de administración de campañas en canales múltiples. [Más información](../msg/gs-messages.md)
* Actividades de flujo de trabajo de campaña nuevas y rediseñadas. [Más información](../workflows/gs-workflows.md)
* Público destinatario con el modelador de consultas. [Más información](../query/query-modeler-overview.md)
* Creación y administración sencillas de perfiles. [Más información](../audience/about-recipients.md)
* Filtros predefinidos. [Más información](../get-started/predefined-filters.md)
* Conversor de HTML para el diseño de correo electrónico. [Más información](../email/existing-content.md)
* SMS con ofertas. [Más información](../msg/offers.md)

## Interfaz de la consola y la web {#console}

Como usuario de Campaign v8, tiene acceso a la nueva interfaz web de Campaign y a la consola v8. Los datos y la configuración se sincronizan de un entorno a otro. Todos los datos y la configuración disponibles en la consola del cliente se pueden ver en la interfaz de usuario web de Campaign desde la navegación izquierda de Explorer. [Más información](../get-started/user-interface.md#user-interface-explorer)

Obtenga más información sobre las funcionalidades admitidas y no admitidas, y la interoperabilidad entre la interfaz de usuario web de Campaign y la consola del cliente de Campaign [en esta página](../get-started/capability-matrix.md).

## Terminología {#terminology}

La mayoría de los conceptos son similares entre la versión 8 de Campaign y Campaign Standard. Sin embargo, hay algunas diferencias. Estos son algunos ejemplos de diferencias terminológicas entre Campaign Standard y la versión 8 de Campaign:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* Los recursos personalizados son **Esquemas**
* Los mensajes se denominan **Envíos**
* Los usuarios de productos son **Operadores**
* Las funciones se configuran con **Derechos asignados**
* Los grupos de seguridad son **Grupos de operadores**
* Las unidades organizativas se administran mediante **Permisos de carpeta**

## Nuevas características {#new-features}

Para que pueda realizar la transición sin problemas a Campaign v8, se han añadido funciones clave de Campaign Standard a Campaign v8. Se detallan en [esta documentación](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es){target="_blank"}.

* **Creación de informes dinámicos**: la creación de informes dinámicos proporciona informes totalmente personalizables y en tiempo real para medir el impacto de las actividades de marketing. Añade acceso a los datos de perfil, lo que permite el análisis demográfico por dimensiones de perfil como sexo, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=es){target="_blank"}.

* **Personalización de marca centralizada**: cada compañía tiene directrices técnicas y visuales de marca. Con Adobe Campaign, puede definir un conjunto de especificaciones para presentar una marca coherente a sus clientes, desde logotipos hasta aspectos técnicos, como el remitente de correos electrónicos, la dirección URL o los dominios. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=es)

* **API de REST**: como usuario migrado de Campaign Standard, puede utilizar las API de REST para crear integraciones para Adobe Campaign y construir su propio ecosistema al interconectar Adobe Campaign con el panel de tecnologías que utiliza. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=es){target="_blank"}.

* **Páginas de aterrizaje** : Se han introducido algunas mejoras en las páginas de aterrizaje de Campaign v8 para garantizar la paridad de las funciones con Campaign Standard. Obtenga más información en las [notas de la versión](../rn/release-notes.md#new-24-4) y la página de aterrizaje [documentación](../landing-pages/get-started-lp.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->
