---
audience: end-user
title: Monitorización y administración de audiencias
description: Obtenga información sobre cómo monitorizar y administrar audiencias en Adobe Campaign Web
badge: label="Beta"
source-git-commit: 21436695f6f4bc9e99bb7983e4705cbbe40f07eb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 3%

---


# Monitorización y administración de audiencias {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Error de audiencia"
>abstract="Los datos de audiencia no están disponibles. Espere al final de la ejecución del flujo de trabajo."

Se puede acceder a la lista de audiencias disponibles para utilizar en Campaign Web desde el **[!UICONTROL Audiencias]** menú.

![](assets/audiences-list.png)

Las audiencias pueden proceder de varias fuentes. El **[!UICONTROL Origen]** columns indica dónde se ha creado una audiencia determinada:

* **[!UICONTROL Adobe Campaign]**: estas audiencias se crean en la consola de Adobe Campaign V8. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=es){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Estas audiencias se crean en Adobe Experience Platform y se integran en Campaign Web mediante la integración de fuentes de Adobe y destinos. Obtenga información sobre cómo configurar esta integración en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

>[!NOTE]
>
>Para utilizar audiencias de Adobe Experience Platform en Campaign, debe configurar la integración con Fuentes y destinos de Adobe. Consulte [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL IU web de Adobe Campaign]**: estas audiencias se crean mediante flujos de trabajo de audiencia web de Campaign. [Obtenga información sobre cómo crear audiencias](create-audience.md)

Para obtener más información sobre una audiencia, ábrala en la lista. Se muestran las propiedades de la audiencia, junto con el número de perfiles incluidos en la audiencia. Puede actualizar el recuento de audiencias en cualquier momento mediante la variable **[!UICONTROL Calcular]** botón.

El **[!UICONTROL Datos]** permite ver los perfiles que forman parte de la audiencia. Puede personalizar esta vista añadiendo más columnas o aprovechando los filtros avanzados para restringir los datos mostrados.

![](assets/audiences-details.png)

Para duplicar o eliminar una audiencia, haga clic en **[!UICONTROL Más acción]** disponible en la lista de audiencias junto al nombre de la audiencia o en una pantalla de detalles de audiencia.