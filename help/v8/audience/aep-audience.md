---
audience: end-user
title: Usar una audiencia de Adobe Experience Platform
description: Aprenda a utilizar una audiencia de Adobe Experience Platform
badge: label="Alpha" type="Positive"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: f7d59309979a063f4491f24c4a9e6deab83a4351
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 50%

---

# Usar una audiencia de Adobe Experience Platform{#aep-audience}

Los conectores Origen y Destino del Cloud Service administrado de Adobe Campaign permiten una integración perfecta entre Adobe Campaign y Adobe Experience Platform.

Una vez creada una audiencia de Adobe Experience Platform y disponible en la consola del cliente, puede utilizarla del mismo modo que lo haría para que una audiencia de Campaign personalice y envíe mensajes.

>[!NOTE]
>
>Para utilizar audiencias de Adobe Experience Platform en Campaign, debe configurar la integración con Fuentes y destinos de Adobe. Consulte [Documentación de Campaign v8 (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html?lang=es){target="_blank"}.


También puede realizar lo siguiente:

* Crear una audiencia nueva. [Más información](segment-builder.md)
* Carga de una audiencia desde un archivo externo. [Más información](file-audience.md)
* Utilice una audiencia de Campaign existente. [Más información](add-audience.md).

Para seleccionar una audiencia de Adobe Experience Platform para el mensaje, siga los pasos a continuación:

1. En la sección **Audiencia** del asistente de creación de envíos, haga clic en el botón **[!UICONTROL Seleccionar la audiencia]**.

   ![](assets/create-audience.png)

1. Elija **[!UICONTROL Seleccionar la audiencia]** para usar una audiencia existente. Para crear una nueva audiencia para usarla en este correo electrónico, elija **Crear la suya propia**. Consulte esta [sección](segment-builder.md).

   Esta pantalla muestra todas las audiencias existentes definidas en la consola del cliente de Adobe Campaign para la carpeta actual. Para elegir una audiencia de Adobe Experience Platform, vaya al `AEP Audiences folder` en la sección de filtro de la pantalla.

   ![](assets/select-audience-folder.png)

   También puede definir una regla para filtrar el origen de las audiencias, como se muestra a continuación:

   ![](assets/filter-on-aep-audience.png)

1. Elija una audiencia y haga clic en **Seleccionar**.

1. Haga clic en **Editar reglas** si desea restringir la audiencia.

   ![](assets/refine-audience.png)

1. Con el generador de reglas, puede enriquecer la audiencia con filtros adicionales o combinando distintas audiencias. Consulte esta [sección](segment-builder.md).

1. Haga clic en **Save**.

También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibe el mensaje. Esto le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. Consulte la [sección](control-group.md).

