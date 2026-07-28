---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d9d1733854bceac52d54e02125dac92b74872c77
workflow-type: tm+mt
source-wordcount: 716
ht-degree: 23%

---

# Notas de la versión {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión"
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

## Versión de julio de 2026 {#26-7-release}

_28 de julio de 2026_

### Nuevas funciones {#26-7-features}

<table>
<thead>
<tr>
<th><strong>Gestión de ofertas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede administrar ofertas de extremo a extremo directamente desde la interfaz de usuario web de Campaign. Configure entornos de oferta y espacios de oferta, cree su catálogo de ofertas y categorías, cree ofertas con reglas de idoneidad y pesos de prioridad, y apruébelas e impleméntelas para usarlas en sus entregas. Las configuraciones avanzadas siguen estando disponibles en la consola del cliente.</p>
<p>Para obtener más información, consulte la <a href="../offers/gs-offer-management.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Configuración de marca</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Los administradores técnicos ahora pueden crear y configurar marcas directamente desde la interfaz de usuario web de Campaign, sin utilizar la consola de cliente. Todas las configuraciones de marca, incluidos los parámetros de identidad, subdominio y protocolos, parámetros de encabezado de correo electrónico y parámetros de seguimiento de URL, ya están disponibles en la interfaz de usuario web.</p>
<p>Para obtener más información, consulte la <a href="../administration/branding/branding-configure.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Recursos públicos en el Designer de correo electrónico</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Al agregar imágenes a tus correos electrónicos, ahora puedes seleccionar <strong>recursos públicos</strong>. Esto le permite elegir una imagen ya disponible en la instancia de Adobe Campaign, como un archivo previamente importado en el Designer de correo electrónico o un recurso público cargado desde la consola del cliente.</p>
<p>Para obtener más información, consulte la <a href="../email/content-components.md#image">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Actividad del flujo de trabajo Carga de datos (RDBMS)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La actividad <strong>Data loading (RDBMS)</strong> ya está disponible en la interfaz de usuario web de Campaign. Utilice esta actividad para cargar datos directamente desde una base de datos relacional externa en el flujo de trabajo. Los datos extraídos están disponibles en todo el flujo de trabajo y se pueden utilizar para el direccionamiento, el enriquecimiento o el procesamiento posterior de datos.</p>
<p>Para obtener más información, consulte la <a href="../workflows/activities/data-loading-rdbms.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Páginas dinámicas de JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Las páginas dinámicas de JavaScript (JSSP) le permiten crear páginas del lado del servidor que generan contenido dinámico cuando se accede a ellas a través de una dirección URL, como API personalizadas, exportaciones o lógica de aplicación web. Ahora puede crear, modificar, duplicar y eliminar estas páginas directamente desde la interfaz de usuario web de Campaign.</p>
<p>Para obtener más información, consulte la <a href="../administration/dynamic-javascript-pages.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#26-7-improvements}

* Se han realizado las siguientes mejoras en la **configuración de esquema personalizada**:
  * La nueva sección **Datos de acción** le permite restringir las acciones disponibles en los registros de un esquema personalizado, independientemente de las reglas de seguridad configuradas en carpetas individuales. [Más información](../administration/schemas-action-data.md)
  * Se han agregado **filtros personalizados** en la sección **Configuración de lista de inventario**. Permiten elegir qué atributos se muestran como campos de acceso rápido en el panel de filtros de la vista de lista. [Más información](../administration/schemas-custom-filters.md)

* Se han realizado las siguientes mejoras en **flujos de trabajo**:
  * La eliminación de una actividad de flujo de trabajo ahora es más flexible: cuando la actividad tiene actividades posteriores, puede elegir eliminarlas todas, eliminar solo la actividad seleccionada o eliminarla mientras mantiene sus actividades posteriores en una nueva rama. [Más información](../workflows/orchestrate-activities.md#delete-activity)
  * Ahora puede desconectar una transición entre dos actividades de flujo de trabajo sin eliminar ninguna de ellas. Esto permite reorganizar un diagrama de flujo de trabajo, por ejemplo, para dejar temporalmente a un lado un grupo de actividades que desee conservar, sin tener que eliminarlas y volver a crearlas. [Más información](../workflows/orchestrate-activities.md#disconnect-transition)
  * Ahora se muestran barras de desplazamiento horizontales y verticales alrededor del lienzo del flujo de trabajo, lo que permite desplazarse por flujos de trabajo grandes arrastrando directamente al área que desea ver. [Más información](../workflows/orchestrate-activities.md)
  * Al guardar o iniciar o reiniciar un flujo de trabajo, ahora se muestra una advertencia si otro usuario ha modificado el flujo de trabajo en la interfaz de usuario web o en la consola del cliente desde que lo abrió. Puede optar por anular los demás cambios con el suyo, volver a cargar el flujo de trabajo para obtener la versión más reciente o cancelar.

* **Dirección de correo electrónico del remitente**: Ahora puede restringir el campo **De correo electrónico** de las entregas a una lista predefinida de direcciones, mediante la opción **NmsDelivery_senderAddressMask**. [Más información](../administration/options.md#restrict-sender-address)
* Se han mejorado **mensajes de error de inicio de sesión**: cuando falla un intento de inicio de sesión, la interfaz de usuario web muestra ahora un mensaje de error más específico para varios escenarios (por ejemplo, cuando el usuario no tiene asignada ninguna zona de seguridad o su dirección IP está restringida).
