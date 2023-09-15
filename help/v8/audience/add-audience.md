---
audience: end-user
title: Selección de una audiencia existente
description: Obtenga información sobre cómo seleccionar una audiencia
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: d05b6f9fec0e56f90d3fe51014fc11d2ed87bb66
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 50%

---


# Selección de una audiencia existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selección de una audiencia existente"
>abstract="Examine la lista para seleccionar una audiencia existente. Utilice el icono &quot;Mostrar filtros&quot; para filtrar la lista o seleccionar una carpeta específica."

En esta sección se explica cómo seleccionar una audiencia existente al definir la población objetivo de un envío de correo electrónico.

También puede realizar lo siguiente:

* Crear una audiencia nueva. [Más información](segment-builder.md)
* Cargar una audiencia desde un archivo externo (solo para correos electrónicos). [Más información](file-audience.md)
* Usar una audiencia de Adobe Experience Platform. [Más información](aep-audience.md).


Para seleccionar una audiencia existente para el mensaje, siga los pasos a continuación:

1. En la sección **Audiencia** del asistente de creación de envíos, haga clic en el botón **[!UICONTROL Seleccionar la audiencia]**.

   ![](assets/create-audience.png)

1. Elija **[!UICONTROL Seleccionar la audiencia]** para usar una audiencia existente. Para crear una nueva audiencia para usarla en este correo electrónico, elija **Crear la suya propia**. Consulte esta [sección](segment-builder.md).

   Esta pantalla muestra todas las audiencias existentes, para la carpeta actual.

   ![](assets/create-audience2.png)

   Las audiencias se crean a partir de **Audiencia** menú izquierdo. También se pueden crear en la consola del cliente.

   Para utilizar audiencias de Adobe Experience Platform, debe configurar la integración con Destinos. Consulte la [Documentación de destinos de Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=es){target="_blank"}.

   >[!IMPORTANT]
   >
   >En esa versión del producto, al crear reglas, seleccionar la audiencia de una entrega o al crear una audiencia en un flujo de trabajo, algunos filtros predefinidos no están disponibles en la interfaz de usuario. Aún puede usarlos. [Más información](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

1. Elija una audiencia y haga clic en **Seleccionar**.
1. Utilice el **Mostrar filtros** para mostrar las opciones de filtrado. Clic **Agregar reglas** para acceder al generador de reglas: el uso del generador de reglas permite crear filtros avanzados para la lista de audiencias. Aprenda a utilizar el generador de reglas en esta [sección](segment-builder.md).

   ![](assets/create-audience4.png)

1. Haga clic en **Save**.

También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibe el mensaje. Esto le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. Obtenga más información en [esta sección](control-group.md).