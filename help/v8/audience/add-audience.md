---
audience: end-user
title: Selección de un público existente
description: Obtenga información sobre cómo seleccionar un público
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 12%

---

# Selección de un público existente {#add-audience}

>[!CONTEXTUALHELP]
>
En esta sección se explica cómo seleccionar una audiencia existente al definir la población objetivo de una entrega. Al definir el objetivo principal de una entrega, también puede:
* [Cree una audiencia única](one-time-audience.md) con el modelador de consultas.
* [Cargar una audiencia desde un archivo externo](file-audience.md) (solo para correos electrónicos).

Se puede acceder a las audiencias a las que se pueden dirigir los envíos desde el menú de la izquierda **Audiencia**. Se originan en varias fuentes, como la consola del cliente, los flujos de trabajo de audiencia web de Campaign o Adobe Experience Platform. [Más información sobre los públicos](manage-audience.md)

Para seleccionar un público existente para el mensaje, siga los pasos a continuación:

1. En la sección **Audience** del asistente de creación de envíos, haga clic en el botón **[!UICONTROL Seleccionar audiencia]** y, a continuación, elija **[!UICONTROL Seleccionar audiencia]**.

   [Esta captura de pantalla muestra el botón **Seleccionar audiencia** en el asistente de creación de envíos.](assets/create-audience.png){zoomable="yes"}

1. Esta pantalla muestra todas las audiencias existentes para la carpeta actual.

   [Esta captura de pantalla muestra la lista de audiencias existentes en la carpeta actual.](assets/create-audience2.png){zoomable="yes"}

   Para elegir una audiencia de Adobe Experience Platform, vaya a `AEP Audiences folder` desde la sección de filtros de la pantalla. [Más información sobre las audiencias de Adobe Experience Platform](manage-audience.md#monitor)

   [Esta captura de pantalla muestra la sección de filtros con la carpeta Audiencias de AEP seleccionada.](assets/select-audience-folder.png){zoomable="yes"}

1. La sección de filtro le permite acceder a las opciones de filtrado para restringir la lista de audiencias. Para ello, haga clic en **Agregar reglas** para acceder al modelador de consultas, que le permite crear filtros avanzados para la lista de audiencias. [Aprenda a utilizar el modelador de consultas](../query/query-modeler-overview.md)

   Por ejemplo, puede definir una regla para filtrar el origen de las audiencias, como se muestra a continuación:

   [Esta captura de pantalla muestra un filtro aplicado a las audiencias según su origen.](assets/filter-on-aep-audience.png){zoomable="yes"}

1. Haga clic en **Confirmar** para agregar su audiencia como destino principal de la entrega. Una vez finalizado, puede refinar la audiencia mediante el modelador de consultas si hace clic en el botón **Editar reglas**.

   [Esta captura de pantalla muestra el botón **Editar reglas** para perfeccionar la audiencia.](assets/refine-audience.png){zoomable="yes"}

1. También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibe el mensaje. Esto le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. [Más información](control-group.md)