---
audience: end-user
title: Matriz de funciones de la consola de cliente/interfaz de usuario web de Campaign
description: Lista de funciones admitidas en la interfaz de usuario web de Campaign
hide: true
hidefromtoc: true
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 69c0ea49a4caff85cd56dbc114fbfaf888ceaf1e
workflow-type: tm+mt
source-wordcount: '1282'
ht-degree: 9%

---

# Matriz de funciones de la consola de cliente/interfaz de usuario web de Campaign {#capabilities-matrix}

Solo se puede acceder a las siguientes funcionalidades desde la consola del cliente de Campaign. Algunos estarán disponibles en una versión posterior de la interfaz de usuario web de Campaign.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Administración de campañas {#campaign-mgt-capabilities}

Con la interfaz de usuario web de Campaign, puede crear campañas en canales múltiples según se detalla [en esta sección](../campaigns/gs-campaigns.md). En la versión actual, las siguientes funcionalidades solo están disponibles en la consola del cliente de Campaign. No se puede acceder a ellas desde la interfaz de usuario web de Campaign, pero algunas pueden ser visibles desde el [Menú Explorador](user-interface.md#user-interface-explorer).

Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y aprender a utilizar estas funcionalidades.

* Calendario de marketing. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#campaign-calendar){target="_blank"}
* Programas y planes. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#work-with-plan-and-program){target="_blank"}
* Proveedores, gestión de presupuesto y costes. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html){target="_blank"}
* Marketing distribuido (marketing central/local). [Más información](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=es){target="_blank"}
* Administración de recursos de marketing (MRM), objetivos, simulaciones y control de costes. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html){target="_blank"}
* Administración de tareas. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html){target="_blank"}

## Canales de comunicación{ #channels-capabilities}

Con la interfaz de usuario web de Campaign, puede crear, diseñar y enviar notificaciones push, por correo electrónico y SMS, y medir su impacto mediante varios informes dedicados, como se detalla a continuación [en esta sección](../msg/gs-messages.md). Sin embargo, los siguientes canales no están disponibles en esta versión.

Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y obtener más información sobre estos canales.

* Correo postal. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-direct-mail/about-direct-mail-channel.html){target="_blank"}
* Mensajería LINE. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html){target="_blank"}
* Centro de llamadas y canales personalizados. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html#other-channels){target="_blank"}
* Marketing social con X (Twitter). [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=es){target="_blank"}

## Páginas de destino y aplicaciones web {#Webapps-capabilities}

Adobe Campaign le permite crear, diseñar y compartir páginas de aterrizaje.  Obtenga más información sobre la página de aterrizaje en la interfaz de usuario web de Campaign [en esta sección](../landing-pages/get-started-lp.md).

Las páginas de aterrizaje se han rediseñado por completo en la interfaz de usuario web de Campaign. Como consecuencia, en la consola del cliente de Campaign, no se puede editar, actualizar ni modificar una página de destino creada en la interfaz web, y a la inversa.

Además, los siguientes tipos de aplicaciones web no están disponibles en la interfaz de usuario web de Campaign. Sin embargo, se pueden ver en la lista de páginas de aterrizaje. Utilice los vínculos proporcionados para examinar la documentación de Campaign Classic v7 y obtener más información sobre estas aplicaciones web.

* Aplicaciones web. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html){target="_blank"}
* Formularios web. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=es){target="_blank"}
* Encuestas en línea. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html){target="_blank"}


## Perfiles, perfiles de prueba y audiencias {#profiles-audiences-capabilities}

Puede crear, administrar y actualizar perfiles y perfiles de prueba tanto en la consola del cliente de Campaign como en la interfaz de usuario web de Campaign. Todos los cambios realizados en una interfaz de usuario se pueden ver en la otra. Tenga en cuenta que el término &quot;destinatario&quot; se ha cambiado a &quot;perfil&quot; en la nueva interfaz de usuario web. Sin embargo, es posible que falten algunas configuraciones de destinatario específicas y parámetros avanzados en la nueva interfaz de usuario web de Campaign.

La composición de audiencias es una nueva funcionalidad que se incluye en la interfaz de usuario web de Campaign. Como consecuencia, en la consola del cliente de Campaign, no se puede editar, actualizar ni modificar una [Audiencia creada con el modelador de consultas](../query/query-modeler-overview.md). Todas las audiencias creadas en la consola del cliente de Campaign o en Adobe Experience Platform están disponibles en la interfaz de usuario web de Campaign.

Trabajos de importación y exportación de una sola toma como se describe en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html#import-jobs){target="_blank"} no están disponibles en la interfaz de usuario web de Campaign. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## Mensajería transaccional {#mc-capabilities}

Las funciones de mensajería transaccional que se incluyen en el paquete de producto del Centro de mensajería no están disponibles en esta versión de la nueva interfaz de usuario web de Campaign. Examine la [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} y obtenga más información sobre las funciones de mensajería en tiempo real, como:

* Creación y ejecución de mensajes en tiempo real en correos electrónicos, SMS y push
* Enriquecimiento y personalización de mensajes
* Activadores (abandono del carro de compras de Adobe Analytics)
* Creación de informes y monitorización de mensajería transaccional

## Diseño de contenido {#content-capabilities}

El nuevo Diseñador de correo electrónico con la interfaz de usuario web de Adobe Campaign le permite crear fácilmente correos electrónicos personalizados y cautivadores con una interfaz intuitiva de arrastrar y soltar. Tanto si comienza desde una pizarra en blanco como si importa contenido existente o aprovecha plantillas existentes, puede diseñar y perfeccionar todo el contenido de cada correo electrónico. [Más información](../email/edit-content.md)

Con esta nueva interfaz de usuario, también puede utilizar recursos de Adobe Experience Manager 6.5 en un contenido de correo electrónico, administrar la sincronización de plantillas de correo electrónico desde Adobe Experience Manager e integrarlas con Adobe Experience Manager as a Cloud Service.

Tenga en cuenta que las siguientes funciones no están disponibles en esta versión del producto. Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y obtener más información sobre estas funciones (funciones con una `*` tampoco son compatibles con la consola del cliente de Campaign).

* AMP para correos electrónicos.  [Obtenga más información en la documentación de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html){target="_blank"}
* Contenido de recursos públicos
* Creación de bloques de personalización personalizada. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}
* Contenido de formularios personalizados (módulo de administración de contenido). [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html){target="_blank"}
* Contenido desde una dirección URL`*`
* Guardado de contenido HTML como plantilla`*`
* Fragmentos de correo electrónico`*`
* Caso de uso multivariable/multilingüe`*`

## Reglas de tipología {#rules-capabilities}

Las reglas de tipología se pueden seleccionar para una entrega o una plantilla de entrega en la interfaz de usuario web de Campaign, aunque la creación, administración y personalización de reglas y reglas de tipología solo están disponibles en la consola del cliente de Campaign.

Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y obtener más información sobre las reglas de tipología.

* Creación de reglas de control. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html){target="_blank"}
* Creación de reglas de fatiga/presión. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=es){target="_blank"}
* Filtrado de la creación de reglas. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* Administración de reglas de tipología. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
* Simulación de campaña. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
* Codificación JavaScript para la creación de reglas de tipología. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}

## Flujos de trabajo {#wf-capabilities}

La nueva interfaz de usuario web de Campaign ofrece una interfaz de lienzo de flujo de trabajo reinventada para diseñar y administrar los procesos. Las actividades clave de flujo de trabajo ya están disponibles en su nuevo diseño, y algunas estarán disponibles en una versión futura. Obtenga más información sobre las funcionalidades del flujo de trabajo, incluidas las protecciones y limitaciones [en esta sección](../workflows/gs-workflows.md)

Tenga en cuenta que las siguientes funcionalidades solo están disponibles en la consola del cliente de Campaign:

* Scripts en flujos de trabajo
* Actividades de ETL: exportación, edición de esquema, carga de datos, extracción de datos, código SQL

## Administración de ofertas {#offer-capabilities}

Adobe Campaign Web permite enviar con las entregas ofertas que se han creado en la consola utilizando **[!UICONTROL Interacción]** módulo. El diseño de la oferta, las reglas de idoneidad y la administración de ofertas solo están disponibles en la consola del cliente de Campaign. [Más información](../msg/offers.md)

Obtenga información sobre cómo administrar un catálogo de ofertas en la  [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=es){target="_blank"}.

## Integraciones con las soluciones de Adobe Experience Cloud {#exc-capabilities}

La nueva IU moderna de Campaign simplifica el diseño y la entrega de las campañas de marketing y aporta coherencia, junto con otras soluciones de Adobe, como Adobe Experience Platform y Adobe Experience Manager.

Las siguientes integraciones están disponibles en la consola del cliente de Adobe Campaign y aún no están disponibles en esta versión de la interfaz de usuario web de Campaign.

Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y obtener más información sobre las reglas de tipología.

* Uso compartido de KPI y uso de datos de Adobe Analytics. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html){target="_blank"}
* Uso compartido de audiencias con Adobe Experience Cloud (Adobe Audience Manager). [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html){target="_blank"}
* Integración con Adobe Target. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html){target="_blank"}
* Integración con Adobe Experience Cloud Triggers. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html){target="_blank"}

## Creación de informes {#reporting-capabilities}

La nueva interfaz de usuario web de Campaign incluye un conjunto de nuevos informes y KPI para todos los canales: informes de envío, informes de campaña e informes globales. Obtenga más información [en esta sección](../reporting/gs-reports.md)

Algunas funciones solo están disponibles desde la consola del cliente. Examine los vínculos proporcionados para examinar [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=es){target="_blank"} y obtenga más información.

* Procesamiento integrado del informe de envío y la bandeja de entrada. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html){target="_blank"}
* Personalizaciones de informes. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html){target="_blank"}
* Análisis descriptivo. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html){target="_blank"}
* Análisis de campañas / Informes de cubos. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=es){target="_blank"}
* El uso compartido del informe se ha programado como PDF y CSV, o vínculo. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html){target="_blank"}
* Exporte/descargue un informe como archivo CSV o de PDF. [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/actions-on-reports.html){target="_blank"}

## Modelado e ingesta de datos {#data-capabilities}

La interfaz de usuario web de Campaign no muestra las siguientes funcionalidades. Solo están disponibles en la consola del cliente.

* Cuentas externas
* Extensión de los esquemas
* Actividades del flujo de trabajo de administración de datos: cargar datos, extracción (archivo), actualizar datos, editar esquema, importar/exportar flujos de trabajo técnicos
* Configuración de Campaign y conexión a sistemas externos

## Aprobaciones {#approvals-capabilities}

La interfaz de usuario web de Campaign no muestra las siguientes funcionalidades. Solo están disponibles en la consola del cliente.

* Aprobación de contenido
* Aprobación de envío
* Aprobación de campaña
* Aprobación del destino
