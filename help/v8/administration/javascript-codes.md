---
title: Trabajo con códigos JavaScript
description: Aprenda a trabajar con códigos JavaScript.
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 2%

---


# Trabajo con códigos JavaScript {#javascript-codes}

<!-- JavaScript codes -->

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_list"
>title="Códigos JavaScript"
>abstract="Códigos JavaScript"

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_create"
>title="Crear código JavaScript"
>abstract="Crear código JavaScript"

## Acerca de los códigos JavaScript {#about}

Los códigos JavaScript permiten crear funciones reutilizables que se pueden utilizar en distintos flujos de trabajo, de forma similar a una biblioteca. Estas funciones se almacenan en el menú **[!UICONTROL Administración]** > **[!UICONTROL Códigos JavaScript]** del panel de navegación izquierdo.

![](assets/javascript-list.png)

Desde la lista JavaScript codes, puede:

* **Duplicar o eliminar un código**: haga clic en el botón de puntos suspensivos y seleccione la acción que desee.
* **Modificar un código**: haga clic en el nombre de un código para abrir sus propiedades. Realice los cambios y guarde los cambios.
* **Crear un nuevo código JavaScript**: Haz clic en el botón **[!UICONTROL Crear código JavaScript]**.

>[!NOTE]
>
>Aunque la ubicación del menú de códigos JavaScript difiere entre la consola de Adobe Campaign y la interfaz de usuario web, la lista es idéntica y funciona como un reflejo.

## Creación de un código JavaScript {#create}

Para crear un código JavaScript, siga estos pasos:

1. Vaya al menú **[!UICONTROL JavaScript codes]** y haga clic en el botón **[!UICONTROL Crear código JavaScript]**.

1. Defina las propiedades del código:

   * **[!UICONTROL Espacio de nombres]**: especifique el espacio de nombres relevante para los recursos personalizados. De forma predeterminada, el área de nombres es &quot;cus&quot;, pero puede variar según la implementación.
   * **[!UICONTROL Nombre]**: El identificador único que se va a usar para hacer referencia al código.
   * **[!UICONTROL Etiqueta]**: La etiqueta descriptiva que se mostrará en la lista de códigos JavaScript.

   ![](assets/javascript-create.png)

   >[!NOTE]
   >
   >Una vez creados, los campos **[!UICONTROL Namespace]** y **[!UICONTROL Name]** no se pueden modificar. Para realizar cambios, duplique el código y actualícelo según sea necesario.
   >
   >En la consola de Campaign, el nombre del código JavaScript aparece como una concatenación de estos dos campos.

1. Haga clic en el botón **[!UICONTROL Crear código]** para definir el código JavaScript. El panel izquierdo incluye dos menús que permiten utilizar funciones predefinidas relacionadas con las condiciones y el formato de fecha.

   ![](assets/javascript-code.png)

1. Haga clic en **[!UICONTROL Confirmar]** para guardar el código.

1. Cuando el código de JavaScript esté listo, haz clic en **[!UICONTROL Crear]**.  El código JavaScript ya está disponible para su uso en todos los flujos de trabajo.

## Uso de un código JavaScript de un flujo de trabajo {#workflow}

### Carga de bibliotecas de código JavaScript {#library}

Puede hacer referencia a códigos JavaScript en los flujos de trabajo para evitar que se vuelva a escribir el código para tareas repetitivas. Para utilizar estos códigos, primero debe cargar la biblioteca correspondiente en el script de inicialización del flujo de trabajo. Esto le permite cargar una vez todas las bibliotecas que contienen las funciones que desea utilizar en el flujo de trabajo.

Para cargar una biblioteca, siga estos pasos:

1. Abra un flujo de trabajo y haga clic en el botón **[!UICONTROL Configuración]**.
1. Vaya a la sección **[!UICONTROL Script de inicialización]** y haga clic en **[!UICONTROL Crear código]**.

   ![](assets/javascript-initialization.png)

1. Utilice la sintaxis siguiente en el código para cargar una biblioteca:

   ```
   loadLibrary("/<namespace>/<name>")
   ```

   * Reemplace `<namespace>` por el área de nombres especificado durante la creación del código de JavaScript.
   * Reemplace `<name>` con el nombre del código JavaScript.

1. Haga clic en **[!UICONTROL Confirmar]** y guarde la configuración.

### Funciones de referencia en flujos de trabajo {#reference}

Una vez cargada la biblioteca JavaScript, puede hacer referencia a las funciones definidas en el código JavaScript directamente dentro del flujo de trabajo, por lo general mediante una actividad **[!UICONTROL JavaScript code]**.

![](assets/javascript-function.png)
