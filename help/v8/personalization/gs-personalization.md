---
title: Introducción al contenido dinámico
description: Aprenda a hacer que su contenido sea dinámico mediante la personalización, el contenido condicional y los bloques de contenido integrados.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: 45f4d070c95861f5f96038df82ae7100860159e0
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 22%

---


# Introducción al contenido dinámico

Para sacar el máximo partido a cada campaña de marketing, Adobe Campaign le ofrece una forma de ofrecer contenido dinámico personalizado que hable con los clientes de su nivel. En función de los datos de perfil, utilice funcionalidades de personalización para crear una experiencia personalizada para diferentes grupos e individuos: puede adaptar los mensajes a cada destinatario específico aprovechando los datos y la información que tiene sobre ellos. Puede ser su nombre, intereses, dónde viven, qué compraron y mucho más.

Utilice Campaign para crear contenido dinámico y enviar mensajes personalizados. Las funcionalidades de personalización se pueden combinar para mejorar sus mensajes y crear una experiencia de usuario personalizada.

## ¿Cómo hacer que su contenido sea dinámico?

Puede hacer que el contenido del mensaje sea dinámico insertando:

* **Campos de personalización**: los campos de personalización se utilizan para la personalización de primer nivel de los mensajes. Puede seleccionar cualquier campo disponible en la base de datos desde el editor de personalización. Para un envío, se puede seleccionar cualquier campo relacionado con el destinatario, el mensaje o el envío. Estos atributos de personalización se pueden insertar en la línea de asunto o en el cuerpo de los mensajes.

   La siguiente sintaxis inserta la ciudad del destinatario en el contenido: &lt;%= recipient.location.city %>.

   ![](assets/perso-subject-line.png){width="800" align="center"}

* **Contenido condicional**: configure el contenido condicional para añadir contenido en función del perfil del destinatario, por ejemplo. Los bloques de texto o las imágenes se insertan cuando se cumple una condición concreta. Puede definir la versión alternativa del contenido cuando la condición no sea verdadera.

* **Bloques de contenido integrados**: Campaign viene con un conjunto de bloques de personalización que contienen un procesamiento específico que puede insertar en los envíos. Por ejemplo, puede agregar un logotipo, un mensaje de saludo o un vínculo a la página espejo de un mensaje de correo electrónico. Los bloques de contenido están disponibles en una entrada dedicada del editor de personalización.

   ![](assets/perso-content-blocks.png){width="800" align="center"}

## Acceso al editor de expresiones {#access}

Adobe Campaign V8 Web proporciona un editor de expresiones en el que puede seleccionar, organizar, personalizar y validar todos los datos para crear una experiencia personalizada para el contenido. El editor de expresiones está disponible para todos los canales en todos los campos con **[!UICONTROL Abrir diálogo de personalización]** , como el campo de línea de asunto o los vínculos de correo electrónico y los componentes de contenido de texto/botón.

>[!NOTE]
>
>Además del editor de expresiones, también puede aprovechar un generador de contenido condicional dedicado al diseñar un correo electrónico. [Aprenda a crear contenido condicional en correos electrónicos](conditions.md)

*Acceso al editor de expresiones desde el campo Nombre del remitente*

![](assets/expression-editor-access.png){width="800" align="center"}

*Acceso al editor de expresiones desde un componente de texto de correo electrónico*

![](assets/expression-editor-access-email.png){width="800" align="center"}

*Acceso al editor de expresiones desde un vínculo en un correo electrónico*

![](assets/perso-link-insert-icon.png){width="800" align="center"}


## Vamos a profundizar

Ahora que comprende cómo hacer que el contenido sea dinámico, es hora de profundizar en estas secciones de documentación para empezar a trabajar con la función.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="Personalización del contenido" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>Adición de personalización</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="Posible cliente" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>Añadir contenido condicional</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="Poco frecuente" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>Añadir bloques de contenido integrados</strong></a>
</div>
<p></td>
</tr></table>