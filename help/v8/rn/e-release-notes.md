---
title: Notas de la versión preliminar de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la próxima versión de la interfaz de usuario web de Campaign
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 965681fabb7696f745f4f958e2961197395c30bb
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 28%

---

# Notas de la versión preliminar {#e-release}

La interfaz de usuario web de Adobe Campaign ofrece continuamente nuevas funciones, mejoras de las funciones existentes y correcciones de errores. Todos los cambios se consolidan al final de cada mes en las [notas de la versión](release-notes.md).

**Las notas de la versión preliminar que se indican a continuación están sujetas a cambios sin previo aviso hasta la fecha de disponibilidad final de la versión**. Los vínculos, las pantallas y la documentación actualizada se publican en las [notas de la versión](release-notes.md), en la fecha de lanzamiento.

## Versión de enero de 2025 {#25-1-release}

**Fecha de la versión**: 5 de febrero de 2025

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
<p>Para obtener más información, consulte la <a href="../content/use-visual-fragments.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Uso de un sistema de terceros para realizar envíos</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede definir envíos externos y plantillas de envío externo en la interfaz de usuario web de Campaign. Con este modo, los mensajes se generan en un archivo de entrada que se puede compartir con el proveedor externo. El modo Envío externo es el predeterminado para el canal de correo directo.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Control y filtrado de los envíos con tipologías</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede crear tipologías y reglas de tipología en la interfaz de usuario web de Adobe Campaign. Una tipología es una colección de reglas de tipología que le permiten controlar, filtrar y priorizar la entrega de envíos. Las tipologías validan que las entregas siempre contienen los elementos necesarios (como un vínculo de baja o una línea de asunto) o reglas de filtrado para excluir grupos de los destinatarios deseados (como suscriptores que se han dado de baja, competidores o clientes que no sean fieles).</p>
<img src="assets/do-not-localize/typology.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>Ahora puede crear enumeraciones directamente mediante la interfaz de usuario web de Adobe Campaign. Una enumeración es una lista de valores sugeridos por el sistema para rellenar campos. Utilice enumeraciones para estandarizar los valores de estos campos, ayudar con la entrada de datos o utilizar en las consultas.</p>
<img src="assets/do-not-localize/enumerations.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>Ahora puede acceder a las opciones técnicas de la interfaz de usuario web de Adobe Campaign y crear sus propias opciones personalizadas para adaptarlas a sus necesidades. Esto resulta particularmente útil cuando se trabaja con actividades de flujo de trabajo de código JavaScript para almacenar datos intermedios.</p>
<img src="assets/do-not-localize/options.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>Ahora puede crear códigos JavaScript en la interfaz de usuario web de Adobe Campaign. Esto le permite crear funciones reutilizables que se pueden utilizar en distintos flujos de trabajo, de forma similar a una biblioteca.</p>
<img src="assets/do-not-localize/javascript.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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

* Filtros recientes y favoritos: para reutilizar rápidamente atributos que se utilizan con frecuencia, ahora puede agregarlos a Favoritos. Esto garantiza que sean fácilmente accesibles para tareas futuras. Además de los favoritos, también puede ver y utilizar los atributos seleccionados más recientemente.


