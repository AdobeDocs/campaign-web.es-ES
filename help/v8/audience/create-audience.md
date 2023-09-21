---
audience: end-user
title: Creación y administración de audiencias
description: Obtenga información sobre cómo crear y administrar audiencias en Adobe Campaign Web
badge: label="Beta"
source-git-commit: d81c143b5ba45bf02558856a250868d43679a63a
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---


# Creación de audiencias {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos-alvo"
>abstract="Desde esta pantalla, puede acceder a la lista de todas las audiencias que se pueden segmentar en los envíos. Clic **Crear** para crear nuevas audiencias en un lienzo visual utilizando varias actividades de flujo de trabajo como **Split** o **Excluir**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Configuración del público"
>abstract="Introduzca el nombre de la audiencia y las opciones adicionales y, a continuación, haga clic en **Crear audiencia** botón."

La web de Campaign le permite crear nuevas audiencias en un lienzo de flujo de trabajo visual. Además de empezar desde cero para crear una audiencia sencilla, también puede aprovechar las actividades de flujo de trabajo para refinar la audiencia. Por ejemplo, puede combinar varias audiencias en una sola, enriquecer la audiencia con atributos externos o dividir una en varias audiencias en función de las reglas que elija.

Una vez que haya creado el flujo de trabajo, las audiencias resultantes se almacenan automáticamente en la base de datos de Campaign junto con las existentes. Estas audiencias pueden segmentarse en campañas o envíos independientes.

## Cree su primera audiencia {#create}

Para crear una audiencia, siga estos pasos:

1. Vaya a **[!UICONTROL Audiencias]** y haga clic en el **[!UICONTROL Crear audiencia]** situado en la esquina superior derecha.
1. Proporcione una etiqueta para la audiencia.
1. Expanda el **[!UICONTROL Opciones adicionales]** para configurar parámetros de audiencia avanzados.

   De forma predeterminada, las audiencias se crean en **[!UICONTROL Perfiles y objetivos]** / **[!UICONTROL Listas]** menú del explorador. Puede cambiar la ubicación de almacenamiento predeterminada mediante las opciones **[!UICONTROL Carpeta]** field.

   ![](assets/audiences-settings.png)

1. Una vez configurados los ajustes de audiencia, haga clic en el icono **[!UICONTROL Crear audiencia]** botón. Aparece un lienzo de flujo de trabajo con dos actividades predeterminadas:

   * **[!UICONTROL Crear audiencia]**: este es el punto de partida del flujo de trabajo, que le permite crear una audiencia y utilizarla como base del flujo de trabajo.

   * **[!UICONTROL Guardar audiencia]**: Representa el paso final del flujo de trabajo, lo que permite guardar los resultados del flujo de trabajo como una nueva audiencia.

1. Abra el **[!UICONTROL Crear audiencia]** y utilice el generador de reglas para definir la población que desea incluir en la audiencia filtrando los datos contenidos en la base de datos. [Obtenga información sobre cómo configurar una actividad Generar audiencia](../workflows/activities/build-audience.md)

1. Si desea realizar operaciones adicionales en la población objetivo del flujo de trabajo, añada tantas actividades como sea necesario y conéctelas. Para obtener más información sobre la configuración de actividades de flujo de trabajo, consulte la [documentación de flujos de trabajo](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Las actividades de canal no están disponibles para su uso en flujos de trabajo de audiencia.

   ![](assets/audience-creation-canvas.png)

1. Configure las variables **[!UICONTROL Guardar audiencia]** actividad para especificar cómo desea guardar la población calculada en sentido ascendente en el flujo de trabajo. [Obtenga información sobre cómo configurar una actividad Guardar audiencia](../workflows/activities/save-audience.md)

1. Cuando el flujo de trabajo esté listo, haga clic en **[!UICONTROL Inicio]** para ejecutarlo.

El flujo de trabajo se guarda en **[!UICONTROL Flujos de trabajo]** , mientras que las audiencias resultantes son accesibles en la **[!UICONTROL Audiencias]** lista.

## Ejemplo de flujo de trabajo de audiencia {#example}

El ejemplo siguiente muestra un flujo de trabajo de audiencia configurado para dirigirse a clientes mujeres que viven en Nueva York y crear dos audiencias nuevas en función de su última compra (equipo de yoga o de running).

![](assets/audiences-example.png)

1. El **[!UICONTROL Crear audiencia]** La actividad se dirige a todos los perfiles femeninos que viven en Nueva York.
1. El **[!UICONTROL Enriquecimiento]** La actividad enriquece a la audiencia con información de la tabla Compras para identificar qué tipo de producto compraron los clientes.
1. El **[!UICONTROL Split]** La actividad divide el flujo de trabajo en dos rutas en función de la última compra de los clientes.
1. El **[!UICONTROL Guardar audiencia]** las actividades al final de cada ruta crean dos nuevas audiencias en la base de datos, incluida la población calculada en cada ruta.

## Monitorización y administración de audiencias {#monitor}

Se puede acceder a la lista de audiencias disponibles para utilizar en Campaign Web desde el **[!UICONTROL Audiencias]** menú.

![](assets/audiences-list.png)

Las audiencias pueden proceder de varias fuentes. El **[!UICONTROL Origen]** columns indica dónde se ha creado una audiencia determinada:

* **[!UICONTROL Adobe Campaign]**: estas audiencias se crean en la consola de Adobe Campaign V8. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=es){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Estas audiencias se crean en Adobe Experience Platform y se integran en Campaign Web mediante la integración de fuentes de Adobe y destinos. Obtenga información sobre cómo configurar esta integración en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL IU web de Adobe Campaign]**: estas audiencias se crean mediante flujos de trabajo de audiencia web de Campaign. [Obtenga información sobre cómo crear audiencias](create-audience.md)

Para obtener más información sobre una audiencia, ábrala en la lista. Se muestran las propiedades de la audiencia, junto con el número de perfiles incluidos en la audiencia. Puede actualizar el recuento de audiencias en cualquier momento mediante la variable **[!UICONTROL Calcular]** botón.

El **[!UICONTROL Datos]** permite ver los perfiles que forman parte de la audiencia. Puede personalizar esta vista añadiendo más columnas o aprovechando los filtros avanzados para restringir los datos mostrados.

![](assets/audiences-details.png)

Para duplicar o eliminar una audiencia, haga clic en **[!UICONTROL Más acción]** disponible en la lista de audiencias junto al nombre de la audiencia o en una pantalla de detalles de audiencia.
