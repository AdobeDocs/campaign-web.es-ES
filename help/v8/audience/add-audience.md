---
audience: end-user
title: Selección de un público existente
description: Obtenga información sobre cómo seleccionar un público
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 18%

---

# Selección de un público existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selección de un público existente"
>abstract="Examine la lista para seleccionar un público existente. Utilice el icono “Mostrar filtros” para filtrar la lista o seleccionar una carpeta específica."

En esta sección se explica cómo seleccionar una audiencia existente al definir la población destino de una envío. Al definir el destino principal de una envío, también puede:
* [Cree una audiencia](one-time-audience.md) única utilizando el consulta modelador.
* [Cargue un audiencia desde un archivo](file-audience.md) externo (solo para correo electrónico).

Audiences que se pueden segmentar en los envíos están accesibles desde el **menú Audiencia** izquierda. Se originan en múltiples fuentes, como la consola del cliente, Campaign audiencia web flujos de trabajo o Adobe Experience Platform. [Más información sobre los públicos](manage-audience.md)

Para seleccionar un público existente para el mensaje, siga los pasos a continuación:

1. En la **sección Audiencia** del asistente de creación de envío, haz clic en el **[!UICONTROL botón Seleccionar audiencia]** y, a continuación, selecciona **[!UICONTROL Seleccionar audiencia]**.

   [Este captura de pantalla muestra el **botón Seleccionar audiencia** en el asistente de creación de envío.](assets/create-audience.png){zoomable="yes"}

1. En esta pantalla se muestran todas las audiencias existentes para la carpeta actual.

   [Este captura de pantalla muestra el lista de audiencias existentes en la carpeta actual.](assets/create-audience2.png){zoomable="yes"}

   Para elegir un audiencia de Adobe Experience Platform, vaya a la `AEP Audiences folder` sección desde el filtro de la pantalla. [Más información sobre Adobe Experience Platform audiencias](manage-audience.md#monitor)

   [Este captura de pantalla muestra la sección del filtro con la carpeta Audiences de AEP seleccionada.](assets/select-audience-folder.png){zoomable="yes"}

1. La sección de filtros permite acceder a opciones de filtrado para restringir el lista de audiencias. Para ello, haga clic en **añadir reglas** para acceder al consulta modelador, que le permite crear filtros avanzadas para el lista de audiencias. [Aprenda a utilizar el modelador de consulta](../query/query-modeler-overview.md)

   Por ejemplo, puede definir una regla para filtrar según la origen de audiencias, como se muestra a continuación:

   [Este captura de pantalla muestra un filtro aplicado a las audiencias en función de su origen.](assets/filter-on-aep-audience.png){zoomable="yes"}

1. Haga clic en **Confirmar** para agregar su audiencia como el destino principal de envío. Una vez finalizado, puede restringir el audiencia utilizando el modelador de consulta haciendo clic en el botón de reglas de **Editar** .

   [Este captura de pantalla muestra las **reglas Editar botón** para perfeccionar el audiencia.](assets/refine-audience.png){zoomable="yes"}

1. También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibe el mensaje. Esto permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo recibieron. [Más información](control-group.md)