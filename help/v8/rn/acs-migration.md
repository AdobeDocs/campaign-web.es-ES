---
audience: end-user
title: Transición de Campaign Standard a la web de Adobe Campaign
description: Interfaz de usuario web de Discover Campaign
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 4f32adbbe360b76d227c431281ef10a47e6a37ba
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 99%

---

# Transición de Campaign Standard a Campaign v8 {#acs-to-ac}

Los usuarios de Adobe Campaign Standard ahora pueden realizar la transición a la versión 8 de Adobe Campaign Managed Cloud Services. Esta transición ofrece varias ventajas:

* **Infraestructura de TI sólida**: la versión 8 de Managed Cloud Services provee una infraestructura de TI más sólida para garantizar un rendimiento, una fiabilidad y una escalabilidad mejorados para las campañas.
* **Soporte mejorado**: el equipo de Managed Cloud Services ofrece asistencia de primer nivel para garantizar una transición fluida y un monitoreo continuo de la plataforma. El soporte incluye solución de problemas y mantenimiento proactivo.
* **Integración con Adobe Experience Platform**: la versión 8 de Managed Cloud Services se conecta perfectamente con Adobe Experience Platform, lo que permite a los clientes aprovechar todo el potencial de sus datos y ofrecer campañas personalizadas e impactantes en todos los canales.
* **Experiencia e interfaz de usuario coherentes**: la transición a la versión 8 de Managed Cloud Services no interrumpe los flujos de trabajo. Los usuarios continúan disfrutando de la interfaz y el experiencia familiares, minimizando la curva de aprendizaje para los equipos.

**Como usuario Campaign Standard en proceso de transición a la versión 8 de Campaign, obtenga más información sobre cómo empezar [en este documento](../../adoption/home.md).**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Funcionalidades clave {#key-features}

Los usuarios de la versión 8 de Campaign tienen acceso a la nueva interfaz web de Campaign y a la consola versión 8. Los datos y la configuración se sincronizan entre entornos. Todos los datos y la configuración disponibles en la consola del cliente se pueden ver en la interfaz de usuario web de Campaign, accesibles desde la navegación izquierda de Explorer. [Más información](../get-started/user-interface.md#user-interface-explorer)

La interfaz de usuario web de Campaign está diseñada para que los expertos en marketing creen y organicen fácilmente las campañas. Las funcionalidades clave de la interfaz de usuario de la web de la versión 8 de Campaign incluyen las siguientes:

* **Experiencia moderna, sencilla y unificada** [Más información](../get-started/connect-to-campaign.md).
* **Nuevas y potentes funcionalidades y procesos fluidos** [Más información](../get-started/user-interface.md).
* **Modelador de consultas simplificado e intuitivo**. [Más información](../query/query-modeler-overview.md).
* **Funcionalidades integradas de administración de campañas en canales múltiples** [Más información](../msg/gs-messages.md).
* **Actividades de flujo de trabajo de campaña rediseñadas**. [Más información](../workflows/gs-workflows.md).
* **Creación y administración sencillas de perfiles**. [Más información](../audience/about-recipients.md).
* **Filtros predefinidos**. [Más información](../get-started/predefined-filters.md).
* **Conversor de HTML para el diseño de correo electrónico**. [Más información](../email/existing-content.md).
* **SMS con ofertas**. [Más información](../msg/offers.md).

La consola del cliente de Campaign está diseñada para que los administradores y desarrolladores configuren y personalicen su entorno. Las funcionalidades clave disponibles en la consola del cliente de Campaign se detallan en [esta documentación](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Obtenga más información sobre las funcionalidades admitidas y no admitidas, así como la interoperabilidad entre la interfaz de usuario web de Campaign y la consola del cliente de Campaign [en esta página](../get-started/capability-matrix.md).

## Terminología {#terminology}

La mayoría de los conceptos son similares entre Campaign v8 y Campaign Standard. Sin embargo, hay algunas diferencias terminológicas. Algunos ejemplos son los siguientes:

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## Funciones específicas {#new-features}

Para garantizar una transición sin problemas a la versión 8 de Campaign, se han añadido funciones clave de Campaign Standard a la versión 8 de Campaign. Estas funciones se detallan en [esta documentación](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es){target=_blank} y solo están disponibles para los usuarios que realicen la transición desde Campaign Standard.

* **Creación de informes dinámicos**: la creación de informes dinámicos proporciona informes personalizables y en tiempo real para medir el impacto de las actividades de marketing. Incluye el acceso a los datos del perfil, lo que permite el análisis demográfico por dimensiones de perfil como género, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. [Más información](../reporting/dynamic-reporting/get-started-reporting.md).

* **Personalización de marca centralizada**: Adobe Campaign permite que las empresas definan directrices técnicas y visuales de marca. Los usuarios pueden presentar una marca coherente a los clientes, desde logotipos hasta aspectos técnicos como el remitente de correos electrónicos, la URL o los dominios. [Más información](../administration/branding/branding-gs.md).

* **API de REST**: los usuarios migrados de Campaign Standard pueden usar las API de REST para crear integraciones para Adobe Campaign y construir ecosistemas al interconectar Adobe Campaign con otras tecnologías. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html){target="_blank"}.

* **Páginas de destino**: las páginas de destino de la versión 8 de Campaign incluyen mejoras para garantizar la paridad de las funciones con Campaign Standard. Obtenga más información en las [notas de la versión](../rn/release-notes.md#new-24-4) y la página de destino [documentación](../landing-pages/get-started-lp.md).

* **Fragmentos visuales**: los fragmentos visuales son componentes visuales reutilizables a los que se puede hacer referencia en uno o varios envíos de correo electrónico o en plantillas de contenido. La modificación de un fragmento actualiza todo el contenido que lo utiliza. Esta funcionalidad permite a los usuarios de marketing generar previamente varios bloques de contenido personalizados para ensamblar mensajes rápidamente en un proceso de diseño mejorado. [Más información](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->