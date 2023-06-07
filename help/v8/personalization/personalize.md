---
title: Personalización del contenido en Campaign
description: Obtenga información sobre cómo personalizar su contenido en la IU de la web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 79%

---


# Personalización de su contenido{#add-personalization}

## Personalizar la línea de asunto de un mensaje {#personalize-subject-line}

Para añadir la personalización en el campo **[!UICONTROL Línea de asunto]** del mensaje, siga los pasos a continuación:

1. Abra una entrega y haga clic en **[!UICONTROL Editar contenido]**.
1. Haga clic en **[!UICONTROL Abrir diálogo de personalización]** en la parte derecha del **[!UICONTROL Línea de asunto]** para correos electrónicos, o el campo **[!UICONTROL Título]** campos para envíos push/SMS.

   ![](assets/perso-subject.png){width="600"}

1. Introduzca la línea de asunto o el título y seleccione los atributos de personalización que desee añadir.

1. Haga clic en **[!UICONTROL Confirmar]** para validar. Los atributos de personalización se añaden al contenido.

## Personalización del contenido del correo electrónico {#personalize-emails}

Para personalizar el contenido del correo electrónico, abra el mensaje en el Diseñador de correo electrónico y realice lo siguiente:

1. Haga clic dentro del bloque de texto.
1. En la barra de herramientas contextual, seleccione **[!UICONTROL Añadir personalización]**.

   ![](assets/perso-add-to-content.png)

1. Escriba el nombre del destinatario en el editor de personalización y confírmelo.

   ![](assets/perso-add-name.png)

   El atributo de personalización se añade al contenido del correo electrónico.

   Puede simular el contenido para comprobar la renderización. [Más información](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. Para añadir un bloque de contenido al correo electrónico, siga los mismos pasos y seleccione un bloque de contenido del último icono.

   ![](assets/perso-insert-block.png)

1. Una vez insertado, el bloque de contenido se añade al contenido del correo electrónico. Se adapta automáticamente al perfil de destinatario cuando se genera la personalización, en el paso de preparación del envío.

   ![](assets/perso-content-block-in-email.png)

## Personalización de vínculos en correos electrónicos {#personalize-links}

Para personalizar un **vínculo**:

1. Seleccione un bloque de texto o una imagen.
1. En la barra de herramientas contextual, seleccione **Insertar vínculo**.

   ![](assets/perso-link.png)

1. Introduzca la etiqueta del vínculo y utilice el botón **Insertar vínculo** para personalizar el vínculo.

   ![](assets/perso-link-insert-icon.png)

1. Utilice el editor de personalización para definir y personalizar el vínculo; confírmelo.

   ![](assets/perso-link-edit.png)


## Personalización de las ofertas {#personalize-offers}

También puede acceder al editor de personalización cuando añada contenido de texto a las representaciones de sus ofertas. Obtenga más información en [esta sección](../content/offers.md).

