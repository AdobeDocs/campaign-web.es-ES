---
title: Últimas notas de la versión
description: Descubra la nueva función que se incluye con la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ba187eaebf299e5d2ee303c4e15180d35a9e6180
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 25%

---

# Notas de la versión  {#latest-release}

<!--Last update: **March 19, 2024**-->

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

## Notas de la versión de abril {#april-24-4-release}

**Fecha de lanzamiento**: 30 de abril de 2024

### Nuevas características {#new-24-4}

Las siguientes funciones están disponibles para todos los usuarios a partir de la versión de abril.

**Nuevas actividades de flujo de trabajo**

* **Actualización de datos** : Utilice esta actividad para realizar actualizaciones masivas de los campos de la base de datos. Varias opciones permiten personalizar la actualización de datos. [Más información](../workflows/activities/update-data.md)
* **Servicios de suscripción** : Utilice esta actividad para suscribirse o cancelar la suscripción de varios perfiles a un servicio o de un servicio en una sola acción. [Más información](../workflows/activities/subscription-services.md)
* **Extraer archivo** : utilice esta actividad para exportar datos de Adobe Campaign a otro sistema como archivo externo. [Más información](../workflows/activities/extract-file.md)
* **Transferir archivo** : utilice esta actividad para recibir o enviar archivos, probar la presencia de archivos o mostrar archivos en un servidor. El protocolo utilizado puede ser el protocolo servidor a servidor o el protocolo HTTP. [Más información](../workflows/activities/transfer-file.md)
* **Prueba** : Utilice esta actividad para habilitar transiciones basadas en condiciones especificadas. [Más información](../workflows/activities/test.md)
* **Código JavaScript** : Utilice esta actividad para ejecutar un fragmento de código JavaScript en el contexto de un flujo de trabajo. [Más información](../workflows/activities/javascript-code.md)
* **Señal externa** : Utilice esta actividad para almacenar en déclencheur la ejecución de un flujo de trabajo desde otro flujo de trabajo* o una llamada de API. [Más información](../workflows/activities/external-signal.md)
* **Consulta incremental** : Utilice esta actividad para consultar la base de datos de forma programada. Cada vez que se ejecuta esta actividad, se excluyen los resultados de las ejecuciones anteriores. Esto le permite dirigirse únicamente a elementos nuevos. [Más información](../workflows/activities/incremental-query.md)

**Plantillas de notificaciones push enriquecidas**

Ahora puede enviar notificaciones push enriquecidas a través de Android. Las notificaciones push enriquecidas son una forma mejorada de notificación móvil que va más allá de los mensajes de texto simples mediante la incorporación de elementos multimedia como imágenes, botones interactivos u otro contenido multimedia enriquecido. [Más información](../push/rich-push.md)

Tenga en cuenta que esta función se encuentra en **Disponibilidad limitada** (LA).

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### Nuevas funciones en disponibilidad limitada {#acs-24-4}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se pueden implementar en ningún otro entorno.
>
>Consulte las siguientes páginas de documentación: [Campaign Standard de la transición a Campaign v8](../rn/acs-migration.md) y [Funciones para usuarios de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Marca** - Como usuario Campaign Standard migrado, los administradores técnicos ahora pueden definir una o varias marcas para centralizar los parámetros que afectan a la identidad de una marca. Esto incluye el logotipo de la marca, el dominio de la URL de acceso de la página de aterrizaje o la configuración del seguimiento de mensajes. Puede crear estas marcas y vincularlas a mensajes o páginas de aterrizaje. Esta configuración se administra en plantillas. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **API de REST** : Como usuario Campaign Standard migrado, puede utilizar las API de REST para crear integraciones para Adobe Campaign y construir su propio ecosistema al interconectar Adobe Campaign con el panel de tecnologías que utiliza. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Informes dinámicos** : Como usuario Campaign Standard migrado, puede acceder a la Creación de informes dinámicos, que proporciona informes totalmente personalizables y en tiempo real para medir el impacto de sus actividades de marketing. Añade acceso a los datos de perfil, lo que permite el análisis demográfico por dimensiones de perfil como sexo, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Mejora de la actividad del archivo de carga** - El **Cargar archivo** la actividad se ha mejorado con varias secciones que le permiten cargar un archivo de muestra, administrar errores y rechazos y eliminar archivos cargados después de ejecutar la actividad. [Más información](../workflows/activities/load-file.md)

* **Páginas de aterrizaje** - Las siguientes mejoras para las páginas de aterrizaje solo están disponibles para los usuarios que realizan la transición desde Campaign Standard:

   * Ahora puede hacer referencia a una página de aterrizaje de suscripción/baja predeterminada al configurar un servicio. Al diseñar un correo electrónico, si define un vínculo a esa página de aterrizaje, los usuarios que envíen el formulario de página de aterrizaje se suscriben o cancelan su suscripción automáticamente a este servicio. [Más información](../audience/manage-services.md#create-service)
   * Una nueva opción en la configuración de la página de aterrizaje permite a los visitantes anónimos acceder a la página de aterrizaje. Si anula la selección de esta opción, solo los usuarios identificados pueden acceder al formulario y enviarlo. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción en la configuración de la página de aterrizaje permite almacenar datos internos adicionales cuando se envía la página de aterrizaje. [Más información](../landing-pages/create-lp.md#create-landing-page)
   * Una nueva opción permite utilizar una página de aterrizaje para varios servicios, lo que la hace dinámica. Al añadir un vínculo a un correo electrónico, si selecciona una página de aterrizaje dinámica, puede seleccionar cualquier servicio. Si selecciona una página de aterrizaje que tiene un servicio específico asociado, este servicio se utilizará automáticamente (no puede seleccionar otro). [Más información](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Ahora se admite contenido condicional en las páginas de aterrizaje. [Más información](../landing-pages/lp-content.md)

### Mejoras generales {#improvements-24-4}

Las mejoras siguientes están disponibles para todos los clientes a partir de la versión de abril.
<!--**Workflow - Copy/Paste into another tab**: -->

* Ahora puede copiar/pegar actividades de un flujo de trabajo en otro flujo de trabajo desde una pestaña diferente del explorador. [Más información](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Todas las actividades de flujo de trabajo ahora permiten administrar sus opciones de ejecución. Esto permite definir el modo de ejecución y el comportamiento de la actividad en caso de errores. [Más información](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* La opción &quot;Do not activate the transition if the population is empty&quot; en **Actividad dividida** le permite elegir si el flujo de trabajo debe pasar a la siguiente actividad cuando el resultado del segmento esté vacío. [Más información](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* Los campos personalizados son atributos adicionales añadidos a los esquemas predeterminados a través de la consola de Adobe Campaign. En la interfaz de usuario web de Campaign, estos campos personalizados ahora están visibles en varias pantallas, por ejemplo, los detalles de un perfil o un perfil de prueba. En la interfaz de usuario web, no se pueden crear campos personalizados, pero ahora se puede modificar la forma en que se muestran. [Más información](../administration/custom-fields.md)


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

Ahora puede utilizar la variable **Generar todos los subconjuntos de la misma tabla** en la opción **Split** actividad de flujo de trabajo para agrupar todos los subconjuntos en una sola transición de salida.

### Modelador de consultas {#24-3-query-modeler}

* El modelador de consultas ya está disponible para su uso en el Diseñador de correo electrónico. Permite crear condiciones al crear contenido condicional.
* Los valores predefinidos ahora están disponibles para atributos de tipo fecha al crear una condición personalizada.
* Los operadores ya no se pueden añadir en una nueva transición del diagrama. Solo se pueden añadir en una transición existente antes de filtrar los componentes para agruparlos.
