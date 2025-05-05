---
audience: end-user
title: Crear públicos
description: Obtenga información sobre cómo crear audiencias en Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 9%

---

# Crear públicos {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos"
>abstract="Desde esta pantalla, puede acceder a la lista de todos los públicos que se pueden segmentar en flujos de trabajo o envíos independientes. Haga clic en **Crear** para crear un nuevo público en un lienzo visual.<br/><br/>Además de empezar desde cero para crear un público sencillo, también puede aprovechar las actividades del flujo de trabajo para detallar su público. Por ejemplo, puede combinar varias audiencias en una sola, enriquecer la audiencia con atributos externos o dividirla en varias audiencias en función de las reglas que elija."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

La web de Campaign le permite crear nuevas audiencias en un lienzo de flujo de trabajo visual. Además de empezar desde cero para crear un público sencillo, también puede aprovechar las actividades del flujo de trabajo para perfeccionar su público. Por ejemplo, puede combinar varias audiencias en una sola, enriquecer la audiencia con atributos externos o dividirla en varias audiencias en función de las reglas que elija.

Una vez que haya creado el flujo de trabajo, las audiencias resultantes se almacenan automáticamente en la base de datos de Campaign junto con las existentes. Estas audiencias pueden segmentarse en flujos de trabajo o envíos independientes.

La **[!UICONTROL columna Origen]** indica los orígenes de las audiencias: **[!UICONTROL Adobe Campaign]** audiencias se crean en la consola de Adobe Campaign v8 o en la interfaz web de usuario, mientras que **[!UICONTROL Adobe Experience Platform:]** las audiencias se crean dentro de Adobe Experience Platform y se integran en Campaign mediante la integración de orígenes y destinos de Adobe Systems.

➡️ [Descubra esta funcionalidad en vídeo](#video)

## Crear tu primer audiencia {#create}

Para crear un audiencia, seguir estos pasos:

1. Vaya al menú **[!UICONTROL Audiencias]** y haga clic en el botón **[!UICONTROL Crear audiencia]** ubicado en la esquina superior derecha.

1. Se crea automáticamente un nuevo flujo de trabajo, que le permite combinar actividades para generar su audiencia. De manera predeterminada, el lienzo contiene dos actividades principales:

   * La actividad de audiencia **de compilación &quot;Consulta&quot;** es el punto de partida de su flujo de trabajo. Le permite crear un audiencia y utilizarlo como base para su flujo de trabajo.

   * El &quot;Nuevo audiencia&quot; **[!UICONTROL Guardar audiencia]** actividad representa el paso final en su flujo de trabajo. Permite guardar los resultados como un nuevo audiencia.

   ![Un lienzo de creación de audiencia en blanco con dos actividades predeterminadas: Generar audiencia y Guardar audiencia.](assets/create-audience-blank.png){zoomable="yes"}

   >[!IMPORTANT]
   >
   >Las flujos de trabajo de audiencia se almacenan en el menú Flujos de **trabajo, junto con los** demás Campaign flujos de trabajo. Están diseñadas específicamente para crear audiencias y se pueden identificar por su lienzo vertical.

1. Para facilitar la lectura, cambie el nombre del flujo de trabajo en el campo **Label** de la configuración del flujo de trabajo. [Aprenda a configurar las opciones del flujo de trabajo](../workflows/workflow-settings.md)

1. Abra la actividad **[!UICONTROL Generar audiencia]** y use el modelador de consultas para definir la población que se incluirá en la audiencia filtrando los datos contenidos en la base de datos. [Aprenda a configurar una actividad Generar audiencia](../workflows/activities/build-audience.md)

1. Si desea realizar operaciones adicionales en la población objetivo en el flujo de trabajo, añada tantas actividades como sea necesario y conéctelas. Para obtener más información sobre cómo configurar flujo de trabajo actividades, consulte la documentación[&#128279;](../workflows/activities/about-activities.md) flujos de trabajo.

   >[!NOTE]
   >
   >Las actividades de canal no están disponibles para su uso en flujos de trabajo de audiencia.

   ![Lienzo de creación de audiencia con varias actividades conectadas para restringir la audiencia.](assets/audience-creation-canvas.png){zoomable="yes"}

1. Configure la actividad **[!UICONTROL Guardar audiencia]** para especificar cómo desea guardar la población calculada en sentido ascendente en el flujo de trabajo. [Aprenda a configurar una actividad Guardar audiencia](../workflows/activities/save-audience.md)

1. Cuando el flujo de trabajo esté listo, haga clic en **[!UICONTROL Iniciar]** para ejecutarlo.

El flujo de trabajo se guarda en la lista **[!UICONTROL Flujos de trabajo]**, mientras que las audiencias resultantes son accesibles en la lista **[!UICONTROL Audiencias]** con la etiqueta definida en la actividad **Guardar audiencia**. Aprenda a monitorizar y administrar las audiencias en [esta sección](manage-audience.md)

Ahora puede utilizar este audiencia como destino principal de una envío. [Más información](add-audience.md)

## Ejemplo de flujo de trabajo de audiencia {#example}

El siguiente ejemplo muestra una flujo de trabajo audiencia configurada para destino a las clientas que viven en Nuevo York y crear dos nuevas audiencias dependiendo de su última compra (equipo de yoga o running).

![Ejemplo de flujo de trabajo de audiencia dirigido a clientes mujeres de Nueva York y dividido en función de su última compra.](assets/audiences-example.png){zoomable="yes"}

1. La actividad **[!UICONTROL Generar audiencia]** se dirige a todos los perfiles femeninos que viven en Nueva York.
1. La **[!UICONTROL actividad de enriquecimiento enriquece]** el audiencia con información de la tabla Compras para identificar qué tipo de producto compraron los clientes.
1. La **[!UICONTROL actividad dividida]** divide el flujo de trabajo en dos rutas según la última compra del cliente.
1. La **[!UICONTROL Guardar audiencia]** actividades al final de cada ruta crean dos nuevas audiencias en la base de datos, incluida la población calculada en cada ruta.

## Editar un audiencia {#edit}

Puede modificar una audiencia generada a partir de una flujo de trabajo siempre que sea necesario volviendo a ejecutar su flujo de trabajo correspondiente. Esto le permite actualizar audiencia datos o restringir el audiencia ajustando el consulta para adaptarlo a sus necesidades.

1. Vaya al menú **Audiencias** y abra la audiencia que desee editar.
1. En la ficha **Información general**, la sección **Último flujo de trabajo** proporciona un vínculo al flujo de trabajo utilizado para generar la audiencia. Haga clic en él para acceder al flujo de trabajo.
1. Realice los cambios que desee y haga clic en el botón **Iniciar** para volver a ejecutar el flujo de trabajo. Una vez finalizada, la audiencia resultante del flujo de trabajo se actualiza automáticamente con los últimos resultados del flujo de trabajo.

De forma predeterminada, al volver a ejecutar una audiencia flujo de trabajo se reemplaza todo el contenido del audiencia con datos nuevos, lo que provoca la pérdida de datos anteriores.

Si prefiere no reemplazar los resultados de audiencia existentes, configure las actividades **Guardar audiencia** para que se ajusten a sus necesidades. Por ejemplo, puede cambiar el campo Etiqueta **de** audiencia para tienda los nuevos resultados en una nueva audiencia o agregar los nuevos resultados a la contenido de audiencia existente sin borrar los datos anteriores. [Aprenda a configurar una Guardar audiencia actividad](../workflows/activities/save-audience.md)

![La Guardar audiencia actividad pantalla de configuración con opciones para ajustar audiencia comportamiento de guardado.](assets/edit-audience-save.png){zoomable="yes"}

## Vídeos explicativos {#video}

Aprenda a versión y administrar audiencias, a seleccionar audiencias para una envío y a definir grupos de control.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)