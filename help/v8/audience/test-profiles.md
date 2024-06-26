---
title: Creación de perfiles de prueba en Campaign
description: Obtenga información sobre cómo crear y administrar perfiles de prueba en Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 20%

---

# Creación y administración de perfiles de prueba {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Crear perfiles de prueba"
>abstract="Los perfiles de prueba son destinatarios adicionales que permiten previsualizar y probar la personalización así como el procesamiento antes de enviar los mensajes. Puede seleccionar un perfil de prueba al obtener una vista previa del contenido de un mensaje y enviar pruebas a los perfiles de prueba para controlar y validar el contenido y la configuración del mensaje."

Los perfiles de prueba se utilizan para enviar pruebas y validar el contenido y la configuración del mensaje. Estos perfiles son destinatarios adicionales que le permiten previsualizar y probar la personalización y el procesamiento antes de enviar los mensajes. Puede seleccionar un perfil de prueba al obtener una vista previa del contenido de un mensaje y enviar pruebas a los perfiles de prueba para controlar y validar el contenido y la configuración del mensaje.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

Los pasos para enviar pruebas a los perfiles de prueba se detallan en [esta sección](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>* Los perfiles de prueba se crean como direcciones semilla en la consola del cliente.
>
>* Los perfiles de prueba se excluyen automáticamente de los informes en las siguientes estadísticas de envío: **[!UICONTROL Clics]**, **[!UICONTROL Aperturas]**, **[!UICONTROL Baja de suscripciones]**.

## Acceso y administración de perfiles de prueba {#access-test-profiles}

Para acceder a la lista de perfiles de prueba, seleccione **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]** en el menú de la izquierda y haga clic en **[!UICONTROL Perfiles de prueba]** pestaña.

![](assets/test-profile-list.png){zoomable="yes"}

* Puede filtrar por un [carpeta](../get-started/permissions.md#folders) mediante la lista desplegable o agregue reglas utilizando [modelador de consultas](../query/query-modeler-overview.md).

  ![](assets/test-profile-list-filters.png){zoomable="yes"}

* Puede duplicar cualquier perfil de prueba y actualizarlo según sea necesario. Los pasos para editar un perfil de prueba son los mismos que cuando [creación de un perfil de prueba](#create-test-profile).

* Para eliminar un perfil de prueba, seleccione la opción correspondiente en la **[!UICONTROL Más acciones]** menú.

  ![](assets/test-profile-list-delete.png){zoomable="yes"}

* Para editar un perfil de prueba, haga clic en el elemento deseado de la lista. Los pasos para editar un perfil de prueba son los mismos que cuando [creación de un perfil de prueba](#create-test-profile).

También puede acceder a los perfiles de prueba a través del **[!UICONTROL Explorer]** vista, desde el **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Direcciones semilla]** nodo.

Desde allí puede examinar, crear y administrar carpetas o subcarpetas, así como comprobar los permisos asociados. [Obtenga información sobre cómo crear carpetas](../get-started/permissions.md#folders)

![](assets/test-profiles-folders.png){zoomable="yes"}

Desde el **[!UICONTROL Explorer]** vista también puede filtrar, eliminar, editar y [crear](#create-test-profile) perfiles de prueba.

## Creación de un perfil de prueba {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Datos adicionales de los perfiles de prueba"
>abstract="Introduzca los datos de personalización utilizados para los envíos creados en los flujos de trabajo de administración de datos y a los que desea asignar un valor específico."

Para crear un perfil de prueba, siga los pasos a continuación:

1. Navegar a **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]** y seleccione la **[!UICONTROL Perfiles de prueba]** pestaña.

1. Haga clic en **[!UICONTROL Crear perfil de prueba]** botón.

   ![](assets/test-profile-create.png){zoomable="yes"}

1. Complete los detalles del perfil de prueba según sea necesario. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png){zoomable="yes"}

   >[!NOTE]
   >
   >El **[!UICONTROL Etiqueta]** El campo se rellena automáticamente con el nombre y los apellidos definidos.

1. De forma predeterminada, los perfiles de prueba se almacenan en **[!UICONTROL Direcciones semilla]** carpeta. Puede cambiarlo navegando a la ubicación deseada. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. En el **[!UICONTROL Información de contacto]** , introduzca la dirección de correo electrónico y otros datos relevantes. La dirección de correo electrónico se muestra entre corchetes después de la etiqueta del perfil de prueba.

   ![](assets/test-profile-address.png){zoomable="yes"}

1. Si selecciona la opción **[!UICONTROL Ya no se puede contactar (por ningún canal)]** incluir en la lista de bloqueados casilla de verificación, el perfil de prueba está a la. Este destinatario ya no está dirigido a ningún canal (correo electrónico, SMS, etc.).

1. En el **[!UICONTROL Datos adicionales]** , introduzca los datos de personalización utilizados para las entregas creadas en los flujos de trabajo de gestión de datos y a los que desea asignar un valor específico. [Más información sobre los flujos de trabajo](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png){zoomable="yes"}

   Asegúrese de que se han definido datos de destino adicionales con un alias que comience por &#39;@&#39; en **[!UICONTROL Enriquecimiento]** actividad de flujo de trabajo. De lo contrario, no puede utilizarlo correctamente con sus direcciones semilla en la actividad de envío. [Descubra más información sobre la actividad Enriquecimiento](../workflows/activities/enrichment.md)

1. Haga clic en el botón **[!UICONTROL Save]**.

El perfil de prueba que acaba de crear ya está listo para utilizarse para enviar una prueba. [Más información](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->
