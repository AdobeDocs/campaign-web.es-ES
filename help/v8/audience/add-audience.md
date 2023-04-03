---
audience: end-user
title: Seleccionar una audiencia
description: Obtenga información sobre cómo seleccionar una audiencia
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alpha" type="Informative"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 8%

---


# Seleccionar una audiencia {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Seleccionar una audiencia existente"
>abstract="Las audiencias se definen en la consola Adobe Campaign v8. Si tiene una integración de Adobe Experience Platform disponible, también debería poder ver las audiencias definidas por Platform."

En esta sección se explica cómo seleccionar una audiencia existente al definir la población objetivo de una entrega de correo electrónico. Si desea crear una audiencia nueva, consulte esta [sección](segment-builder.md).

1. En el **Audiencia** del asistente de creación de envíos, haga clic en el botón **[!UICONTROL Seleccionar la audiencia]** botón.

   ![](assets/create-audience.png)

1. Choose **[!UICONTROL Seleccionar la audiencia]** para usar una audiencia existente. Para crear una nueva audiencia para usarla en este correo electrónico, elija **Cree sus propios**. Consulte esta [sección](segment-builder.md).

   Esta pantalla muestra todas las audiencias existentes definidas en la consola de Adobe Campaign o en Adobe Experience Platform.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Para aprovechar las audiencias de Adobe Experience Platform, debe configurar la integración con Destinations. Consulte la [Documentación de destinos](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=es){target="_blank"}.

1. Elija una audiencia y haga clic en **Select**.

1. Haga clic en **Editar reglas** si desea restringir la audiencia.

   ![](assets/create-audience3.png)

1. Con el generador de reglas, puede enriquecer la audiencia con filtros adicionales o combinando distintas audiencias. Consulte esta [sección](segment-builder.md).

   ![](assets/create-audience4.png)

1. Haga clic en **Save**.

También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibe el mensaje. Esto le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de contactos que no lo hicieron. Consulte [sección](control-group.md).