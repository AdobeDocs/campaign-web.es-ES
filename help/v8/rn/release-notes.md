---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# Notas de la versión  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión "
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

Los cambios y las mejoras disponibles con las versiones anteriores se muestran [en esta página](release-notes-24.md).

## Versión de octubre de 2024 {#24-10-release}

**Fecha de publicación**: 29 de octubre de 2024

Las siguientes funciones y mejoras están disponibles a partir de la versión de octubre.

### Funciones

<table>
<thead>
<tr>
<th><strong>Cuentas externas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ahora puede configurar y administrar cuentas externas directamente a través de la interfaz de usuario web de Adobe Campaign. Esta nueva función facilita la configuración de diferentes tipos de cuentas externas, como los correos electrónicos rechazados (POP3) o las instancias de ejecución.</p>
<p>Para obtener más información, consulte la <a href="../administration/external-account.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Mensajería transaccional</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>La mensajería transaccional (Centro de mensajes) ya está disponible en la interfaz de usuario web de Campaign. Este complemento se ha diseñado para activar mensajes que se generan a partir de eventos desencadenados desde los sistemas de información y pueden ser: una factura, una confirmación de pedido, una confirmación de envío, un cambio de contraseña, una notificación de no disponibilidad del producto, el estado de la cuenta, una creación de cuenta en un sitio web, etc.</p>
<p>Para obtener más información, consulte la <a href="../transactional-messaging/transactional.md">documentación detallada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Mejoras

* **Actividades del flujo de trabajo**: ahora puede mover una actividad y todos sus nodos secundarios de una transición a otra dentro de un flujo de trabajo. Hay disponible un botón **Mover** dedicado en el panel de propiedades de la actividad para realizar esto. [Más información](../workflows/orchestrate-activities.md#move)

* **Actividad de enriquecimiento del flujo de trabajo**

   * Ahora puede definir un Alias y una Etiqueta al crear un nuevo campo en la actividad **Enriquecimiento**. [Más información](../workflows/activities/enrichment.md#collection-settings)
   * Ahora puede añadir ofertas para cada perfil en la actividad **Enriquecimiento**. [Más información](../workflows/activities/enrichment.md##add-offers)

* **Distribución de valores**: al acceder a la lista de campos para personalización, ahora puede comprobar cómo se distribuyen los valores para cada campo. Una ventana emergente dedicada muestra el número y el porcentaje de cada valor. [Más información](../query/build-query.md#distribution-values-query)

* **Información de versión y sistema**: ahora puede obtener acceso a los detalles de las versiones de la instancia, tanto para la consola de cliente como para la interfaz de usuario web. En esta nueva sección también se muestran todos los paquetes integrados instalados en el entorno. [Más información](../get-started/user-interface.md#user-interface-about)

* **Listas**: ahora puede reordenar fácilmente los valores de una lista. [Más información](../get-started/work-with-folders.md)

* **Envío**: ahora puede acceder a la variable de envío desde los campos de personalización. [Más información](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)