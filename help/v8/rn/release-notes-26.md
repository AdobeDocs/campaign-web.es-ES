---
title: Notas de la versión anterior de la interfaz de usuario web de Campaign v8
description: Notas de la versión de la interfaz de usuario web de Campaign 2026
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 4eae8f0ea3c176a12e040f7406aac699e14a5ba8
workflow-type: ht
source-wordcount: '1204'
ht-degree: 100%

---

# Notas de la versión 2026 {#2026-release}

Esta página enumera todos los cambios y mejoras disponibles en las **versiones de 2026**. Las notas de la versión más recientes están disponibles en [esta página](release-notes.md).

## Versión de abril de 2026 {#26-4-release}

_29 de abril de 2026_

### Mejora {#26-4-improvement}

La sección **Datos de enriquecimiento** ya está disponible en la actividad de flujo de trabajo **Generar público** (tipo de consulta). Puede ver, añadir, editar y quitar **datos adicionales** directamente desde la interfaz de usuario web de Campaign. Al igual que en la actividad **Enriquecimiento**, puede añadir atributos de enriquecimiento únicos, vínculos de colección y expresiones.

[Más información](../workflows/activities/build-audience.md)

## Versión de marzo de 2026 {#26-3-release}

_24 de marzo_ de 2026_

### Nuevas funciones {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Creación de esquemas (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La función de creación de esquemas ya está disponible para todos los clientes (GA). Esta capacidad le permite crear y administrar esquemas directamente desde la interfaz de usuario web de Campaign. Puede crear nuevas tablas, ampliar los esquemas existentes y crear formularios personalizados. Puede definir estructuras de datos personalizados para satisfacer sus necesidades empresariales específicas sin necesidad de acceder a la consola del cliente.</p>
<p>Para obtener más información, consulte la <a href="../administration/schemas.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Temas en el Diseñador de correo electrónico (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Los temas proporcionan una experiencia de creación mejorada para los correos electrónicos, ya que le permiten definir estilos de temas reutilizables que se ajusten a las directrices de su marca. Ahora puede utilizar variables de temáticas en fragmentos, lo que garantiza un estilo coherente en todas las plantillas de correo electrónico. Esta función le permite crear correos electrónicos más rápido con módulos predefinidos que abstraen elementos de contenido como títulos, descripciones, imágenes y vínculos, a la vez que mantienen la coherencia de la marca.</p>
<p>Nota: esta funcionalidad solo está disponible para un conjunto de organizaciones (disponibilidad limitada) y se implementará globalmente en una versión futura.</p>
<p>Para obtener más información, consulte la <a href="../email/apply-email-themes.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integración de modelos de Firefly personalizados y modelos de generación de imágenes de terceros</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Permita la integración total de modelos de Firefly estándar y personalizados, junto con modelos de imagen de terceros aprobados, para proporcionar mayor flexibilidad, control y alineación de marca al generar imágenes.</p>
<p>Elija el modelo adecuado para sus necesidades:</p>
<ul><li> <strong>Modelo de Adobe</strong> (con tecnología Firefly Image Model 4) para generar imágenes inmediatamente sin necesidad de configuración adicional</li><li> <strong>Modelo de partner</strong> (con tecnología Gemini 2.5 Flash) para funciones especializadas</li><li><strong>Modelos personalizados</strong> (modelos específicos de la marca entrenados en sus propios recursos) para la generación coherente con la marca que se ajuste con precisión a la identidad, estilo y directrices visuales de la marca.</li></ul>
<p>Para obtener más información, consulte la <a href="../content/generative-models.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Actividad de envío automatizado</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La actividad de flujo de trabajo de <strong>Envío automatizado</strong> ya está disponible en la paleta de flujos de trabajo. Puede utilizarlo para crear o ejecutar acciones de envío (preparar, enviar una prueba, preparar e iniciar, etc.) directamente en el flujo de trabajo. Seleccione un envío existente creado fuera del flujo de trabajo para reutilizarlo en cada ejecución o cree un nuevo envío a partir de una plantilla cada vez que se ejecute la actividad.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Para obtener más información, consulte la <a href="../workflows/activities/automated-delivery.md">documentación detallada.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Varias ramas de flujo de trabajo y Unirse a la actividad</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>Ahora se admiten <strong>varias ramas</strong>. En lugar de usar una <strong>Fork</strong>, puede hacer clic en <strong>Add branch</strong> en la barra de herramientas. La actividad <strong>AND-join</strong> también se ha mejorado. Ahora es una actividad <strong>Join</strong> genérica que le permite elegir entre las opciones de unión AND y OR.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Para obtener más información, consulte las páginas de documentación de <a href="../workflows/orchestrate-activities.md#toolbar">Orquestar actividades</a> y <a href="../workflows/activities/join.md">Unir</a>.</p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#26-3-improvements}

* La actividad **Iniciar** flujo de trabajo se ha añadido para mejorar la compatibilidad con la consola del cliente. Esta actividad es opcional y no se inserta de forma predeterminada en los flujos de trabajo nuevos. Sin embargo, se añade automáticamente a los flujos de trabajo existentes.
  [Más información](../workflows/activities/about-activities.md#flow-control)
* El campo de selección de zona horaria de la configuración **Programar** de un envío se ha movido debajo del campo **Fecha de contacto**. [Más información](../msg/create-deliveries.md#gs-schedule)

## Versión de febrero de 2026 {#26-2-release}

_17 de febrero de 2026_

### Nuevas funciones {#26-2-features}

<!--
table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<!--
table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table
-->

<table>
<thead>
<tr>
<th><strong>Vista de cronología en el inventario de campañas</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El inventario de campañas ahora incluye una vista de Cronología que le permite visualizar y administrar las campañas a lo largo del tiempo: cambie entre una lista y una cronología, navegue por semana, mes o día, utilice el botón Hoy para ir a la fecha actual y abra los detalles de la campaña (estado, flujos de trabajo, envíos) en un panel derecho, con los mismos filtros y búsquedas que la vista de lista.</p>
<p>Para obtener más información, consulte la <a href="../campaigns/manage-campaigns.md#timeline">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Creación de esquemas (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear y administrar esquemas directamente desde la interfaz de usuario web de Campaign. Esta función le permite crear nuevas tablas, ampliar esquemas existentes y crear formularios personalizados. Puede definir estructuras de datos personalizados para satisfacer sus necesidades empresariales específicas sin necesidad de acceder a la consola del cliente.</p>
<p>Nota: esta funcionalidad solo está disponible para un conjunto de organizaciones (disponibilidad limitada) y se implementará globalmente en una versión futura.</p>
<p>Para obtener más información, consulte la <a href="../administration/schemas.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

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
<p>La función Envío multilingüe ya está disponible para todos los clientes (disponibilidad general). Esta función permite enviar varios mensajes en diferentes idiomas desde la interfaz de usuario web de Adobe Campaign. Puede elegir el idioma predeterminado de su envío, así como los diferentes idiomas en los que se puede realizar el envío. También puede obtener una vista previa de estos envíos en los idiomas que haya elegido. 
<p>Para obtener más información, consulte la <a href="../msg/multilingual.md">documentación detallada</a>.</p>
<p>Se han realizado las siguientes mejoras en las notificaciones push multilingües:</p>
<ul>
<li>Ahora puede rellenar rápidamente todas las variantes de idioma cargando un archivo CSV con su contenido multilingüe. <a href="../msg/multilingual.md#csv-upload">Leer más</a>
</li>
<li>Ahora se admiten notificaciones push enriquecidas.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Enriquecimiento del perfil en mensajes transaccionales (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>El enriquecimiento de perfil en la capacidad de mensajes transaccionales ya está disponible para todos los clientes (GA). Además de los correos electrónicos, ahora también se admiten notificaciones push y SMS. Esta funcionalidad le permite personalizar mensajes transaccionales vinculando campos de base de datos de Adobe Campaign al contenido del mensaje. Puede seleccionar asignaciones de destinatario, columnas de enriquecimiento y una clave de reconciliación para garantizar una personalización precisa y en tiempo real mientras mantiene los umbrales de rendimiento.</p>
<p>Para obtener más información, consulte la <a href="../transactional-messaging/profile-enrichment.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Copias en tiempo real y de idioma de Adobe Experience Manager</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La integración de contenido de Adobe Experience Manager le permite acceder a todas las copias de idiomas y en tiempo real creadas en Adobe Experience Manager directamente en Campaign al crear envíos. Puede actualizar el contenido en tiempo real para recuperar las últimas versiones de Adobe Experience Manager. Esta integración elimina la sincronización manual de contenido entre Adobe Experience Manager y Campaign, lo que optimiza el flujo de trabajo de la campaña en varios idiomas.</p>
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
<p>Los experimentos de contenido en la web de Adobe Campaign le permiten definir varias variantes de envío de pruebas A/B para medir cuál ofrece el mejor rendimiento para el público destinatario. Puede modificar el contenido, el asunto o el remitente del correo para probar diferentes versiones y determinar cuál de ellas ofrece los mejores resultados. Puede realizar pruebas A/B en varios elementos de correo electrónico, como la línea de asunto, el nombre del remitente y el contenido del cuerpo del correo electrónico.</p>
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
<p>La función de envío continuo le permite añadir nuevos destinatarios a un envío ya existente. Este tipo de envío evita tener que crear uno nuevo cada vez, lo que resulta más eficaz para las alertas de bajo volumen o las notificaciones enviadas cuando es necesario. Un envío continuo crea una sola instancia de envío. Todos los registros de envío (broadLog) y los registros de seguimiento hacen referencia a este envío, lo que simplifica la monitorización y la creación de informes.</p>
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
<p>El proceso de aprobación ayuda a coordinar varias partes interesadas y garantiza el control de calidad antes de realizar los envíos. Utilice aprobaciones cuando su organización requiera que equipos diferentes lo validen, como administradores de marketing que revisan contenido o analistas de datos que validan públicos destinatarios.</p>
<p>Para obtener más información, consulte la <a href="../campaigns/campaign-approvals.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#26-1-improvements}

* Los informes dinámicos ahora admiten notificaciones push y SMS. [Más información](../reporting/dynamic-reporting/get-started-reporting.md)
* Filtros predefinidos: una nueva opción “Filtro compartido” permite poner un filtro predefinido a disposición de otros usuarios de la organización. [Más información](../get-started/predefined-filters.md#share-filter)
* Los campos de personalización creados en Adobe Experience Manager, como Nombre, Correo electrónico, Fecha y Dirección, ahora se incluyen y están disponibles al utilizar la plantilla de contenido.
* La evaluación de la calidad del contenido ahora comprueba los problemas de legibilidad, coherencia y eficacia independientemente de las directrices de marca, identificando mensajes poco claros, tono incoherente o lagunas estructurales. [Más información](../content/brands-score.md)
