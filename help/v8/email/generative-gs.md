---
audience: end-user
title: Introducción al asistente de IA
description: Introducción al asistente de IA
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 8%

---

# Trabajo con el Asistente de IA {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Asistente de IA"
>abstract="Después de crear y personalizar su envío, utilice el asistente de IA para mejorar su contenido. Esta función simplifica la personalización y la mejora de contenido, ya que le permite ajustar el contenido al describir lo que desea generar."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Definición del contexto con el asistente de IA de Campaign"
>abstract="Para utilizar el contenido seleccionado como entrada para contenido generación, active el botón de **alternancia Mejorar con contenido** actual. También puede cargar los recursos de su marca para utilizarlos como fuente. Si no utiliza la contenido seleccionada, es obligatorio cargar y seleccionar marca activos."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Términos de la IA generativa de Adobe"
>abstract="El acceso a esta función depende de su aceptación de las Adobe Experience Cloud Directrices del usuario de IA generativa. Revise cualquier resultado de esta función para comprobar su exactitud y asegúrese de que es adecuada para su caso de uso."
>additional-url="https://www.adobe.com/es/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directrices del usuario de IA generativa de Adobe"

>[!INFO]
>
>Sumérjase en una experiencia práctica con [nuestra vista previa de características en vivo](https://experienceleague.adobe.com/es/apps/journey-optimizer/ai-assistant-content-accelerator), diseñada para permitirle explorar sus características de primera mano y comprender plenamente sus capacidades.

A medida que la industria marketing se vuelve más competitiva, las marcas buscan formas eficientes de generar contenido impactantes rápidamente. AI Assistant en Adobe Campaign Web, impulsado por Microsoft Azure OpenAI y Adobe Systems Firefly, es la capacidad de generación de contenido de IA de Adobe Systems que transforma la forma en que los especialistas en marketing crean contenido profesionales y marca consistentes a través de canales gustar correo electrónico, SMS y notificaciones push. Con modelos avanzados de GenAI y un profundo conocimiento de las pautas de marca, AI Assistant genera automáticamente contenido personalizados, atractivos y efectivos basados en el objetivo marketing, optimizando contenido para estilos, diseños, tonos y más marca delineados.

AI Assistant simplifica la creación y ejecución de campañas de marketing en varios canales, como correo electrónico, SMS y notificaciones push, lo que ahorra tiempo, mejora la eficacia y genera mejores resultados.

>[!IMPORTANT]
>
>* Antes de usar esta capacidad, revise las [protecciones y limitaciones](#generative-guardrails) relacionadas.
>
>* Debe aceptar un [acuerdo de usuario](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) antes de usar el Asistente de IA en Adobe Campaign Web. Para obtener más información, póngase en contacto con su representante Adobe.

## Acceso al asistente de IA {#generative-access}

El asistente de IA para correos electrónicos, notificaciones push y SMS ahora se encuentra en General Availability (GA) y disponible para todos los usuarios. A continuación se detallan los permisos y pasos necesarios para conceder acceso a los usuarios.

+++ Obtenga información sobre cómo asignar permisos relacionados con la generación de contenido

1. **Crear perfil de producto** - En [Admin Console](https://stage.adminconsole.adobe.com/), cree un perfil de producto con el siguiente patrón específico:
   `Campaign - <instance-name> - AIAssistant`

1. **Agregar usuarios** - Agregue el usuario requerido a ese perfil de producto,\
   o\
   **Crear grupo de usuarios** y agregue ese grupo de usuarios al perfil de productos; a continuación, agregue usuarios a ese perfil de productos.

Obtenga información sobre cómo definir permisos en Campaign en [esta sección](../get-started/permissions.md).

+++

## Mecanismos de protección y limitaciones {#generative-guardrails}

A continuación se enumeran las directrices generales para usar AI Assistant en Adobe Campaign web para la generación correo electrónico:

* La calidad de los contenido generados depende en gran medida del objetivo marketing o del mensaje que defina. Utilice un indicador bien definido para que el modelo GenAI se interprete con precisión.
* Cargue marca activos para garantizar una contenido precisa y marca. De lo contrario, contenido se basa en información disponible públicamente. El contenido cargado puede tener los siguientes formatos: archivos PDF, JPEG, PNG o ZIP (con formatos de archivo compatibles).
* El tamaño máximo de los recursos de marca cargados es de 50 MB. Los archivos más grandes o varias imágenes pueden aumentar el tiempo de procesamiento.
* Use [plantillas de correo electrónico integradas](../email/create-email-templates.md), plantillas específicas de marca o plantillas personalizadas para crear sus contenido correo electrónico con el Asistente de IA. Se recomiendan plantillas de correo electrónico con hasta 8 a 10 imágenes.
* Informe de cualquier resultado problemático utilizando los iconos pulgar arriba, pulgar abajo o indicador al seleccionar variantes.
* El uso del Asistente de IA está sujeto a las Adobe Experience Cloud Directrices del usuario de IA generativa. [Más información](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Como parte del compromiso de Adobe con la transparencia en el uso de herramientas de IA generativa en la creación de medios, Adobe aplica Content Credentials cuando se descarga o exporta contenido o un proyecto que incluye un recurso generado por Firefly. [Más información](https://helpx.adobe.com/firefly/using/content-credentials.html).

Las siguientes limitaciones se aplican a AI Assistant en Adobe Campaign Web:

* Actualmente, el asistente de IA en la web de Adobe Campaign solo está disponible en inglés. Las entradas que no sean en inglés pueden producir resultados incoherentes o erróneos. Los problemas que surjan de las respuestas que no sean en inglés no se abordarán ni mejorarán en este momento.
* Solo disponible para los canales de correo electrónico, push y SMS.
* Es posible que las contenido de GenAI no siempre sean precisas. Comparta sus comentarios para que los ingenieros puedan perfeccionar los modelos.
* Puede cargar varias marca activos pero solo puede impulsar una para una generación específica.

## Capacidades de generación de contenido de AI Assistant {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[Generación de correo electrónico con AI Assistant]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>Generación de correo electrónico con el asistente de IA</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[Generación de SMS con el asistente de IA]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>Generación de SMS con el asistente de IA</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[Impulse la generación notificación con AI Assistant]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Impulse la generación notificación con AI Assistant</strong></a>
</div>
<p></td>
</tr></table>