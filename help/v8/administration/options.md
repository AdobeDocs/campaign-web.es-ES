---
title: Configurar  [!DNL Campaign] opciones
description: Obtenga información sobre cómo configurar las opciones de Campaign y crear sus propias opciones personalizadas.
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---


# Configurar las opciones de [!DNL Campaign] {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Opciones"
>abstract="Opciones"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Opción Crear"
>abstract="Opción Crear"

Adobe Campaign Web incluye opciones técnicas que le permiten configurar la aplicación de forma más específica. Algunas de estas opciones están integradas, mientras que otras se pueden añadir manualmente según sea necesario.

>[!IMPORTANT]
>
>Las opciones integradas están preconfiguradas y solo deben modificarlas los usuarios avanzados. Si tiene alguna pregunta o solicitud, póngase en contacto con el representante del Adobe.

## Acceso a opciones de Campaign {#access}

Las opciones están disponibles en el menú **[!UICONTROL Administración]** / **[!UICONTROL Opciones]**. Utilice el panel de filtros para reducir la lista y encontrar rápidamente la opción que necesita.

![](assets/options-list.png)

>[!NOTE]
>
>Aunque la ubicación del menú de opciones difiere entre la consola de Adobe Campaign y la interfaz de usuario web, la lista es idéntica y funciona como un reflejo. Para obtener más información sobre las opciones disponibles, consulte la lista de opciones en [Documentación de Campaign v7](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}

En la lista de opciones, puede:

* **Duplicar o eliminar una opción**: haga clic en el botón de puntos suspensivos y seleccione la acción que desee.
* **Modificar una opción**: haga clic en el nombre de la opción para abrir sus propiedades. Realice los cambios y guarde los cambios.
* **Crear una opción personalizada**: haga clic en el botón **[!UICONTROL Crear opción]**.

## Crear una opción {#create}

La interfaz de usuario web de Adobe Campaign le permite crear sus propias opciones personalizadas para adaptarlas a sus necesidades. Esto es especialmente útil cuando se trabaja con **[!UICONTROL JavaScript code]** actividades de flujo de trabajo para almacenar datos intermedios.

Para crear una opción:

1. Acceda a la lista de opciones y haga clic en **[!UICONTROL Crear opción]**.
1. Introduzca un nombre para la opción, seleccione su tipo y defina el valor deseado.
1. Haga clic en **[!UICONTROL Crear]** para crear la opción.

   ![](assets/options-create.png)

Las opciones pueden actuar como un espacio de almacenamiento temporal para los datos, lo que proporciona las siguientes ventajas:

* Valores Escritos: Las opciones admiten tipos de datos específicos, como fechas, números enteros, cadenas...
* Flexibilidad: las opciones permiten a los usuarios almacenar y recuperar datos de forma eficaz sin la sobrecarga que supone la administración de tablas de base de datos.

En el ejemplo siguiente, creamos una opción personalizada denominada `sampleOption` con el valor inicial &quot;a&quot;. Una actividad **[!UICONTROL JavaScript code]** en un flujo de trabajo modifica el valor de esta opción y la almacena en una variable. El valor actualizado se muestra en los registros del flujo de trabajo y se refleja en el menú **[!UICONTROL Opciones]**.

1. Cree la opción.

   ![](assets/options-sample-create.png)

1. Configure una actividad **[!UICONTROL JavaScript code]** e inicie el flujo de trabajo.

   ![](assets/options-sample-javascript.png)

1. Ejecute el flujo de trabajo para ver el valor actualizado en los registros de flujo de trabajo.

   ![](assets/options-sample-logs.png)

1. El valor actualizado ahora está visible en el menú **[!UICONTROL Opciones]**.

   ![](assets/options-sample-updated.png)
