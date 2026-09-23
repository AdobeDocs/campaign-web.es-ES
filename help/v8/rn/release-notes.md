---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 73553f19c6e88256f0e9f38479bdfc292a3221f8
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 38%
---
# Notas de la versión {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión"
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

## Versión de septiembre de 2026 {#26-9-release}

_22 de septiembre de 2026_

### Nuevas funciones {#26-9-features}

<table>
<thead>
<tr>
<th><strong>Canal LINE</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign ahora es compatible con el canal <strong>LINE</strong>, una popular aplicación de mensajería instantánea. Cree y envíe mensajes de LINE mediante contenido de texto, imagen o vídeo, en envíos independientes o en flujos de trabajo, junto con sus otros canales. <a href="../line/get-started-line.md">Más información</a></p>
</td>
</tr>
</tbody>
</table>

### Mejoras {#26-9-improvements}

* **Acceso de navegación lateral**: Los administradores ahora pueden ocultar entradas de menú específicas de la navegación lateral. [Más información](../administration/schemas-browse-access.md#screen-def)
* **Tipos de aprobación adicionales**: Ahora puede requerir aprobaciones de presupuesto y de inicio de entrega para los envíos de Campaign, además de aprobaciones de contenido y de destino. [Más información](../campaigns/campaign-approvals.md#configure-approvals)
* **Segmentación de SMS basada en visitantes**: La asignación de destino de visitante ya está disponible para los envíos de SMS. [Más información](../sms/create-sms.md)
* **Botón Cancelar del flujo de trabajo**: Un nuevo botón **Cancelar** le permite revertir los cambios no guardados en un flujo de trabajo. [Más información](../workflows/orchestrate-activities.md#save-cancel)
* **Anulación de duplicación con varios valores**: La opción **Siguiendo una lista de valores** ahora admite varios atributos. [Más información](../workflows/activities/deduplication.md#deduplication-configuration)
* **Asignación de destino móvil**: Ahora puede crear asignaciones de destino para destinos de aplicaciones móviles. [Más información](../administration/target-mappings.md#create-mapping)
* **Enriquecimiento de la base de datos externa**: Ahora puede enriquecer datos de una base de datos externa en la actividad **Enrichment** o **Build audience**. [Más información](../workflows/activities/enrichment.md#external-data)
* **Reconciliación de audiencias de archivo**: ahora puede configurar si desea importar destinatarios a la base de datos al segmentar una audiencia desde un archivo. [Más información](../audience/file-audience.md#upload)
* **Uniones directas en colecciones**: Al seleccionar un atributo directamente de una colección, ahora puede elegir cómo se crea la condición: mediante la opción predeterminada recomendada, una función de agregado o una unión directa avanzada. [Más información](../query/build-query.md#links)

