---
audience: end-user
title: Transición de Campaign Standard a la web de Adobe Campaign
description: Interfaz de usuario web de Discover Campaign
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 16%

---

# Transición de Campaign Standard a Campaign v8 {#acs-to-ac}

Los usuarios de Adobe Campaign Standard ahora pueden pasar a Adobe Campaign Managed Cloud Services v8. Esta transición ofrece varias ventajas:

* **Infraestructura de TI sólida**: Managed Cloud Services v8 proporciona una infraestructura de TI más sólida, lo que garantiza un rendimiento, fiabilidad y escalabilidad mejorados para las campañas.
* **Soporte mejorado**: El equipo de Cloud Services administrados ofrece asistencia de primera para garantizar una transición sin problemas y una supervisión continua de la plataforma. La asistencia incluye solución de problemas y mantenimiento proactivo.
* **Integración con Adobe Experience Platform**: Managed Cloud Services v8 se conecta sin problemas con Adobe Experience Platform, lo que permite a los usuarios aprovechar al máximo sus datos y ofrecer campañas personalizadas e impactantes en todos los canales.
* **Experiencia e interfaz de usuario coherentes**: La transición a Managed Cloud Services v8 no interrumpe los flujos de trabajo. Los usuarios siguen disfrutando de la interfaz y la experiencia conocidas, lo que minimiza la curva de aprendizaje de los equipos.

**Como usuario Campaign Standard en proceso de transición a Campaign v8, obtenga más información sobre cómo empezar [en este documento](../../adoption/home.md).**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## Funcionalidades clave {#key-features}

Los usuarios de Campaign v8 tienen acceso a la nueva interfaz web de Campaign y a la consola v8. Los datos y la configuración se sincronizan entre entornos. Todos los datos y la configuración disponibles en la consola del cliente se pueden ver en la interfaz de usuario web de Campaign, a la que se puede acceder desde el menú de navegación izquierdo del explorador. [Más información](../get-started/user-interface.md#user-interface-explorer)

La interfaz de usuario web de Campaign está diseñada para que los especialistas en marketing creen y organicen fácilmente campañas. Las funciones clave de la interfaz de usuario web de Campaign v8 incluyen:

* **Experiencia moderna, cordial y unificada**. [Más información](../get-started/connect-to-campaign.md).
* **Nuevas y potentes funciones y procesos sin problemas**. [Más información](../get-started/user-interface.md).
* **Modelador de consultas simplificado e intuitivo**. [Más información](../query/query-modeler-overview.md).
* **Funciones integradas de administración de campañas en canales múltiples**. [Más información](../msg/gs-messages.md).
* **Actividades de flujo de trabajo de campaña rediseñadas**. [Más información](../workflows/gs-workflows.md).
* **Fácil creación y administración de perfiles**. [Más información](../audience/about-recipients.md).
* **Filtros predefinidos**. [Más información](../get-started/predefined-filters.md).
* **Convertidor de HTML para diseño de correo electrónico**. [Más información](../email/existing-content.md).
* **SMS con ofertas**. [Más información](../msg/offers.md).

La consola del cliente de Campaign está diseñada para que los administradores y desarrolladores configuren y personalicen su entorno. Las funcionalidades clave disponibles en la consola del cliente de Campaign se detallan en [esta documentación](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/new/whats-new){target="_blank"}.

>[!NOTE]
>
>Obtenga más información acerca de las funcionalidades admitidas y no admitidas, así como la interoperabilidad entre la interfaz de usuario web de Campaign y la consola de cliente de Campaign [en esta página](../get-started/capability-matrix.md).

## Terminología {#terminology}

La mayoría de los conceptos son similares entre Campaign v8 y Campaign Standard. Sin embargo, existen algunas diferencias terminológicas. Algunos ejemplos son:

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

Para garantizar una transición sin problemas a Campaign v8, se han añadido funciones clave de Campaign Standard a Campaign v8. Estas características se detallan en [esta documentación](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es){target="_blank} y solo están disponibles para los usuarios que realizan la transición desde Campaign Standard.

* **Informes dinámicos**: los informes dinámicos proporcionan informes personalizables en tiempo real para medir el impacto de las actividades de marketing. Incluye acceso a datos de perfil para el análisis demográfico por dimensiones como sexo, ciudad y edad, junto con datos funcionales de la campaña de correo electrónico como aperturas y clics. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=es){target="_blank"}.

* **Personalización de marca centralizada**: Adobe Campaign permite que las empresas definan directrices técnicas y visuales de marca. Los usuarios pueden presentar una marca coherente a los clientes, desde logotipos hasta aspectos técnicos como el remitente de correos electrónicos, la URL o los dominios. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=es).

* **API de REST**: los usuarios migrados de Campaign Standard pueden usar las API de REST para crear integraciones para Adobe Campaign y construir ecosistemas al interconectar Adobe Campaign con otras tecnologías. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=es){target="_blank"}.

* **Páginas de destino**: Las páginas de destino de la versión 8 de Campaign incluyen mejoras para garantizar la paridad de las características con Campaign Standard. Obtenga más información en las [notas de la versión](../rn/release-notes.md#new-24-4) y la página de aterrizaje [documentación](../landing-pages/get-started-lp.md).

* **Fragmentos visuales**: Los fragmentos visuales son componentes visuales reutilizables a los que se hace referencia en uno o varios envíos de correo electrónico o plantillas de contenido. La modificación de un fragmento actualiza todo el contenido que lo utiliza. Esta funcionalidad permite a los usuarios de marketing generar previamente varios bloques de contenido personalizados para ensamblar mensajes rápidamente en un proceso de diseño mejorado. [Más información](../content/use-visual-fragments.md).

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->