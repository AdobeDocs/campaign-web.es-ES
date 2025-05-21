---
title: Creación de perfiles de prueba en Campaign
description: Obtenga información sobre cómo crear y administrar perfiles de prueba en Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 15%

---

# Creación y administración de perfiles de prueba {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Crear perfiles de prueba"
>abstract="Los perfiles de prueba son destinatarios adicionales que permiten previsualizar y probar la personalización así como el procesamiento antes de enviar los mensajes. Puede seleccionar un perfil de prueba al obtener una vista previa del contenido de un mensaje y enviar pruebas a los perfiles de prueba para controlar y validar el contenido y la configuración del mensaje."

Los perfiles de prueba se utilizan para enviar pruebas y validar el contenido y la configuración del mensaje. Estos perfiles son destinatarios adicionales que le permiten previsualizar y probar la personalización y el procesamiento antes de enviar los mensajes. Puede seleccionar un perfil de prueba al obtener una vista previa del contenido de un mensaje y enviar pruebas a los perfiles de prueba para controlar y validar el contenido y la configuración del mensaje.

➡️ [Descubra esta funcionalidad en vídeo](#video)

<!--Learn more about test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=es){target="_blank"}.-->

Los pasos para enviar pruebas a perfiles de prueba se detallan en [esta sección](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>* Los perfiles de prueba se crean como direcciones semilla en la consola del cliente.
>
>* Los perfiles de prueba se excluyen automáticamente de los informes en las siguientes estadísticas de envío: **[!UICONTROL Clics]**, **[!UICONTROL Aperturas]**, **[!UICONTROL Cancelaciones de suscripciones]**.

## Acceso y administración de perfiles de prueba {#access-test-profiles}

Para obtener acceso a la lista de perfiles de prueba, seleccione **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]** en el menú de la izquierda y haga clic en la ficha **[!UICONTROL Perfiles de prueba]**.

![Vista de lista de perfiles de prueba](assets/test-profile-list.png){zoomable="yes"}

* Puede filtrar una [carpeta](../get-started/permissions.md#folders) específica mediante la lista desplegable o agregar reglas mediante [modelador de consultas](../query/query-modeler-overview.md).

  ![Filtros de lista de perfiles de prueba](assets/test-profile-list-filters.png){zoomable="yes"}

* Puede duplicar cualquier perfil de prueba y actualizarlo según sea necesario. Los pasos para editar un perfil de prueba son los mismos que al [crear un perfil de prueba](#create-test-profile).

* Para eliminar un perfil de prueba, seleccione la opción correspondiente en el menú **[!UICONTROL Más acciones]**.

  ![Eliminar opción de perfil de prueba](assets/test-profile-list-delete.png){zoomable="yes"}

* Para editar un perfil de prueba, haga clic en el elemento deseado de la lista. Los pasos para editar un perfil de prueba son los mismos que al [crear un perfil de prueba](#create-test-profile).

También puede acceder a los perfiles de prueba a través de la vista **[!UICONTROL Explorer]**, desde el nodo **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]**.

Desde allí, puede examinar, crear y administrar carpetas o subcarpetas, así como comprobar los permisos asociados. [Más información sobre cómo crear carpetas](../get-started/permissions.md#folders)

![Vista de carpetas de perfiles de prueba](assets/test-profiles-folders.png){zoomable="yes"}

Desde la vista **[!UICONTROL Explorador]**, también puede filtrar, eliminar, editar y [crear](#create-test-profile) perfiles de prueba.

## Creación de un perfil de prueba {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Datos adicionales de los perfiles de prueba"
>abstract="Introduzca los datos de personalización utilizados para los envíos creados en los flujos de trabajo de administración de datos y a los que desea asignar un valor específico."

Para crear un perfil de prueba, siga los pasos a continuación:

1. Vaya a **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]** y seleccione la pestaña **[!UICONTROL Perfiles de prueba]**.

1. Haga clic en el botón **[!UICONTROL Crear perfil de prueba]**.

   ![Botón Crear perfil de prueba](assets/test-profile-create.png){zoomable="yes"}

1. Complete los detalles del perfil de prueba según sea necesario. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![Formulario de detalles del perfil de prueba](assets/test-profile-details.png){zoomable="yes"}

   >[!NOTE]
   >
   >El campo **[!UICONTROL Etiqueta]** se rellena automáticamente con el nombre y los apellidos definidos.

1. De manera predeterminada, los perfiles de prueba se almacenan en la carpeta **[!UICONTROL Seed addresses]**. Puede cambiarlo navegando a la ubicación deseada. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. En la sección **[!UICONTROL Información de contacto]**, escriba la dirección de correo electrónico y otros datos relevantes. La dirección de correo electrónico se muestra entre corchetes después de la etiqueta del perfil de prueba.

   ![Sección de información de contacto](assets/test-profile-address.png){zoomable="yes"}

1. Si selecciona la casilla de verificación **[!UICONTROL No longer contact (by any channel)]**, el perfil de prueba está a la lista de bloqueados de la. Este destinatario ya no está dirigido a ningún canal (correo electrónico, SMS, etc.).

1. En la pestaña **[!UICONTROL Datos adicionales]**, introduzca los datos de personalización utilizados para las entregas creadas en los flujos de trabajo de gestión de datos y a los que desea asignar un valor específico. [Más información sobre los flujos de trabajo](../workflows/gs-workflows.md)

   ![Ficha de datos adicionales](assets/test-profile-additional-data.png){zoomable="yes"}

   Asegúrese de que se hayan definido datos de destino adicionales con un alias que comience por &#39;@&#39; en la actividad de flujo de trabajo **[!UICONTROL Enrichment]**. De lo contrario, no puede utilizarlo correctamente con sus direcciones semilla en la actividad de envío. [Más información sobre la actividad de enriquecimiento](../workflows/activities/enrichment.md)

1. Haga clic en el botón **[!UICONTROL Save]**.

El perfil de prueba que acaba de crear ya está listo para utilizarse para enviar una prueba. [Más información](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## Vídeos explicativos {#video}

Obtenga información sobre cómo crear y administrar perfiles de prueba mediante la interfaz de usuario web de Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3442898?quality=12&captions=spa)