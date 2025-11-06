---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ca1a437f8a8a25c0a15b9148e9c73271795f16c7
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 64%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

Los cambios y mejoras disponibles con las versiones anteriores se listan en las páginas de [2024](release-notes-24.md) y [2025](release-notes-25.md).

## Versión de octubre de 2025 {#25-10-updates}

_3 de noviembre de 2025_

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

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

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

<table>
<thead>
<tr>
<th><strong>Integración con Adobe GenStudio</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Para mejorar la eficacia del marketing y mantener la coherencia de la marca, ahora puede integrar sin problemas las experiencias de GenStudio for Performance Marketing con Campaign. Esto le permite aprovechar la creación de contenido con potencia IA de GenStudio junto con las funcionalidades de orquestación avanzadas de Campaign.<p>
<p>Para obtener más información, consulte la <a href="../integrations/genstudio.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Compatibilidad con el modo oscuro en el Diseñador de correo electrónico</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Email Designer ahora permite cambiar a la vista de modo oscuro, donde también puede definir ajustes personalizados específicos. Tenga en cuenta que la renderización final depende del cliente de correo electrónico del destinatario y no todos los clientes de correo electrónico admiten el modo oscuro.</p>
<p>Para obtener más información, consulte la <a href="../email/dark-mode.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### Mejoras {#25-10-improvements}

* En las entregas creadas en la consola del cliente, la sección **Audience** ahora indica si se ha definido una condición dinámica para los destinos de prueba. <!-- [Learn more](../msg/gs-deliveries.md#access)-->

* Ahora puede cambiar entre el generador de reglas nuevo y el heredado al configurar una condición mediante la capacidad de contenido condicional de Email Designer. <!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* Ahora puede seleccionar vínculos de recopilación, como compras, en la definición de pantalla del esquema Recipients. Esto muestra los datos relacionados en las pantallas de perfil a través de una pestaña dedicada. <!-- [Learn more](../administration/schemas.md#collection-lists)-->

* Como administrador de Campaign, ahora puede configurar conexiones a Salesforce CRM y Microsoft Dynamics.
  [Más información](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

