---
title: Cree contenido condicional
description: Obtenga información sobre cómo definir condiciones para personalizar su contenido en la IU de la web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 1dfd557b22de9888ab8d3a1f0479b45d59a86f93
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 3%

---

# Creación de contenido condicional{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Cree contenido condicional"
>abstract="Cree contenido condicional para definir una personalización dinámica basada en el perfil del destinatario, sustituyendo automáticamente los bloques de texto y las imágenes cuando se cumplen determinadas condiciones. Esta función puede llevar las campañas a otro nivel y ofrecer experiencias personalizadas y enfocadas a la audiencia."

El contenido condicional es una práctica funcionalidad que permite crear una personalización dinámica basada en el perfil del destinatario y reemplazar automáticamente bloques de texto e imágenes cuando se cumplen determinadas condiciones. Esta función puede llevar las campañas a otro nivel y ofrecer experiencias personalizadas y enfocadas a la audiencia.

Al configurar los campos de contenido condicional, se puede crear una personalización dinámica avanzada basada en el perfil del destinatario, por ejemplo. Los bloques de texto, los vínculos, la línea de asunto o las imágenes se sustituyen en el contenido del mensaje cuando se cumple una condición concreta. Por ejemplo, puede mostrar &quot;Sr.&quot; o &quot;Sra.&quot; según el valor del campo Género en la base de datos de Adobe Campaign, o incluir un vínculo diferente basado en el idioma preferido del destinatario.

## Cómo generar contenido condicional

Para crear contenido condicional, debe crear condiciones en el editor de expresiones con una función de ayuda específica. Este método está disponible para todos los canales de envío en cualquier campo en el que pueda acceder al editor de expresiones, como el campo de línea de asunto o los vínculos de correo electrónico y los componentes de contenido de texto/botón. [Descubra dónde añadir contenido dinámico](gs-personalization.md/#access)

Además del editor de expresiones, puede aprovechar un generador de contenido condicional dedicado al diseñar un correo electrónico que le permita generar condiciones mediante atributos de perfil.

## Creación de condiciones en el editor de expresiones {#condition-perso-editor}

Para definir un contenido condicional para una entrega;, siga los pasos a continuación. En este ejemplo, deseamos crear contenido condicional basado en el idioma de los destinatarios (francés o inglés).

1. Abra una entrega y edite el contenido.

1. Busque el campo donde desea agregar contenido condicional y haga clic en **[!UICONTROL Abrir diálogo de personalización]** para abrir el editor de expresiones. En este ejemplo, queremos añadir contenido condicional a un mensaje SMS:

   ![](assets/open-perso-editor-sms.png)

1. En el editor de personalización, vaya a **[!UICONTROL Funciones de ayuda]** menú izquierdo.

1. Haga clic en el icono &quot;+&quot; junto al **If** función para iniciar la condición. Se añade la siguiente línea a la pantalla central:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Reemplazar `<FIELD>` mediante un campo de personalización. Por ejemplo, el idioma del destinatario: `recipient.language`.
   * Reemplazar `<VALUE>` por el valor que se va a satisfacer. Por ejemplo, `'French'`.
   * Reemplazar `Ìnsert content here` por el contenido que desea mostrar a los perfiles que cumplen la condición especificada anteriormente.

     ![](assets/condition-sample1.png)

1. Especifique el contenido que se debe mostrar si los destinatarios no cumplen la condición. Para ello, haga lo siguiente:

   1. Añadir un **else** Helper function: Coloque el cursor antes de la etiqueta de cierre de expresión `%>` y haga clic en `+` junto al **Else** función.

      >[!NOTE]
      >
      >Cada vez que se añade una función de ayuda, se abre (`<%`) y cierre (`%>`) las etiquetas se añaden automáticamente antes y después de la función. Ejemplo después de agregar una función de ayuda &quot;Else&quot; dentro de una expresión:
      >
      >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
      >
      >Asegúrese de quitar estas etiquetas para evitar errores de sintaxis. En este ejemplo, se corrigió la expresión después de quitar el **Else** etiquetas de función es:
      >
      >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

   1. Reemplazar `Ìnsert content here` por el contenido que desea mostrar a los perfiles que no cumplen la condición.

      ![](assets/condition-sample2.png)

   También puede utilizar la variable **else if** función de ayuda para crear condiciones con varias variantes de contenido. Por ejemplo, la expresión siguiente muestra tres variantes de un mensaje según el idioma de los destinatarios:

   ![](assets/condition-sample3.png)

1. Una vez que la condición esté lista, puede guardar el contenido y comprobar su renderización simulando el contenido.

## Creación de contenido condicional en correos electrónicos  {#condition-condition-builder}

El contenido condicional de los correos electrónicos se puede crear de dos formas:
* En el editor de expresiones creando una condición con funciones de ayuda,
* En un generador de contenido condicional específico al que se puede acceder al diseñar un correo electrónico.

Encontrará información detallada sobre cómo crear condiciones con el editor de expresiones [aquí](#condition-perso-editor).

La sección siguiente le guiará a través de los pasos para crear condiciones mediante el generador de contenido condicional del diseñador de correo electrónico. En este ejemplo, crearemos un mensaje de correo electrónico con varias variantes según el idioma de los destinatarios. Para ello, siga estos pasos:

1. Cree o abra una entrega de correo electrónico, edite su contenido y haga clic en **[!UICONTROL Editar cuerpo del correo electrónico]** para abrir el espacio de trabajo de diseño de correo electrónico.

1. Seleccione un componente de contenido y haga clic en **[!UICONTROL Habilitar contenido condicional]**.

   ![](assets/condition-email-enable.png)

1. El **[!UICONTROL Contenido condicional]** Este panel se abre en el lado izquierdo de la pantalla. En este panel, puede crear varias variantes del componente de contenido seleccionado mediante condiciones.

1. Configure su primera variante. Para ello, pase el ratón sobre **[!UICONTROL Variante - 1]** en el **[!UICONTROL Contenido condicional]** y haga clic en el **[!UICONTROL Añadir condición]** icono.

1. Aparecerá un generador de reglas. Utilice los atributos de perfil para crear la condición para la primera variante del mensaje y haga clic en **[!UICONTROL Confirmar]**. En este ejemplo, se crea una regla para destinatarios cuyo idioma es &quot;francés&quot;.

   ![](assets/condition-email-rule.png)

1. La regla ahora está asociada a la variante. Para mejorar la legibilidad, se recomienda cambiar el nombre de la variante haciendo clic en el menú de los tres puntos.

   Ahora configure cómo debe mostrarse el componente si se cumple la regla al enviar el mensaje. En este ejemplo, deseamos mostrar el texto en francés si es el idioma preferido del destinatario.

   ![](assets/condition-email-variant1.png)

1. Añada tantas variantes como sea necesario para el componente de contenido. Puede cambiar en cualquier momento entre las distintas variantes para comprobar cómo se mostrará el componente de contenido en función de las reglas condicionales.

   >[!NOTE]
   >Si ninguna de las reglas definidas en las variantes se cumple al enviar el mensaje, el componente de contenido mostrará el contenido definido en la variable **[!UICONTROL Variante predeterminada]** desde el **[!UICONTROL Contenido condicional]** panel.
