---
title: Notas de la versión anterior de la interfaz de usuario web de Campaign v8
description: Notas de la versión de la interfaz de usuario web de Campaign 2024
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '2532'
ht-degree: 100%

---

# Notas de la versión 2024 {#2024-release}

Esta página enumera todos los cambios y mejoras disponibles con las **versiones de 2024**. Las notas de la versión más recientes están disponibles en [esta página](release-notes.md).


## Versión de octubre de 2024 {#24-10-release}

**Fecha de publicación**: 29 de octubre de 2024

Las siguientes funciones y mejoras están disponibles a partir de la versión de octubre.

### Funciones

<table>
<thead>
<tr>
<th><strong>Cuentas externas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede configurar y administrar cuentas externas directamente a través de la interfaz de usuario web de Adobe Campaign. Esta nueva función facilita la configuración de diferentes tipos de cuentas externas, como los correos electrónicos rechazados (POP3) o las instancias de ejecución.</p>
<p>Para obtener más información, consulte la <a href="../administration/external-account.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Mensajería transaccional</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La mensajería transaccional (Centro de mensajes) ya está disponible en la interfaz de usuario web de Campaign. Este complemento se ha diseñado para activar mensajes que se generan a partir de eventos desencadenados desde los sistemas de información y pueden ser: una factura, una confirmación de pedido, una confirmación de envío, un cambio de contraseña, una notificación de no disponibilidad del producto, el estado de la cuenta, una creación de cuenta en un sitio web, etc.</p>
<p>Para obtener más información, consulte la <a href="../transactional-messaging/transactional.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>


### Mejoras

* **Actividades del flujo de trabajo**: ahora puede mover una actividad y todos sus nodos secundarios de una transición a otra dentro de un flujo de trabajo. Hay disponible un botón **Mover** dedicado en el panel de propiedades de la actividad para realizar esto. [Más información](../workflows/orchestrate-activities.md#move)

* **Actividad de enriquecimiento del flujo de trabajo**

   * Ahora puede definir un Alias y una Etiqueta al crear un nuevo campo en la actividad **Enriquecimiento**. [Más información](../workflows/activities/enrichment.md#collection-settings)
   * Ahora puede añadir ofertas para cada perfil en la actividad **Enriquecimiento**. [Más información](../workflows/activities/enrichment.md##add-offers)

* **Distribución de valores**: al acceder a la lista de campos para personalización, ahora puede comprobar cómo se distribuyen los valores para cada campo. Una ventana emergente dedicada muestra el número y el porcentaje de cada valor. [Más información](../query/build-query.md#distribution-values-query)

* **Información de versión y sistema**: ahora puede obtener acceso a los detalles de las versiones de la instancia, tanto para la consola de cliente como para la interfaz de usuario web. En esta nueva sección también se muestran todos los paquetes integrados instalados en el entorno. [Más información](../get-started/user-interface.md#user-interface-about)

* **Listas**: ahora puede reordenar fácilmente los valores de una lista. [Más información](../get-started/work-with-folders.md)

* **Envío**: ahora puede acceder a la variable de envío desde los campos de personalización. [Más información](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## Actualizaciones de septiembre {#9-2024}

<table>
<thead>
<tr>
<th><strong>Asistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Una vez que haya creado y adaptado su mensaje, llévelo al siguiente nivel con el Asistente de IA de Adobe Campaign Web. Esta potente herramienta le permite optimizar el impacto de su contenido mediante la generación de una serie de atractivos textos, títulos principales e imágenes visualmente atractivas.</p>
<p>Sumérjase en una experiencia práctica con <a href="https://experienceleague.adobe.com/es/apps/journey-optimizer/ai-assistant-content-accelerator">nuestra previsualización de funciones en vivo</a>, diseñada para que explore las funciones en primera persona y comprenda plenamente todo su potencial.</a>.</p>
<p>Para obtener más información, consulte la <a href="../content/generative-gs.md">documentación detallada</a>.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Fecha de disponibilidad: 12 de septiembre</p>
</td>
</tr>
</tbody>
</table>

## Versión de agosto {#24-8-release}

**Fecha de lanzamiento**: 3 de septiembre de 2024

Las siguientes funciones y mejoras están disponibles a partir de la versión de agosto.

* **Parámetros SMTP**: la configuración de SMTP está ahora disponible en la configuración de envío de correo electrónico. [Más información](../advanced-settings/delivery-settings.md#smtp)

* **Variables globales**: ahora puede definir variables globales para los valores de los envíos. [Más información](../advanced-settings/delivery-settings.md#variables-delivery)

### Nuevas funciones en disponibilidad limitada {#acs-24-8}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se pueden implementar en ningún otro entorno.
>
>Consulte las siguientes páginas de documentación: [Campaign Standard de la transición a Campaign v8](../rn/acs-migration.md) y [Funciones para usuarios de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es){target="_blank"}.

* **Promoción de la marca para correo directo**: ahora los administradores técnicos pueden definir una o varias marcas para centralizar los parámetros que afectan a la identidad de una marca. Esto incluye el logotipo de la marca, el dominio de la URL de acceso de la página de destino o la configuración del seguimiento de mensajes. Ahora puede crear estas marcas y vincularlas a mensajes o páginas de destino. Esta configuración se administra en plantillas. [Más información](../administration/branding/branding-assign.md)

* **Suscripciones con páginas de destino**: ahora puede vincular una página de destino a un servicio y enviar un mensaje de confirmación cuando los usuarios la validen. [Más información](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Fragmentos visuales**: ahora puede archivar fragmentos de contenido visual. [Más información](../content/create-fragment.md#archive)

* **Captcha en páginas de destino**: ahora puede añadir captcha para proteger su página de destino contra spam y abusos causados por bots. Esto no es intrusivo para los clientes, ya que no requiere ninguna interacción por parte de ellos y se basa en las interacciones con el sitio. [Más información](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=es){target="_blank"}.-->


## Notas de la versión de julio {#24-7-release}

**Fecha de lanzamiento**: 30-31 de julio de 2024

Las siguientes funciones y mejoras están disponibles para todos los usuarios a partir de la versión de julio.

### Fragmentos de contenido {#24-7-1}

Ahora puede crear y utilizar fragmentos de contenido. Un fragmento de contenido es un componente reutilizable al que se puede hacer referencia en uno o varios mensajes. Al modificar un fragmento, se actualiza todo el contenido que lo utiliza. Esta funcionalidad se utiliza para la construcción previa de múltiples bloques de contenido personalizado que pueden ser utilizados por los usuarios de marketing para combinar rápidamente los contenidos de correo electrónico en un proceso de diseño mejorado.

Hay dos tipos de fragmentos disponibles:

* **Los fragmentos de expresión** son expresiones predefinidas que están disponibles en una entrada dedicada en el editor de expresiones.
* **Los fragmentos visuales** son bloques visuales predefinidos que se pueden reutilizar en varios envíos de correo electrónico o en plantillas de contenido. [Más información](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >**Los fragmentos visuales** están en disponibilidad limitada (LA). Esta capacidad está restringida a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

### Grupo de reventado {#24-7-2}

Un **grupo de reventado** es una lista de direcciones semilla. Se utiliza para incluir direcciones específicas en los envíos y, a continuación, concentrarse en los perfiles que no coinciden con los criterios objetivo definidos. De este modo, los destinatarios que estén fuera del público del envío pueden recibirlo como lo haría cualquier otro destinatario objetivo. Puede utilizar direcciones semilla al enviar pruebas o para proteger la lista de su campaña de correo. [Más información](../audience/trap-group.md)

### Plantillas de notificaciones push enriquecidas {#24-7-3}

Ahora puede enviar notificaciones push enriquecidas. Las notificaciones push enriquecidas son una forma mejorada de notificación móvil que va más allá de los mensajes de texto simples mediante la incorporación de elementos multimedia como imágenes, botones interactivos u otro contenido con medios enriquecidos. Con esta versión, ya está disponible un conjunto de plantillas para notificaciones push enriquecidas para sus aplicaciones de iOS y Android.

[Más información](../push/rich-push.md)

>[!AVAILABILITY]
>
>Esta capacidad requiere una actualización a la versión 8.6.3 de Campaign<!--or v8.7.2-->. Obtenga más información en las [Notas de la versión](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/releases/release-notes){target="_blank"} de la consola del cliente de la versión 8 de Campaign.

### Mejoras {#improvements-24-7}

**Administración de carpetas**: ahora puede administrar permisos y restricciones de las carpetas.

## Notas de la versión de junio {#24-6-release}

**Fecha de lanzamiento**: 18 y 19 de junio de 2024

Las siguientes funciones y mejoras están disponibles para todos los usuarios a partir de la versión de junio.


### Planes y programas {#24-6-4}

Ahora puede crear planes y programas para organizar sus campañas. Al definir una jerarquía de carpetas, puede organizar sus campañas en programas, y sus programas en planes. [Más información](../administration/plans-programs.md)

### Mejoras {#improvements-24-6}

* **Reconciliación en la actividad de enriquecimiento**: la actividad de **enriquecimiento** se puede utilizar ahora para reconciliar los datos del esquema de la base de datos de Campaign con los datos de otro esquema o con los datos procedentes de un esquema temporal como, por ejemplo, los datos cargados mediante una actividad Cargar archivo. Por ejemplo, puede utilizar esta opción para reconciliar el país de un perfil, especificado en un archivo cargado, con uno de los países disponibles en la tabla dedicada de la base de datos de Campaign. [Más información](../workflows/activities/enrichment.md)


### Nueva función en disponibilidad limitada {#acs-24-6}

>[!AVAILABILITY]
>
>Las siguiente funcionalidad está en disponibilidad limitada (LA). Está restringida a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

* **Alertas de envío**

La función de alertas de envío es un sistema de administración de alertas que permite a un grupo de usuarios recibir automáticamente notificaciones que contienen información sobre la ejecución de sus envíos. [Más información](../msg/delivery-alerting.md)


## Notas de la versión de mayo {#24-5-release}

**Fecha de lanzamiento**: 21 de mayo de 2024

Las siguientes funciones y mejoras están disponibles para todos los usuarios a partir de la versión de mayo.

### Pista de auditoría  {#24-5-1}

La nueva función **Pista de auditoría** proporciona un registro detallado y cronológico de todas las acciones y eventos que se han realizado en su instancia de Adobe Campaign en tiempo real. Ofrece un método cómodo para rastrear todos los cambios en los datos de Campaign, abordando consultas como: el estado de los flujos de trabajo, las personas más recientes para modificarlos o las actividades realizadas por los usuarios dentro de la instancia. [Más información](../reporting/audit-trail.md)

### Campos personalizados {#24-5-2}

**Campos personalizados** son atributos adicionales añadidos a los esquemas predeterminados a través de la consola de Adobe Campaign. En la interfaz de usuario web de Campaign, estos campos personalizados ahora están visibles en varias pantallas, por ejemplo, los detalles de un perfil o un perfil de prueba. En la interfaz de usuario web, no se pueden crear campos personalizados, pero ahora se puede modificar la forma en que se muestran. [Más información](../administration/schemas-custom-fields.md)

### Creación de vínculos entre tablas {#24-5-3}

Ahora puede crear vínculos con otra tabla en la actividad de flujo de trabajo **Enriquecimiento**. Utilice la nueva sección **Definición de vínculo** en los parámetros de la actividad para crear un vínculo entre los datos de la tabla de trabajo y la base de datos de Adobe Campaign. Por ejemplo, si carga datos de un archivo que contiene el número de cuenta, el país y el correo electrónico de los destinatarios, ahora puede crear un vínculo hacia la tabla del país para actualizar esta información en sus perfiles. [Más información](../workflows/activities/enrichment.md#create-links)

### Mejoras generales {#improvements-24-5}

* **Correo directo**: ahora puede aprovechar el editor de expresiones para seleccionar los atributos que se mostrarán en los archivos de extracción de correo directo. [Más información](../direct-mail/content-direct-mail.md)

* **Administración de carpetas**: ahora puede crear una subcarpeta de un tipo diferente a la carpeta principal. [Más información](../get-started/permissions.md#folders)

* **Globalización**: como parte de nuestro esfuerzo continuo por ofrecer una experiencia de usuario unificada, armonizamos la terminología empleada en los productos y las aplicaciones de Adobe Experience Cloud. Esto afecta al término alemán “Titel”, que se ha cambiado a “Label” cuando está relacionado con el nombre de un objeto. Los cambios se implementarán progresivamente en la interfaz de usuario y en la documentación.


## Notas de la versión de abril {#april-24-4-release}

**Fecha de lanzamiento**: 2 de mayo de 2024

### Nuevas funciones {#new-24-4}

Las siguientes funciones están disponibles para todos los usuarios a partir de la versión de abril.

**Nuevas actividades de flujo de trabajo**

* **Actualización de datos**: utilice esta actividad para realizar actualizaciones masivas de los campos de la base de datos. Varias opciones permiten personalizar la actualización de los datos. [Más información](../workflows/activities/update-data.md)
* **Servicios de suscripción**: utilice esta actividad para suscribir o cancelar la suscripción de varios perfiles a un servicio o de un servicio en una sola acción. [Más información](../workflows/activities/subscription-services.md)
* **Extraer archivo**: utilice esta actividad para exportar datos de Adobe Campaign a otro sistema como archivo externo. [Más información](../workflows/activities/extract-file.md)
* **Transferir archivo**: use esta actividad para recibir o enviar archivos, probar la presencia de archivos o mostrar archivos en un servidor. El protocolo utilizado puede ser el protocolo servidor a servidor o el protocolo HTTP. [Más información](../workflows/activities/transfer-file.md)
* **Prueba**: utilice esta actividad para habilitar transiciones basadas en condiciones especificadas. [Más información](../workflows/activities/test.md)
* **Código JavaScript**: utilice esta actividad para ejecutar un fragmento de código JavaScript en el contexto de un flujo de trabajo. [Más información](../workflows/activities/javascript-code.md)
* **Señal externa**: utilice esta actividad para activar la ejecución de un flujo de trabajo desde otro flujo de trabajo o una llamada de API. [Más información](../workflows/activities/external-signal.md)
* **Consulta incremental**: utilice esta actividad para consultar la base de datos de forma programada. Cada vez que se ejecuta esta actividad, se excluyen los resultados de las ejecuciones anteriores. Esto permite segmentar solo elementos nuevos. [Más información](../workflows/activities/incremental-query.md)

**Plantillas de notificaciones push enriquecidas**

Ahora puede enviar notificaciones push enriquecidas a través de Android. Las notificaciones push enriquecidas son una forma mejorada de notificación móvil que va más allá de los simples mensajes de texto al incorporar elementos multimedia como imágenes, botones interactivos u otro contenido con medios enriquecidos. [Más información](../push/rich-push.md)

Tenga en cuenta que esta función se encuentra en **Disponibilidad limitada** (LA).


### Nuevas funciones en disponibilidad limitada {#acs-24-4}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se pueden implementar en ningún otro entorno.
>
>Consulte las siguientes páginas de documentación: [Campaign Standard de la transición a Campaign v8](../rn/acs-migration.md) y [Funciones para usuarios de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es).

* **Promoción de la marca**: como usuario migrado de Campaign Standard, ahora los administradores técnicos pueden definir una o varias marcas para centralizar los parámetros que afectan a la identidad de una marca. Esto incluye el logotipo de la marca, el dominio de la URL de acceso de la página de destino o la configuración del seguimiento de mensajes. Con Adobe Campaign, puede crear estas marcas y vincularlas a mensajes o páginas de destino. Esta configuración se administra en plantillas. [Más información](../administration/branding/branding-gs.md)

* **API de REST**: como usuario migrado de Campaign Standard, puede utilizar las API de REST para crear integraciones para Adobe Campaign y generar su propio ecosistema interconectando Adobe Campaign con el panel de tecnologías que emplea. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=es)

* **Creación de informes dinámicos**: como usuario migrado de Campaign Standard, puede acceder a la Creación de informes dinámicos, que proporciona informes totalmente personalizables y en tiempo real para medir el impacto de sus actividades de marketing. Este añade acceso a los datos de perfil, lo que permite el análisis demográfico por dimensiones de perfil como sexo, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. [Más información](../reporting/dynamic-reporting/get-started-reporting.md)

* **Páginas de destino**: las siguientes mejoras para las páginas de destino solo están disponibles para los usuarios que realizan la transición desde Campaign Standard:

   * Ahora puede hacer referencia a una página de destino de suscripción/baja predeterminada al configurar un servicio. Al diseñar un correo electrónico, si define un vínculo a esa página de destino, los usuarios que envíen el formulario de página de destino se suscriben o cancelan su suscripción automáticamente a este servicio. [Más información](../audience/manage-services.md#create-service)
   * Una nueva opción en la configuración de la página de destino permite a los visitantes anónimos acceder a la página de destino. Si anula la selección de esta opción, solo los usuarios identificados pueden acceder al formulario y enviarlo. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción en la configuración de la página de destino permite almacenar datos internos adicionales cuando se envía la página de destino. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción permite utilizar una página de destino para varios servicios, lo que la hace dinámica. Al añadir un vínculo a un correo electrónico, si selecciona una página de destino dinámica, puede seleccionar cualquier servicio. Si selecciona una página de destino que tiene un servicio específico asociado, este servicio se utilizará automáticamente (no puede seleccionar otro). [Más información](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Ahora se admite contenido condicional en las páginas de destino. [Más información](../landing-pages/lp-content.md)

### Mejoras generales {#improvements-24-4}

Las mejoras siguientes están disponibles para todos los clientes a partir de la versión de abril.

* La actividad **Cargar archivo** se ha mejorado con varias secciones que le permiten cargar un archivo de muestra, administrar errores y rechazos y eliminar archivos cargados después de ejecutar la actividad. [Más información](../workflows/activities/load-file.md)


* Ahora puede **copiar/pegar actividades** de un flujo de trabajo a otro desde una pestaña diferente del explorador. [Más información](../workflows/orchestrate-activities.md#copy-activities-copy)

* Todas las actividades de flujo de trabajo ahora permiten administrar sus **opciones de ejecución**. Esto permite definir el modo de ejecución y el comportamiento de la actividad en caso de errores. [Más información](../workflows/orchestrate-activities.md#execution-options-execution)

* La opción “Do not activate the transition if the population is empty” (No activar la transición si la población está vacía) en **Actividad dividida** le permite elegir si el flujo de trabajo debe pasar a la siguiente actividad cuando el resultado del segmento esté vacío. [Más información](../workflows/activities/split.md)

## Notas de la versión de marzo {#24-3-release}

>[!AVAILABILITY]
>
>Esta versión está disponible para todos los usuarios a partir de la [versión 8.6 de Campaign (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es). Obtenga más información sobre las versiones y actualizaciones de la consola de cliente de Adobe Campaign en la [documentación de la versión 8 de Campaign (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=es){target="_blank"}.

**Fecha de lanzamiento**: 19 y 20 de marzo de 2024

### Canal de correo directo {#24-3-dm}

El canal de **correo directo** ya está disponible para su uso en flujos de trabajo y envíos independientes. El correo directo es un canal sin conexión que le permite crear, personalizar y generar archivos de extracción, así como compartirlos con sus proveedores de correo directo para enviarles correos a sus clientes.

### Nueva actividad de flujo de trabajo Cambiar fuente de datos {#24-3-change-data-source}

La nueva actividad de direccionamiento **Cambiar fuente de datos** permite cambiar la fuente de datos de la tabla de trabajo de su flujo de trabajo. Esta actividad proporciona más flexibilidad al permitirle administrar datos en sus diferentes bases de datos y mejorar los rendimientos.

### Mejora de la actividad de flujo de trabajo División {#24-3-split}

Ahora puede utilizar la opción **Generar todos los subconjuntos de la misma tabla** en la actividad de flujo de trabajo **División** para agrupar todos los subconjuntos en una sola transición de salida.

### Modelador de consultas {#24-3-query-modeler}

* El modelador de consultas ya está disponible para su uso en el Diseñador de correo electrónico. Permite crear condiciones al crear contenido condicional.
* Los valores predefinidos ahora están disponibles para los atributos de tipo fecha al crear una condición personalizada.
* Los operadores ya no se pueden añadir en una nueva transición del diagrama. Solo se pueden añadir en una transición existente antes de filtrar los componentes para agruparlos.