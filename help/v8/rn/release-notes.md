---
title: Últimas notas de la versión
description: Descubra la nueva función que se incluye con la interfaz de usuario web de Campaign
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 5%

---

# Notas de la versión  {#latest-release}

<!--Last update: **March 19, 2024**-->

Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de entrega continua que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Por favor, compruébelos regularmente.

>[!AVAILABILITY]
>
>Esta versión está disponible para todos los usuarios a partir de [Versión v8.6 de Campaign (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=es). Obtenga más información acerca de las versiones y actualizaciones de la consola del cliente de Adobe Campaign en [Documentación de Campaign v8 (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=es){target="_blank"}.

## Versión de marzo {#24-3-release}

**Fecha de lanzamiento**: 19 y 20 de marzo de 2024

### Canal de correo directo {#24-3-dm}

**Correo directo** El canal ya está disponible para su uso en flujos de trabajo y como envíos independientes. El correo postal es un canal sin conexión que le permite crear, personalizar y generar archivos de extracción, así como compartirlo con sus proveedores de correo postal para enviar correo a sus clientes.

![](../assets/do-not-localize/direct-mail.gif)

### Nueva actividad de flujo de trabajo Cambiar fuente de datos {#24-3-change-data-source}

El **Cambiar fuente de datos** la actividad de segmentación le permite cambiar la fuente de datos utilizada por la tabla de trabajo del flujo de trabajo. Esta actividad proporciona más flexibilidad al permitirle administrar datos en sus diferentes bases de datos y mejorar el rendimiento.

![](../assets/do-not-localize/change-data-source.gif)

### Mejora de actividad de flujo de trabajo dividido {#24-3-split}

Ahora puede utilizar la variable **Generar todos los subconjuntos de la misma tabla** en la opción **Split** actividad de flujo de trabajo para agrupar todos los subconjuntos en una sola transición de salida.

### Modelador de consultas {#24-3-query-modeler}

* El modelador de consultas ya está disponible para su uso en el Diseñador de correo electrónico. Permite crear condiciones al crear contenido condicional.
* Los valores predefinidos ahora están disponibles para atributos de tipo fecha al crear una condición personalizada.
* Los operadores ya no se pueden añadir en una nueva transición del diagrama. Solo se pueden añadir en una transición existente antes de filtrar los componentes para agruparlos.
