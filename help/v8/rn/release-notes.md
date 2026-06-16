---
title: Notas de la versión de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la última versión de la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 6581a2d6ab44b711ed6aea6736d60f932a7ce315
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 45%

---

# Notas de la versión {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de la versión"
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, las notas de la versión de Campaign se actualizan varias veces al mes, con las últimas funciones, mejoras y correcciones. Le recomendamos que las revise regularmente."

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.

## Versión de junio de 2026 {#26-6-release}

_16 de junio de 2026_

### Mejoras {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* Ahora puede exportar datos desde cualquier pantalla de lista, incluidos los registros de seguimiento. Busque la lista y simplemente haga clic en el botón exportar. La exportación incluye las filas cargadas actualmente y tiene en cuenta las columnas mostradas en pantalla y cualquier búsqueda o filtro activo. [Más información](../get-started/list-filters.md)

* Las actividades de flujo de trabajo **Deduplication** y **End** ahora admiten varias transiciones entrantes. Cuándo
hay más de una transición entrante disponible, use la sección **Conjuntos para unirse** en la actividad
propiedades para seleccionar qué transiciones conectar. Obtenga más información en estas páginas: [Anulación de duplicación](../workflows/activities/deduplication.md),

<!--
[End](../workflows/activities/end.md)
-->

* Los parámetros avanzados ahora se exponen en la sección **Enrichment data** de las actividades de flujo de trabajo **Build audience** (query type) y **Enrichment**. Estos parámetros le permiten ajustar con precisión cómo se generan los datos de enriquecimiento, lo que incluye la agrupación, la deduplicación, la administración de claves principales y los datos de eventos entrantes. [Más información](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
