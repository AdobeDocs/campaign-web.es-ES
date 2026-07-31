---
audience: end-user
title: Introducción a la generación de contenido
description: Introducción a la generación de contenido
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
TQID: https://experienceleague.adobe.com/jpw4u-Vy7M2Q9qRyQ2J3rJ-Mr8UKLUpxhw39tglbbNc
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
source-git-commit: d4e22ba88bcb6dc74d22e8a927c1640f21d75d3e
workflow-type: tm+mt
source-wordcount: 887
ht-degree: 20%

---

# Trabajo con Generar contenido {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="Generar contenido"
>abstract="Después de crear y personalizar su envío, utilice IA para mejorar su contenido. Esta función simplifica el proceso de personalización y mejora del contenido, ya que le permite ajustar el contenido al describir lo que desea generar."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Defina el contexto con Generar contenido en Campaign"
>abstract="Para utilizar el contenido seleccionado como entrada para la generación de contenido, active el conmutador **Mejorar con el contenido actual**. También puede cargar los recursos de su marca para utilizarlos como fuente. Si no utiliza el contenido seleccionado, es obligatorio cargar y seleccionar los recursos de marca."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Términos de la IA generativa de Adobe"
>abstract="El acceso a esta función está sujeto a su acuerdo con las directrices de usuario de la IA generativa de Adobe Experience Cloud. Revise cualquier resultado de esta función para verificar su exactitud y asegúrese de que sea adecuado para su caso de uso."
>additional-url="https://www.adobe.com/es/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Directrices del usuario de IA generativa de Adobe"

>[!INFO]
>
>Sumérjase en una experiencia práctica con [nuestra vista previa de características en vivo](https://experienceleague.adobe.com/es/apps/journey-optimizer/ai-assistant-content-accelerator), diseñada para permitirle explorar sus características de primera mano y comprender plenamente sus capacidades.

A medida que la industria del marketing se vuelve más competitiva, las marcas buscan formas eficientes de generar contenido impactante rápidamente. Generar contenido en la web de Adobe Campaign, con tecnología Microsoft Azure OpenAI y Adobe Firefly, es la capacidad de generación de contenido de IA de Adobe que transforma la forma en que los especialistas en marketing crean contenido profesional y coherente con la marca en canales como correo electrónico, SMS y notificaciones push. Con los modelos avanzados de GenAI y una comprensión profunda de las directrices de marca, Generar contenido genera automáticamente contenido personalizado, atractivo y eficaz en función del objetivo de marketing, optimizando el contenido para los estilos, los diseños, el tono y mucho más descritos por la marca.

Generate Content admite la generación **en varios idiomas**, lo que le permite llegar a diversas audiencias globales y participar en ellas. Generar contenido está disponible en los siguientes idiomas:

<table style="table-layout:fixed; margin-top: 0px; margin-bottom: 0px;">
  <tbody>
    <tr style="border: 0;background-color: #FFFFFF;">
      <td>
        <ul>
          <li>Chino (Hong Kong)</li>
          <li>Chino (simplificado)</li>
          <li>Chino (Taiwán)</li>
          <li>Neerlandés</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Francés</li>
          <li>Alemán</li>
          <li>Italiano</li>
          <li>Japonés</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Noruego</li>
          <li>Portugués</li>
          <li>Español</li>
          <li>Sueco</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

Generar contenido simplifica la creación y ejecución de campañas de marketing en varios canales, como correo electrónico, SMS y notificaciones push, lo que ahorra tiempo, mejora la eficacia y mejora los resultados.

>[!IMPORTANT]
>
>* Antes de usar esta capacidad, revise las [protecciones y limitaciones](#generative-guardrails) relacionadas.
>
>* Debe aceptar un [acuerdo de usuario](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) antes de usar IA para generar contenido en Adobe Campaign Web. Para obtener más información, póngase en contacto con su representante Adobe.

## Acceder a Generar contenido {#generative-access}

La generación de contenido para correos electrónicos, notificaciones push, páginas de aterrizaje y SMS ahora está en General Availability (GA) y disponible para todos los usuarios. A continuación se detallan los permisos y pasos necesarios para conceder acceso a los usuarios.

+++ Aprenda a asignar permisos relacionados con la generación de contenido

1. **Acceda a [Admin Console](https://adminconsole.adobe.com/)**, vaya al menú de **Productos** y, a continuación, seleccione **Nube administrada de Adobe Campaign**.

1. Acceda a la instancia para la que desea conceder permisos y, a continuación, haga clic en **Nuevo perfil** para crear un nuevo perfil de producto con el siguiente nombre de perfil de producto específico:

   `Campaign - <instance-name> - AIAssistant`

1. Configure el perfil del producto con los permisos necesarios para acceder a Generar contenido.

1. **Agregar usuarios o grupos de usuarios**. Elija una de las siguientes opciones:
   * **Agregar usuarios individuales**: Agregue los usuarios necesarios directamente al perfil del producto.
   * **Agregar grupos de usuarios**: cree un grupo de usuarios, agregue usuarios a ese grupo y, a continuación, agregue el grupo de usuarios al perfil de producto.

Obtenga información sobre cómo definir permisos en Campaign en [esta sección](../get-started/permissions.md).

+++

## Mecanismos de protección y limitaciones {#generative-guardrails}

A continuación, se enumeran las directrices generales para utilizar IA para generar contenido en Adobe Campaign Web para la generación de correo electrónico:

* La calidad del contenido generado depende en gran medida del objetivo de marketing o del prompt que defina. Utilice un indicador bien definido para que el modelo GenAI interprete con precisión.
* Cargue recursos de marca para garantizar un contenido preciso y sin marca. De lo contrario, el contenido se basa en información disponible públicamente. El contenido cargado puede tener los siguientes formatos: archivos PDF, JPEG, PNG o ZIP (con formatos de archivo compatibles).
* El tamaño máximo de los recursos de marca cargados es de 50 MB. Los archivos de mayor tamaño o las numerosas imágenes pueden aumentar el tiempo de procesamiento.
* Use [plantillas de correo electrónico](../content/create-email-templates.md), plantillas específicas de la marca o plantillas personalizadas para crear el contenido de su correo electrónico mediante IA. Se recomiendan plantillas de correo electrónico con hasta 8-10 imágenes.
* Informe de cualquier salida problemática mediante los iconos de miniaturas hacia arriba, miniaturas hacia abajo o indicadores al seleccionar variantes.
* El uso de Generar contenido está sujeto a las Directrices del usuario de IA generativa de Adobe Experience Cloud. [Más información](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Como parte del compromiso de Adobe con la transparencia en el uso de herramientas de IA generativa en la creación de medios, Adobe aplica Content Credentials cuando se descarga o exporta contenido o un proyecto que incluye un recurso generado por Firefly. [Más información](https://helpx.adobe.com/firefly/using/content-credentials.html).

Las siguientes limitaciones se aplican a Generar contenido en Adobe Campaign Web:

* Generar contenido en la web de Adobe Campaign solo se admite actualmente en inglés. Las entradas que no sean en inglés pueden producir resultados incoherentes o erróneos. Los problemas que surjan de las respuestas que no sean en inglés no se abordarán ni mejorarán en este momento.
* Solo disponible para los canales de correo electrónico, push y SMS.
* Puede que el contenido de GenAI no siempre sea preciso. Comparta sus comentarios para que los ingenieros puedan refinar los modelos.
* Puede cargar varios recursos de marca, pero solo puede aprovechar uno para una generación específica.

## Generar capacidades de contenido {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-full-content.md">
<img alt="[Generación de contenido completo con Generar contenido]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-full-content.md"><strong>Generación de contenido completo con Generar contenido</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-text.md">
<img alt="[Generación de contenido de texto con Generar contenido]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-text.md"><strong>Generación de texto con contenido generado</strong>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="[Generación de imágenes con Generar contenido]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-image.md"><strong>Generación de imágenes con contenido generado</strong></a>
</div>
<p></td>
</tr></table>