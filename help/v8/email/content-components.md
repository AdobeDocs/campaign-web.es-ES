---
audience: end-user
title: Uso de los componentes de contenido del diseñador de correo electrónico
description: Aprenda a utilizar los componentes de contenido en los correos electrónicos
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 65%

---

# Usar componentes de contenido {#content-components}

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="Acerca del contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de un correo electrónico."

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="Acerca del contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de una página de aterrizaje."

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="Acerca del contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que puede utilizar para crear el diseño de un fragmento de contenido."

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="Acerca del contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de una plantilla."

Al crear el contenido del correo electrónico, los componentes **[!UICONTROL Contenido]** le permiten personalizar aún más el correo electrónico con componentes sin procesar y vacíos que puede utilizar una vez colocados en un correo electrónico.

Puede agregar tantos **[!UICONTROL Contenidos]** como necesite dentro de una **[!UICONTROL Estructura]**, que define el diseño del correo electrónico.

## Añadir componentes de contenido {#add-content-components}

Para añadir componentes de contenido al correo electrónico y ajustarlos a sus necesidades, siga los pasos a continuación.

1. En el Designer de correo electrónico, usa un [contenido existente](existing-content.md) o arrastra y suelta una **[!UICONTROL Estructura]** en el contenido vacío para definir el diseño del correo electrónico. [Descubra cómo](create-email-content.md)

1. Arrastre y suelte el **[!UICONTROL Contenido]** de su elección dentro de las estructuras relevantes.

   ![](assets/email_designer_add_content_components.png){zoomable="yes"}

   >[!NOTE]
   >
   >Puede añadir varios componentes en una sola estructura y en cada columna de una estructura.

1. Ajuste las opciones de cada componente con la ficha **[!UICONTROL Configuración]** contextual. Por ejemplo, puede elegir mostrarlo solo en equipos de escritorio o dispositivos móviles, o en ambos. También puede administrar las opciones de vínculo desde esta pestaña. [Más información sobre la administración de vínculos](message-tracking.md)

1. Ajuste los atributos de estilo de cada componente mediante la ficha **[!UICONTROL Style]**. Por ejemplo, puede cambiar el estilo, el relleno o el margen del texto de cada componente. [Obtenga más información sobre la alineación y el relleno](alignment-and-padding.md)

   ![](assets/email_designer_content_components_settings.png){zoomable="yes"}

1. Desde el menú avanzado de su **[!UICONTROL Contenido]** en el panel derecho, puede eliminar o duplicar fácilmente cualquier componente de contenido según sea necesario.

## Contenedor {#container}

Puede añadir un contenedor simple dentro del cual añadir otro componente de contenido. Esto le permite aplicar un estilo específico al contenedor, que es diferente del componente utilizado adentro.

Por ejemplo, agregue el componente **[!UICONTROL Contenedor]** y el componente [Botón](#button) dentro de ese contenedor. Puede utilizar un fondo específico para el contenedor y otro para el botón.

![](assets/email_designer_container_component.png){zoomable="yes"}

## Botón {#buttons}

Utilice el componente **[!UICONTROL Botón]** para insertar uno o varios botones en el correo electrónico y redirigir el público de correo electrónico a otra página.

1. En la lista **[!UICONTROL Contenidos]**, arrastre y suelte el componente **[!UICONTROL Botón]** en un componente de **[!UICONTROL Estructura]**.

   ![](assets/email_designer_13.png){zoomable="yes"}

1. Haga clic en el botón recién añadido para personalizar el texto y tener acceso a las pestañas **[!UICONTROL Configuración]** y **[!UICONTROL Estilos]**.

   ![](assets/email_designer_14.png){zoomable="yes"}

1. Desde las pestañas **[!UICONTROL Configuración]**, en el campo **[!UICONTROL URL]**, añada la dirección URL a la que desee redirigir al hacer clic en el botón.

1. Elija cómo se muestra el contenido con la lista desplegable **[!UICONTROL Destinatario]**

   * **[!UICONTROL Ninguna]**: abre el vínculo en el mismo marco en el que se hizo clic (predeterminado).
   * **[!UICONTROL En blanco]**: abre el vínculo en una nueva ventana o pestaña.
   * **[!UICONTROL Propio]**: abre el vínculo en el mismo marco en el que se hizo clic.
   * **[!UICONTROL Principal]**: abre el vínculo en el marco principal.
   * **[!UICONTROL Superior]**: abre el vínculo en todo el cuerpo de la ventana.

   ![](assets/email_designer_15.png){zoomable="yes"}

1. Puede personalizar aún más el botón cambiando atributos de estilo como **[!UICONTROL Borde]**, **[!UICONTROL Tamaño]**, **[!UICONTROL Margen]**, etc. de la ficha **[!UICONTROL Estilos]**.

## Texto {#text}

Utilice el componente **[!UICONTROL Texto]** para insertar texto en el correo electrónico y ajustar el estilo (borde, tamaño, relleno, etc.) uso de las pestañas **[!UICONTROL Configuración]** y **[!UICONTROL Estilos]**.

1. En el menú **[!UICONTROL Contenido]**, arrastre y suelte **[!UICONTROL Texto]** en un componente **[!UICONTROL Estructura]**.

   ![](assets/email_designer_11.png){zoomable="yes"}

1. Haga clic en el componente recién agregado para personalizar el texto y tener acceso a las pestañas **[!UICONTROL Configuración]** y **[!UICONTROL Estilos]**.

1. Cambie el texto con las siguientes opciones disponibles en la barra de herramientas contextual:

   ![](assets/email_designer_27.png){zoomable="yes"}

   * **[!UICONTROL Cambiar estilo de texto]**: aplicar negrita, cursiva, subrayado o tachado al texto.
   * **Cambiar alineación**: elegir entre alineación izquierda, derecha, centro o justificada para el texto.
   * **[!UICONTROL Crear lista]**: añadir viñetas o listas numéricas al texto.
   * **[!UICONTROL Definir encabezado]**: añadir hasta seis niveles de encabezado al texto.
   * **Tamaño de fuente**: seleccionar el tamaño de fuente del texto en píxeles.
   * **[!UICONTROL Editar imagen]**: añadir una imagen o un recurso al componente de texto.
   * **[!UICONTROL Mostrar el código fuente]**: mostrar el código fuente del texto. No se puede modificar.
   * **[!UICONTROL Duplicar]**: añadir una copia del componente de texto.
   * **[!UICONTROL Eliminar]**: eliminar el componente de texto seleccionado del correo electrónico.
   * **[!UICONTROL Añadir personalización]**: añadir campos de personalización para personalizar el contenido de los datos de perfiles.
   * **[!UICONTROL Habilitar contenido condicional]**: añadir contenido condicional para adaptar el contenido del componente a los perfiles de destino.

1. Ajuste los demás atributos de estilo, como el color del texto, la familia de fuentes, el borde, el relleno, el margen, etc. de la ficha **[!UICONTROL Estilos]**.

   ![](assets/email_designer_12.png){zoomable="yes"}

## Divisor {#divider}

Utilice el componente **[!UICONTROL Divisor]** para insertar una línea divisoria y organizar el diseño y el contenido del correo electrónico.

Puede ajustar atributos de estilo como el color, el estilo y la altura de la línea desde la pestaña **[!UICONTROL Estilos]**.

![](assets/email_designer_16.png){zoomable="yes"}

## HTML {#HTML}

Utilice el componente **[!UICONTROL HTML]** para copiar y pegar las diferentes partes del HTML existente. Esto le permite crear componentes de HTML modulares gratuitos para reutilizar contenido externo.

1. En **[!UICONTROL Componentes]**, arrastre y suelte el componente **[!UICONTROL HTML]** en un componente de **[!UICONTROL Estructura]**.

   ![](assets/email_designer_22.png){zoomable="yes"}

1. Haga clic en el componente recién agregado y, a continuación, seleccione **[!UICONTROL Mostrar el código fuente]** de la barra de herramientas contextual para añadir el HTML.

   ![](assets/email_designer_23.png){zoomable="yes"}

>[!NOTE]
>
>Para hacer que un contenido externo sea compatible con el Designer de correo electrónico, el Adobe recomienda [crear un mensaje desde cero](create-email-content.md) y copiar el contenido del correo electrónico existente en los componentes.

## Imagen {#image}

Utilice el componente **[!UICONTROL Imagen]** para insertar un archivo de imagen desde el equipo en el correo electrónico.

1. Desde el menú **[!UICONTROL Contenido]**, arrastre y suelte la **[!UICONTROL Imagen]** en un componente de **[!UICONTROL Estructura]**.

   ![](assets/email_designer_9.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Examinar]** para elegir un archivo de imagen de sus recursos. También puedes elegir **[!UICONTROL Importar tus medios]**.

   Para obtener más información sobre cómo cargar y agregar recursos en Adobe Experience Manager, consulte [Documentación de Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/add-assets.html).

   ![](assets/email_designer_28.png){zoomable="yes"}

1. Desplácese por las carpetas para localizar el recurso específico que necesita o utilice la barra de búsqueda para encontrarlo de forma eficaz.

   Cuando encuentre el recurso que busca, haga clic en **[!UICONTROL Seleccionar]**.

   ![](assets/email_designer_29.png){zoomable="yes"}

1. Haga clic en el componente que acaba de agregar y configure las propiedades de la imagen con la pestaña **[!UICONTROL Configuración]**:

   * **[!UICONTROL Título de la imagen]** permite definir un título para la imagen.
   * **[!UICONTROL Texto alternativo]** permite definir el pie de ilustración vinculado a la imagen. Esto corresponde al atributo HTML alt.

   ![](assets/email_designer_10.png){zoomable="yes"}

1. Puede añadir un vínculo para redirigir la audiencia a otro contenido. [Más información](message-tracking.md)

1. Ajuste los demás atributos de estilo como margen, borde, etc. usando la ficha **[!UICONTROL Estilos]**.

## Social {#social}

Utilice el componente **[!UICONTROL Social]** para insertar vínculos a páginas de redes sociales en el contenido del correo electrónico.

1. Desde el menú **[!UICONTROL Componentes]**, arrastre y suelte el componente **[!UICONTROL Social]** en un componente de **[!UICONTROL Estructura]**.

1. Haga clic en el componente recién añadido.

1. En el campo **[!UICONTROL Social]** de la pestaña **[!UICONTROL Configuración]**, elija los medios sociales que desea agregar o quitar.

   ![](assets/email_designer_20.png){zoomable="yes"}

1. Elija el tamaño de los iconos en el campo **[!UICONTROL Tamaño de las imágenes]**.

1. Haga clic en cada uno de sus iconos de redes sociales para configurar la **[!UICONTROL URL]** a la que se redirige su público.

   ![](assets/email_designer_21.png){zoomable="yes"}

1. También puede cambiar los iconos de cada uno de sus medios sociales si es necesario en el campo **[!UICONTROL Source]**.

1. Ajuste los demás atributos de estilo como estilo, margen, borde, etc. de la ficha **[!UICONTROL Estilos]**.
