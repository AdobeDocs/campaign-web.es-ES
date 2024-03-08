---
audience: end-user
title: Monitorizar y administrar públicos
description: Obtenga información sobre cómo monitorizar y administrar audiencias en Adobe Campaign Web
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 23%

---

# Monitorizar y administrar públicos {#monitor-manage}

## ¿Qué es una audiencia? {#what}

La audiencia es el destinatario principal del envío: los perfiles que reciben los mensajes. El tipo de público destinatario depende de la asignación de destino definida en la plantilla de envíos. Obtenga más información sobre las plantillas de envío en [esta página](../msg/delivery-template.md).

Para definir la población de una audiencia, puede:

* [Crear nuevas audiencias](create-audience.md) desde el **[!UICONTROL Audiencias]** menú,
* [Seleccionar una audiencia existente](add-audience.md) creado como una lista en la consola del cliente o procedente de Adobe Experience Platform,
* [Crear una audiencia nueva](../query/query-modeler-overview.md) con el modelador de consultas definiendo y combinando criterios de filtrado,
* [Uso de una audiencia de un archivo externo](file-audience.md). Esta opción solo está disponible para envíos de correo electrónico independientes y no se puede utilizar en envíos de campañas.

Al segmentar una audiencia, también puede definir lo siguiente **grupos de control** para evitar enviar mensajes a una parte de la audiencia y medir el impacto de las campañas. [Obtenga información sobre cómo establecer un grupo de control](control-group.md)

>[!NOTE]
>
>Al enviar mensajes en el contexto de un flujo de trabajo de campaña, la audiencia se define en una **Crear audiencia** actividad de flujo de trabajo. En este contexto, no se puede cargar un público destinatario de un archivo para un envío de correo electrónico, y el público destinatario se define solo en esta actividad dedicada. Obtenga información sobre cómo definir la audiencia de su envío en un flujo de trabajo de campaña en [esta sección](../workflows/activities/build-audience.md)

## Monitorización de audiencias {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Propiedades"
>abstract="Aquí puede encontrar un resumen de las propiedades del público, como su origen, carpeta de almacenamiento o estado. Haga clic en el vínculo en la sección **Último flujo de trabajo** para abrir el flujo de trabajo que se ha utilizado para crear el público."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Tamaño de público"
>abstract="Aquí puede encontrar el número total de perfiles dentro del público. Haga clic en el botón Calcular para actualizar y volver a calcular los resultados del público."

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Error de público"
>abstract="Los datos de público no están disponibles. Espere al final de la ejecución del flujo de trabajo."

Se puede acceder a la lista de audiencias disponibles para utilizar en Campaign Web desde el **[!UICONTROL Audiencias]** menú.

![](assets/audiences-list.png){zoomable=&quot;yes&quot;}

Las audiencias pueden proceder de varias fuentes. El **[!UICONTROL Origen]** columns indica dónde se ha creado una audiencia determinada:

* **[!UICONTROL Adobe Campaign]**: estas audiencias se crean en la consola de Adobe Campaign V8. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=es){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Estas audiencias se crean en Adobe Experience Platform y se integran en Campaign Web mediante la integración de fuentes de Adobe y destinos. Obtenga información sobre cómo configurar esta integración en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

  ➡️ [Descubra esta función en vídeo](#video)

* **[!UICONTROL IU web de Adobe Campaign]**: estas audiencias se crean mediante flujos de trabajo de audiencia web de Campaign. [Obtenga información sobre cómo crear audiencias](create-audience.md)

Para obtener más información sobre una audiencia, ábrala en la lista. Se muestran las propiedades de la audiencia, junto con el número de perfiles incluidos en la audiencia. Puede actualizar el recuento de audiencias en cualquier momento mediante la variable **[!UICONTROL Calcular]** botón.

El **[!UICONTROL Datos]** permite ver los perfiles que forman parte de la audiencia. Puede personalizar esta vista añadiendo más columnas o aprovechando los filtros avanzados para restringir los datos mostrados.

![](assets/audiences-details.png){zoomable=&quot;yes&quot;}

Para duplicar o eliminar una audiencia, haga clic en **[!UICONTROL Más acción]** disponible en la lista de audiencias junto al nombre de la audiencia o en una pantalla de detalles de audiencia.

## Vídeo explicativo {#video}

Obtenga información sobre cómo crear un destino para utilizar una audiencia de Experience Platform en la interfaz de usuario web de Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Encontrará información detallada sobre cómo configurar la integración de fuentes de Adobe y destinos en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.
