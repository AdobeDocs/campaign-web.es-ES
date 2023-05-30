---
title: Personalización del contenido en Campaign
description: Obtenga información sobre cómo personalizar su contenido en la IU de la web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 48d5684201f006add0ceb467129dbbcf98465c5b
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 67%

---


# Personalización de su contenido{#add-personalization}

Para sacar el máximo partido a cada campaña de marketing, Adobe Campaign le ofrece una forma de ofrecer contenido personalizado que hable con los clientes de su nivel. En función de los datos de perfil, utilice funcionalidades de personalización para crear una experiencia personalizada para diferentes grupos e individuos: puede adaptar los mensajes a cada destinatario específico aprovechando los datos y la información que tiene sobre ellos. Puede ser su nombre, intereses, dónde viven, qué compraron y mucho más.

Utilice Campaign para crear contenido dinámico y enviar mensajes personalizados. Las funcionalidades de personalización se pueden combinar para mejorar sus mensajes y crear una experiencia de usuario personalizada.

Puede personalizar el contenido del mensaje haciendo lo siguiente:

* Inserción dinámica de **campos de personalización**

   Los campos de personalización se utilizan para la personalización de primer nivel de los mensajes. Puede seleccionar cualquier campo disponible en la base de datos desde el editor de personalización. Para un envío, se puede seleccionar cualquier campo relacionado con el destinatario, el mensaje o el envío. Estos atributos de personalización se pueden insertar en la línea de asunto o en el cuerpo de los mensajes.

   ![](assets/perso-subject-line.png)

   La siguiente sintaxis inserta la ciudad del destinatario en el contenido: &lt;%= recipient.location.city %>.

* Inserción predefinida de los **bloques de contenido**

   Campaign incluye un conjunto de bloques de personalización que contienen una renderización específica que puede insertar en los envíos. Por ejemplo, puede agregar un logotipo, un mensaje de saludo o un vínculo a la página espejo de un mensaje de correo electrónico. Los bloques de contenido están disponibles en una entrada dedicada del editor de personalización.

   ![](assets/perso-content-blocks.png)

* Crear **contenido condicional**

   Configure el contenido condicional para añadir personalización dinámica basada en el perfil del destinatario, por ejemplo. Los bloques de texto o las imágenes se insertan cuando una condición en particular es verdadera. Puede definir la versión alternativa del contenido cuando la condición no sea verdadera.


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

1. Una vez insertado, el bloque de contenido se añade al contenido del correo electrónico. Se adapta automáticamente al perfil de destinatario cuando se genera la personalización, en el paso de preparación de la entrega.

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

## Bloques de contenido integrados {#ootb-content-blocks}

Descripción de los bloques de contenido integrados:

* **[!UICONTROL Habilitado por Adobe Campaign]**: inserta el logotipo “Habilitado por Adobe Campaign”.
* **[!UICONTROL Función de formateo para nombres propios]**: genera la función JavaScript **[!UICONTROL toSmartCase]**, que cambia la primera letra de cada palabra a mayúscula.
* **[!UICONTROL Saludos]**: inserta los saludos con el nombre completo del destinatario, seguidos de una coma. Ejemplo: “Hola, John Doe”.
* **[!UICONTROL Insertar logotipo]**: inserta un logotipo que se define en la configuración de la instancia.
* **[!UICONTROL Enlace a página espejo]**: inserta un enlace a la [página espejo](../content/mirror-page.md). El formato predeterminado es: “Si no puede ver este mensaje correctamente, haga clic aquí”.
* **[!UICONTROL URL de la página espejo]**: inserta la dirección URL de la página espejo, permite que los diseñadores de envío comprueben el vínculo.
* **[!UICONTROL URL de aceptación de la oferta en modo unitario]**: inserta una URL que permite establecer una oferta como **[!UICONTROL Aceptada]**. (Este bloque está disponible si el módulo Interacción está habilitado)
* **[!UICONTROL Confirmación del registro]**: inserta un vínculo que permite confirmar la suscripción.
* **[!UICONTROL Vínculo de registro]**: inserta un vínculo de suscripción. Este vínculo se define en la configuración de la instancia. El contenido predeterminado es: “Para registrarse, haga clic aquí”.
* **[!UICONTROL Vínculo de registro (con referencia)]**: inserta un vínculo de suscripción que permite identificar el visitante y el envío. Este vínculo se define en la configuración de la instancia.
* **[!UICONTROL URL de la página de registro]**: inserta una URL de suscripción.
* **[!UICONTROL Estilo de los correos electrónicos de contenido]** y **[!UICONTROL Estilo de las notificaciones]**: generan un código que da formato a un correo electrónico con estilos HTML predefinidos.
* **[!UICONTROL Vínculo de baja]**: inserta un vínculo que permite cancelar la suscripción a todos los envíos (lista de bloqueados). El contenido asociado predeterminado es el siguiente: “Usted recibe este mensaje porque ha estado en contacto con ***nombre de la organización*** o un afiliado. Para dejar de recibir mensajes de ***nombre de la organización*** haga clic aquí”.
