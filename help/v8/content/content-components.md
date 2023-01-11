---
audience: end-user
title: Uso de los componentes de contenido del diseñador de correo electrónico
description: Aprenda a utilizar componentes de contenido en los correos electrónicos
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '1085'
ht-degree: 0%

---

# Uso de los componentes de contenido del Diseñador de correo electrónico {#content-components}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="Acerca de los componentes de contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de un correo electrónico."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="Acerca de los componentes de contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de una página de aterrizaje."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="Acerca de los componentes de contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de un fragmento."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="Acerca de los componentes de contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de una plantilla."

## Añadir componentes de contenido {#add-content-components}

Para añadir componentes de contenido al correo electrónico y ajustarlos a sus necesidades, siga los pasos a continuación.

1. En el Diseñador de correo electrónico, utilice un contenido existente o arrastre y suelte **[!UICONTROL Componentes de estructura]** en el contenido vacío para definir el diseño del correo electrónico. [Descubra cómo](create-email-content.md)

1. Para acceder a la **[!UICONTROL Componentes de contenido]** , seleccione el botón correspondiente en el panel izquierdo del Diseñador de correo electrónico.

   ![](assets/email_designer_content_components.png)

1. Arrastre y suelte los componentes de contenido que desee dentro de los componentes de estructura relevantes.

   ![](assets/email_designer_add_content_components.png)

   >[!NOTE]
   >
   >Puede añadir varios componentes en un único componente de estructura y en cada columna de un componente de estructura.

1. Ajuste los atributos de estilo para cada componente mediante el **[!UICONTROL Configuración de componentes]** a la derecha. Por ejemplo, puede cambiar el estilo, el relleno o el margen del texto de cada componente. [Obtenga más información sobre la alineación y el relleno](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png)

Al crear el contenido del correo electrónico desde cero, **[!UICONTROL Componentes de contenido]** le permite personalizar aún más su correo electrónico con componentes sin procesar y vacíos que puede utilizar una vez colocados en un correo electrónico.
Puede agregar tantos **[!UICONTROL Componentes de contenido]** como necesita dentro de un **[!UICONTROL Componente de estructura]** que define el diseño del correo electrónico.

## Contenedor {#container}

Puede añadir un contenedor simple dentro del cual podrá añadir otro componente de contenido. Esto le permite aplicar un estilo específico al contenedor, que será diferente del componente utilizado dentro.

Por ejemplo, agregue un **[!UICONTROL Contenedor]** y, a continuación, agregue un [Botón](#button) dentro de ese contenedor. Puede utilizar un fondo específico para el contenedor y otro para el botón .

![](assets/email_designer_container_component.png)

## Botón {#buttons}

Utilice la variable **[!UICONTROL Botón]** para insertar uno o varios botones en el correo electrónico y redirigir la audiencia de correo electrónico a otra página.

1. De **[!UICONTROL Componentes de contenido]**, arrastre y suelte el **[!UICONTROL Botón]** en un **[!UICONTROL Componente de estructura]**.

   ![](assets/email_designer_13.png)

1. Haga clic en el botón recién agregado para personalizar el texto y tener acceso al **[!UICONTROL Configuración de componentes]** en el panel derecho del Diseñador de correo electrónico.

   ![](assets/email_designer_14.png)

1. En el **[!UICONTROL Vínculo]** , añada la dirección URL a la que desee redirigir al hacer clic en el botón .

1. Elija cómo se redirigirá a su audiencia con la variable **[!UICONTROL Target]** lista desplegable:

   * **[!UICONTROL Ninguna]**: abre el vínculo en el mismo marco en el que se hizo clic (predeterminado).
   * **[!UICONTROL En blanco]**: abre el vínculo en una nueva ventana o pestaña.
   * **[!UICONTROL Self]**: abre el vínculo en el mismo marco en el que se hizo clic.
   * **[!UICONTROL Principal]**: abre el vínculo en el marco principal.
   * **[!UICONTROL Superior]**: abre el vínculo en todo el cuerpo de la ventana.

   ![](assets/email_designer_15.png)

1. Puede personalizar aún más el botón cambiando atributos de estilo como **[!UICONTROL Borde]**, **[!UICONTROL Tamaño]**, **[!UICONTROL Margen]**, etc. de la variable **[!UICONTROL Configuración de componentes]** panel.

## Texto {#text}

Utilice la variable **[!UICONTROL Texto]** para insertar texto en el correo electrónico y ajustar el estilo (borde, tamaño, relleno, etc.) usando la variable **[!UICONTROL Configuración de componentes]** panel.

1. De **[!UICONTROL Componentes de contenido]**, arrastrar y soltar **[!UICONTROL Texto]** en un **[!UICONTROL Componente de estructura]**.

   ![](assets/email_designer_11.png)

1. Haga clic en el componente recién agregado para personalizar el texto y tener acceso al **[!UICONTROL Configuración de componentes]** en el panel derecho del diseñador de correo electrónico.

1. Cambie el texto con las siguientes opciones disponibles en la barra de herramientas:

   ![](assets/email_designer_27.png)

   * **[!UICONTROL Cambiar estilo de texto]**: aplique negrita, cursiva, subrayado o tachado al texto.
   * **Cambiar alineación**: elija entre alineación izquierda, derecha, centro o justificada para el texto.
   * **[!UICONTROL Crear lista]**: añada viñetas o listas numéricas al texto.
   * **[!UICONTROL Definir encabezado]**: añada hasta seis niveles de encabezado al texto.
   * **Tamaño de fuente**: seleccione el tamaño de fuente del texto en píxeles.
   * **[!UICONTROL Editar imagen]**: añada una imagen o un recurso al componente de texto.
   * **[!UICONTROL Mostrar el código fuente]**: muestre el código fuente del texto. No se puede modificar.
   * **[!UICONTROL Duplicar]**: añada una copia del componente de texto.
   * **[!UICONTROL Eliminar]**: elimine el componente de texto seleccionado del correo electrónico.
   * **[!UICONTROL Añadir personalización]**: añada campos personalizados para personalizar el contenido de los datos de perfiles.
   * **[!UICONTROL Habilitar contenido condicional]**: añada contenido condicional para adaptar el contenido del componente a los perfiles de destino.

1. Ajuste los demás atributos de estilo, como el color del texto, la familia de fuentes, el borde, el relleno, el margen, etc. de la variable **[!UICONTROL Configuración de componentes]** panel.

   ![](assets/email_designer_12.png)

## Divisor {#divider}

Utilice la variable **[!UICONTROL Divisor]** para insertar una línea divisoria y organizar el diseño y el contenido del correo electrónico.

Puede ajustar atributos de estilo, como el color de la línea, el estilo y la altura desde la **[!UICONTROL Configuración de componentes]** panel.

![](assets/email_designer_16.png)

## HTML {#HTML}

Utilice la variable **[!UICONTROL HTML]** para copiar y pegar las diferentes partes del HTML existente. Esto le permite crear componentes de HTML modulares gratuitos para reutilizar contenido externo.

1. De **[!UICONTROL Componentes de contenido]**, arrastre y suelte el **[!UICONTROL HTML]** en un **[!UICONTROL Componente de estructura]**.

   ![](assets/email_designer_22.png)

1. Haga clic en el componente recién agregado y, a continuación, seleccione **[!UICONTROL Mostrar el código fuente]** de la barra de herramientas contextual para añadir el HTML.

   ![](assets/email_designer_23.png)

>[!NOTE]
>
>Para hacer que un contenido externo sea compatible con el Diseñador de correo electrónico, Adobe recomienda crear un mensaje desde cero y copiar el contenido del correo electrónico existente en los componentes.

## Imagen {#image}

Utilice la variable **[!UICONTROL Imagen]** para insertar un archivo de imagen desde el equipo en el correo electrónico.

1. En **[!UICONTROL Componentes de contenido]**, arrastrar y soltar **[!UICONTROL Imagen]** en un **[!UICONTROL Componente de estructura]**.

   ![](assets/email_designer_9.png)

1. Haga clic en **[!UICONTROL Examinar]** para elegir un archivo de imagen de los recursos.

1. Haga clic en el componente recién agregado y configure las propiedades de la imagen utilizando la variable **[!UICONTROL Configuración de componentes]** panel:

   * **[!UICONTROL Título de imagen]** permite definir un título para la imagen.
   * **[!UICONTROL Texto alternativo]** permite definir el rótulo vinculado a la imagen. Esto corresponde al atributo del HTML alternativo.

   ![](assets/email_designer_10.png)

1. Ajuste los demás atributos de estilo, como margen, borde, etc. o agregando un vínculo para redirigir a la audiencia a otro contenido de la **[!UICONTROL Configuración de componentes]** panel.

## Social {#social}

Utilice la variable **[!UICONTROL Social]** para insertar vínculos a páginas de medios sociales en el contenido del correo electrónico.

1. De **[!UICONTROL Componentes de contenido]**, arrastre y suelte el **[!UICONTROL Social]** en un **[!UICONTROL Componente de estructura]**.

1. Haga clic en el componente recién agregado.

1. En el **[!UICONTROL Social]** del campo **[!UICONTROL Configuración de componentes]** , elija qué medios sociales desea agregar o quitar.

   ![](assets/email_designer_20.png)

1. Elija el tamaño de los iconos en la **[!UICONTROL Tamaño de las imágenes]** campo .

1. Haga clic en cada uno de los iconos de los medios sociales para configurar la variable **[!UICONTROL URL]** al que se redirigirá la audiencia.

   ![](assets/email_designer_21.png)

1. También puede cambiar los iconos de cada uno de los medios sociales si es necesario en la sección **[!UICONTROL Imagen]** campo .

1. Ajuste los demás atributos de estilo, como estilo, margen, borde, etc. de la variable **[!UICONTROL Configuración de componentes]** panel.
