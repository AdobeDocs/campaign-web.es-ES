---
title: Introducción a Adobe Campaign v8 para especialistas en marketing
description: Descubra la funcionalidad clave de Campaign v8. Está dirigido a los especialistas en marketing que migran de Campaign Standard a Campaign v8.
role: User
level: Beginner, Experienced
exl-id: 514da15d-325b-4d28-9a58-50c1ae2e4925
source-git-commit: 09794df17632df243bf736d08a5a53319d79bf5f
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 19%

---

# Introducción para especialistas en marketing {#acs-gs-marketers}

Esta guía proporciona información general sobre las funcionalidades clave de Campaign v8 para los especialistas en marketing que realizan la transición de Campaign Standard a Campaign v8.

Puede acceder a Adobe Campaign v8 a través de la consola del cliente o la interfaz de usuario web. La interfaz web permite crear, administrar y ejecutar acciones de marketing clave. La nueva interfaz de Adobe Campaign Web ofrece una experiencia de usuario moderna e intuitiva para simplificar el diseño y el envío de las campañas de marketing. [Más información](../../v8/get-started/user-interface.md).

Con la migración, todos los datos de Campaign Standard se importan en Campaign v8, lo que garantiza una transición sin problemas con una interrupción mínima de las operaciones en curso.

Puede seguir utilizando sus credenciales existentes para iniciar sesión y conectarse a la nueva instancia de Adobe Campaign v8. Una vez que haya iniciado sesión, podrá comprobar que todos sus perfiles y flujos de trabajo se están migrando, lo que le permite seguir trabajando en sus campañas.

La diferencia principal está en la interfaz de usuario. A continuación, se muestra una comparación del mismo flujo de trabajo en las dos interfaces:

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de entrega continua, que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Consulte las [Notas de la versión](../../v8/rn/release-notes.md) con regularidad para ver las actualizaciones más recientes.

## Descubra la interfaz de usuario web de Campaign {#acs-gs-marketers-ui}

En el siguiente vídeo, aprenderá a acceder a la interfaz de usuario web de Campaign y a navegar por ella, así como a personalizar las listas de inventario.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

Para obtener más información, consulte la siguiente documentación:

1. [Descubra la interfaz de usuario web de Campaign](../../v8/get-started/user-interface.md)

1. [Examinar y filtrar listas](../../v8/get-started/list-filters.md)


## Creación y administración de perfiles y audiencias {#acs-gs-marketers-profiles-and-audiences}

Los conceptos generales para crear y administrar perfiles y audiencias en Campaign v8 son los mismos que en Adobe Campaign Standard. Aprenda a empezar con perfiles y audiencias en [esta sección](../../v8/audience/gs-audiences-recipients.md).

A continuación encontrará algunos vínculos útiles con los que empezar.

### Administración de perfiles {#acs-gs-marketers-profiles}

En Adobe Campaign, un perfil es un registro almacenado en la base de datos que sirve como componente clave para crear audiencias para envíos y añadir datos de personalización al contenido.

1. Obtenga información sobre cómo acceder, administrar y explorar perfiles mediante la interfaz de usuario web de Campaign en este vídeo:

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   Obtenga más información en la documentación de [Introducción a los perfiles](../../v8/audience/about-recipients.md).

1. Obtenga información sobre cómo crear y administrar perfiles de prueba en Campaign v8

   >[!VIDEO](https://video.tv.adobe.com/v/3442844?quality=12&learn=on){transcript=true}

### Administrar audiencias {#acs-gs-marketers-audiences}

Las audiencias son conjuntos de perfiles que comparten comportamientos o características similares. Esta colección de personas se puede generar, seleccionar o cargar. Una vez creados, los públicos pueden aprovecharse como población destinatario de los envíos.

En este vídeo, aprenderá a crear y administrar audiencias, a seleccionar audiencias para una entrega y a definir grupos de control:

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

Consulte [Introducción a las audiencias](../../v8/audience/manage-audience.md){target="_blank"} para obtener más información.

Al igual que en Campaign Standard, puede agregar un grupo de control al envío. Puede definir un grupo de control para evitar enviar mensajes a una parte de la audiencia y comparar el comportamiento tras la entrega con el destinatario principal. Esta opción le ayuda a medir el impacto de su campaña.
Aprenda a [establecer un grupo de control](../../v8/audience/control-group.md){target="_blank"}.

>[!AVAILABILITY]
>
>* Todas las audiencias creadas mediante la actividad Campaign Standard Query se transforman en filtros predefinidos en Campaign v8 durante la transición. Campaign v8 también admite la actividad Query.
>
>* La audiencia de lectura se transforma en actividad de consulta con [filtro predefinido](../../v8/query/build-query.md)
>
>* El filtro predefinido solo toma el valor más reciente después de la migración de la audiencia a Campaign v8.
>
>* Las audiencias de tipo de archivo de Campaign Standard se migran como de tipo lista sin dimensiones.

### Administración de las suscripciones {#acs-gs-marketers-sub}

Puede administrar y crear sus servicios, como boletines informativos, y comprobar las suscripciones o cancelaciones de suscripción a estos servicios. Los pasos clave son globalmente los mismos que en Campaign Standard. Obtenga más información en las páginas siguientes:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="Poco frecuente" src="assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>Creación de servicios de suscripción</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="Poco frecuente" src="assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>Administrar suscriptores<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="Validación" src="assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/send-to-subscribers"><strong>Enviar mensajes a los suscriptores de un servicio</strong></a>
</div>
<p>
</td>
</tr>
</table>

## Uso de planes, programas y campañas {#acs-gs-marketers-plans}

La versión 8 de Adobe Campaign le permite configurar la jerarquía de carpetas para planes y programas de marketing. Las capacidades de los planes, programas y campañas son similares con Campaign Standard y con Campaign v8.

Obtenga más información en la [documentación de planes y programas](../../v8/administration/plans-programs.md).

A continuación encontrará vínculos útiles con los que empezar. Los cambios que pueden afectar a su experiencia del usuario se resaltan en las Notas de disponibilidad.


### Creación de una campaña {#acs-gs-marketers-campaign}

Adobe Campaign le permite organizar fácilmente sus iniciativas de marketing segmentadas mediante la función de administración de campañas integrada. Con la capacidad de definir una programación, puede planificar la duración y el tiempo de las campañas para alinearlas con los objetivos estratégicos y maximizar la participación del público destinatario.

![Flujo de campaña](assets/campaign-flow.png)

Siga la documentación siguiente para obtener más información sobre las campañas:

1. [Introducción a las campañas](../../v8/campaigns/gs-campaigns.md)
1. [Acceso y administración de campañas](../../v8/campaigns/manage-campaigns.md)
1. [Cree su primera campaña](../../v8/campaigns/create-campaigns.md)


### Creación de un flujo de trabajo {#acs-gs-marketers-wf}

La interfaz de usuario del flujo de trabajo se ha reinventado completamente en la interfaz de usuario web de Campaign para facilitar el uso, la configuración, la ejecución y la resolución de problemas. Como ya ha experimentado en Campaign Standard, con los flujos de trabajo puede organizar la gama completa de procesos y tareas, mejorar la velocidad y la escala de cada aspecto de sus campañas de marketing, desde la creación de segmentos y la preparación de mensajes hasta la entrega. Además, puede sincronizar sus canales con una interfaz única y fácil de usar para la orquestación de campañas.

Descubra cómo funcionan los flujos de trabajo y cómo crear un flujo de trabajo de objetivo en este vídeo:

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

Obtenga más información con la [documentación de flujo de trabajo](../../v8/workflows/gs-workflows.md).

La interfaz de usuario web de Adobe Campaign incluye un modelador de consultas en flujos de trabajo que simplifica el proceso de filtrar la base de datos en función de varios criterios. [Más información acerca del modelador de consultas](../../v8/query/query-modeler-overview.md)

Para comprender el propósito y la funcionalidad de cada actividad dentro de su flujo de trabajo, explore la información detallada disponible en [actividades de flujo de trabajo](../../v8/workflows/activities/about-activities.md)

Maximice la eficiencia de su flujo de trabajo revisando las [protecciones y limitaciones de los flujos de trabajo](../../v8/get-started/guardrails.md).

>[!AVAILABILITY]
>
>* El historial y los registros [de ejecución del flujo de trabajo](../../v8/workflows/start-monitor-workflows.md#logs-tasks) están disponibles en Adobe Campaign v8.
>
>* Los registros históricos de los flujos de trabajo ejecutados en la instancia de Campaign Standard no se migran a Campaign v8.
>
>* Las unidades organizativas se asignan al concepto de carpeta para su asignación y garantizar un control de acceso similar.
>

## Creación y administración de entregas {#acs-gs-marketers-deliveries}

Con la interfaz de usuario web de Campaign, como experto en marketing, puede crear envíos independientes desde el menú izquierdo de **Envíos** o envíos en el contexto de un flujo de trabajo, incluido o no en una campaña. Los pasos clave están alineados con la experiencia anterior en Campaign Standard. Aprenda a crear una entrega en la siguiente sección: [Documentación de creación y administración de entregas](../../v8/msg/gs-deliveries.md).

Vínculos útiles:

* **Plantillas de envío**: para acelerar y mejorar el proceso de diseño, puede crear plantillas de envío para reutilizar fácilmente el contenido y la configuración personalizados en sus campañas. Esta funcionalidad le permite estandarizar la apariencia creativa para ejecutar y lanzar campañas con mayor rapidez./ Obtenga más información en la página [Plantilla de envíos](../../v8/msg/delivery-template.md).

* **Configuración de envío**: la configuración de envío son parámetros de envío técnicos definidos en la plantilla de envío. Se pueden sobrecargar para cada envío. Esta configuración está disponible desde el botón Settings disponible al editar una entrega o una plantilla de envíos. Obtenga más información en la sección [Configuración de envío](../../v8/advanced-settings/delivery-settings.md).

* **Contenido dinámico**: las funciones de contenido dinámico de Adobe Campaign Web le permiten personalizar el contenido en función de la información que haya recopilado sobre sus destinatarios. Al utilizar contenido dinámico, se asegura de que sus esfuerzos de marketing sean más relevantes, lo que evita la comercialización de productos o servicios no deseados o innecesarios. Obtenga más información en la sección [Contenido dinámico](../../v8/personalization/gs-personalization.md).

* **Pruebas**: una vez definido el contenido de su envío, puede usar perfiles y perfiles de prueba para previsualizarlo y probarlo antes de enviar el mensaje. Este paso es crucial para garantizar que sea preciso, pero también que no contenga errores ni en la configuración del contenido ni en la personalización. Ver [vista previa y prueba](../../v8/preview-test/preview-test.md).

* **Programación**: puede establecer la fecha y la hora exacta para enviar los mensajes. Al elegir el momento más apropiado para el mensaje de marketing, puede maximizar las tasas de apertura.

   * Aprenda a [programar un envío independiente](../../v8/msg/gs-deliveries.md#gs-schedule)
   * Aprenda a [programar un envío en un flujo de trabajo](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)

* **Agregar ofertas**: puede agregar ofertas a las entregas en la interfaz de usuario web de Adobe Campaign. Estas ofertas están disponibles en el menú de la izquierda Ofertas, que le permite acceder a la lista de ofertas.  Aprenda a [agregar ofertas a sus mensajes](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* Se han migrado los envíos en estado de borrador o terminado.
>
>* Los envíos que se encuentran en uno de los siguientes estados se han migrado a Adobe Campaign v8, pero deben prepararse de nuevo: En tránsito/En curso/Cancelado/Reintento en curso/Error de preparación.
>
>* Los envíos que se encuentran en uno de los siguientes estados se han migrado como envíos cancelados: Para envíos cancelados/Reintento en curso.
>
>* Los vínculos de seguimiento, los vínculos de URL de páginas espejo y los vínculos de suscripción/cancelación de suscripción funcionan como en Campaign Standard.
>
>Vea también las secciones siguientes: [Seguimiento y supervisión](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}, [Promoción de marca](https://experienceleague.adobe.com/es/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} en Adobe Campaign.

### Envío de correo electrónico {#acs-gs-marketers-email}

Obtenga información sobre cómo crear un envío de correo electrónico desde cero, definir la audiencia, diseñar el contenido, simular la previsualización y enviar una prueba en este vídeo:

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

Aprenda a crear su primer correo electrónico de destino en [Crear su primera documentación de correo electrónico](../../v8/email/create-email.md)

En Campaign v8, los pasos detallados para crear, probar y enviar un envío de correo electrónico son similares a Campaign Standard.

1. **Diseñar y definir contenido**

   El diseñador de correo electrónico de Campaign v8 es similar al disponible en Campaign Standard. Como recordatorio, el editor de correo electrónico heredado de Campaign Standard[quedó obsoleto](https://experienceleague.adobe.com/es/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} hace unos años. Ya debería haber realizado la transición a Campaign Email Designer para crear y personalizar el contenido del correo electrónico.

   Obtén información sobre cómo navegar por el Diseñador de correo electrónico. Obtenga información sobre cómo estructurar y diseñar un correo electrónico desde cero, cómo personalizarlo y probarlo en el siguiente vídeo:

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   El Diseñador de correo electrónico le permite crear correos electrónicos personalizados y cautivadores con una interfaz intuitiva para arrastrar y soltar. Obtenga más información en la [documentación de Designer por correo electrónico](../../v8/email/get-started-email-designer.md)

   Obtenga información sobre cómo crear un correo electrónico cargando HTML, cómo hacerlo compatible con el Designer de correo electrónico y cómo convertirlo en una plantilla en este vídeo:

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   Un fragmento de contenido es un componente reutilizable al que se puede hacer referencia en uno o varios mensajes. Obtenga más información acerca de [fragmentos de contenido](../../v8/content/fragments.md) para simplificar la creación del envío de correo electrónico.

   Para un proceso de diseño acelerado y mejorado, puede crear plantillas independientes para reutilizar fácilmente el contenido personalizado en Adobe Campaign. Ver [Crear plantillas de correo electrónico](../../v8/content/create-email-templates.md)

1. **Vista previa y prueba**

   Obtenga información sobre cómo previsualizar el contenido y la personalización de los mensajes de correo electrónico, enviar entregas de prueba (pruebas) y comprobar el procesamiento de los correos electrónicos en clientes populares de escritorio, móviles y web en este vídeo:

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **Enviar correo electrónico y registros de comprobación**

   Una vez definido el contenido, la audiencia y la programación, estará listo para preparar la entrega por correo electrónico. Obtenga más información en las siguientes secciones:

   * [Preparación y envío de un correo electrónico](../../v8/monitor/prepare-send.md)
   * [Monitorización de los registros de envío](../../v8/monitor/delivery-logs.md)


### Envío de SMS {#acs-gs-marketers-sms}

Los envíos SMS proporcionan una forma práctica y eficaz de enviar mensajes de texto a los dispositivos móviles de los clientes. Con esta función, puede crear, personalizar y previsualizar mensajes basados en texto para una comunicación eficaz.

En Campaign v8, los pasos detallados para crear, probar y enviar un envío SMS son similares a Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="Posible cliente" src="assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/sms/create-sms"><strong>Creación de un envío SMS</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="Poco frecuente" src="assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/sms/content-sms"><strong>Diseño de un envío de SMS<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="Validación" src="assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/sms/send-sms"><strong>Previsualizar y enviar un envío de SMS</strong></a>
</div>
<p>
</td>
</tr></table>

### Notificaciones push {#acs-gs-marketers-push}

Las notificaciones push son esenciales para llegar a los usuarios de su aplicación móvil, incluso cuando no estén utilizando activamente la aplicación. Sirven para varios fines, como proporcionar actualizaciones, impulsar acciones específicas y notificar ofertas.

En Campaign v8, los pasos detallados para crear, probar y enviar una entrega de notificaciones push son similares a Campaign Standard.


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/push/create-push">
<img alt="Posible cliente" src="assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/push/create-push"><strong>Creación de un envío push</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/push/content-push">
<img alt="Poco frecuente" src="assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/push/content-push"><strong>Diseño de un envío push<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/push/send-push">
<img alt="Validación" src="assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/msg/push/send-push"><strong>Previsualizar y enviar un envío push</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>* Adobe Campaign v8 es compatible con Android y con el canal push de iOS. Para la transición de flujos de trabajo y envíos existentes mediante el canal push, conéctese con su administrador de transición de Adobe Campaign. Más información sobre [Configuración de canal](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
>
>* Tenga en cuenta que SDK V4 para aplicaciones móviles estaba [obsoleto en Campaign Standard](https://experienceleague.adobe.com/es/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} hace unos años. Ya debería haber realizado la transición a Adobe Experience Platform SDK, que es el mismo que se usa en Campaign v8.
> 

### Correo directo {#acs-gs-marketers-direct-mail}

El correo directo es un canal sin conexión que le permite producir archivos para enviar de forma masiva cartas personalizadas a sus clientes, como postales, folletos o catálogos. Al crear un envío de correo directo, Adobe Campaign genera automáticamente un archivo de extracción que contiene todos los perfiles de destino y los datos seleccionados, como las direcciones postales y los atributos de perfil.

>[!VIDEO](https://video.tv.adobe.com/v/3433316/?learn=on)

En Campaign v8, los pasos detallados para crear, probar y enviar una entrega de correo directo son similares a los de Campaign Standard.

1. [Creación de envíos de correo directo](../../v8/direct-mail/create-direct-mail.md)
1. [Definir el archivo de extracción](../../v8/direct-mail/content-direct-mail.md)
1. [Previsualización y envío](../../v8/direct-mail/send-direct-mail.md)

>[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

### Canal en la aplicación {#acs-gs-marketers-in-app}

Tenga en cuenta que el canal en la aplicación no está disponible en Campaign v8. Si necesita enviar notificaciones en la aplicación, póngase en contacto con su representante de Adobe.

## Creación y administración de páginas de destino {#acs-gs-marketers-lp}

La interfaz de usuario web de Adobe Campaign v8 viene con una experiencia de usuario reimaginada para las páginas de aterrizaje. Campaign le permite crear, diseñar y compartir páginas de aterrizaje. Adobe Campaign le permite dirigir a los usuarios a formularios en línea, donde pueden actualizar sus datos, optar por suscribirse a darse de baja de la recepción de comunicaciones, o suscribirse a un servicio específico, como una Newsletter.

Como usuario de Campaign Standard que realiza la transición a Campaign v8, las páginas de aterrizaje existentes se han migrado a la interfaz de usuario web de Campaign. Puede acceder a la misma gama de funcionalidades.

Obtenga más información acerca de las páginas de aterrizaje en las siguientes secciones:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="Posible cliente" src="assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/landing-pages/create-lp"><strong>Creación de páginas de destino</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="Validación" src="assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/landing-pages/lp-content"><strong>Páginas de destino de diseño</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="Validación" src="assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/es/docs/campaign-web/v8/landing-pages/lp-templates"><strong>Trabajar con plantillas de página de aterrizaje</strong></a>
</div>
<p>
</td>
</tr></table>


## Creación de informes {#acs-gs-marketers-reporting}

Adobe Campaign proporciona un conjunto de [herramientas de informes](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"}. Como administrador, puede crear y configurar informes para compartirlos con otros usuarios de Campaign.

El conjunto de herramientas de creación de informes de Adobe Campaign proporciona información valiosa sobre la eficacia de sus esfuerzos de marketing, lo que le permite optimizar sus campañas para obtener el máximo impacto. Obtenga más información en la [documentación de informes](../../v8/reporting/gs-reports.md).

Además, alineado con la experiencia de Adobe Campaign Standard, el sistema de informes dinámico está disponible en Campaign v8 para sus envíos de correo electrónico. Proporciona informes totalmente personalizables y en tiempo real para medir el impacto de las actividades de marketing. Este añade acceso a los datos de perfil, lo que permite el análisis demográfico por dimensiones de perfil como sexo, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. Obtenga más información en la [documentación de informes dinámicos](https://experienceleague.adobe.com/es/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"}

>[!AVAILABILITY]
>
>* [Los informes dinámicos](https://experienceleague.adobe.com/es/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} se pueden usar para informar sobre envíos de correo electrónico, campañas con envíos de correo electrónico y mensajes transaccionales. También está disponible el análisis demográfico por dimensión de Perfil.
>
> * Los informes de la [interfaz de usuario web de Adobe Campaign](../../v8/reporting/campaign-reports.md) también están disponibles para todos los usuarios que realizan la transición de Adobe Campaign Standard a Adobe Campaign v8.

Adobe Campaign ofrece tres informes diferentes:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="Validación" src="./assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>Informes de campaña</strong></a>
</div>
<p>
<div>
<p>Proporcione información detallada sobre el rendimiento, la eficacia y los resultados de sus envíos individuales, lo que le proporcionará una visión general completa.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="Posible cliente" src="assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>Informes de envío</strong>
</div>
<p>
<div>
<p>Ofrezca un análisis exhaustivo del rendimiento de cada envío, por canal: tasas de éxito, participación de la audiencia y otras métricas esenciales. Le permiten evaluar la eficacia y el impacto generales de la campaña.</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="Informes globales" src="assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/global-report/global-reports"><strong> Informes globales</strong></a>
</div>
<p>
<div>
<p>Ofrezca un resumen general consolidado de las métricas de tráfico y participación para cada canal dentro de la instancia de Campaign. Estos informes constan de varios widgets, cada uno de los cuales ofrece una perspectiva distinta sobre el rendimiento de la campaña o el envío.</p>
</div>
<p>
</td>
</tr>
</table>
