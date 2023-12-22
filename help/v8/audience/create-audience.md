---
audience: end-user
title: Crear públicos
description: Obtenga información sobre cómo crear audiencias en Adobe Campaign Web
badge: label="Beta"
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: bc1b4186b5869d104c6b14e09160f28bf3e28f95
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 10%

---

# Crear públicos {#create-audiences}



>[!CONTEXTUALHELP]
>id="acw_homepage_rn1"
>title="Composición de audiencia"
>abstract="Cree nuevas audiencias en un lienzo de flujo de trabajo visual. Además de empezar desde cero para crear una audiencia sencilla, también puede aprovechar las actividades de flujo de trabajo para refinar la audiencia. Combine varias audiencias en una sola, enriquezca la audiencia con atributos externos o divida una en varias audiencias en función de las reglas que elija."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Consulte las notas de la versión"


>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos"
>abstract="Desde esta pantalla, puede acceder a la lista de todos los públicos que se pueden segmentar en los envíos. Haga clic en **Crear** para crear nuevos públicos en un lienzo visual utilizando varias actividades de flujo de trabajo como **División** o **Excluir**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Configuración del público"
>abstract="Introduzca el nombre de público y las opciones adicionales y, a continuación, haga clic en el botón **Crear público**."

La web de Campaign le permite crear nuevas audiencias en un lienzo de flujo de trabajo visual. Además de empezar desde cero para crear una audiencia sencilla, también puede aprovechar las actividades de flujo de trabajo para refinar la audiencia. Por ejemplo, puede combinar varias audiencias en una sola, enriquecer la audiencia con atributos externos o dividir una en varias audiencias en función de las reglas que elija.

Una vez que haya creado el flujo de trabajo, las audiencias resultantes se almacenan automáticamente en la base de datos de Campaign junto con las existentes. Estas audiencias pueden segmentarse en flujos de trabajo o envíos independientes.

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

El flujo de trabajo se guarda en **[!UICONTROL Flujos de trabajo]** , mientras que las audiencias resultantes son accesibles en la **[!UICONTROL Audiencias]** lista. [Obtenga información sobre cómo monitorizar y administrar audiencias](manage-audience.md)

Ahora puede utilizar esta audiencia como el destinatario principal de una entrega. [Más información](add-audience.md)

## Ejemplo de flujo de trabajo de audiencia {#example}

El ejemplo siguiente muestra un flujo de trabajo de audiencia configurado para dirigirse a clientes mujeres que viven en Nueva York y crear dos audiencias nuevas en función de su última compra (equipo de yoga o de running).

![](assets/audiences-example.png)

1. El **[!UICONTROL Crear audiencia]** La actividad se dirige a todos los perfiles femeninos que viven en Nueva York.
1. El **[!UICONTROL Enriquecimiento]** La actividad enriquece a la audiencia con información de la tabla Compras para identificar qué tipo de producto compraron los clientes.
1. El **[!UICONTROL Split]** La actividad divide el flujo de trabajo en dos rutas en función de la última compra de los clientes.
1. El **[!UICONTROL Guardar audiencia]** las actividades al final de cada ruta crean dos nuevas audiencias en la base de datos, incluida la población calculada en cada ruta.
