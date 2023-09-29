---
audience: end-user
title: Introducción al Ayudante de contenido
description: Introducción al Ayudante de contenido
badge: label="Alfa"
source-git-commit: 2b499b854110cd317b47b9a7d3884467869624f1
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---


# Introducción al Ayudante de contenido {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Ayudante de contenido"
>abstract="Una vez que haya creado y personalizado su envío, puede utilizar el Ayudante de contenido para mejorar el contenido. Esta función simplifica el proceso de personalización y mejora de contenido, ya que le permite ajustar el contenido al describir lo que desea generar."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definir contexto para la generación de contenido"
>abstract="Para utilizar el contenido seleccionado como entrada para la generación de contenido, active la variable **Mejorar con contenido actual** alternar. También puede cargar los recursos de su marca para utilizarlos como fuente. Si no utiliza el contenido seleccionado, es obligatorio cargar y seleccionar recursos de una marca."

El asistente de contenido, con tecnología de IA generativa, es una herramienta valiosa para mejorar el contenido del correo electrónico. Simplifica la personalización y la mejora de contenido, optimizando las entregas de correo electrónico para que resuenen mejor en la audiencia.

Esta función ahorra tiempo y garantiza una calidad coherente al generar automáticamente contenido de correo electrónico completo. Al utilizar la IA generativa, puede crear correos electrónicos atractivos sin esfuerzo, lo que mejora la eficacia y la eficiencia de su comunicación.

<!--
You can the Campaign Content Assistant in your emails to: [generate images](generative-image.md), [generate text content](generative-content.md), [generate the full HTML content](generative-email.md).-->

>[!NOTE]
>
>Esta funcionalidad está disponible en su versión de Alpha y sujeta a cambios sin previo aviso. Se activará a principios de octubre.

## Mecanismos de protección y limitaciones {#generative-guardrails}

A continuación, se enumeran las directrices generales para utilizar el Asistente de contenido para la generación de correo electrónico:

* La calidad del contenido generado se ve fuertemente influida por el objetivo de marketing que defina. Utilice un indicador bien definido para el modelo GenAI para interpretar con precisión. 
* Cargue el recurso de la marca para tener información precisa sobre el contenido de la marca. De lo contrario, el contenido se basa en información disponible públicamente. El contenido cargado puede ser: archivos de PDF, documentos de Microsoft Word, JPEG, PNG o archivos ZIP (con formatos de archivo compatibles).
* El tamaño recomendado para el recurso de marca cargado es inferior a 10 MB. Los archivos más grandes o muchas imágenes pueden funcionar, pero el tiempo de procesamiento aumenta.
* Utilice plantillas de correo electrónico creadas por Adobe Campaign o, preferiblemente, [plantillas de correo electrónico integradas](../content/email-sample-templates.md) para crear el contenido del correo electrónico. Se recomienda una plantilla de correo electrónico con hasta 8-10 imágenes.


Las siguientes limitaciones se aplican al Asistente de contenido de Campaign:

* El idioma admitido es solo inglés
* Solo disponible para el canal de correo electrónico
* Puede que el contenido de GenAI no siempre sea preciso: comparta sus comentarios para que nuestros ingenieros puedan perfeccionar los modelos
* Puede cargar varios recursos de marca, pero solo puede aprovechar uno para una generación específica


<!--
<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Text generation" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Text generation with the Content Assistant</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="Image generation" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>Image generation with the Content Assistant</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="Email generation" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>Email generation with the Content Assistant</strong></a>
</div>
<p></td>
</tr></table>
-->

