---
audience: end-user
title: Creación de audiencias
description: Obtenga información sobre cómo crear audiencias en Adobe Campaign Web
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 1%

---


# Creación de audiencias {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos-alvo"
>abstract="Desde esta pantalla, puede crear y combinar audiencias en un lienzo visual. Añada varias actividades de flujo de trabajo, como **Split** o **Excluir** para generar audiencias nuevas y refinadas."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Configuración del público"
>abstract="Introduzca el nombre de la audiencia y las opciones adicionales y, a continuación, haga clic en **Crear audiencia** botón."

La web de Campaign le permite crear nuevas audiencias en un lienzo de flujo de trabajo visual. Además de empezar desde cero para crear una audiencia sencilla, también puede aprovechar las actividades de flujo de trabajo para refinar las audiencias. Por ejemplo, puede crear varias audiencias en una sola, enriquecer las audiencias con atributos externos o dividir una audiencia determinada en varias.

Una vez que haya creado el flujo de trabajo, las audiencias resultantes se almacenan automáticamente en la base de datos de Campaign junto con las existentes. Estas audiencias pueden segmentarse en campañas o envíos independientes.

Los pasos principales para crear una audiencia son los siguientes:

1. Cree un flujo de trabajo de audiencia.
1. Configure una actividad Generar audiencia para consultar la base de datos según sus necesidades.
1. Añada actividades de flujo de trabajo para restringir la audiencia (opcional).
1. Configure una actividad Guardar audiencia.
1. Ejecute el flujo de trabajo para guardar las audiencias resultantes en la base de datos.


## Cree su primera audiencia {#create}

Para crear una audiencia, siga estos pasos:

1. Vaya a **[!UICONTROL Audiencias]** y haga clic en el **[!UICONTROL Crear audiencia]** situado en la esquina superior derecha.
1. Proporcione una etiqueta para la audiencia.
1. Expanda el **[!UICONTROL Opciones adicionales]** para configurar parámetros de audiencia avanzados.

   De forma predeterminada, las audiencias se crean en **[!UICONTROL Perfiles y objetivos]** / **[!UICONTROL Listas]** menú del explorador. Puede cambiar la ubicación de almacenamiento predeterminada mediante las opciones **[!UICONTROL Carpeta]** field.

   ![](assets/audiences-settings.png)

1. Una vez configurados los ajustes de audiencia, haga clic en el icono **[!UICONTROL Crear audiencia]** botón.

1. Aparece un lienzo de flujo de trabajo con dos actividades predeterminadas:

   * **[!UICONTROL Crear audiencia]**: este es el punto de partida del flujo de trabajo, que le permite crear una audiencia y utilizarla como base del flujo de trabajo. [Obtenga información sobre cómo configurar una actividad Generar audiencia](../workflows/activities/build-audience.md)

   * **[!UICONTROL Guardar audiencia]**: Representa el paso final del flujo de trabajo, lo que permite guardar los resultados como una nueva audiencia. [Obtenga información sobre cómo configurar una actividad Guardar audiencia](../workflows/activities/save-audience.md)

1. Si desea realizar una operación adicional después de **[!UICONTROL Crear audiencia]** actividad, añada tantas actividades como sea necesario al flujo de trabajo. Para obtener más información sobre la configuración de actividades de flujo de trabajo, consulte la [documentación de flujos de trabajo](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Las actividades de canal no están disponibles para su uso en flujos de trabajo de audiencia.

   ![](assets/audience-creation-canvas.png)

1. Cuando el flujo de trabajo esté listo, haga clic en **[!UICONTROL Inicio]** para ejecutarlo.

1. El flujo de trabajo se guarda en **[!UICONTROL Flujos de trabajo]** , mientras que las audiencias resultantes son accesibles en la **[!UICONTROL Audiencias]** lista. [Obtenga información sobre cómo monitorizar y administrar audiencias](access-audiences.md)

## Ejemplo de flujo de trabajo de audiencia {#example}

El ejemplo siguiente muestra un flujo de trabajo de audiencia configurado para dirigirse a clientes mujeres que viven en Nueva York y crear dos audiencias nuevas según su centro de interés en Yoga o Running gear. Las dos audiencias se enriquecen con información adicional relacionada con las compras de los clientes.

AÑADIR CAPTURA DE PANTALLA

1. La actividad Generar audiencia se dirige a todos los perfiles femeninos que viven en Nueva York.
1. La actividad Enrichment enriquece la audiencia con atributos de la tabla Purchases.
1. La actividad Split divide el flujo de trabajo en dos rutas en función de los centros de interés de los clientes.
1. Las actividades Guardar audiencia al final de cada ruta para guardar cada audiencia en la base de datos.
