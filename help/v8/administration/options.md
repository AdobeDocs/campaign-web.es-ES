---
title: 'Configurar opciones de  [!DNL Campaign] '
description: Obtenga información sobre cómo configurar las opciones de Campaign y crear sus propias opciones personalizadas.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Configurar opciones de [!DNL Campaign] {#options}

>[!CONTEXTUALHELP]
>
[!CONTEXTUALHELP]

Adobe Campaign Web incluye opciones técnicas que permiten configurar la aplicación de forma más específica. Algunas de estas opciones están integradas, mientras que otras se pueden añadir manualmente según sea necesario.

>[!IMPORTANT]\
Las opciones integradas están preconfiguradas y solo deben modificarlas los usuarios avanzados. Si tiene alguna pregunta o solicitud, póngase en contacto con su representante de Adobe.

## Acceso a opciones de Campaign {#access}

Las opciones están disponibles en el menú **[!UICONTROL Administración]** / **[!UICONTROL Opciones]**. Utilice el panel de filtros para reducir la lista y localizar rápidamente la opción que necesite.

![](assets/options-list.png)\
[Lista de opciones mostrada en el menú Administración / Opciones]

>[!NOTE]\
Aunque la ubicación del menú de opciones difiere entre la consola de Adobe Campaign y la interfaz de usuario web, la lista es idéntica y funciona como un reflejo. Para obtener más información sobre las opciones disponibles, consulte la lista de opciones en [Documentación de Campaign v7](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}.

En la lista de opciones, puede:

* **Duplicar o eliminar una opción**: haga clic en el botón de puntos suspensivos y seleccione la acción que desee.
* **Modificar una opción**: haga clic en el nombre de la opción para abrir sus propiedades. Realice los cambios y guarde los cambios.
* **Crear una opción personalizada**: haga clic en el botón **[!UICONTROL Crear opción]**.

## Crear una opción {#create}

La interfaz de usuario web de Adobe Campaign le permite crear opciones personalizadas para satisfacer sus necesidades. Esto es especialmente útil cuando se trabaja con **[!UICONTROL JavaScript code]** actividades de flujo de trabajo para almacenar datos intermedios.

Para crear una opción:

1. Acceda a la lista de opciones y haga clic en **[!UICONTROL Crear opción]**.
1. Introduzca un nombre para la opción, seleccione su tipo y defina el valor deseado.
1. Haga clic en **[!UICONTROL Crear]** para crear la opción.

![Crear interfaz de opciones que muestra campos para nombre, tipo y valor](assets/options-create.png)

Las opciones pueden actuar como almacenamiento temporal de datos, lo que ofrece las siguientes ventajas:

* Valores ingresados: las opciones admiten tipos de datos específicos, como fechas, números enteros, cadenas, etc.
* Flexibilidad: las opciones permiten a los usuarios almacenar y recuperar datos de forma eficaz sin la sobrecarga que supone la administración de tablas de base de datos.

En el ejemplo siguiente, se crea una opción personalizada denominada `sampleOption` con el valor inicial &quot;a&quot;. Una actividad **[!UICONTROL JavaScript code]** en un flujo de trabajo modifica el valor de esta opción y la almacena en una variable. El valor actualizado se muestra en los registros del flujo de trabajo y se refleja en el menú **[!UICONTROL Opciones]**.

1. Cree la opción.

   ![Interfaz de creación de opciones personalizadas que muestra el nombre `sampleOption` y el valor inicial &quot;a&quot;](assets/options-sample-create.png)

1. Configure una actividad **[!UICONTROL JavaScript code]** e inicie el flujo de trabajo.

   ![Interfaz de configuración de actividad de código JavaScript](assets/options-sample-javascript.png)

1. Ejecute el flujo de trabajo para ver el valor actualizado en los registros de flujo de trabajo.

   ![Registros de trabajo que muestran el valor actualizado de la opción personalizada](assets/options-sample-logs.png)

1. El valor actualizado ahora está visible en el menú **[!UICONTROL Opciones]**.

   ![Menú de opciones que muestra el valor actualizado de la opción personalizada](assets/options-sample-updated.png)