---
audience: end-user
title: Crear públicos
description: Obtenga información sobre cómo crear audiencias en Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: ba7ba504a8ea62ad6ecea65f9b93ee5848077201
workflow-type: tm+mt
source-wordcount: '1015'
ht-degree: 13%

---

# Crear públicos {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos"
>abstract="Desde esta pantalla, puede acceder a la lista de todos los públicos que se pueden segmentar en flujos de trabajo o envíos independientes. Haga clic en **Crear** para crear un nuevo público en un lienzo visual.<br/><br/>Además de empezar desde cero para crear un público sencillo, también puede aprovechar las actividades del flujo de trabajo para detallar su público. Por ejemplo, puede combinar varios públicos en uno solo, enriquecerlo con atributos externos o dividirlo en varios públicos en función de las reglas que elija."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

## Acerca de la creación de audiencias

La web de Campaign le permite crear nuevas audiencias en un lienzo de flujo de trabajo visual. Además de empezar desde cero para crear un público sencillo, también puede aprovechar las actividades del flujo de trabajo para perfeccionar su público. Por ejemplo, puede combinar varios públicos en uno solo, enriquecerlo con atributos externos o dividirlo en varios públicos en función de las reglas que elija.

Una vez que haya creado el flujo de trabajo, las audiencias resultantes se almacenan automáticamente en la base de datos de Campaign junto con las existentes. Estas audiencias pueden segmentarse en flujos de trabajo o envíos independientes.

La columna **[!UICONTROL Origin]** indica el origen de las audiencias: Las audiencias de **[!UICONTROL Adobe Campaign]** se crean en la consola de Adobe Campaign v8 o en la interfaz de usuario web, mientras que las audiencias de **[!UICONTROL Adobe Experience Platform:]** se crean en Adobe Experience Platform y se integran en Campaign mediante la integración de fuentes y destinos de Adobe.

➡️ [Descubra esta funcionalidad en vídeo](#video)

## Permisos para grupos de operadores personalizados

Al crear una audiencia nueva, se crea automáticamente un flujo de trabajo que se almacena en la carpeta **[!UICONTROL Perfiles y objetivos]** / **[!UICONTROL Trabajos]** / **[!UICONTROL Flujos de trabajo de segmentación]**.

Si se le asigna un grupo de operadores personalizado y encuentra el error &quot;No tiene derechos&quot; al crear audiencias, debe asegurarse de que el grupo de operadores tenga los permisos necesarios para esta carpeta.

Para resolver esto, un administrador debe agregar su grupo de operadores personalizados a la sección de seguridad de carpetas de la consola de Campaign. [Obtenga información sobre cómo administrar permisos en carpetas](../get-started/permissions.md#folder-permissions)

## Cree su primera audiencia {#create}

Para crear una audiencia, siga estos pasos:

1. Vaya al menú **[!UICONTROL Audiencias]** y haga clic en el botón **[!UICONTROL Crear audiencia]** ubicado en la esquina superior derecha.

1. Se crea automáticamente un nuevo flujo de trabajo, que le permite combinar actividades para generar su audiencia. De forma predeterminada, el lienzo contiene dos actividades principales:

   * La actividad &quot;Consulta&quot; **[!UICONTROL Generar audiencia]** es el punto de partida del flujo de trabajo. Permite crear una audiencia y utilizarla como base para el flujo de trabajo.

   * La actividad &quot;Nueva audiencia&quot; **[!UICONTROL Guardar audiencia]** representa el paso final del flujo de trabajo. Permite guardar los resultados como una nueva audiencia.

   ![Lienzo de creación de audiencia en blanco con dos actividades predeterminadas: Generar audiencia y Guardar audiencia.](assets/create-audience-blank.png){zoomable="yes"}

   >[!IMPORTANT]
   >
   >Los flujos de trabajo de audiencia se almacenan en el menú **Flujos de trabajo** junto con el resto de flujos de trabajo de la campaña. Están diseñadas específicamente para crear audiencias y se pueden identificar por su lienzo vertical.

1. Para facilitar la lectura, cambie el nombre del flujo de trabajo en el campo **Label** de la configuración del flujo de trabajo. [Aprenda a configurar las opciones del flujo de trabajo](../workflows/workflow-settings.md)

1. Abra la actividad **[!UICONTROL Generar audiencia]** y use el modelador de consultas para definir la población que se incluirá en la audiencia filtrando los datos contenidos en la base de datos. [Aprenda a configurar una actividad Generar audiencia](../workflows/activities/build-audience.md)

1. Si desea realizar operaciones adicionales en la población objetivo en el flujo de trabajo, añada tantas actividades como sea necesario y conéctelas. Para obtener más información sobre cómo configurar las actividades de flujo de trabajo, consulte la [documentación de flujos de trabajo](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Las actividades de canal no están disponibles para su uso en flujos de trabajo de audiencia.

   ![Lienzo de creación de audiencia con varias actividades conectadas para restringir la audiencia.](assets/audience-creation-canvas.png){zoomable="yes"}

1. Configure la actividad **[!UICONTROL Guardar audiencia]** para especificar cómo desea guardar la población calculada en sentido ascendente en el flujo de trabajo. [Aprenda a configurar una actividad Guardar audiencia](../workflows/activities/save-audience.md)

1. Cuando el flujo de trabajo esté listo, haga clic en **[!UICONTROL Iniciar]** para ejecutarlo.

El flujo de trabajo se guarda en la lista **[!UICONTROL Flujos de trabajo]**, mientras que las audiencias resultantes son accesibles en la lista **[!UICONTROL Audiencias]** con la etiqueta definida en la actividad **Guardar audiencia**. Aprenda a monitorizar y administrar las audiencias en [esta sección](manage-audience.md)

Ahora puede utilizar esta audiencia como el destinatario principal de una entrega. [Más información](add-audience.md)

## Ejemplo de flujo de trabajo de audiencia {#example}

El ejemplo siguiente muestra un flujo de trabajo de audiencia configurado para dirigirse a clientes mujeres que viven en Nueva York y crear dos audiencias nuevas en función de su última compra (equipo de yoga o de running).

![Ejemplo de flujo de trabajo de audiencia dirigido a clientes mujeres de Nueva York y dividido en función de su última compra.](assets/audiences-example.png){zoomable="yes"}

1. La actividad **[!UICONTROL Generar audiencia]** se dirige a todos los perfiles femeninos que viven en Nueva York.
1. La actividad **[!UICONTROL Enrichment]** enriquece a la audiencia con información de la tabla Purchases para identificar qué tipo de producto compraron los clientes.
1. La actividad **[!UICONTROL Split]** divide el flujo de trabajo en dos rutas en función de la última compra de los clientes.
1. Las actividades **[!UICONTROL Guardar audiencia]** al final de cada ruta crean dos audiencias nuevas en la base de datos, incluida la población calculada en cada ruta.

## Editar una audiencia {#edit}

Puede modificar una audiencia generada a partir de un flujo de trabajo siempre que sea necesario volviendo a ejecutar su flujo de trabajo correspondiente. Esto le permite actualizar los datos de audiencia o refinar la audiencia ajustando la consulta para adaptarla a sus necesidades.

1. Vaya al menú **Audiencias** y abra la audiencia que desee editar.
1. En la ficha **Información general**, la sección **Último flujo de trabajo** proporciona un vínculo al flujo de trabajo utilizado para generar la audiencia. Haga clic en él para acceder al flujo de trabajo.
1. Realice los cambios que desee y haga clic en el botón **Iniciar** para volver a ejecutar el flujo de trabajo. Una vez finalizada, la audiencia resultante del flujo de trabajo se actualiza automáticamente con los últimos resultados del flujo de trabajo.

De forma predeterminada, al volver a ejecutar un flujo de trabajo de audiencia, se sustituye todo el contenido de la audiencia por datos nuevos, lo que provoca la pérdida de datos anteriores.

Si prefiere no reemplazar los resultados de audiencia existentes, configure las actividades **Guardar audiencia** para que se ajusten a sus necesidades. Por ejemplo, puede cambiar el campo **Etiqueta de audiencia** para almacenar los nuevos resultados en una audiencia nueva o agregar los nuevos resultados al contenido de audiencia existente sin borrar los datos anteriores. [Aprenda a configurar una actividad Guardar audiencia](../workflows/activities/save-audience.md)

![Pantalla de configuración de Guardar actividad de audiencia con opciones para ajustar el comportamiento al guardar audiencias.](assets/edit-audience-save.png){zoomable="yes"}

## Vídeos explicativos {#video}

Obtenga información sobre cómo crear y administrar audiencias, cómo seleccionar audiencias para una entrega y definir grupos de control.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)