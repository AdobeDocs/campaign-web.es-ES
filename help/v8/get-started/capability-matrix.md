---
audience: end-user
title: Matriz de funciones de la consola de cliente/interfaz de usuario web de Campaign
description: Lista de funciones admitidas en la interfaz de usuario web de Campaign
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 45e5b528837614cdbd537d0a92e71265f65f97db
workflow-type: tm+mt
source-wordcount: '2151'
ht-degree: 3%

---

# Consola de cliente de Campaign y web de Campaign {#capabilities-matrix}

Las funciones clave de Campaign están disponibles en la interfaz de usuario web de Campaign. Esta interfaz fue diseñada principalmente para que los especialistas en marketing planifiquen, inicien y midan sus campañas de marketing. Se muestran todas las funciones [en esta página](../rn/whats-new.md).

La personalización de la plataforma de Campaign en función de las necesidades comerciales y de datos, y la conexión a otros sistemas se administran en la consola del cliente de Campaign. Como consecuencia, algunas configuraciones y funciones solo se pueden acceder, crear o administrar desde la consola del cliente de Campaign. Algunos estarán disponibles en una actualización posterior de la interfaz de usuario web de Campaign.

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## Administración de campañas {#campaign-mgt-capabilities}

Con la interfaz de usuario web de Campaign, puede crear campañas en canales múltiples según se detalla [en esta sección](../campaigns/gs-campaigns.md). Las siguientes funcionalidades solo están disponibles en la consola del cliente de Campaign. No se puede acceder a ellas desde la interfaz de usuario web de Campaign, pero algunas pueden ser visibles desde el [Menú Explorador](user-interface.md#user-interface-explorer).

Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y aprender a utilizar estas funcionalidades.

* **Calendario de marketing**. El calendario de campañas muestra todos los programas, planes, campañas y envíos en una cronología global. Esta funcionalidad solo está disponible en la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#campaign-calendar){target="_blank"}
* **Programas y planes**. Cada campaña pertenece a un programa que pertenece a un plan. En la interfaz de usuario web de Campaign, todas las campañas están asociadas a un plan y programa integrados predeterminados. Solo puede crear y administrar planes y programas en la consola de cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#work-with-plan-and-program){target="_blank"}
* **Proveedores, gestión de presupuesto y costes**. Puede configurar los proveedores de servicios implicados en los trabajos realizados en las campañas, incluidas las estructuras de coste, y administrar los presupuestos dentro de cada programa y campaña. Esta funcionalidad solo está disponible en la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html){target="_blank"}
* **Marketing distribuido** (Marketing central/local). Adobe Campaign ofrece una aplicación de marketing distribuido para implementar campañas cooperativas entre entidades centrales (sede central, departamentos de marketing, etc.) y entidades locales (puntos de venta, agencias regionales, etc.). Esta funcionalidad solo está disponible en la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=es){target="_blank"}
* **Gestión de recursos de marketing** (MRM), objetivos, simulaciones y control de costes. Adobe Campaign ofrece una aplicación de administración de recursos de marketing (MRM) que le permite controlar las acciones de marketing de forma cooperativa mediante la administración completa y el seguimiento en tiempo real de las tareas, los presupuestos y los recursos de marketing implicados. Esta funcionalidad solo está disponible en la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html){target="_blank"}
* **Administración de tareas**. Como parte de la aplicación MRM, las tareas de Campaign se pueden crear, asignar, rastrear y monitorizar desde el panel de campañas. Esta funcionalidad solo está disponible en la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html){target="_blank"}

## Canales de comunicación {#channels-capabilities}

Con la interfaz de usuario web de Campaign, puede crear, diseñar y enviar **email**, **SMS** y **notificaciones push**, y mida su impacto utilizando varios informes específicos, como se detalla a continuación [en esta sección](../msg/gs-messages.md). Sin embargo, actualmente están disponibles los siguientes canales **no** disponible: en la aplicación, correo postal, LINE, centro de llamadas/canal personalizado, marketing social con X (Twitter).

Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y obtener más información sobre estos canales.

* **Correo directo**. El canal de correo postal le permite enviar una correspondencia física a sus clientes, clientes, proveedores u otros, como avisos, facturas, declaraciones, ofertas de marketing y mucho más. Este canal solo está disponible en la consola de cliente.  [Más información](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-direct-mail/about-direct-mail-channel.html){target="_blank"}
* **Mensajería LINE**. LINE es una aplicación gratuita de mensajería instantánea, llamadas de voz y vídeo, disponible en todos los dispositivos móviles y en PC. Adobe Campaign le permite enviar mensajes de LINE únicamente desde la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html){target="_blank"}
* **Centro de llamadas y canales personalizados**. El centro de llamadas y otros canales personalizados se pueden implementar en el entorno de Campaign. Estos canales solo pueden estar disponibles en la consola del cliente. [Obtenga más información en la documentación de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html#other-channels){target="_blank"}
* **Marketing social** con X (Twitter). Interactúa con sus clientes a través de X (Twitter) publicando mensajes y enviando mensajes directos. Esta capacidad, que viene con el complemento de marketing social, solo está disponible desde la consola del cliente: [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=es){target="_blank"}

## Páginas de destino y aplicaciones web {#Webapps-capabilities}

Adobe Campaign le permite crear, diseñar y compartir páginas de aterrizaje. La experiencia de las páginas de aterrizaje se ha reinventado por completo en la nueva interfaz. Descubra cómo crear, diseñar y publicar páginas de aterrizaje en la interfaz de usuario web de Campaign [en esta sección](../landing-pages/get-started-lp.md).

Como consecuencia, en la consola del cliente de Campaign, no se puede editar, actualizar ni modificar una página de destino creada en la interfaz web, y a la inversa. Los siguientes tipos de aplicaciones web no están disponibles en la interfaz de usuario web de Campaign. Sin embargo, se pueden ver en la lista de páginas de aterrizaje. Utilice los vínculos proporcionados para examinar la documentación de Campaign Classic v7 y obtener más información sobre estas aplicaciones web:

* **Aplicaciones web**. Adobe Campaign permite crear y publicar aplicaciones web dinámicas e interactivas con datos precargados de la base de datos y contenido adaptado a los derechos del usuario conectado. Esta funcionalidad solo está disponible en la consola del cliente. [Obtenga más información en la documentación de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html){target="_blank"}
* **Formularios web**. Las páginas web y de destino diseñadas en la consola del cliente son visibles en la interfaz de usuario web de Campaign, pero no se pueden editar ni modificar. Algunas opciones pueden diferir entre el diseñador de páginas web de la consola del cliente y el diseñador de páginas de aterrizaje que se incluye con la interfaz de usuario web de Campaign. [Obtenga más información en la documentación de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=es){target="_blank"}
* **Encuestas en línea**. Puede crear encuestas en línea y recopilar respuestas solo de la consola del cliente. Esta capacidad no está disponible en la interfaz de usuario web de Campaign.  [Obtenga más información en la documentación de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html){target="_blank"}


## Perfiles, perfiles de prueba y audiencias {#profiles-audiences-capabilities}

Puede crear, administrar y actualizar perfiles y perfiles de prueba tanto en la consola del cliente de Campaign como en la interfaz de usuario web de Campaign. Todos los cambios realizados en una interfaz de usuario se pueden ver en la otra. Sin embargo, es posible que falten algunas configuraciones de destinatario específicas y parámetros avanzados en la nueva interfaz de usuario web de Campaign.

Tenga en cuenta que el término &quot;destinatario&quot; se ha cambiado a &quot;perfil&quot; en la nueva interfaz de usuario web y que &quot;Direcciones semilla&quot; ahora son &quot;Perfiles de prueba&quot;

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Todas las audiencias creadas en la consola del cliente de Campaign o en Adobe Experience Platform están disponibles en la interfaz de usuario web de Campaign.

Trabajos de importación y exportación de una sola toma como se describe en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html#import-jobs){target="_blank"} no están disponibles en la interfaz de usuario web de Campaign. <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## Mensajería transaccional {#mc-capabilities}

Actualmente, las funciones de mensajería transaccional que vienen con el paquete de producto del Centro de mensajería no están disponibles en la nueva interfaz de usuario web de Campaign.

Examine la [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} y obtenga más información sobre las funciones de mensajería en tiempo real, como:

* Creación y ejecución de mensajes en tiempo real en correos electrónicos, SMS y push
* Enriquecimiento y personalización de mensajes
* Creación de informes y monitorización de mensajería transaccional

## Diseño de contenido {#content-capabilities}

El nuevo Diseñador de correo electrónico con la interfaz de usuario web de Adobe Campaign le permite crear fácilmente correos electrónicos personalizados y cautivadores con una interfaz intuitiva de arrastrar y soltar. Tanto si comienza desde una pizarra en blanco como si importa contenido existente o aprovecha plantillas existentes, puede diseñar y perfeccionar todo el contenido de cada correo electrónico. [Más información](../email/edit-content.md)

Con esta nueva interfaz de usuario, puede administrar la sincronización de plantillas de correo electrónico desde Adobe Experience Manager e integrarla con Adobe Experience Manager as a Cloud Service.

Tenga en cuenta que las siguientes funcionalidades no están disponibles por ahora en la interfaz de usuario web de Campaign. Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y obtener más información sobre estas funciones.

* **Creación de bloques de personalización personalizados**. Además de los bloques personalizados predeterminados, puede crear bloques personalizados desde la consola del cliente. Esta capacidad no está disponible en la interfaz de usuario web de Campaign. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}
* **Contenido de formularios personalizados**. El módulo Content management permite crear y administrar formularios para ayudar a los usuarios a crear contenido en Campaign. Esta funcionalidad solo está disponible con la consola del cliente. [Obtenga más información en la documentación de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html){target="_blank"}
* **AMP para correos electrónicos**. El nuevo formato de AMP para correo electrónico le permite incluir componentes de AMP en los mensajes y mejorar la experiencia de correo electrónico con un contenido enriquecido y procesable. Esta funcionalidad solo está disponible en la consola del cliente. [Obtenga más información en la documentación de Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## Tipologías y reglas de tipología {#rules-capabilities}

Las tipologías son conjuntos de reglas de tipología que se ejecutan durante la fase de preparación para aplicar fácilmente varias reglas de filtrado a un envío a la vez. Permiten a los especialistas en marketing estandarizar las prácticas comerciales en todas las entregas, ya que les permiten controlar, filtrar y priorizar la entrega de entregas.

Se pueden seleccionar reglas de tipología para una entrega o una plantilla de entrega en la interfaz de usuario web de Campaign, según se detallen [en esta sección](../advanced-settings/delivery-settings.md#typology). Sin embargo, las reglas y la creación, administración y personalización de reglas de tipología solo están disponibles en la consola del cliente de Campaign.

Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y obtener más información sobre las reglas de tipología:

* Creación de reglas de control. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html){target="_blank"}
* Creación de reglas de fatiga/presión. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=es){target="_blank"}
* Filtrado de la creación de reglas. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* Administración de reglas de tipología. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
* Simulación de campaña. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
* Codificación JavaScript para la creación de reglas de tipología. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}

## Flujos de trabajo {#wf-capabilities}

La nueva interfaz de usuario web de Campaign ofrece una interfaz de lienzo de flujo de trabajo reinventada para diseñar y administrar los procesos. Las actividades clave de flujo de trabajo ya están disponibles en su nuevo diseño, y algunas se incluirán en una actualización futura. Obtenga más información sobre las funcionalidades del flujo de trabajo, incluidas las protecciones y limitaciones [en esta sección](../get-started/guardrails.md).

Tenga en cuenta que las siguientes funcionalidades solo están disponibles en la consola del cliente de Campaign:

* Scripts en flujos de trabajo
* Actividades de ETL: exportación, edición de esquema, carga de datos, extracción de datos, código SQL

Obtenga más información acerca de las actividades de flujo de trabajo disponibles en la documentación de flujo de trabajo de la consola Adobe Campaign v8 [aquí](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html){target="_blank"}.

## Administración de ofertas {#offer-capabilities}

Puede enviar ofertas en los envíos creados en la interfaz de usuario web de Adobe Campaign. Estas ofertas deben haberse creado en la consola del cliente con la variable **[!UICONTROL Interacción]** módulo. El diseño de la oferta, las reglas de idoneidad y la administración de ofertas solo están disponibles en la consola del cliente de Campaign. [Más información](../msg/offers.md)

Obtenga información sobre cómo administrar un catálogo de ofertas en la [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=es){target="_blank"}.

## Integraciones con las soluciones de Adobe Experience Cloud {#exc-capabilities}

La nueva IU moderna de Campaign simplifica el diseño y la entrega de las campañas de marketing y aporta coherencia, junto con otras soluciones de Adobe, como Adobe Experience Platform y Adobe Experience Manager.

Las siguientes integraciones están disponibles en la consola del cliente de Adobe Campaign y aún no están disponibles en la interfaz de usuario web de Campaign. Utilice los vínculos proporcionados para examinar la documentación de Campaign v8 (consola de cliente) y obtener más información sobre estas integraciones:

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

## Modelado e ingesta de datos {#data-capabilities}

La interfaz de usuario web de Campaign no muestra las siguientes funcionalidades. Solo están disponibles en la consola del cliente.

Examine los vínculos proporcionados en la [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=es){target="_blank"} para obtener más información.

* **Cuentas externas**. Adobe Campaign incluye un conjunto de cuentas externas predefinidas para conectarse con sistemas externos. Como administrador del sistema de Campaign, puede crear y administrar cuentas externas solo desde la consola del cliente.[Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/external-accounts.html){target="_blank"}
* **Creación y extensión de esquemas**. La creación, modificación y extensión de esquemas está restringida a usuarios avanzados. Estas funciones solo están disponibles desde la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html){target="_blank"}
* **Administración de datos** actividades de flujo de trabajo. La administración de datos combina un conjunto de actividades para resolver problemas de objetivos complejos ofreciendo herramientas más eficientes y flexibles. Estas actividades incluyen: Carga de datos, Extracción (archivo), Actualización de datos, Edición de esquemas, Importación/exportación de flujos de trabajo técnicos. Solo están disponibles en la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#data-management){target="_blank"}
* **Acceso de datos federado**. La configuración de Campaign y la conexión a sistemas externos están restringidas a usuarios avanzados y solo están disponibles desde la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=es){target="_blank"}

## Aprobaciones {#approvals-capabilities}

La interfaz de usuario web de Campaign no muestra la administración de aprobaciones para contenido, envíos, flujos de trabajo, campañas y objetivos. Solo están disponibles en la consola del cliente.

Obtenga información sobre cómo administrar aprobaciones en flujos de trabajo en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html){target="_blank"}.


Obtenga información sobre cómo administrar las aprobaciones de entrega, contenido y segmentación en campañas en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html){target="_blank"}.


## Permisos {#permissions-capabilities}

Los usuarios de Campaign solo pueden acceder a la interfaz de usuario web de Campaign con su Adobe ID a través del Sistema Identity Management de Adobe (IMS). Los permisos concedidos a los usuarios también se aplican en la interfaz de usuario web de Campaign.

Los permisos se definen en la consola del cliente de Adobe Admin Console y Adobe Campaign según se detalla [en esta sección](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=es). No es posible realizar ninguna acción sobre los permisos desde la interfaz de usuario web de Adobe Campaign.


## Monitorización {#monitoring-capabilities}

Las funciones de monitorización de la plataforma Campaign solo están disponibles en la consola del cliente y en el panel de control de Campaign. No aparecen en la interfaz de usuario web de Campaign.

Examine los vínculos proporcionados a la documentación de Campaign v8 (consola de cliente) y al Panel de control para obtener más información.

* [Supervisión del flujo de trabajo](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html){target="_blank"}
* [Mapa de calor del flujo de trabajo](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html){target="_blank"}
* [Monitorización del rendimiento](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=es){target="_blank"}
* [Monitorización de entrega](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html){target="_blank"}




