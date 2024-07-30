---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 86214576e08df6596860826bb6511c1f4138c2ad
workflow-type: tm+mt
source-wordcount: '1937'
ht-degree: 97%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

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

Un **grupo de reventado** es una lista de direcciones semilla. Se utiliza para incluir direcciones específicas en los envíos y, a continuación, concentrarse en los perfiles que no coinciden con los criterios objetivo definidos. De este modo, los destinatarios que estén fuera del público del envío pueden recibirlo como lo haría cualquier otro destinatario objetivo. Puede utilizar direcciones semilla al enviar pruebas o para proteger la lista de correo. [Más información](../audience/trap-group.md)

### Plantillas de notificaciones push enriquecidas {#24-7-3}

Ahora puede enviar notificaciones push enriquecidas. Las notificaciones push enriquecidas son una forma mejorada de notificación móvil que va más allá de los mensajes de texto simples mediante la incorporación de elementos multimedia como imágenes, botones interactivos u otro contenido con medios enriquecidos. Con esta versión, ya está disponible un conjunto de plantillas para notificaciones push enriquecidas para sus aplicaciones de iOS y Android.

>[!AVAILABILITY]
>
>Esta capacidad requiere una actualización de Campaign v8.6.3 <!--or v8.7.2-->. Obtenga más información en la consola de cliente de Campaign v8 [notas de la versión](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/releases/release-notes){target="_blank"}.

### Mejoras {#improvements-24-7}

**Administración de carpetas**: ahora puede administrar permisos y restricciones de las carpetas.

## Notas de la versión de junio {#24-6-release}

**Fecha de lanzamiento**: 18 y 19 de junio de 2024

Las siguientes funciones y mejoras están disponibles para todos los usuarios a partir de la versión de junio.

### Alertas de envío {#24-6-3}

La función de alertas de envío es un sistema de administración de alertas que permite a un grupo de usuarios recibir automáticamente notificaciones que contienen información sobre la ejecución de sus envíos. [Más información](../msg/delivery-alerting.md)

### Planes y programas {#24-6-4}

Ahora puede crear planes y programas para organizar sus campañas. Al definir una jerarquía de carpetas, puede organizar sus campañas en programas, y sus programas en planes. [Más información](../administration/plans-programs.md)

### Mejoras {#improvements-24-6}

* **Reconciliación en la actividad de enriquecimiento**: la actividad de **enriquecimiento** se puede utilizar ahora para reconciliar los datos del esquema de la base de datos de Campaign con los datos de otro esquema o con los datos procedentes de un esquema temporal como, por ejemplo, los datos cargados mediante una actividad Cargar archivo. Por ejemplo, puede utilizar esta opción para reconciliar el país de un perfil, especificado en un archivo cargado, con uno de los países disponibles en la tabla dedicada de la base de datos de Campaign. [Más información](../workflows/activities/enrichment.md)

## Notas de la versión de mayo {#24-5-release}

**Fecha de lanzamiento**: 21 de mayo de 2024

Las siguientes funciones y mejoras están disponibles para todos los usuarios a partir de la versión de mayo.

### Pista de auditoría  {#24-5-1}

La nueva función **Pista de auditoría** proporciona un registro detallado y cronológico de todas las acciones y eventos que se han realizado en su instancia de Adobe Campaign en tiempo real. Ofrece un método cómodo para rastrear todos los cambios en los datos de Campaign, abordando consultas como: el estado de los flujos de trabajo, las personas más recientes para modificarlos o las actividades realizadas por los usuarios dentro de la instancia. [Más información](../reporting/audit-trail.md)

### Campos personalizados {#24-5-2}

**Campos personalizados** son atributos adicionales añadidos a los esquemas predeterminados a través de la consola de Adobe Campaign. En la interfaz de usuario web de Campaign, estos campos personalizados ahora están visibles en varias pantallas, por ejemplo, los detalles de un perfil o un perfil de prueba. En la interfaz de usuario web, no se pueden crear campos personalizados, pero ahora se puede modificar la forma en que se muestran. [Más información](../administration/custom-fields.md)

### Creación de vínculos entre tablas {#24-5-3}

Ahora puede crear vínculos con otra tabla en la actividad de flujo de trabajo **Enriquecimiento**. Utilice la nueva sección **Definición de vínculo** en los parámetros de la actividad para crear un vínculo entre los datos de la tabla de trabajo y la base de datos de Adobe Campaign. Por ejemplo, si carga datos de un archivo que contiene el número de cuenta, el país y el correo electrónico de los destinatarios, ahora puede crear un vínculo hacia la tabla del país para actualizar esta información en sus perfiles. [Más información](../workflows/activities/enrichment.md#create-links)

### Mejoras generales {#improvements-24-5}

* **Correo directo**: ahora puede aprovechar el editor de expresiones para seleccionar los atributos que se mostrarán en los archivos de extracción de correo directo. [Más información](../direct-mail/content-direct-mail.md)

* **Administración de carpetas**: ahora puede crear una subcarpeta de un tipo diferente a la carpeta principal. [Más información](../get-started/permissions.md#folders)

* **Globalización**: como parte de nuestro esfuerzo continuo por ofrecer una experiencia de usuario unificada, armonizamos la terminología empleada en los productos y las aplicaciones de Adobe Experience Cloud. Esto afecta al término alemán “Titel”, que se ha cambiado a “Label” cuando está relacionado con el nombre de un objeto. Los cambios se implementarán progresivamente en la interfaz de usuario y en la documentación.


## Notas de la versión de abril {#april-24-4-release}

**Fecha de lanzamiento**: 2 de mayo de 2024

### Nuevas características {#new-24-4}

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

Ahora puede enviar notificaciones push enriquecidas a través de Android. Las notificaciones push enriquecidas son una forma mejorada de notificación móvil que va más allá de los mensajes de texto simples mediante la incorporación de elementos multimedia como imágenes, botones interactivos u otro contenido con medios enriquecidos. [Más información](../push/rich-push.md)

Tenga en cuenta que esta función se encuentra en **Disponibilidad limitada** (LA).


### Nuevas funciones en disponibilidad limitada {#acs-24-4}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se pueden implementar en ningún otro entorno.
>
>Consulte las siguientes páginas de documentación: [Campaign Standard de la transición a Campaign v8](../rn/acs-migration.md) y [Funciones para usuarios de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es).

* **Personalización de marca**: como usuario Campaign Standard migrado, los administradores técnicos ahora pueden definir una o varias marcas para centralizar los parámetros que afectan a la identidad de una marca. Esto incluye el logotipo de la marca, el dominio de la URL de acceso de la página de aterrizaje o la configuración del seguimiento de mensajes. Con Adobe Campaign, puede crear estas marcas y vincularlas a mensajes o páginas de aterrizaje. Esta configuración se administra en plantillas. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=es)

* **API de REST**: como usuario migrado de Campaign Standard, puede utilizar las API de REST para crear integraciones para Adobe Campaign y generar su propio ecosistema interconectando Adobe Campaign con el panel de tecnologías que emplea. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=es)

* **Creación de informes dinámicos**: como usuario migrado de Campaign Standard, puede acceder a la Creación de informes dinámicos, que proporciona informes totalmente personalizables y en tiempo real para medir el impacto de sus actividades de marketing. Añade acceso a los datos del perfil, lo que permite el análisis demográfico por dimensiones de perfil como sexo, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=es)

* **Páginas de aterrizaje**: las siguientes mejoras para las páginas de aterrizaje solo están disponibles para los usuarios que realizan la transición desde Campaign Standard:

   * Ahora puede hacer referencia a una página de aterrizaje de suscripción/baja predeterminada al configurar un servicio. Al diseñar un correo electrónico, si define un vínculo a esa página de aterrizaje, los usuarios que envíen el formulario de página de aterrizaje se suscriben o cancelan su suscripción automáticamente a este servicio. [Más información](../audience/manage-services.md#create-service)
   * Una nueva opción en la configuración de la página de aterrizaje permite a los visitantes anónimos acceder a la página de aterrizaje. Si anula la selección de esta opción, solo los usuarios identificados pueden acceder al formulario y enviarlo. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción en la configuración de la página de aterrizaje permite almacenar datos internos adicionales cuando se envía la página de aterrizaje. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción permite utilizar una página de aterrizaje para varios servicios, lo que la hace dinámica. Al añadir un vínculo a un correo electrónico, si selecciona una página de aterrizaje dinámica, puede seleccionar cualquier servicio. Si selecciona una página de aterrizaje que tiene un servicio específico asociado, este servicio se utilizará automáticamente (no puede seleccionar otro). [Más información](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Ahora se admite contenido condicional en las páginas de aterrizaje. [Más información](../landing-pages/lp-content.md)

### Mejoras generales {#improvements-24-4}

Las mejoras siguientes están disponibles para todos los clientes a partir de la versión de abril.

* La actividad **Cargar archivo** se ha mejorado con varias secciones que le permiten cargar un archivo de muestra, administrar errores y rechazos y eliminar archivos cargados después de ejecutar la actividad. [Más información](../workflows/activities/load-file.md)


* Ahora puede **copiar/pegar actividades** de un flujo de trabajo a otro desde una pestaña diferente del explorador. [Más información](../workflows/orchestrate-activities.md#copy-activities-copy)

* Todas las actividades de flujo de trabajo ahora permiten administrar sus **opciones de ejecución**. Esto permite definir el modo de ejecución y el comportamiento de la actividad en caso de errores. [Más información](../workflows/orchestrate-activities.md#execution-options-execution)

* La opción “Do not activate the transition if the population is empty” (No activar la transición si la población está vacía) en **Actividad dividida** le permite elegir si el flujo de trabajo debe pasar a la siguiente actividad cuando el resultado del segmento esté vacío. [Más información](../workflows/activities/split.md)

## Notas de la versión de marzo {#24-3-release}

>[!AVAILABILITY]
>
>Esta versión está disponible para todos los usuarios a partir de la [versión 8.6 de Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es). Obtenga más información sobre las versiones y actualizaciones de la consola de cliente de Adobe Campaign en la [documentación de la versión 8 de Campaign (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=es){target="_blank"}.

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
