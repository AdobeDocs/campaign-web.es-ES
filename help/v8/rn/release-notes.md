---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 100%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

Los cambios y mejoras disponibles con las versiones anteriores se listan en las páginas de [2024](release-notes-24.md) y [2025](release-notes-25.md).

## Actualizaciones del 25 de octubre {#25-9-updates}

_9 de octubre de 2025_

<table>
<thead>
<tr>
<th><strong>Funciones multilingües para la mensajería transaccional, notificaciones push y SMS (LA-Disponibilidad limitada)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede enviar varios mensajes transaccionales, notificaciones push y mensajes SMS en diferentes idiomas en la interfaz de usuario web de Adobe Campaign. La función Envío multilingüe le permite elegir el idioma predeterminado de su entrega, así como los diferentes idiomas en los que se puede realizar el envío. También puede obtener una vista previa de estos envíos en los idiomas que haya elegido. </p>
<p>Nota: esta funcionalidad solo está disponible para un conjunto de organizaciones (disponibilidad limitada) y se implementará globalmente en una versión futura.</p>
<p>Para obtener más información, consulte la <a href="../msg/multilingual.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Enriquecimiento del perfil en mensajes transaccionales (LA-Disponibilidad limitada)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Esta funcionalidad le permite personalizar mensajes transaccionales vinculando campos de base de datos de Adobe Campaign al contenido del mensaje. Puede seleccionar asignaciones de destinatario, columnas de enriquecimiento y una clave de reconciliación para garantizar una personalización precisa y en tiempo real mientras mantiene los umbrales de rendimiento.</p>
<p>Nota: Esta funcionalidad solo está disponible para un conjunto de organizaciones (disponibilidad limitada) y se implementará a nivel global en una versión futura. Esta función solo está disponible actualmente en los correos electrónicos.</p>
<p>Para obtener más información, consulte la <a href="../transactional-messaging/profile-enrichment.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>


## Versión de septiembre de 2025 {#25-9-release}

_23 de septiembre de 2025_

Las siguientes funciones están disponibles a partir de la versión de septiembre.

<table>
<thead>
<tr>
<th><strong>Canal personalizado para envíos de API</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora, directamente desde la interfaz de usuario de Adobe Campaign web, puede organizar y ejecutar envíos basados en canales de API personalizados. Estos envíos pueden ser independientes o formar parte de un flujo de trabajo. La configuración del canal de API personalizado se realiza en la consola.</p>
<p>Para obtener más información, consulte la <a href="../call-center/gs-custom-channel.md">documentación detallada</a>.</p>
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
<p>Como administrador de Campaign, ahora puede configurar nuevas conexiones con sistemas externos desde la interfaz de usuario web de Campaign. También puede ver, actualizar y administrar cuentas externas existentes.</p>
<p>Para obtener más información, consulte la <a href="../administration/create-external-account.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Bloqueo de contenido de correo electrónico</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora Campaign le permite bloquear contenido en las plantillas de correo electrónico, ya sea bloqueando toda la plantilla o estructuras y componentes específicos. Esto le permite evitar ediciones o eliminaciones no intencionadas, lo que le proporciona un mayor control sobre la personalización de las plantillas y mejora la eficacia y fiabilidad de sus campañas de correo electrónico.</p>
<p>Para obtener más información, consulte la <a href="../content/content-locking.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### Mejoras {#25-9-improvements}

* Se ha añadido un conjunto de operadores nuevos al configurar una condición mediante la capacidad de contenido condicional del diseñador de correo electrónico.
* La dimensión de filtrado ya está disponible en la actividad de flujo de trabajo **Generar público**. Para verla o cambiarla, haga clic en el icono situado junto a la dimensión de segmentación. [Más información](../workflows/activities/build-audience.md#build-audience-configuration).
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

