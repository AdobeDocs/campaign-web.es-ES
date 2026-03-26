---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 28%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

## Versión de marzo de 2026 {#26-3-release}

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
<p>La función de creación de esquemas ya está disponible para todos los clientes (GA). Esta capacidad le permite crear y administrar esquemas directamente desde la interfaz de usuario web de Campaign. Puede crear nuevas tablas, ampliar los esquemas existentes y crear formularios personalizados. Puede definir estructuras de datos personalizadas para satisfacer sus necesidades empresariales específicas sin necesidad de acceder a la consola del cliente.</p>
<p>Para obtener más información, consulte la <a href="../administration/schemas.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Temas en el correo electrónico Designer (LA)</strong><br/></th> 
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
<ul><li> <strong>Modelo Adobe</strong> (con tecnología Firefly Image Model 4) para generar imágenes inmediatamente sin necesidad de configuración adicional</li><li> <strong>Modelo de socio</strong> (con tecnología Gemini 2.5 Flash) para funciones especializadas</li><li><strong>Modelos personalizados</strong> (modelos específicos de la marca entrenados en sus propios recursos) para la generación sin marca que se ajuste con precisión a su identidad de marca, estilo y directrices visuales.</li></ul>
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
<p>La actividad de flujo de trabajo <strong>Envío automatizado</strong> ya está disponible en la paleta de flujos de trabajo. Puede utilizarlo para crear o ejecutar acciones de envío (preparar, enviar una prueba, preparar e iniciar, etc.) directamente dentro del flujo de trabajo. Seleccione una entrega existente creada fuera del flujo de trabajo para reutilizarla en cada ejecución o cree una nueva entrega a partir de una plantilla cada vez que se ejecute la actividad.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Para obtener más información, consulte <a href="../workflows/activities/automated-delivery.md">documentación detallada.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Varias ramas de flujo de trabajo y una actividad</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>Ahora se admiten <strong>varias ramas</strong>. En lugar de usar <strong>Fork</strong>, puedes hacer clic en <strong>Agregar rama</strong> en la barra de herramientas. La actividad <strong>AND-join</strong> también se ha mejorado. Ahora es una actividad <strong>Join</strong> genérica que le permite elegir entre las opciones de unión AND y OR.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Para obtener más información, consulte las páginas de documentación de <a href="../workflows/orchestrate-activities.md#toolbar">Organizar actividades</a> y <a href="../workflows/activities/join.md">Unirse</a>.</p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#26-3-improvements}

* La actividad de flujo de trabajo **Start** se ha agregado para mejorar la compatibilidad con la consola del cliente. Esta actividad es opcional y no se inserta de forma predeterminada en los nuevos flujos de trabajo. Sin embargo, se añade automáticamente a los flujos de trabajo existentes.
  [Más información](../workflows/activities/about-activities.md#flow-control)
* El campo de selección de zona horaria de la configuración **Programar** de una entrega se ha movido debajo del campo **Fecha de contacto**. [Más información](../msg/create-deliveries.md#gs-schedule)