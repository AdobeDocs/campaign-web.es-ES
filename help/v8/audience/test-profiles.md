---
title: Crear prueba perfiles en Campaign
description: Aprenda a crear y administrar perfiles prueba en Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 15%

---

# Creación y administración de perfiles de prueba {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Crear perfiles de prueba"
>abstract="Los perfiles de prueba son destinatarios adicionales que permiten previsualizar y probar la personalización así como el procesamiento antes de enviar los mensajes. Puede seleccionar un perfil de prueba al obtener una vista previa del contenido de un mensaje y enviar pruebas a los perfiles de prueba para controlar y validar el contenido y la configuración del mensaje."

Los perfiles de prueba se utilizan para enviar pruebas y validar los contenido y la configuración del mensaje. Estos perfiles son destinatarios adicionales que le permiten previsualización y prueba la personalización y el procesamiento antes de enviar los mensajes. Puede seleccionar un perfil de prueba al obtener una vista previa de un contenido de mensaje y enviar pruebas a los perfiles de prueba para controlar y validar la contenido y la configuración del mensaje.

➡️ [Descubra esta funcionalidad en vídeo](#video)

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

En esta sección](../preview-test/test-deliveries.md#test-profiles) se describen [los pasos para enviar pruebas a prueba perfiles.

>[!NOTE]
>
>* Los perfiles de prueba se crean como direcciones semilla en la consola del cliente.
>
>* Los perfiles de prueba se excluyen automáticamente de los informes en las siguientes estadísticas de envío: **[!UICONTROL Clics,**[!UICONTROL  Aperturas ]**]**]**y**[!UICONTROL  Bajas de suscripción.

## Acceso y administrar perfiles prueba {#access-test-profiles}

Para acceder al prueba perfil lista, seleccione **[!UICONTROL Administración de]** clientes > **[!UICONTROL Perfiles]** en el menú de la izquierda y haga clic en el **[!UICONTROL pestaña Probar perfiles]** .

![Prueba perfil lista vista](assets/test-profile-list.png){zoomable="yes"}

* Puede filtrar en una carpeta específica [mediante el lista desplegable o agregar reglas con el modelador](../query/query-modeler-overview.md) consulta[](../get-started/permissions.md#folders).

  ![Prueba perfil lista filtros](assets/test-profile-list-filters.png){zoomable="yes"}

* Puede duplicado cualquier perfil prueba y actualizarla según resulte necesario. Los pasos para editar un perfil de prueba son los mismos que al [crear un perfil prueba](#create-test-profile).

* Para eliminar un perfil prueba, seleccione la opción correspondiente en el **[!UICONTROL menú Más acciones]** .

  ![Eliminar prueba opción perfil](assets/test-profile-list-delete.png){zoomable="yes"}

* Para editar una perfil prueba, haga clic en el elemento deseado del lista. Los pasos para editar un perfil de prueba son los mismos que al [crear un perfil prueba](#create-test-profile).

También puede acceder a prueba perfiles a través del **[!UICONTROL vista Explorer]**, desde las **[!UICONTROL direcciones]** de Recursos ]**>**[!UICONTROL  Campaign Administración ]**>**[!UICONTROL  Semilla nodo.

Desde allí, puede examinar, crear y administrar carpetas o subcarpetas, así como comprobar los permisos asociados. [Aprenda a crear carpetas](../get-started/permissions.md#folders)

![Carpetas de perfiles de prueba vista](assets/test-profiles-folders.png){zoomable="yes"}

Desde Explorer **** vista, también puede filtrar, eliminar, editar y [crear](#create-test-profile) prueba perfiles.

## Creación de un perfil de prueba {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Datos adicionales de los perfiles de prueba"
>abstract="Introduzca los datos de personalización utilizados para los envíos creados en los flujos de trabajo de administración de datos y a los que desea asignar un valor específico."

Para crear una perfil de prueba, seguir los pasos siguientes:

1. Examinar a **[!UICONTROL Administración de]** clientes > **[!UICONTROL Perfiles]** y seleccione la **[!UICONTROL pestaña Probar perfiles]** .

1. Haga clic en la **[!UICONTROL Crear prueba perfil]** botón.

   ![Crear prueba perfil botón](assets/test-profile-create.png){zoomable="yes"}

1. Complete la prueba perfil detalles según sea necesario. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![Formulario de detalles del perfil de prueba](assets/test-profile-details.png){zoomable="yes"}

   >[!NOTE]
   >
   >El **[!UICONTROL campo Etiquetar]** se rellena automáticamente con el nombre y los apellidos definidos.

1. De forma predeterminada, prueba perfiles se almacenan en la **[!UICONTROL carpeta de direcciones]** semilla. Puede cambiarla desplazándose a la ubicación deseada. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. En la sección Información ]**de**[!UICONTROL  contacto, introduzca la dirección correo electrónico y otros datos relevantes. La dirección del correo electrónico se muestra entre corchetes después del prueba perfil etiqueta.

   ![Sección Información de contacto](assets/test-profile-address.png){zoomable="yes"}

1. Si selecciona la **[!UICONTROL casilla Ya no se puede contactar (por cualquier canal),]** el perfil de prueba está en la lista de denegación. Estas destinatario ya no están dirigidas a ningún canal (correo electrónico, SMS, etc.).

1. En el **[!UICONTROL pestaña Datos]** adicionales, introduzca los datos personalización utilizados para los envíos creados en el flujos de trabajo de administración de datos y a los que desea asignar un valor específico. [Más información sobre flujos de trabajo](../workflows/gs-workflows.md)

   ![Datos adicionales pestaña](assets/test-profile-additional-data.png){zoomable="yes"}

   Asegúrese de que los datos de destino adicionales se hayan definido con un alias que comience con &quot;@&quot; en la **[!UICONTROL actividad de flujo de trabajo enriquecimiento]** . De lo contrario, no podrá utilizarlo correctamente con los direcciones semilla en el actividad envío. [Obtenga más información sobre el actividad de enriquecimiento](../workflows/activities/enrichment.md)

1. Haga clic en el botón **[!UICONTROL Save]**.

El prueba perfil que acaba de crear ya está listo para ser utilizado para enviar una prueba. [Más información](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## Vídeos explicativos {#video}

Aprenda a crear y administrar perfiles prueba utilizando la interfaz de Campaign Web usuario.

>[!VIDEO](https://video.tv.adobe.com/v/3442844?quality=12)