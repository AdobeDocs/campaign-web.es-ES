---
audience: end-user
title: Selección de un público existente
description: Obtenga información sobre cómo seleccionar un público
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Disponibilidad limitada"
source-git-commit: 703196ad2bb504eb1d50008af110f952d8045eaa
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 31%

---


# Selección de un público existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selección de un público existente"
>abstract="Examine la lista para seleccionar un público existente. Utilice el icono “Mostrar filtros” para filtrar la lista o seleccionar una carpeta específica."

En esta sección se explica cómo seleccionar una audiencia existente al definir la población objetivo de una entrega. Al definir el objetivo principal de una entrega, también puede:

* [Crear una audiencia única](one-time-audience.md) uso del modelador de consultas.
* [Carga de una audiencia desde un archivo externo](file-audience.md) (solo para correos electrónicos).

Se puede acceder a las audiencias a las que se pueden dirigir los envíos desde el **Audiencia** menú izquierdo. Se originan en varias fuentes, como la consola del cliente, los flujos de trabajo de audiencia web de Campaign o Adobe Experience Platform. [Obtenga información sobre cómo monitorizar y administrar audiencias](manage-audience.md)

Para seleccionar un público existente para el mensaje, siga los pasos a continuación:

1. Desde el **Audiencia** del asistente de creación de entregas, haga clic en **[!UICONTROL Seleccionar audiencia]** y luego elija **[!UICONTROL Seleccionar audiencia]** para utilizar una audiencia existente.

   ![](assets/create-audience.png)

1. Esta pantalla muestra todas las audiencias existentes, para la carpeta actual.

   ![](assets/create-audience2.png)

   Para elegir una audiencia de Adobe Experience Platform, vaya al `AEP Audiences folder` en la sección de filtro de la pantalla. [Aprenda a utilizar una audiencia de Adobe Experience Platform](aep-audience.md)

   ![](assets/select-audience-folder.png)

1. La sección de filtro le permite acceder a las opciones de filtrado para restringir la lista de audiencias. Para ello, haga clic en **Agregar reglas** para acceder al modelador de consultas, que permite crear filtros avanzados para la lista de audiencias. [Aprenda a utilizar el modelador de consultas](../query/query-modeler-overview.md)

1. Clic **Confirmar** para añadir la audiencia como destinatario principal de la entrega. Una vez finalizado, aún puede refinar la audiencia mediante el modelador de consultas haciendo clic en **Editar reglas** botón.

   ![](assets/refine-audience.png)

   También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibe el mensaje. Esto le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. [Más información](control-group.md)
