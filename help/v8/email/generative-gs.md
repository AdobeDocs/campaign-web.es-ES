---
audience: end-user
title: Introducción al asistente de IA
description: Introducción al asistente de IA
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 7de6d85036eac7289e7fcf3a82a7c11be12d9c6e
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 32%

---

# Introducción al asistente de IA {#generative-gs}

>[!BEGINSHADEBOX]

**Tabla de contenido**

* Introducción al asistente de IA
* [Generación de correo electrónico con el asistente de IA](generative-content.md)
* [Generación de SMS con el asistente de IA](generative-sms.md)
* [Generación de notificaciones push con el asistente de IA](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Asistente de IA"
>abstract="Una vez que haya creado y personalizado su envío, puede utilizar el Asistente de IA para mejorar el contenido.  Esta funcionalidad simplifica el proceso de personalización y mejora del contenido, ya que le permite ajustar el contenido al describir lo que desea generar."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definición del contexto con el asistente de IA de Campaign"
>abstract="Para utilizar el contenido seleccionado como entrada para la generación de contenido, active la alternancia **Mejorar con contenido actual**. También puede cargar los recursos de su marca para utilizarlos como fuente. Si no utiliza el contenido seleccionado, es obligatorio cargar y seleccionar recursos de una marca."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Términos de la IA generativa de Adobe"
>abstract="El acceso a esta función está sujeto a su acuerdo con las directrices de usuario de IA generativa de Adobe Experience Cloud. Revise la exactitud de los resultados de esta función y asegurarse de que son adecuados para su caso de uso."
>additional-url="https://www.adobe.com/es/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directrices del usuario de IA generativa de Adobe"

A medida que el sector de marketing se vuelve más competitivo, las marcas buscan formas eficientes de generar contenido impactante de manera eficiente y rápida. El asistente de IA en Campaign, con tecnología de Azure OpenAI, es la capacidad de generación de contenido de IA de Adobe que revoluciona la forma en que los especialistas en marketing crean contenido profesional y coherente con la marca en canales como correo electrónico, SMS y push. Con los modelos avanzados de GenAI y una comprensión profunda de las directrices de marca, el asistente de IA genera automáticamente contenido personalizado, atractivo y eficaz en función del objetivo de marketing, con contenido optimizado para los estilos, diseños, tonos y mucho más definidos por la marca.

AI Assistant hace que la creación y ejecución de campañas de marketing en canales como correo electrónico, SMS y push sea intuitiva, sencilla y sin complicaciones, a la vez que ahorra tiempo, mejora la eficacia y obtiene mejores resultados.

>[!NOTE]
>
>Esta funcionalidad está disponible en su versión de Beta y sujeta a cambios sin previo aviso.

## Mecanismos de protección y limitaciones {#generative-guardrails}

A continuación, se enumeran las directrices generales para utilizar el asistente de IA en Campaign para la generación de correo electrónico:

* La calidad del contenido generado se ve fuertemente influida por el objetivo de marketing que defina. Utilice un indicador bien definido para el modelo GenAI para interpretar con precisión. 
* Cargue el recurso de la marca para tener información precisa sobre el contenido de la marca. De lo contrario, el contenido se basa en información disponible públicamente. El contenido cargado puede tener los siguientes formatos: PDF, JPEG, PNG o archivos ZIP (con formatos de archivo compatibles).
* El tamaño máximo del recurso de marca cargado es de 50 MB. Los archivos más grandes o muchas imágenes pueden funcionar, pero el tiempo de procesamiento aumenta.
* Use plantillas de correo electrónico creadas por Adobe Campaign, preferiblemente [plantillas de correo electrónico integradas](../email/create-email-templates.md), una plantilla específica de marca o una plantilla personalizada para crear el contenido de su correo electrónico. Se recomienda una plantilla de correo electrónico con hasta 8-10 imágenes.
* Asegúrese de informar de cualquier salida problemática utilizando los iconos de miniatura hacia arriba, pulgar hacia abajo o indicador al seleccionar variantes.
* El uso del asistente de IA está sujeto a las Directrices del usuario de IA generativa de Adobe Experience Cloud. [Más información](https://www.adobe.com/es/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

Las siguientes limitaciones se aplican al asistente de IA en Campaign:

* El idioma admitido es solo inglés.
* Solo disponible para los canales de correo electrónico, push y SMS.
* Puede que el contenido de GenAI no siempre sea preciso: comparta sus comentarios para que nuestros ingenieros puedan perfeccionar los modelos.
* Puede cargar varios recursos de marca, pero solo puede aprovechar uno para una generación específica.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="Generación de correo electrónico" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Generación de correo electrónico con el asistente de IA</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="Generación de SMS" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Generación de SMS con el asistente de IA</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Generación push" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Generación de notificaciones push con el asistente de IA</strong></a>
</div>
<p></td>
</tr></table>
