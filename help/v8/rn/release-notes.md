---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 36d2b7a67ef087d628151199a223ceee54f84180
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 31%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

Los cambios y mejoras disponibles con las versiones anteriores se listan en las páginas de [2024](release-notes-24.md) y [2025](release-notes-25.md).

## Versión de enero de 2026 {#26-1-release}

_27 de enero de 2026_

### Nuevas funciones {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Funciones de envío multilingües (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La función Entrega multilingüe ya está disponible para todos los clientes (GA). Esta función le permite enviar varios mensajes en diferentes idiomas en la interfaz de usuario web de Adobe Campaign. Puede elegir el idioma predeterminado de la entrega, así como los diferentes idiomas en los que se puede realizar la entrega. También puede obtener una vista previa de estos envíos en los idiomas que haya elegido.  
<p>Para obtener más información, consulte la <a href="../msg/multilingual.md">documentación detallada</a>.</p>
<p>Se han realizado las siguientes mejoras en las notificaciones push multilingües:</p>
<ul>
<li>Ahora puede rellenar rápidamente todas las variantes de idioma cargando un archivo CSV que contenga su contenido multilingüe. <a href="../msg/multilingual.md#csv-upload">Más información</a>
</li>
<li>Ahora se admiten notificaciones push enriquecidas.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Enriquecimiento de perfil en mensajes transaccionales (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El enriquecimiento de perfil en la capacidad de mensajes transaccionales ya está disponible para todos los clientes (GA). Además de los correos electrónicos, ahora también se admiten notificaciones push y SMS. Esta función le permite personalizar mensajes transaccionales vinculando campos de base de datos de Adobe Campaign al contenido del mensaje. Puede seleccionar asignaciones de destinatario, columnas de enriquecimiento y una clave de reconciliación para garantizar una personalización precisa y en tiempo real mientras mantiene los umbrales de rendimiento.</p>
<p>Para obtener más información, consulte la <a href="../transactional-messaging/profile-enrichment.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager Live y copias de idioma</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La integración de contenido de Adobe Experience Manager le permite acceder a todos los idiomas y Live Copies creados en Adobe Experience Manager directamente en Campaign al crear envíos. Puede actualizar el contenido en tiempo real para recuperar las últimas versiones de Adobe Experience Manager. Esta integración elimina la sincronización manual de contenido entre Adobe Experience Manager y Campaign, lo que optimiza el flujo de trabajo de la campaña en varios idiomas.</p>
<p>Para obtener más información, consulte la <a href="../integrations/aem-multilingual.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Experimentos de contenido: pruebas A/B</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Los experimentos de contenido en la web de Adobe Campaign le permiten definir varias variantes de envío de pruebas A/B para medir cuál ofrece el mejor rendimiento para la audiencia de destino. Puede variar el contenido, el asunto o el remitente de la entrega para probar diferentes versiones y determinar qué variante produce los mejores resultados. Puede realizar pruebas A/B en varios elementos de correo electrónico, como la línea de asunto, el nombre del remitente y el contenido del cuerpo del correo electrónico.</p>
<p>Para obtener más información, consulte la <a href="../email/ab-testing.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Actividad de envío continuo</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La actividad Continuous delivery permite agregar nuevos destinatarios a una entrega existente. Este tipo de entrega evita tener que crear una nueva cada vez, lo que lo hace más eficiente para alertas de bajo volumen o notificaciones enviadas según sea necesario. Un envío continuo crea una sola instancia de envío. Todos los registros de envío (broadLog) y los registros de seguimiento hacen referencia a este envío, lo que simplifica la monitorización y la creación de informes.</p>
<p>Para obtener más información, consulte la <a href="../workflows/activities/continuous-delivery.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Administración de aprobación de campañas</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El proceso de aprobación ayuda a coordinar varias partes interesadas y garantiza el control de calidad antes de realizar las entregas. Utilice aprobaciones cuando su organización requiera que equipos diferentes lo validen, como administradores de marketing que revisan contenido o analistas de datos que validan audiencias de destino.</p>
<p>Para obtener más información, consulte la <a href="../campaigns/campaign-approvals.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#26-1-improvements}

* Los informes dinámicos ahora admiten notificaciones push y SMS. [Más información](../reporting/dynamic-reporting/get-started-reporting.md)
* Filtros predefinidos: una nueva opción &quot;Filtro compartido&quot; permite poner un filtro predefinido a disposición de otros usuarios de la organización. [Más información](../get-started/predefined-filters.md#share-filter)
* Los campos de personalización creados en Adobe Experience Manager, como Nombre, Correo electrónico, Fecha y Dirección, ahora se incluyen y están disponibles al utilizar la plantilla de contenido.
* La evaluación de la calidad del contenido ahora comprueba los problemas de legibilidad, coherencia y eficacia independientemente de las directrices de marca, identificando mensajes poco claros, tono incoherente o lagunas estructurales. [Más información](../content/brands-score.md)
