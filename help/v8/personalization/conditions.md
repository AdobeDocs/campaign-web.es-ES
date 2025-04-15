---
title: Creación de contenido condicional
description: Aprenda a definir condiciones para personalizar el contenido en Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1069'
ht-degree: 6%

---

# Generación de contenido condicional {#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Añadir contenido condicional"
>abstract="Configure campos de contenido condicional para crear una personalización dinámica avanzada basada en el perfil del destinatario. Los bloques de texto, los vínculos, la línea de asunto o las imágenes se sustituyen en el contenido del mensaje cuando se cumple una condición en concreto."

## Introducción al contenido condicional {#gs}

El contenido condicional es una función potente que permite la personalización dinámica basada en los datos de perfil del destinatario. Reemplaza automáticamente bloques de texto e imágenes cuando se cumplen condiciones específicas. Esta función mejora las campañas y ofrece a la audiencia experiencias personalizadas y con objetivos muy precisos.

Al configurar los campos de contenido condicional, se puede crear una personalización dinámica avanzada basada en el perfil del destinatario. Por ejemplo, los bloques de texto, los vínculos, las líneas de asunto y las imágenes se sustituyen en el contenido del mensaje cuando se cumple una condición concreta. Por ejemplo, puede mostrar &quot;Sr.&quot; o &quot;Sra.&quot; según el valor del campo Gender en la base de datos de Adobe Campaign o incluir un vínculo diferente basado en el idioma preferido del destinatario.

Para crear contenido condicional, configure las condiciones en **editor de expresiones** con funciones de ayuda específicas. Este método está disponible para todos los canales de envío en cualquier campo en el que pueda acceder al editor de expresiones, como la línea de asunto, los vínculos de correo electrónico y los componentes de contenido de texto/botón. [Obtenga información sobre cómo acceder al editor de expresiones](gs-personalization.md#access).

Además, use el generador de contenido condicional **dedicado** al diseñar un mensaje de correo electrónico para crear varias variantes para un elemento del cuerpo del correo electrónico. [Aprenda a crear contenido condicional en correos electrónicos](#condition-condition-builder).

## Creación de condiciones en el editor de expresiones {#condition-perso-editor}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_conditions"
>title="Condiciones"
>abstract="Este menú le permite aprovechar las funciones de ayuda para definir contenido condicional."

Para definir contenido condicional para una entrega mediante el editor de expresiones, siga estos pasos. En este ejemplo, el contenido condicional se crea en función del idioma de los destinatarios (francés o inglés).

1. Abra una entrega y vaya a la sección de edición de contenido.

1. Busque el campo donde desea agregar contenido condicional. Por ejemplo, añadir contenido condicional a un mensaje SMS.

1. Haga clic en el icono **[!UICONTROL Abrir cuadro de diálogo de personalización]** situado junto al campo para abrir el editor de expresiones.

   ![Captura de pantalla que muestra el icono del cuadro de diálogo Abrir personalización junto al campo en el editor de mensajes SMS.](assets/open-perso-editor-sms.png){zoomable="yes"}

1. En el editor de personalización, vaya al menú **[!UICONTROL Condiciones]** de la izquierda.

1. Para empezar a crear la condición, haga clic en el icono &quot;+&quot; junto a la función **If**. Se agrega la línea siguiente a la pantalla central: `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Reemplazar `<FIELD>` por un campo personalizado, como el idioma del destinatario: `recipient.language`.
   * Reemplazar `<VALUE>` con el valor que se va a satisfacer, como `'French'`.
   * Reemplazar `Insert content here` por el contenido que se mostrará a los perfiles que cumplan la condición especificada.

     ![Captura de pantalla que muestra una condición de muestra en el editor de expresiones con marcadores de posición para el campo, el valor y el contenido.](assets/condition-sample1.png){zoomable="yes"}{width="800" align="center"}

1. Especifique el contenido que se mostrará si los destinatarios no cumplen la condición. Usar una función de ayuda **else**:

   1. Coloque el cursor antes de la etiqueta de cierre de expresión `%>` y haga clic en `+` junto a la función **Else**.

   1. Reemplace `Insert content here` por el contenido que se mostrará a los perfiles que no cumplan la condición de la función if.

   ![Captura de pantalla que muestra la función Else agregada a la condición en el editor de expresiones.](assets/condition-sample2.png){zoomable="yes"}{width="800" align="center"}

   Utilice la función de ayuda **else if** para generar condiciones con múltiples variantes de contenido. Por ejemplo, la expresión siguiente muestra tres variantes de un mensaje según el idioma de los destinatarios:

   ![Captura de pantalla que muestra una condición con varias variantes según el idioma de los destinatarios.](assets/condition-sample3.png){zoomable="yes"}{width="800" align="center"}

   >[!NOTE]
   >
   >Cada vez que se agrega una función auxiliar, las etiquetas opening (`<%`) y closing (`%>`) se agregan automáticamente antes y después de la función.
   >
   >Ejemplo después de agregar una función de ayuda &quot;Else&quot; dentro de una expresión:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Asegúrese de quitar estas etiquetas para evitar errores de sintaxis. En este ejemplo, la expresión corregida después de quitar las etiquetas de función **else** es:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Guarde el contenido y compruebe su renderización simulando el contenido.

## Creación de contenido condicional en correos electrónicos {#condition-condition-builder}

El contenido condicional de los correos electrónicos se puede crear de dos formas:
* En el editor de expresiones, cree una condición con funciones de ayuda.
* En un generador de contenido condicional específico al que se puede acceder al diseñar un correo electrónico.

En la siguiente sección se proporcionan instrucciones paso a paso para crear condiciones mediante la función de contenido condicional de Email Designer. Encontrará información detallada sobre cómo crear condiciones usando el editor de expresiones [aquí](#condition-perso-editor).

En este ejemplo, se crea un mensaje de correo electrónico con varias variantes en función del idioma de los destinatarios. Siga estos pasos:

1. Cree o abra una entrega por correo electrónico, edite su contenido y haga clic en el botón **[!UICONTROL Editar cuerpo del correo electrónico]** para abrir el área de trabajo de diseño del correo electrónico.

1. Seleccione un componente de contenido y haga clic en el icono **[!UICONTROL Habilitar contenido condicional]**.

   ![Captura de pantalla que muestra el icono Habilitar contenido condicional en el diseñador de correo electrónico.](assets/condition-email-enable.png){zoomable="yes"}{width="800" align="center"}

1. El panel **[!UICONTROL Contenido condicional]** se abre en el lado izquierdo de la pantalla. En este panel, cree varias variantes del componente de contenido seleccionado mediante condiciones.

1. Configure su primera variante. Pase el ratón sobre **[!UICONTROL Variante - 1]** en el panel **[!UICONTROL Contenido condicional]** y haga clic en el botón **[!UICONTROL Agregar condición]**.

   ![Captura de pantalla que muestra el botón Agregar condición en el panel Contenido condicional.](assets/condition-add-condition.png){zoomable="yes"}{width="800" align="center"}

1. Se abre el modelador de consultas, que le permite crear una condición filtrando los datos de perfil del destinatario. [Aprenda a trabajar con el modelador de consultas](../query/query-modeler-overview.md).

   Una vez que la condición de la primera variante del mensaje esté lista, haz clic en **[!UICONTROL Confirmar]**. En este ejemplo, se crea una regla para los destinatarios cuyo idioma es &quot;francés&quot;.

   ![Captura de pantalla que muestra una condición dirigida a destinatarios cuyo idioma es el francés.](assets/condition-example.png){zoomable="yes"}{width="800" align="center"}

1. La regla ahora está asociada a la variante. Para mejorar la legibilidad, cambie el nombre de la variante haciendo clic en el menú de los tres puntos.

1. Configure cómo debe mostrarse el componente si se cumple la regla al enviar el mensaje. En este ejemplo, se muestra el texto en francés si es el idioma preferido del destinatario.

   ![Captura de pantalla que muestra la variante de texto en francés en el diseñador de correo electrónico.](assets/condition-email-variant1.png){zoomable="yes"}{width="800" align="center"}

1. Añada tantas variantes como sea necesario para el componente de contenido. Cambie entre las variantes en cualquier momento para comprobar cómo se mostrará el componente de contenido en función de sus reglas condicionales.

   >[!NOTE]
   >Si ninguna de las reglas definidas en las variantes se cumple al enviar el mensaje, el componente de contenido mostrará el contenido definido en la **[!UICONTROL variante predeterminada]** del panel **[!UICONTROL Contenido condicional]**.

## Usar variables para contenido condicional {#variables-conditional}

Las variables se pueden utilizar para el contenido condicional del envío.

Más información sobre [agregar variables a un envío](../advanced-settings/delivery-settings.md#variables-delivery).

Elija el elemento en el que desea colocar el contenido condicional.

![Captura de pantalla que muestra el uso de variables para contenido condicional.](assets/variables-conditional.png){zoomable="yes"}

Para usar la variable, configure la condición con el botón **[!UICONTROL Editar expresión]**, como se muestra a continuación. En este ejemplo, esta imagen se muestra cuando el valor de la variable es `launch`.

![Captura de pantalla que muestra una condición que usa una variable con el valor &#39;launch&#39;.](assets/variables-condition.png){zoomable="yes"}

Cree otra variante con el valor `reminder`, por ejemplo, donde se muestre una imagen diferente.