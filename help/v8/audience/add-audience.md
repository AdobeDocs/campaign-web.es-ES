---
audience: end-user
title: Selección de una audiencia existente
description: Obtenga información sobre cómo seleccionar una audiencia
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 89%

---


# Selección de una audiencia existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selección de una audiencia existente"
>abstract="Las audiencias se definen en la consola Adobe Campaign v8. Si tiene una integración de Adobe Experience Platform disponible, también debería poder ver las audiencias definidas por Platform."

En esta sección se explica cómo seleccionar una audiencia existente al definir la población objetivo de un envío de correo electrónico.

También puede realizar lo siguiente:

* Crear una audiencia nueva. [Más información](segment-builder.md)
* Carga de una audiencia desde un archivo externo. [Más información](file-audience.md)
* Usar una audiencia de Adobe Experience Platform. [Más información](aep-audience.md).


Para seleccionar una audiencia existente para el mensaje, siga los pasos a continuación:

1. En la sección **Audiencia** del asistente de creación de envíos, haga clic en el botón **[!UICONTROL Seleccionar la audiencia]**.

   ![](assets/create-audience.png)

1. Elija **[!UICONTROL Seleccionar la audiencia]** para usar una audiencia existente. Para crear una nueva audiencia para usarla en este correo electrónico, elija **Crear la suya propia**. Consulte esta [sección](segment-builder.md).

   Esta pantalla muestra todas las audiencias existentes definidas en la consola del cliente de Adobe Campaign para la carpeta actual.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Para aprovechar las audiencias de Adobe Experience Platform, debe configurar la integración con Destinos. Consulte la [documentación de Destinos](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=es){target="_blank"}.

1. Elija una audiencia y haga clic en **Seleccionar**.

1. Haga clic en **Editar reglas** si desea restringir la audiencia.

   ![](assets/create-audience3.png)

1. Con el generador de reglas, puede enriquecer la audiencia con filtros adicionales o combinando distintas audiencias. Consulte esta [sección](segment-builder.md).

   ![](assets/create-audience4.png)

1. Haga clic en **Save**.

También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibe el mensaje. Esto le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. Obtenga más información en [esta sección](control-group.md).