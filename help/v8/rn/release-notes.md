---
title: Últimas notas de la versión
description: Descubra la nueva función que se incluye con la interfaz de usuario web de Campaign
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 8%

---

# Notas de la versión  {#latest-release}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Novedades"
>abstract="Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de entrega continua que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Las notas de la versión se actualizan varias veces al mes. **Ya está activa la versión de marzo**, incluido el canal de correo postal, la nueva actividad de flujo de trabajo Cambiar fuente de datos y otras mejoras."


<!--Last update: **March 19, 2024**-->

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de entrega continua que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Por favor, compruébelos regularmente.

>[!AVAILABILITY]
>
>Esta versión está disponible para todos los usuarios a partir de [Versión v8.6 de Campaign (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es). Obtenga más información acerca de las versiones y actualizaciones de la consola del cliente de Adobe Campaign en [Documentación de Campaign v8 (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=es){target="_blank"}.

## Notas de la versión de marzo {#24-3-release}

**Fecha de lanzamiento**: 19 y 20 de marzo de 2024

### Canal de correo directo {#24-3-dm}

**Correo directo** El canal ya está disponible para su uso en flujos de trabajo y como envíos independientes. El correo postal es un canal sin conexión que le permite crear, personalizar y generar archivos de extracción, así como compartirlo con sus proveedores de correo postal para enviar correo a sus clientes. [Más información](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Nueva actividad de flujo de trabajo Cambiar fuente de datos {#24-3-change-data-source}

El **Cambiar fuente de datos** la actividad de segmentación le permite cambiar la fuente de datos utilizada por la tabla de trabajo del flujo de trabajo. Esta actividad proporciona más flexibilidad al permitirle administrar datos en sus diferentes bases de datos y mejorar el rendimiento. [Más información](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Mejora de actividad de flujo de trabajo dividido {#24-3-split}

Ahora puede utilizar la variable **Generar todos los subconjuntos de la misma tabla** en la opción **Split** actividad de flujo de trabajo para agrupar todos los subconjuntos en una sola transición de salida. [Más información](../workflows/activities/split.md)

### Modelador de consultas {#24-3-query-modeler}

* El modelador de consultas ya está disponible para su uso en el Diseñador de correo electrónico. Permite crear condiciones al crear contenido condicional. [Más información](../personalization/conditions.md)
* Los valores predefinidos ahora están disponibles para atributos de tipo fecha al crear una condición personalizada. [Más información](../query/build-query.md)
* Los operadores ya no se pueden añadir en una nueva transición del diagrama. Solo se pueden añadir en una transición existente antes de filtrar los componentes para agruparlos. [Más información](../query/build-query.md)
