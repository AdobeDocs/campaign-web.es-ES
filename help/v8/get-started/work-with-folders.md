---
audience: end-user
title: Trabajar con carpetas
description: Obtenga información sobre cómo administrar una carpeta en Adobe Campaign
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: 6901533f1f5c45ce9ebf77a4f1095d8476c6a21b
workflow-type: ht
source-wordcount: '721'
ht-degree: 100%

---

# Trabajo con carpetas {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="Propiedades de carpetas"
>abstract="Propiedades de carpetas"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="Seguridad de carpetas"
>abstract="Seguridad de carpetas"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="Programación de carpetas"
>abstract="Programación de carpetas"

## Acerca de las carpetas {#about-folders}

Las carpetas son objetos de Adobe Campaign que permiten organizar los componentes y los datos.

Puede crear, cambiar el nombre, reordenar y mover carpetas en el árbol de navegación. También puede eliminarlos según sus derechos.

![Interfaz de carpetas que muestra la organización de carpetas](assets/folders.png){zoomable="yes"}

Puede configurar un tipo de carpeta. Por ejemplo: una carpeta de envíos. El icono de carpeta cambia según su tipo.

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="Restricciones de carpetas"
>abstract="Las carpetas Objetos creados automáticamente y Flujos de trabajo técnicos están restringidas y no se pueden ver en el panel lateral izquierdo."

>[!IMPORTANT]
>
>Las carpetas **[!UICONTROL Objetos creados automáticamente]** y **[!UICONTROL Flujos de trabajo técnicos]** están restringidas y no se pueden ver en el panel lateral izquierdo.


## Creación de una nueva carpeta {#create-a-folder}

Para crear una carpeta nueva en la interfaz de usuario de Adobe Campaign Web, siga estos pasos:

1. En **[!UICONTROL Explorer]**, vaya a la carpeta en la que desea crear una nueva. En el menú **[!UICONTROL …]**, encontrará **[!UICONTROL Crear nueva carpeta]**

![Crear nueva opción de carpeta en el menú Explorer](assets/folder_create.png){zoomable="yes"}

Cuando crea una carpeta nueva, el tipo de carpeta predeterminado es el tipo de la carpeta principal. En este ejemplo, se crea una carpeta en la carpeta **[!UICONTROL Envíos]**.

![Nueva carpeta creada en la carpeta Envíos](assets/folder_new.png){zoomable="yes"}

1. Cambie el tipo de carpeta haciendo clic en el icono de tipo de carpeta si es necesario, y seleccione el tipo deseado de la lista presentada, como se muestra a continuación:

![Interfaz de selección de tipo de carpeta](assets/folder_type.png){zoomable="yes"}

Configure el tipo de carpeta haciendo clic en el botón **[!UICONTROL Confirmar]**.

Si desea crear una carpeta sin un tipo específico, elija el tipo **[!UICONTROL Carpeta genérica]**.

También puede [crear y administrar carpetas en la consola de Adobe Campaign](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/config/configuration/folders-and-views).

## Reordenar carpetas {#reorder-folders}

Puede reordenar las carpetas según sus necesidades. Para ello, haga clic en **[!UICONTROL Reordenar carpetas]** como se muestra a continuación.

En este ejemplo, la carpeta **Envíos** contiene cuatro subcarpetas.

![Reordenar la interfaz de carpetas que muestra la jerarquía de carpetas](assets/folder-reorder.png){zoomable="yes"}

Puede cambiar el orden de las carpetas mediante la acción de **arrastrar y soltar** o usando las **flechas arriba y abajo**

![Funcionalidad Arrastrar y soltar para reordenar las carpetas](assets/folder-draganddrop.png){zoomable="yes"}

### Carpetas favoritas {#favorite-folders}

>[!CONTEXTUALHELP]
>id="acw_folder_favorites"
>title="Favoritos"
>abstract="Sus carpetas favoritas se mostrarán en la parte superior de la pestaña izquierda."

Las carpetas que se han marcado como &quot;Favoritas&quot; siempre se mostrarán en la parte superior de la pestaña izquierda.

Puede añadir carpetas como favoritas haciendo clic en el botón con el símbolo estrella situado en la esquina superior derecha cuando visualice una carpeta.

![Captura de pantalla de la ubicación de carpetas favoritas](assets/folders-favorite.png){zoomable="yes"}

## Eliminación de una carpeta {#delete-a-folder}

>[!CAUTION]
>
>Al eliminar una carpeta, también se eliminan todos los datos almacenados en ella.

Para eliminar una carpeta, selecciónela en el árbol de **[!UICONTROL Explorer]** y haga clic en el menú **[!UICONTROL …]**. Elija **[!UICONTROL Eliminar carpeta]**.

![Eliminar opción de carpeta en el menú de Explorer](assets/folder_delete.png){zoomable="yes"}

## Distribución de valores en una carpeta {#distribution-values-folder}

La distribución de valores ayuda a comprender el porcentaje de un valor en una columna dentro de una tabla.

Para ver la distribución de valores en una carpeta, proceda como se indica a continuación.

Por ejemplo, entre los envíos, se desea conocer la distribución de valores de la columna **Canal**.

Para obtener esta información, vaya a la carpeta **[!UICONTROL Envíos]** y haga clic en el icono **[!UICONTROL Configurar columnas]**.

En la ventana **[!UICONTROL Configurar columnas]**, haga clic en el icono **[!UICONTROL Información]** de la columna de la que desee información. A continuación, haga clic en el botón **[!UICONTROL Distribución de valores]**.

![Interfaz de distribución de valores para envíos](assets/values_deliveries.png){zoomable="yes"}

Obtendrá el porcentaje de los valores de la columna **[!UICONTROL Canal]**.

![Distribución porcentual de los valores en la columna Canal](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
>Para las columnas con muchos valores, solo se mostrarán los primeros veinte valores. Una notificación de **[!UICONTROL Carga parcial]** le avisa de esto.

También puede ver la distribución de valores de un vínculo.

En la lista de atributos, haga clic en el botón **+** situado junto al vínculo deseado, como se muestra a continuación. Esto añade el vínculo a las **[!UICONTROL Columnas de salida]**. Ahora puede acceder al icono **[!UICONTROL Información]**, que le permite ver la distribución de sus valores. Si no desea mantener el vínculo en las **[!UICONTROL Columnas de salida]**, haga clic en el botón **[!UICONTROL Cancelar]**.

![Distribución de valores de un vínculo en columnas de resultados](assets/values_link.png){zoomable="yes"}

También es posible visualizar la distribución de valores en un modelador de consultas. [Más información aquí](../query/build-query.md#distribution-of-values-in-a-query).

### Filtro de los valores {#filter-values}

Mediante los **[!UICONTROL filtros avanzados]** en la ventana de distribución de valores, puede filtrar los resultados según las condiciones especificadas.

En el ejemplo de la lista de envíos anterior, que muestra la distribución por canal, puede filtrarla para mostrar solo los envíos con el estado **Finalizado**.

![Filtros avanzados aplicados a la distribución de valores](assets/values_filter.png){zoomable="yes"}