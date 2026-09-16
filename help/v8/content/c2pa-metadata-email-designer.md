---
audience: end-user
product: campaign
title: Metadatos de C2PA en el diseñador de correo electrónico y de páginas de destino
description: Descubra qué sucede con los metadatos de C2PA ya adjuntos a una imagen a medida que se mueve a través del correo electrónico y el diseñador de páginas de aterrizaje en la interfaz de usuario web de Adobe Campaign.
topic: Content Management
role: User
level: Beginner
source-git-commit: 645352d9e2ba12d5430ddf1b62852077344c3016
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 4%
---

# Metadatos de C2PA en el diseñador de correo electrónico y de páginas de destino {#c2pa-email-landing-page-designer}

>[!BEGINSHADEBOX]

**En esta página:** Descubra qué sucede con los metadatos de C2PA ya adjuntos a una imagen a medida que se mueve a través del correo electrónico y el diseñador de la página de aterrizaje en la interfaz de usuario web de Adobe Campaign.

>[!ENDSHADEBOX]

>[!INFO]
>
>Están surgiendo nuevas leyes en torno a la transparencia generativa de la IA, y Adobe está trabajando para cumplir con los requisitos aplicables en todas las jurisdicciones. Los metadatos de C2PA son la herramienta de procedencia que utiliza Adobe para cumplir los requisitos de estas leyes.

El diseñador de correo electrónico y páginas de aterrizaje no genera ni edita imágenes por sí mismo. Hace referencia a imágenes que ya se generaron o editaron con IA generativa en otra herramienta de Adobe, como Generate Content, Adobe Express o Firefly, o en un modelo de socio. Los metadatos de C2PA ya adjuntos a esas imágenes se conservan y no se modifican a medida que crea, publica y envía.

## Los metadatos de C2PA se conservan a medida que crea y envía {#c2pa-preserved}

La siguiente tabla resume lo que sucede con los metadatos de C2PA en cada paso de creación y envío de contenido con el diseñador de correo electrónico y la página de aterrizaje.

| Acción | ¿Qué sucede? | ¿Se conservan los metadatos de C2PA? | Ejemplo |
| --- | --- | --- | --- |
| **Insertar una imagen en una plantilla** | El diseñador agrega una referencia a una imagen ya generada o editada con IA generativa en cualquier otra parte, como Generar contenido, Adobe Express, Firefly o un modelo de socio. El archivo de imagen en sí no cambia. | Sí, sin cambios | Se inserta un banner generado por Firefly en una plantilla de correo electrónico. |
| **Cambiar el tamaño, cambiar la posición o agregar texto alternativo** | Mostrar solo las propiedades en el cambio de HTML de la plantilla. El archivo de imagen no se vuelve a codificar. | Sí, sin cambios | Se cambia el tamaño de una imagen para adaptarla a un diseño móvil y al texto alternativo especificado. |
| **Publicar** | El correo electrónico o la página de aterrizaje se publican y la imagen se almacena para su envío. | Sí, sin cambios | Se publica una campaña y sus imágenes se almacenan para su envío. |
| **Enviar un correo electrónico o ver una página de aterrizaje** | La imagen se envía a la bandeja de entrada del destinatario o se muestra en la página activa. | Sí, sin cambios | Un destinatario abre el correo electrónico y descarga la imagen; las credenciales siguen coincidiendo con el original. |

## Tipos de contenido y su ámbito {#c2pa-content-types}

* **Imágenes**: Cubiertas. Los metadatos de C2PA ya adjuntos a una imagen se conservan a medida que se insertan, ajustan, publican y entregan, como se muestra arriba.
* **Vídeo, audio, texto**: No aplicable. El diseñador de correo electrónico y páginas de aterrizaje no genera ni edita estos tipos de contenido con IA generativa.

## Qué sucede a medida que se mueve el contenido {#c2pa-content-moves}

Los metadatos de C2PA viajan con la imagen a través del correo electrónico y el diseñador de la página de aterrizaje en la interfaz de usuario web de Adobe Campaign, desde el editor hasta el almacenamiento y la bandeja de entrada del destinatario o la página en directo. En ninguno de estos pasos se crea, cambia ni elimina ninguna credencial.

Si una imagen no lleva metadatos de C2PA de IA generativa, ya que no se generó ni editó con IA generativa, no aparecerá ninguna credencial en ella aquí. Eso es esperable, no un error.

## Comprobación de credenciales {#c2pa-checking-credential}

Todavía no hay una forma de inspeccionar una Content Credential directamente dentro del diseñador de correo electrónico o de la página de aterrizaje.

## Recursos adicionales

* [Trabajar con Generar contenido](generative-gs.md)
* [Transparencia de contenido de IA generativa](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/overview/content-transparency)