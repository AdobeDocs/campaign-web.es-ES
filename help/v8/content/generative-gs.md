---
audience: end-user
title: Introducción al Asistente de IA
description: Introducción al Asistente de IA
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 22%

---

# Trabajo con el Asistente de IA {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Asistente de IA"
>abstract="Después de crear y personalizar su envío, utilice el asistente de IA para mejorar su contenido. Esta función simplifica el proceso de personalización y mejora del contenido, ya que le permite ajustar el contenido al describir lo que desea generar."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definición del contexto con el asistente de IA de Campaign"
>abstract="Para utilizar el contenido seleccionado como entrada para la generación de contenido, active el conmutador **Mejorar con el contenido actual**. También puede cargar los recursos de su marca para utilizarlos como fuente. Si no utiliza el contenido seleccionado, es obligatorio cargar y seleccionar los recursos de marca."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Términos de la IA generativa de Adobe"
>abstract="El acceso a esta función está sujeto a su acuerdo con las directrices de usuario de la IA generativa de Adobe Experience Cloud. Revise cualquier resultado de esta función para verificar su exactitud y asegúrese de que sea adecuado para su caso de uso."
>additional-url="https://www.adobe.com/es/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directrices del usuario de IA generativa de Adobe"

>[!INFO]
>
>Sumérjase en una experiencia práctica con [nuestra vista previa de características en vivo](https://experienceleague.adobe.com/es/apps/journey-optimizer/ai-assistant-content-accelerator), diseñada para permitirle explorar sus características de primera mano y comprender plenamente sus capacidades.

A medida que la industria del marketing se vuelve más competitiva, las marcas buscan formas eficientes de generar contenido impactante rápidamente. AI Assistant de Adobe Campaign Web, con tecnología Microsoft Azure OpenAI y Adobe Firefly, es la capacidad de generación de contenido de IA de Adobe que transforma la forma en que los especialistas en marketing crean contenido profesional y coherente con la marca en canales como correo electrónico, SMS y notificaciones push. Con los modelos avanzados de GenAI y una comprensión profunda de las directrices de marca, el asistente de IA genera automáticamente contenido personalizado, atractivo y eficaz en función del objetivo de marketing, optimizando el contenido para los estilos, diseños, tonos y más descritos por la marca.

AI Assistant simplifica la creación y ejecución de campañas de marketing en varios canales, como correo electrónico, SMS y notificaciones push, lo que ahorra tiempo, mejora la eficacia y genera mejores resultados.

>[!IMPORTANT]
>
>* Antes de usar esta capacidad, revise las [protecciones y limitaciones](#generative-guardrails) relacionadas.
>
>* Debe aceptar un [acuerdo de usuario](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) antes de usar el Asistente de IA en Adobe Campaign Web. Para obtener más información, póngase en contacto con su representante Adobe.

## Acceder al asistente de IA {#generative-access}

El asistente de IA para correos electrónicos, notificaciones push, páginas de aterrizaje y SMS ahora está en General Availability (GA) y disponible para todos los usuarios. A continuación se detallan los permisos y pasos necesarios para conceder acceso a los usuarios.

+++ Obtenga información sobre cómo asignar permisos relacionados con la generación de contenido

1. **Crear perfil de producto** - En [Admin Console](https://stage.adminconsole.adobe.com/), cree un perfil de producto con el siguiente patrón específico:
   `Campaign - <instance-name> - AIAssistant`

1. **Agregar usuarios** - Agregue el usuario requerido a ese perfil de producto,\
   o\
   **Crear grupo de usuarios** y agregue ese grupo de usuarios al perfil de productos; a continuación, agregue usuarios a ese perfil de productos.

Obtenga información sobre cómo definir permisos en Campaign en [esta sección](../get-started/permissions.md).

+++

## Mecanismos de protección y limitaciones {#generative-guardrails}

A continuación, se enumeran las directrices generales para utilizar el asistente de IA en la web de Adobe Campaign para la generación de correo electrónico:

* La calidad del contenido generado depende en gran medida del objetivo de marketing o del prompt que defina. Utilice un indicador bien definido para que el modelo GenAI interprete con precisión.
* Cargue recursos de marca para garantizar un contenido preciso y sin marca. De lo contrario, el contenido se basa en información disponible públicamente. El contenido cargado puede tener los siguientes formatos: archivos PDF, JPEG, PNG o ZIP (con formatos de archivo compatibles).
* El tamaño máximo de los recursos de marca cargados es de 50 MB. Los archivos de mayor tamaño o las numerosas imágenes pueden aumentar el tiempo de procesamiento.
* Use [plantillas de correo electrónico](../content/create-email-templates.md), plantillas específicas de la marca o plantillas personalizadas para crear el contenido de su correo electrónico con el Ayudante de IA. Se recomiendan plantillas de correo electrónico con hasta 8-10 imágenes.
* Informe de cualquier salida problemática mediante los iconos de miniaturas hacia arriba, miniaturas hacia abajo o indicadores al seleccionar variantes.
* El uso del asistente de IA está sujeto a las Directrices del usuario de IA generativa de Adobe Experience Cloud. [Más información](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Como parte del compromiso de Adobe con la transparencia en el uso de herramientas de IA generativa en la creación de medios, Adobe aplica Content Credentials cuando se descarga o exporta contenido o un proyecto que incluye un recurso generado por Firefly. [Más información](https://helpx.adobe.com/es/firefly/using/content-credentials.html).

Las siguientes limitaciones se aplican a AI Assistant en Adobe Campaign Web:

* Actualmente, el asistente de IA en la web de Adobe Campaign solo está disponible en inglés. Las entradas que no sean en inglés pueden producir resultados incoherentes o erróneos. Los problemas que surjan de las respuestas que no sean en inglés no se abordarán ni mejorarán en este momento.
* Solo disponible para los canales de correo electrónico, push y SMS.
* Puede que el contenido de GenAI no siempre sea preciso. Comparta sus comentarios para que los ingenieros puedan refinar los modelos.
* Puede cargar varios recursos de marca, pero solo puede aprovechar uno para una generación específica.

## Funcionalidades de generación de contenido del asistente de IA {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-full-content.md">
<img alt="[Generación de contenido completo con el asistente de IA]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-full-content.md"><strong>Generación de contenido completo con el Asistente de IA</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-text.md">
<img alt="[Generación de contenido de texto con el asistente de IA]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-text.md"><strong>Generación de texto con el Asistente de IA</strong>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="[Generación de imágenes con el asistente de IA]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-image.md"><strong>Generación de imágenes con el asistente de IA</strong></a>
</div>
<p></td>
</tr></table>