---
title: Notas de la versión anterior de la interfaz de usuario web de Campaign v8
description: Versiones de la interfaz de usuario web de Campaign de 2025
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 8ec342d565bc8418c202cdba834d74a99cff3a47
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 98%

---

# Notas de la versión de 2025 {#2025-release}

Esta página enumera todos los cambios y mejoras disponibles con las **versiones de 2025**. Las notas de la versión más recientes están disponibles en [esta página](release-notes.md).

## Versión de abril de 2025 {#25-4-release}

**Fecha de lanzamiento**: 29 de abril de 2025

### Nuevas características {#25-4-features}

Las siguientes funciones están disponibles para todos los usuarios a partir de la versión de abril.

<table>
<thead>
<tr>
<th><strong>Canal de centro de llamadas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El canal del centro de llamadas ahora está disponible en la interfaz de usuario de Campaign Web. Este canal se refiere a un método de comunicación utilizado para administrar y rastrear comunicaciones o interacciones que se gestionan a través de un centro de llamadas, generalmente llamadas telefónicas realizadas por agentes a clientes o clientes potenciales.</p>
<p>Nota: Los informes no están disponibles en la interfaz de usuario web para el canal del centro de llamadas. Debe navegar a la consola del cliente para acceder a los informes.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Para obtener más información, consulte la <a href="../call-center/gs-call-center.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Nuevo generador de reglas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora hay disponible un nuevo generador de reglas para definir condiciones complejas en una interfaz de usuario mejorada. Puede cambiar del generador de reglas antiguo al nuevo según sea necesario.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Para obtener más información, consulte la <a href="../query/query-modeler-overview.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Creación de cuentas externas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Como administrador de Campaign, ahora puede configurar nuevas conexiones con sistemas externos desde la interfaz de usuario de Campaign Web.
También puede ver, actualizar y administrar cuentas externas existentes.</p>
<p>Para obtener más información, consulte la <a href="../administration/external-account.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#25-4-improvements}

**Mejoras generales en la interfaz**

* Las opciones Descripción del campo, Añadir a favoritos y Distribución de valores para los atributos del esquema ahora son más visibles en la interfaz de usuario. Para obtener más información, consulte la [documentación detallada](../get-started/attributes.md).
* En la interfaz, la fecha y la hora ahora se muestran según el idioma principal establecido en las preferencias de Experience League. Esta mejora solo está disponible para varios idiomas. Para ver la lista completa de idiomas admitidos, consulte la [documentación detallada](https://experienceleague.adobe.com/es/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Editor de correo electrónico**: para mejorar la accesibilidad en la interfaz de usuario de Campaign Web, hay dos campos nuevos disponibles en el Diseñador de correo electrónico. Estos se corresponden con el elemento `title` y el atributo lang en el elemento `html` del contenido del correo electrónico. Puede definir esta configuración además del campo preencabezado, en la sección cuerpo del correo electrónico. Para obtener más información, consulte la [documentación detallada](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Esquemas**

* Ahora puede editar el esquema temporal de una lista desde la interfaz de usuario de Campaign Web. Para obtener más información, consulte la [documentación detallada](../audience/manage-audience.md).
* Ahora puede obtener una vista previa de los campos personalizados de un esquema en una pantalla de ejemplo. Para obtener más información, consulte la [documentación detallada](../administration/custom-fields.md#add).
* Ahora puede mover campos personalizados a la lista arrastrando y soltando. Para obtener más información, consulte la [documentación detallada](../administration/custom-fields.md#add).


### Nuevas funciones en disponibilidad limitada {#25-4-features-la}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se pueden implementar en ningún otro entorno. Estos requieren actualizar el servidor de Campaign a la versión 8.7.4.
>
>Consulte las siguientes páginas de documentación: [transición de Campaign Standard a la versión 8 de Campaign](../rn/acs-migration.md) y las [Funciones para usuarios de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es).

* **Creación de envíos multilingües**: ahora puede mandar varios envíos de correo electrónico en diferentes idiomas en la interfaz de usuario de Adobe Campaign Web. La función Envío multilingüe le permite elegir el idioma predeterminado de su entrega, así como los diferentes idiomas en los que se puede realizar el envío. También puede previsualizar estos envíos en los idiomas que haya elegido. Para obtener más información, consulte la [documentación detallada](../email/edit-content.md).

* **Informes dinámicos para envíos multilingües**: ahora los informes dinámicos están disponibles para los envíos de correo electrónico multilingües. Para obtener más información, consulte la [documentación detallada](../reporting/global-reports.md).

* **Compatibilidad con la API REST de SMS (LA)**: la API REST de mensajería transaccional ya está disponible para el canal de SMS. Cuando el correo electrónico como el teléfono móvil están presentes en la carga útil, puede utilizar el campo &quot;wishedChannel&quot; para especificar el canal. Si no se proporciona, el correo electrónico se utilizará de forma predeterminada a menos que wishedChannel solicite explícitamente un SMS. Para obtener más información, consulte la [documentación detallada](https://experienceleague.adobe.com/es/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

## Versión de febrero de 2025 {#25-2-release}

**Fecha de lanzamiento**: 18 de febrero de 2025

Las siguientes funciones y mejoras están disponibles a partir de la versión de febrero.

### Funciones {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Creación de reglas empresariales (reglas de tipología)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear tipologías y reglas de tipología en la interfaz de usuario de Adobe Campaign Web. Las tipologías permiten controlar, filtrar y priorizar la entrega de envíos. Le permiten asegurarse de que los envíos siempre contengan componentes obligatorios (como un vínculo de cancelación de suscripción o una línea de asunto) o reglas de filtrado para excluir grupos de su público (como suscriptores que han cancelado la suscripción, competidores o clientes que no sean fieles).</p>
<img src="assets/do-not-localize/typology.gif">
<p>Para obtener más información, consulte la <a href="../administration/typologies.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Asignaciones de público destinatario</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear asignaciones de público destinatario en la interfaz de usuario de Campaign Web. Las asignaciones de público destinatario definen cómo los distintos canales de envío (correo electrónico, SMS o notificaciones push) se vinculan a los campos de datos de un esquema. La asignación de público destinatario permite definir el público: perfiles, beneficiarios de contratos, operadores, suscriptores, clientes potenciales, etc.</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>Para obtener más información, consulte la <a href="../administration/target-mappings.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Detalles del esquema</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede acceder a los detalles de un esquema seleccionando su nombre en la lista. Ahora se puede acceder a la edición de campos personalizados desde el botón <b>Editar campos personalizados</b> disponible en los detalles del esquema.</p>
<img src="assets/do-not-localize/schemas.gif">
<p>Para obtener más información, consulte la <a href="../administration/schemas.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

## Versión de enero de 2025 {#25-1-release}

**Fecha de lanzamiento**: 5 de febrero de 2025

Las siguientes funciones y mejoras están disponibles a partir de la versión de enero.

### Funciones {#25-1-features}


<table>
<thead>
<tr>
<th><strong>Crear y utilizar fragmentos visuales</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Los fragmentos visuales son bloques visuales predefinidos que se pueden reutilizar en varios envíos de correo electrónico o en plantillas de contenido. Esta función ya está disponible para todos los clientes que ejecuten la versión 8.6.4 o superior del servidor.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>Para obtener más información, consulte la <a href="../content/use-visual-fragments.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Uso de un sistema de terceros para remitir envíos</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede definir envíos externos y plantillas de envío externo en la interfaz de Campaign Web. En este modo, los mensajes se compilan en un archivo de salida que se puede compartir con su proveedor externo. De forma predeterminada, el modo de envío externo es el que se utiliza para el canal de correo directo.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>Para obtener más información, consulte la <a href="../msg/send-external-deliveries.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Administrar las enumeraciones</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear enumeraciones directamente mediante la interfaz de usuario de Adobe Campaign Web. Una enumeración es una lista de valores sugeridos por el sistema para rellenar los campos. Utilice las enumeraciones para estandarizar los valores de estos campos, facilitar la introducción de datos o utilizarlas en las consultas.</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>Para obtener más información, consulte la <a href="../administration/enumerations.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Crear opciones personalizadas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede acceder a las opciones técnicas de la interfaz de usuario de Adobe Campaign Web y crear sus propias opciones personalizadas para adaptarlas a sus necesidades. Esto resulta particularmente útil cuando se trabaja con actividades de flujo de trabajo de código JavaScript para almacenar datos intermedios.</p>
<img src="assets/do-not-localize/options.gif">
<p>Para obtener más información, consulte la <a href="../administration/options.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Definir y llamar códigos JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear códigos JavaScript en la interfaz de usuario de Adobe Campaign Web. Esto le permite crear funciones reutilizables que se pueden utilizar en distintos flujos de trabajo, de forma similar a una biblioteca.</p>
<img src="assets/do-not-localize/javascript.gif">
<p>Para obtener más información, consulte la <a href="../administration/javascript-codes.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Generación de la página de aterrizaje con el Asistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El Asistente de IA ya está disponible con los envíos de la página de aterrizaje, lo que le permite generar texto, imágenes o diseños de página completos.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>Para obtener más información sobre el Asistente de IA, consulte la <a href="../email/generative-lp.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>


### Mejoras {#25-1-improvements}

* Personalice la visualización de los campos personalizados en la interfaz:

   * Ahora puede seleccionar campos personalizados adicionales para mostrarlos en la interfaz
   * Ahora puede establecer reglas para mostrar campos personalizados de tipo vínculo, como restringir valores de lista basados en la entrada de otro campo
   * Ahora puede organizar los campos en la interfaz con más flexibilidad: los campos pueden abarcar una sola columna o agruparse en subsecciones para una mejor organización
   * Ahora puede establecer campos específicos como de solo lectura

* Filtros recientes y favoritos: para reutilizar rápidamente atributos que se utilizan con frecuencia, ahora puede añadirlos a favoritos. Esto garantiza que sean fácilmente accesibles para tareas futuras. Además de los favoritos, también puede ver y utilizar los atributos seleccionados más recientemente.

* Cuentas externas: el nuevo tipo de **[!UICONTROL Enrutamiento]** está disponible para su selección al crear una nueva cuenta externa. Le permite configurar una cuenta externa específica para utilizarla en los envíos externos. [Más información](../administration/external-account.md#routing)
