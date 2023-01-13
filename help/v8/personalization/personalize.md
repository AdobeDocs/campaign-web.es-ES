---
title: Personalización del contenido en Campaign
description: Obtenga información sobre cómo personalizar el contenido en la interfaz de usuario web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 0d74cababf2b4d66d3b2ce9b0ae2a0f00cb1cdef
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 2%

---

# Personalización del contenido{#add-personalization}

![](../assets/do-not-localize/badge.png)

Puede personalizar el contenido del mensaje:

* Inserción dinámica **campos personalizados**

   Los campos personalizados se utilizan para la personalización de primer nivel de los mensajes. Puede seleccionar cualquier campo disponible en la base de datos desde el editor de personalización. Para una entrega, se puede seleccionar cualquier campo relacionado con el destinatario, el mensaje o la entrega. Estos atributos de personalización se pueden insertar en la línea de asunto o en el cuerpo de los mensajes.

   ![](assets/perso-subject-line.png)

   La siguiente sintaxis inserta la ciudad del destinatario en el contenido: &lt;%= recipient.location.city %>.

* Inserción predefinida **bloques de contenido**

   Campaign viene con un conjunto de bloques personalizados que contienen una renderización específica que puede insertar en los envíos. Por ejemplo, puede añadir un logotipo, un mensaje de saludo o un vínculo a la página espejo del mensaje. Los bloques de contenido están disponibles desde una entrada dedicada en el editor de personalización.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Personalización de la línea de asunto del correo electrónico {#personalize-subject-line}

Para añadir personalización en la variable **[!UICONTROL Línea de asunto]** del mensaje, siga los pasos a continuación:

1. Haga clic en el **Abrir cuadro de diálogo de personalización** a la derecha del **Línea de asunto** campo .
1. Introduzca el contenido de la línea de asunto y seleccione los atributos de personalización que desea añadir.
1. Haga clic en **Confirmar** para validar. Los atributos de personalización se añaden a la línea de asunto.

![](assets/perso-subject.png)

## Personalización del contenido del correo electrónico {#personalize-emails}

Para personalizar el contenido del correo electrónico, abra el mensaje en el Diseñador de correo electrónico y:

1. Haga clic dentro de un bloque de texto.
1. En la barra de herramientas contextual, seleccione **Añadir personalización**.

   ![](assets/perso-add-to-content.png)

1. Inserte el nombre del destinatario en el editor de personalización y confirme.

   ![](assets/perso-add-name.png)

   El atributo de personalización se añade al contenido del correo electrónico.

   Puede simular el contenido para comprobar la renderización. [Más información](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)


## Personalización de vínculos en correos electrónicos {#personalize-links}

Para personalizar un **vínculo**:

1. Seleccione un bloque de texto o una imagen.
1. En la barra de herramientas contextual, seleccione **Añadir personalización**.

   ![](assets/perso-link.png)

1. Utilice el editor de personalización para definir y personalizar el vínculo.

## Personalización de las ofertas {#personalize-offers}

También puede acceder al editor de personalización cuando añada contenido de tipo texto a las representaciones de sus ofertas. Obtenga más información en [esta sección](../content/offers.md).
