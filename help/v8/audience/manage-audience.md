---
audience: end-user
title: Monitorización y administración de audiencias
description: Obtenga información sobre cómo monitorizar y administrar audiencias en Adobe Campaign Web
badge: label="Beta"
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 523a43bef4f179740a96039ac2fc5f4f858aa1dc
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 13%

---

# Monitorización y administración de audiencias {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Propiedades"
>abstract="Aquí puede encontrar un resumen de las propiedades de la audiencia, como su origen, carpeta de almacenamiento o estado. Haga clic en el vínculo en la **Último flujo de trabajo** para abrir el flujo de trabajo que se ha utilizado para crear la audiencia."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Tamaño de audiencia"
>abstract="Aquí puede encontrar el número total de perfiles dentro de la audiencia. Haga clic en el botón Calcular para actualizar y volver a calcular los resultados de la audiencia."

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Error de público"
>abstract="Los datos de público no están disponibles. Espere al final de la ejecución del flujo de trabajo."

El público destinatario es el destinatario principal de su envío: los destinatarios que reciben los mensajes. El tipo de público destinatario depende de la asignación de destino definida en la plantilla de envíos. Obtenga más información sobre las plantillas de envío en [esta página](../msg/delivery-template.md).

Para definir la población de una audiencia, puede:

* [Crear nuevas audiencias](create-audience.md) desde el **[!UICONTROL Audiencias]** menú,
* [Seleccionar una audiencia existente](add-audience.md) creado como una lista en la consola del cliente o procedente de Adobe Experience Platform,
* [Crear una audiencia nueva](../query/query-modeler-overview.md) con el modelador de consultas definiendo y combinando criterios de filtrado,
* [Uso de una audiencia de un archivo externo](file-audience.md). Esta opción solo está disponible para envíos de correo electrónico independientes y no se puede utilizar en envíos de campañas.

Al segmentar una audiencia, también puede definir lo siguiente **grupos de control** para evitar enviar mensajes a una parte de la audiencia y medir el impacto de las campañas. [Obtenga información sobre cómo establecer un grupo de control](control-group.md)

>[!NOTE]
>
>Al enviar mensajes en el contexto de un flujo de trabajo de campaña, la audiencia se define en una **Crear audiencia** actividad de flujo de trabajo. En este contexto, no se puede cargar un público destinatario de un archivo para un envío de correo electrónico, y el público destinatario se define solo en esta actividad dedicada. Obtenga información sobre cómo definir la audiencia de su envío en un flujo de trabajo de campaña en [esta sección](../workflows/activities/build-audience.md)

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
