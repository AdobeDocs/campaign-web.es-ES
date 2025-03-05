---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: ht
source-wordcount: '770'
ht-degree: 100%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

Los cambios y las mejoras disponibles con las versiones anteriores se muestran [en esta página](release-notes-24.md).

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