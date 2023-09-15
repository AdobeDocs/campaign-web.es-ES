---
audience: end-user
title: Creación de audiencias
description: Obtenga información sobre cómo crear audiencias en Adobe Campaign Web
badge: label="Beta"
source-git-commit: 4b005f3feb70b8c5cf0f4cd9c5ba54547bd9261a
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 2%

---


# Creación de audiencias {#create-audiences}


>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Configuración del público"
>abstract="Introduzca el nombre de la audiencia y las opciones adicionales."

La web de Campaign le permite crear flujos de trabajo en los que puede combinar audiencias existentes en un lienzo visual. Mediante la incorporación de varias actividades de flujo de trabajo como **Split** o **Excluir**, puede generar audiencias nuevas y refinadas.

Una vez que haya creado el flujo de trabajo, las audiencias resultantes se almacenan automáticamente en Campaign Web junto con las existentes. Estas audiencias pueden segmentarse en campañas o envíos independientes.

Para crear una audiencia, siga estos pasos:

1. Vaya a **[!UICONTROL Audiencias]** y haga clic en el **[!UICONTROL Crear audiencia]** situado en la esquina superior derecha.
1. Proporcione una etiqueta para la audiencia.
1. Expanda el **[!UICONTROL Opciones adicionales]** para configurar parámetros de audiencia avanzados.

   De forma predeterminada, las audiencias se crean en **[!UICONTROL Perfiles y objetivos]** / **[!UICONTROL Listas]** menú del explorador. Puede cambiar la ubicación de almacenamiento predeterminada mediante las opciones **[!UICONTROL Carpeta]** field.

   ![](assets/audiences-settings.png)

1. Una vez configurados los ajustes de audiencia, haga clic en el icono **[!UICONTROL Crear audiencia]** botón.

1. Aparece un lienzo de flujo de trabajo con dos actividades predeterminadas:

   * **[!UICONTROL Crear audiencia]**: este es el punto de partida del flujo de trabajo, que le permite crear una audiencia y utilizarla como base del flujo de trabajo.
   * **[!UICONTROL Guardar audiencia]**: Representa el paso final del flujo de trabajo, lo que permite guardar los resultados como una nueva audiencia.

1. Personalice el flujo de trabajo añadiendo tantas actividades como sea necesario. Para obtener más información sobre la configuración de actividades de flujo de trabajo, consulte la [documentación de flujos de trabajo](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Las actividades de canal no están disponibles para su uso en flujos de trabajo de audiencia.

   ![](assets/audience-creation-canvas.png)

1. Cuando el flujo de trabajo esté listo, haga clic en **[!UICONTROL Inicio]** para ejecutarlo.

1. El flujo de trabajo se guarda en **[!UICONTROL Flujos de trabajo]** , mientras que las audiencias resultantes son accesibles en la **[!UICONTROL Audiencias]** lista. [Obtenga información sobre cómo monitorizar y administrar audiencias](access-audiences.md)
