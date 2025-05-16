---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: b730eeeaab5bfc87e8c9c10b6e25bed0e484fb64
workflow-type: ht
source-wordcount: '737'
ht-degree: 100%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

Los cambios y mejoras disponibles con las versiones anteriores se recogen en las versiones de [2024](release-notes-24.md) y [2025](release-notes-25.md).

## Actualizaciones de mayo de 2025 {#25-5-release}

<table>
<thead>
<tr>
<th><strong>Puntuación de alineación con la marca (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La función de puntuación de alineación con la marca proporciona comentarios claros directamente en el diseñador de correo electrónico, lo que le ayuda a ver si el contenido se ajusta al tono, el estilo y las directrices de la marca. Esta función está disponible en Beta.</p>
<p>Para obtener más información, consulte la <a href="../content/brands-score.md">documentación detallada</a>.</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

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

