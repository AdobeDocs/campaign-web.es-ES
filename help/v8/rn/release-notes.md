---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 56%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Adobe Campaign versiones de interfaz de usuario Web funcionan con un modelo de envío continuo, que permite un enfoque escalable y por fases para el implementación de características. En consecuencia, estos Notas de la versión se actualizan varias veces al mes. Revíselos regularmente.

En este Página](release-notes-24.md) se enumeran [los cambios y mejoras disponibles en versiones anteriores.

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
<p>Ahora puede crear tipologías y reglas de tipología en la interfaz de usuario de Adobe Campaign Web. Las tipologías controlan, filtran y priorizan el envío de envíos. Las tipologías validan que los envíos siempre contengan componentes obligatorios (como un vincular de baja o una línea de asunto) o reglas de filtrado para excluir grupos de su audiencia (gustar no suscriptores, competidores o clientes que no sean fidelizados).</p>
<img src="assets/do-not-localize/typology.gif" alt="Ilustración de creación de reglas de tipología en Adobe Campaign interfaz Web de Usuario">
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
<p>Ahora puede crear asignaciones de público destinatario en la interfaz de usuario de Campaign Web. Las asignaciones de público destinatario definen cómo los distintos canales de envío (correo electrónico, SMS o notificaciones push) se vinculan a los campos de datos de un esquema. El asignación de destino define los audiencia objetivo: perfiles, beneficiarios de contratos, operadores, suscriptores, prospectos y otros.</p>
<img src="assets/do-not-localize/target-mapping.gif" alt="Ilustración de destino creación de asignaciones en Adobe Campaign interfaz Web de Usuario">
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
<p>Ahora puede acceder a los detalles de un esquema seleccionando su nombre en la lista. Ahora se puede acceder a la edición de campos personalizados desde los <b>campos</b> personalizados Editar botón disponibles en los detalles de esquema.</p>
<img src="assets/do-not-localize/schemas.gif" alt="Ilustración de detalles de esquema y edición de campos personalizados en Adobe Campaign interfaz web del usuario">
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
<p>Los fragmentos visuales son bloques visuales predefinidos que se pueden reutilizar en varias entregas correo electrónico o en plantillas contenido. Esta función ya está disponible para todos los clientes que ejecuten la versión 8.6.4 o superior del servidor.</p>
<img src="assets/do-not-localize/visual-fragment.gif" alt="Ilustración de creación y uso de fragmentos visuales en Adobe Campaign interfaz Web de Usuario">
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
<img src="assets/do-not-localize/external-delivery.gif" alt="Ilustración de configuración de envío externo en Adobe Campaign interfaz Web del usuario">
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
<p>Ahora puede crear enumeraciones directamente mediante la interfaz de usuario de Adobe Campaign Web. Una enumeración es una lista de valores sugeridos por el sistema para rellenar los campos. Utilice enumeraciones para estandarizar los valores de estos campos, ayudar con la entrada de datos o utilizarlos dentro de las consultas.</p>
<img src="assets/do-not-localize/enumerations.gif" alt="Ilustración de administración de lista desglosada en Adobe Campaign interfaz Web de Usuario">
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
<img src="assets/do-not-localize/options.gif" alt="Ilustración de creación de opciones personalizadas en Adobe Campaign interfaz Web de Usuario">
<p>Para obtener más información, consulte la <a href="../administration/options.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Definir y llamar a códigos JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear códigos JavaScript en la interfaz de usuario de Adobe Campaign Web. Esto le permite crear funciones reutilizables que se pueden utilizar en toda flujos de trabajo, de forma similar a un biblioteca.</p>
<img src="assets/do-not-localize/javascript.gif" alt="Ilustración de creación de código de JavaScript en Adobe Campaign interfaz web del usuario">
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
<img src="assets/do-not-localize/ai-lp.gif" alt="Ilustración de uso de AI Assistant para la generación de página de aterrizaje en Adobe Campaign interfaz de usuario web">
<p>Para obtener más información sobre el Asistente de IA, consulte la <a href="../email/generative-lp.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#25-1-improvements}

* Personalice la visualización de los campos personalizados en la interfaz:
   * Seleccione campos personalizados adicionales para mostrar en la interfaz.
   * Defina reglas para mostrar campos personalizados de tipo vincular, como restringir lista valores en función de la entrada de otro campo.
   * Organice los campos en la interfaz de manera más flexible: los campos pueden abarcar una sola columna o agruparse en subsecciones para una mejor organización.
   * Definir campos específicos como de solo lectura.

* Recientes y Favoritos filtros: añadir atributos utilizados frecuentemente en Favoritos para un acceso rápido. Además de favoritos, vista y utilice los atributos seleccionados más recientemente.

* Cuentas externas: el nuevo tipo de **[!UICONTROL Enrutamiento]** está disponible para su selección al crear una nueva cuenta externa. Le permite configurar una cuenta externa específica para utilizarla en los envíos externos. [Más información](../administration/external-account.md#routing).