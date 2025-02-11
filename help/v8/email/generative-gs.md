---
audience: end-user
title: Introducción al Acelerador de contenido del Asistente de IA
description: Introducción al acelerador de contenido del asistente de IA
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 25%

---

# Trabajo con el Acelerador de contenido del Asistente de IA  {#generative-gs}


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
>abstract="El acceso a esta función está sujeto a su acuerdo con las directrices de usuario de IA generativa de Adobe Experience Cloud. Revise la exactitud de los resultados de esta función y asegúrese de que son adecuados para su caso de uso."
>additional-url="https://www.adobe.com/es/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directrices del usuario de IA generativa de Adobe"

>[!INFO]
>
>Sumérjase en una experiencia práctica con [nuestra vista previa de características en vivo](https://experienceleague.adobe.com/es/apps/journey-optimizer/ai-assistant-content-accelerator), diseñada para permitirle explorar sus características de primera mano y comprender plenamente sus capacidades.


A medida que el sector de marketing se vuelve más competitivo, las marcas buscan formas eficientes de generar contenido impactante de manera eficiente y rápida. El acelerador de contenido asistente de IA de Adobe Campaign Web, con tecnología Microsoft Azure OpenAI y Adobe Firefly, es la capacidad de generación de contenido de IA de Adobe que revoluciona la forma en que los especialistas en marketing crean contenido profesional y coherente con la marca en canales como correo electrónico, SMS y push. Con los modelos avanzados de GenAI y una comprensión profunda de las directrices de marca, el asistente de IA genera automáticamente contenido personalizado, atractivo y eficaz en función del objetivo de marketing, con contenido optimizado para los estilos, diseños, tonos y mucho más definidos por la marca.

El Asistente de IA hace que la creación y ejecución de campañas de marketing en canales como correo electrónico, SMS y push sea intuitiva, sencilla y sin complicaciones, a la vez que ahorra tiempo, mejora la eficacia y obtiene mejores resultados.

>[!IMPORTANT]
>
>* Antes de empezar a usar esta capacidad, lea [Protecciones y limitaciones](#generative-guardrails) relacionadas.
>
>* Debe aceptar un [acuerdo de usuario](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) para poder usar el acelerador de contenido del asistente de IA en Adobe Campaign Web. Para obtener más información, póngase en contacto con su representante Adobe.

## Acceso al acelerador de contenido del asistente de IA {#generative-access}

El acelerador de contenido asistente de IA para correos electrónicos, notificaciones push y SMS ahora está en General Availability (GA) y disponible para todos los usuarios. A continuación se detallan los permisos y pasos necesarios para conceder acceso a los usuarios.

+++  Aprenda a asignar permisos relacionados con la generación de contenido

1. **Crear perfil de producto** - En [Admin Console](https://stage.adminconsole.adobe.com/), cree un perfil de producto con el siguiente patrón específico:
   `Campaign - <instance-name> - AIAssistant`

1. **Agregar usuarios** - Agregue el usuario requerido a ese perfil de producto,
o
   **Crear grupo de usuarios** y agregar ese grupo de usuarios al perfil de productos y agregar usuarios a ese perfil de productos.

Obtenga información sobre cómo definir permisos en Campaign en [esta sección](../get-started/permissions.md).

+++

## Mecanismos de protección y limitaciones {#generative-guardrails}

A continuación, se enumeran las directrices generales para utilizar el acelerador de contenido asistente de IA en Adobe Campaign Web para la generación de correo electrónico:

* La calidad del contenido generado se ve fuertemente influida por el objetivo de marketing que defina. Utilice un indicador bien definido para el modelo GenAI para interpretar con precisión. 
* Cargue el recurso de la marca para tener información precisa sobre el contenido de la marca. De lo contrario, el contenido se basa en información disponible públicamente. El contenido cargado puede tener los siguientes formatos: PDF, JPEG, PNG o archivos ZIP (con formatos de archivo compatibles).
* El tamaño máximo del recurso de marca cargado es de 50 MB. Los archivos más grandes o muchas imágenes pueden funcionar, pero el tiempo de procesamiento aumenta.
* Utilice [plantillas de correo electrónico](../email/create-email-templates.md), plantilla específica de la marca o plantilla personalizada para crear el contenido de su correo electrónico mediante el acelerador de contenido. Se recomiendan plantillas de correo electrónico con hasta 8-10 imágenes.
* Asegúrese de informar de cualquier salida problemática utilizando los iconos de miniatura hacia arriba, pulgar hacia abajo o indicador al seleccionar variantes.
* El uso del asistente de IA está sujeto a las Directrices del usuario de IA generativa de Adobe Experience Cloud. [Más información](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Como parte del compromiso de Adobe de fomentar la transparencia en el uso de herramientas de IA generativa en la creación de medios, Adobe aplicará Contentes credentials cuando se descargue o exporte contenido o un proyecto que incluya un recurso generado por el Firefly. [Más información](https://helpx.adobe.com/firefly/using/content-credentials.html)

Las siguientes limitaciones se aplican al acelerador de contenido del asistente de IA en Adobe Campaign Web:

* El acelerador de contenido del asistente de IA en la web de Adobe Campaign solo es compatible actualmente en inglés. Las entradas que no sean en inglés pueden producir resultados incoherentes o erróneos. En este momento no se abordarán ni mejorarán los problemas que surjan de las respuestas que no sean en inglés.
* Solo disponible para los canales de correo electrónico, push y SMS.
* Puede que el contenido de GenAI no siempre sea preciso: comparta sus comentarios para que nuestros ingenieros puedan perfeccionar los modelos.
* Puede cargar varios recursos de marca, pero solo puede aprovechar uno para una generación específica.

## Funcionalidades de generación de contenido del asistente de IA {#generative-features}

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
