---
title: Creación de perfiles de prueba en Campaign
description: Obtenga información sobre cómo crear y administrar perfiles de prueba en Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
adge: label="LA"
source-git-commit: 6610095b2af486bf64a1d875b5fb793cbfdc391d
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 3%

---

# Creación y administración de perfiles de prueba {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Crear perfiles de prueba"
>abstract="Los perfiles de prueba se crean como direcciones semilla. Son destinatarios adicionales en la base de datos utilizada para dirigirse a perfiles ficticios que no coinciden con los criterios de destino definidos."

Los perfiles de prueba se crean como direcciones semilla. Son destinatarios adicionales en la base de datos utilizada para dirigirse a perfiles ficticios que no coinciden con los criterios de destino definidos. Permiten previsualizar y probar la personalización y el procesamiento antes de realizar la entrega mediante la entrega de pruebas.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

Los pasos para enviar mensajes de prueba a las direcciones semilla se detallan en [esta sección](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>Los perfiles de prueba se excluyen automáticamente de los informes en las siguientes estadísticas de envío: **[!UICONTROL Clics]**, **[!UICONTROL Aperturas]**, **[!UICONTROL Baja de suscripciones]**.

## Acceso y administración de perfiles de prueba {#access-test-profiles}

Para acceder a la lista de plantillas de contenido, seleccione **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]** en el menú de la izquierda y seleccione. **[!UICONTROL Perfiles de prueba]** pestaña.

Puede filtrar por un [carpeta](../get-started/permissions.md#folders) mediante la lista desplegable o agregue reglas utilizando [modelador de consultas](../query/query-modeler-overview.md).

Para editar un perfil de prueba, haga clic en el elemento deseado de la lista.

Para eliminar un perfil de prueba, seleccione la opción correspondiente en la **[!UICONTROL Más acciones]** menú.

## Creación de un perfil de prueba {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Datos adicionales de perfiles de prueba"
>abstract="Introduzca los datos de personalización utilizados para las entregas creadas en los flujos de trabajo de gestión de datos y a los que desea asignar un valor específico."

Para crear un perfil de prueba, siga los pasos a continuación.

1. Navegar a **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]**.

1. Seleccione el **[!UICONTROL Perfiles de prueba]** pestaña.

   ![](assets/test-profile-list.png)

1. Haga clic en **[!UICONTROL Crear perfil de prueba]** botón.

1. Complete los detalles del perfil de prueba. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >La etiqueta de la dirección se rellena automáticamente con el nombre y los apellidos definidos.

1. De forma predeterminada, los perfiles de prueba se almacenan en **[!UICONTROL Direcciones semilla]** carpeta. Puede cambiarlo navegando a la ubicación deseada. [Más información](#seed-addresses-folders)

   ![](assets/test-profile-folder.png)

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. En el **[!UICONTROL Información de contacto]** , introduzca la dirección de correo electrónico y otros datos relevantes. La dirección de correo electrónico se muestra entre corchetes después de la etiqueta del perfil de prueba.

   ![](assets/test-profile-address.png)

1. Si selecciona la opción **[!UICONTROL Ya no se puede contactar (por ningún canal)]** , el perfil se encuentra en la lista de bloqueados de la. Este destinatario ya no está dirigido a ningún canal (correo electrónico, SMS, etc.).

1. En el **[!UICONTROL Datos adicionales]** , introduzca los datos de personalización utilizados para las entregas creadas en los flujos de trabajo de gestión de datos y a los que desea asignar un valor específico. [Más información sobre los flujos de trabajo](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png)

   Asegúrese de que se han definido datos de destino adicionales con un alias que comience por &#39;@&#39; en **[!UICONTROL Enriquecimiento]** actividad de flujo de trabajo. De lo contrario, no puede utilizarlo correctamente con sus direcciones semilla en la actividad de envío. [Descubra más información sobre la actividad Enriquecimiento](../workflows/activities/enrichment.md)

1. Haga clic en el botón **[!UICONTROL Save]**.

El perfil de prueba que acaba de crear ya está listo para utilizarse para enviar una prueba. [Más información](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## Administración de carpetas de direcciones semilla {#seed-addresses-folders}

Las direcciones semilla se almacenan en un nodo específico de la jerarquía de Adobe Campaign: **[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Direcciones semilla]**.

Para organizar los perfiles de prueba, puede crear subcarpetas desde la lista desplegable Más acciones. [Obtenga información sobre cómo crear carpetas](../get-started/permissions.md#folders)

![](assets/test-profile-sub-folders.png)

También puede crear un perfil de prueba a partir de cualquier **[!UICONTROL Direcciones semilla]** carpeta o subcarpeta. Complete todos los detalles de la misma manera que lo haría desde el **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]** menú. [Más información](#create-test-profile)

Para editar un perfil de prueba, haga clic en su etiqueta desde el **[!UICONTROL Perfiles de prueba]** o desde la carpeta en la que está almacenada.


