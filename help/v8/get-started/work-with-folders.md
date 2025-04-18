---
audience: end-user
title: Trabajar con carpetas
description: Obtenga información sobre cómo administrar una carpeta en Adobe Campaign
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 25%

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
>id="acw_folder_restrictions"
>title="Restricciones de carpetas"
>abstract="Restricciones de carpetas"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="Programación de carpetas"
>abstract="Programación de carpetas"

## Acerca de las carpetas {#about-folders}

Las carpetas son objetos de Adobe Campaign que permiten organizar los componentes y los datos.

Puede crear, cambiar el nombre, reordenar y mover carpetas en el árbol de navegación. También puede eliminarlos en función de sus derechos.

![Interfaz de carpetas que muestra la organización de carpetas](assets/folders.png){zoomable="yes"}

Puede configurar un tipo de carpeta. Por ejemplo, una carpeta de envíos. El icono de carpeta cambia según su tipo.

## Creación de una nueva carpeta {#create-a-folder}

Para crear una carpeta nueva en la interfaz de usuario de Adobe Campaign Web, siga estos pasos:

1. En **[!UICONTROL el Explorador]**, vaya a la carpeta donde desea crear la nueva carpeta. En el **[!UICONTROL menú ...]** , seleccione **[!UICONTROL Crear nueva carpeta]**.

![Crear nueva opción de carpeta en el menú del Explorador](assets/folder_create.png){zoomable="yes"}

Al crear una carpeta nueva, el tipo de carpeta toma como valor predeterminado el tipo de carpeta principal. En este ejemplo, se crea una carpeta en la **[!UICONTROL carpeta Deliverys]** .

![Nueva carpeta creada en la carpeta Envíos](assets/folder_new.png){zoomable="yes"}

1. Cambie el tipo de carpeta haciendo clic en el icono de tipo de carpeta si es necesario y seleccione el tipo deseado en la lista presentada, como se muestra a continuación:

![Interfaz de selección de tipo Carpeta](assets/folder_type.png){zoomable="yes"}

Para configurar el tipo de carpeta, haga clic en Confirmar **** botón.

Si desea crear una carpeta sin un tipo específico, seleccione el **[!UICONTROL tipo de Carpeta]** genérico.

También puede [crear y administrar carpetas en la consola de Adobe Campaign](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/config/configuration/folders-and-views).

## Reordenar carpetas {#reorder-folders}

Puede cambiar el orden de las carpetas según sus necesidades. Para hacerlo, haga clic en Reordenar **[!UICONTROL carpetas]**, como se muestra a continuación.

En este ejemplo, la **carpeta Deliveries** contiene cuatro subcarpetas.

![Reordenar la interfaz de carpetas que muestra la jerarquía de carpetas](assets/folder-reorder.png){zoomable="yes"}

Puede cambiar el orden de las carpetas arrastrando y soltando **o usando** flechas arriba y abajo **.**

![Funcionalidad de arrastrar y soltar para reordenar carpetas](assets/folder-draganddrop.png){zoomable="yes"}

## Eliminación de una carpeta {#delete-a-folder}

>[!CAUTION]
>
>Al eliminar una carpeta, también se eliminan todos los datos almacenados en ella.

Para eliminar una carpeta, selecciónela en el **[!UICONTROL árbol del explorador]** y haga clic en el **[!UICONTROL menú...]** Elija **[!UICONTROL Eliminar carpeta]**.

![Eliminar opción de carpeta en el menú del Explorador](assets/folder_delete.png){zoomable="yes"}

## Distribución de valores en una carpeta {#distribution-values-folder}

La distribución de valores ayuda a comprender el porcentaje de un valor en una columna dentro de una tabla.

Para vista la distribución de valores en una carpeta, proceda como se explica a continuación.

Por ejemplo, entre las entregas, es posible que desee conocer la distribución de los valores en la columna **Canal**.

Para obtener esta información, vaya a la carpeta **[!UICONTROL Deliveries]** y haga clic en el icono **[!UICONTROL Configurar columnas]**.

En la ventana **[!UICONTROL Configurar columnas]**, haga clic en el icono **[!UICONTROL Información]** relacionado con la columna que desea analizar. A continuación, haga clic en el botón **[!UICONTROL Distribución de valores]**.

![Distribución de la interfaz de valores para los envíos](assets/values_deliveries.png){zoomable="yes"}

Verá el porcentaje de valores en la **[!UICONTROL columna Canal]** .

![Distribución porcentual de los valores en la columna Canal](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
>Para las columnas con muchos valores, solo se muestran los veinte primeros valores. Una notificación **[!UICONTROL Carga parcial]** le advierte.

También puede ver la distribución de los valores de un vínculo.

En la lista de atributos, haga clic en el botón **+** situado junto al vínculo deseado, como se muestra a continuación. Esto añade el vínculo a las **[!UICONTROL Columnas de salida]**. Ahora puede acceder al **[!UICONTROL icono Información]** , lo que le permite vista la distribución de sus valores. Si no desea mantener la vincular en las **[!UICONTROL columnas]** Output, haga clic en la **[!UICONTROL botón Cancelar]** .

![Distribución de valores de un vincular en Output columnas](assets/values_link.png){zoomable="yes"}

También es posible vista la distribución de valores en un modelador de consulta. [Más información aquí](../query/build-query.md#distribution-of-values-in-a-query).

### Filtro de los valores {#filter-values}

Mediante el **[!UICONTROL filtros]** Avanzadas en la ventana de distribución de valores, puede filtrar los resultados en función de condiciones especificadas.

En el ejemplo del envío lista anterior, que muestra la distribución por canal, puede filtrarlo para mostrar solo las entregas con el estado Finished ****.

![Filtros avanzados aplicados a la distribución de valores](assets/values_filter.png){zoomable="yes"}