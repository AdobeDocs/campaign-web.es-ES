---
audience: end-user
title: Diseño de una entrega de correo directo
description: Aprenda a diseñar su envío de correo postal con Adobe Campaign Web
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 3%

---

# Diseño del archivo de extracción {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Contenido del archivo de extracción"
>abstract="Haga clic en **Editar contenido** para empezar a diseñar el archivo de extracción requerido por su proveedor de correo postal. Esto le permite definir las propiedades del archivo, como su etiqueta y formato, y especificar las columnas que desea incluir en el archivo."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Propiedades del archivo"
>abstract="Configure las propiedades del archivo de extracción, como su nombre y formato. Puede personalizar el nombre del archivo mediante atributos de la base de datos mediante el editor de expresiones."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Contenido"
>abstract="En esta sección, especifique las columnas que desea mostrar en el archivo de extracción. Una vez finalizado, puede obtener una previsualización del archivo de extracción mediante la variable **Simular contenido** botón."

Para diseñar el contenido del archivo de extracción generado por su envío de correo postal, haga clic en **[!UICONTROL Editar contenido]** en la página de envío y, a continuación, configure las propiedades y el contenido del archivo.

## Configuración de las propiedades del archivo de extracción {#properties}

1. En el **[!UICONTROL Nombre de archivo]** , especifique el nombre que desee para el archivo de extracción. Puede personalizar el nombre del archivo mediante los atributos de la base de datos. Para ello, haga clic en el **[!UICONTROL Abrir diálogo de personalización]** para abrir el editor de expresiones. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

1. En el **[!UICONTROL Formato de archivo]** , elija el formato deseado para el archivo de extracción; **Texto**, **Texto con ancho fijo con columnas**, **CSV (Excel)** o **XML**.

1. Expanda el **[!UICONTROL Formato de extracción]** para acceder a opciones específicas relacionadas con el formato del archivo de extracción. Los valores disponibles dependen del formato seleccionado.

+++ Opciones de formato de extracción disponibles

   * **[!UICONTROL Usar primera línea como encabezado de columna]** (Formato texto/CSV (Excel)): active esta opción para utilizar la primera columna como encabezado.
   * **[!UICONTROL Separador de columnas]** (Formato de texto): especifique el carácter que se utilizará como separador de columnas en el archivo de extracción.
   * **[!UICONTROL Delimitador de cadenas]** (Formato de texto): especifica cómo delimitar cadenas en el archivo de extracción.
   * **[!UICONTROL Final de línea]** (Formato de texto): especifica cómo delimitar el final de las líneas en el archivo de extracción.
   * **[!UICONTROL Codificación]**: elija la codificación del archivo de extracción.
   * **[!UICONTROL Formato de fecha y separadores]**: especifica cómo se debe dar formato a las fechas en el archivo de extracción.
   * **[!UICONTROL Formato de número]**: especifique el formato de los números en el archivo de extracción.
   * **[!UICONTROL Exportar etiquetas en lugar de valores internos de enumeraciones]**: Active esta opción en caso de que exporte valores de enumeración y desee recuperar etiquetas de columnas, que son más fáciles de entender, en lugar de ID internos.

+++

1. Alternar en **[!UICONTROL Cantidad solicitada]** para restringir el número de destinatarios de su envío.

   ![](assets/dm-content-details.png){zoomable=&quot;yes&quot;}

## Configuración de las columnas del archivo de extracción {#content}

En el **[!UICONTROL Contenido]** , especifique las columnas que se mostrarán en el archivo de extracción. Para ello, siga estos pasos:

1. Haga clic en **[!UICONTROL Añadir atributo]** para crear una nueva columna.
1. Seleccione el atributo que se mostrará en la columna y confirme la acción. Una vez añadida la columna, puede cambiar su etiqueta y modificar el atributo asociado con el icono de edición.
1. Repita estos pasos para agregar tantas columnas como sea necesario para el archivo de extracción.
1. Para ordenar el archivo de extracción con una de las columnas, haga clic en el icono en la **[!UICONTROL Ordenando]** y seleccione el método de clasificación deseado.
1. Para cambiar la posición de una columna, utilice las flechas arriba y abajo.

![](assets/dm-content-attributes.png)

Ahora puede obtener una vista previa del archivo de extracción y realizar la entrega para generar el archivo de extracción. [Obtenga información sobre cómo probar y enviar mensajes de correo directo](send-direct-mail.md)
