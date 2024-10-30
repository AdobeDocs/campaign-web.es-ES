---
title: Creación de contenido condicional
description: Aprenda a definir condiciones para personalizar el contenido en Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: f57e0f2de12780ff9f90c2c5f1933b0e9bffe493
workflow-type: tm+mt
source-wordcount: '1011'
ht-degree: 6%

---

# Generación de contenido condicional{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Añadir contenido condicional"
>abstract="Configure campos de contenido condicional para crear una personalización dinámica avanzada basada en el perfil del destinatario. Los bloques de texto, los vínculos, la línea de asunto o las imágenes se sustituyen en el contenido del mensaje cuando se cumple una condición en concreto."

## Introducción al contenido condicional {#gs}

El contenido condicional es una práctica funcionalidad que permite crear una personalización dinámica basada en los datos de perfil del destinatario, sustituyendo automáticamente los bloques de texto y las imágenes cuando se cumplen determinadas condiciones. Esta función puede llevar las campañas a otro nivel y ofrecer experiencias personalizadas y enfocadas al público.

Al configurar los campos de contenido condicional, se puede crear una personalización dinámica avanzada basada en el perfil del destinatario, por ejemplo. Los bloques de texto, los vínculos, la línea de asunto o las imágenes se sustituyen en el contenido del mensaje cuando se cumple una condición concreta. Por ejemplo, puede mostrar &quot;Sr.&quot; o &quot;Sra.&quot; según el valor del campo Género en la base de datos de Adobe Campaign, o incluir un vínculo diferente basado en el idioma preferido del destinatario.

Para crear contenido condicional, debe crear condiciones en el **editor de expresiones** con funciones de ayuda específicas. Este método está disponible para todos los canales de envío en cualquier campo en el que pueda acceder al editor de expresiones, como la línea de asunto o los vínculos de correo electrónico y los componentes de contenido de texto/botón. [Obtenga información sobre cómo acceder al editor de expresiones](gs-personalization.md#access)

Además del editor de expresiones, puede aprovechar un generador de contenido condicional **dedicado** al diseñar un mensaje de correo electrónico que le permita crear varias variantes para un elemento del cuerpo del correo electrónico. [Aprenda a crear contenido condicional en correos electrónicos](#condition-condition-builder)

## Creación de condiciones en el editor de expresiones {#condition-perso-editor}

Para definir contenido condicional para una entrega mediante el editor de expresiones, siga los pasos a continuación. En este ejemplo, deseamos crear contenido condicional basado en el idioma de los destinatarios (francés o inglés).

1. Abra una entrega y vaya a la sección de edición de contenido.

1. Busque el campo donde desea agregar contenido condicional. Por ejemplo, puede añadir contenido condicional a un mensaje SMS.

1. Haga clic en el icono **[!UICONTROL Abrir cuadro de diálogo de personalización]** situado junto al campo para abrir el editor de expresiones.

   ![](assets/open-perso-editor-sms.png){zoomable="yes"}

1. En el editor de personalización, vaya al menú **[!UICONTROL Condiciones]** de la izquierda.

1. Para empezar a crear la condición, haga clic en el icono &quot;+&quot; junto a la función **If**. Se agrega la línea siguiente a la pantalla central:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Reemplazar `<FIELD>` por un campo personalizado, como el idioma del destinatario: `recipient.language`.
   * Reemplazar `<VALUE>` con el valor que se debe satisfacer. Por ejemplo, `'French'`.
   * Reemplace `Ìnsert content here` por el contenido que desea mostrar a los perfiles que cumplen la condición especificada.

     ![](assets/condition-sample1.png){zoomable="yes"}{width="800" align="center"}

1. Especifique el contenido que se debe mostrar si los destinatarios no cumplen la condición. Para ello, use una función de ayuda **else**:

   1. Coloque el cursor antes de la etiqueta de cierre de expresión `%>` y haga clic en `+` junto a la función **Else**.

   1. Reemplace `Ìnsert content here` por el contenido que desee mostrar a los perfiles que no cumplan la condición de la función if.

   ![](assets/condition-sample2.png){zoomable="yes"}{width="800" align="center"}

   También puede usar la función de ayuda **else if** para generar condiciones con múltiples variantes de contenido. Por ejemplo, la expresión siguiente muestra tres variantes de un mensaje según el idioma de los destinatarios:

   ![](assets/condition-sample3.png){zoomable="yes"}{width="800" align="center"}

   >[!NOTE]
   >
   >Cada vez que se agrega una función de ayuda, las etiquetas de apertura (`<%`) y cierre (`%>`) se agregan automáticamente antes y después de la función.
   >
   >Ejemplo después de agregar una función de ayuda &quot;Else&quot; dentro de una expresión: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Asegúrese de quitar estas etiquetas para evitar errores de sintaxis. En este ejemplo, la expresión corregida después de quitar las etiquetas de función **else** es:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Una vez que la condición esté lista, puede guardar el contenido y comprobar su renderización simulando el contenido.

## Creación de contenido condicional en correos electrónicos {#condition-condition-builder}

El contenido condicional de los correos electrónicos se puede crear de dos formas:
* En el editor de expresiones creando una condición con funciones de ayuda,
* En un generador de contenido condicional específico al que se puede acceder al diseñar un correo electrónico.

En la siguiente sección se proporcionan instrucciones paso a paso sobre cómo crear condiciones mediante la capacidad de contenido condicional de Email Designer. Encontrará información detallada sobre cómo crear condiciones utilizando el editor de expresiones [aquí](#condition-perso-editor).

En este ejemplo, deseamos crear un mensaje de correo electrónico con varias variantes basadas en el idioma de los destinatarios. Siga estos pasos:

1. Cree o abra una entrega por correo electrónico, edite su contenido y haga clic en el botón **[!UICONTROL Editar cuerpo del correo electrónico]** para abrir el área de trabajo de diseño del correo electrónico.

1. Seleccione un componente de contenido y haga clic en el icono **[!UICONTROL Habilitar contenido condicional]**.

   ![](assets/condition-email-enable.png){zoomable="yes"}{width="800" align="center"}

1. El panel **[!UICONTROL Contenido condicional]** se abre en el lado izquierdo de la pantalla. En este panel, puede crear varias variantes del componente de contenido seleccionado mediante condiciones.

1. Configure su primera variante. Pase el ratón sobre **[!UICONTROL Variante - 1]** en el panel **[!UICONTROL Contenido condicional]** y haga clic en el botón **[!UICONTROL Agregar condición]**.

   ![](assets/condition-add-condition.png){zoomable="yes"}{width="800" align="center"}

1. Se abrirá el modelador de consultas. Permite generar una condición filtrando los datos de perfil del destinatario. [Aprenda a trabajar con el modelador de consultas](../query/query-modeler-overview.md).

   Una vez que la condición de la primera variante del mensaje esté lista, haz clic en **[!UICONTROL Confirmar]**. En este ejemplo, se crea una regla para destinatarios cuyo idioma es &quot;francés&quot;.

   ![](assets/condition-example.png){zoomable="yes"}{width="800" align="center"}

1. La regla ahora está asociada a la variante. Para mejorar la legibilidad, se recomienda cambiar el nombre de la variante haciendo clic en el menú de los tres puntos.

1. Configure cómo debe mostrarse el componente si se cumple la regla al enviar el mensaje. En este ejemplo, deseamos mostrar el texto en francés si es el idioma preferido del destinatario.

   ![](assets/condition-email-variant1.png){zoomable="yes"}{width="800" align="center"}

1. Añada tantas variantes como sea necesario para el componente de contenido. Puede cambiar entre las variantes en cualquier momento para comprobar cómo se mostrará el componente de contenido en función de sus reglas condicionales.

   >[!NOTE]
   >Si ninguna de las reglas definidas en las variantes se cumple al enviar el mensaje, el componente de contenido mostrará el contenido definido en la **[!UICONTROL variante predeterminada]** del panel **[!UICONTROL Contenido condicional]**.

## Usar variables para contenido condicional {#variables-conditional}

Las variables se pueden utilizar para el contenido condicional en el envío.

Más información sobre [agregar variables a un envío](../advanced-settings/delivery-settings.md#variables-delivery).

Elija el elemento en el que desea colocar un contenido condicional.

![](assets/variables-conditional.png){zoomable="yes"}

Para usar la variable, configure la condición con el botón **[!UICONTROL Editar expresión]**, como se muestra a continuación.
En este ejemplo, esta imagen se muestra cuando el valor de la variable es `launch`.

![](assets/variables-condition.png){zoomable="yes"}

También puede crear otra variante con el valor `reminder`, por ejemplo, donde se muestra una imagen diferente.
