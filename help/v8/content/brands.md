---
audience: end-user
title: Administrar marca
description: Aprenda a crear y administrar las directrices de marca
hide: true
hidefromtoc: true
badge: label="Beta" type="Informative"
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 2%

---

# Crear y administrar sus marcas {#brands}

>[!AVAILABILITY]
>
>Esta capacidad se presenta como una versión beta privada. Estará disponible de forma progresiva para todos los clientes en próximas versiones.

Las directrices de marca son un conjunto completo de reglas y estándares que definen la identidad visual y verbal de una marca. Sirven como referencia para garantizar una representación de marca coherente en todos los canales de marketing y comunicación.

En [!DNL Adobe Campaign Web], los usuarios pueden escribir y organizar manualmente la información de marca o cargar documentos de directrices de marca para la extracción automática de datos.

## Acceso a marcas {#generative-access}

Para acceder al menú **[!UICONTROL Marcas]** en [!DNL Adobe Campaign Web], los usuarios deben tener asignados los perfiles de producto **[!UICONTROL Administrador (administrador)]** y **[!UICONTROL Kit de marca]** para crear y administrar marcas. Para obtener acceso de solo lectura, los usuarios necesitan el perfil de producto [!UICONTROL Asistente de IA].

[Más información](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Aprenda a asignar permisos relacionados con la marca

1. En la página de inicio de [Admin Console](https://adminconsole.adobe.com/enterprise), acceda a su producto de Campaign.

   ![Página de inicio de Admin Console con acceso al producto de Campaign](assets/brands_admin_1.png)

1. Seleccione **[!DNL Product profile]** según el nivel de permisos que desee otorgar al usuario.

   ![Selección de perfil de producto en Admin Console](assets/brands_admin_2.png)

1. Haga clic en **[!DNL Add users]** para asignar el perfil de producto seleccionado.

   ![Agregar opción de usuarios en Admin Console](assets/brands_admin_3.png)

1. Escriba el nombre, el grupo de usuarios o la dirección de correo electrónico del usuario.

1. Haga clic en **Guardar** para aplicar los cambios.

Los permisos de los usuarios que ya están asignados a esta función se actualizan automáticamente.

+++

## Cree su marca {#create-brand-kit}

Para crear y administrar las directrices de marca, siga los pasos a continuación.

Los usuarios pueden introducir los detalles manualmente o cargar un documento de directrices de marca para extraer la información automáticamente:

1. En el menú **[!UICONTROL Administración de contenido]**, seleccione **[!UICONTROL Marcas]**.

1. En el menú **[!UICONTROL Marcas]**, haga clic en **[!UICONTROL Crear marca]**.

   ![Menú de marcas con la opción Crear marca](assets/brands_1.png)

1. Escriba un **[!UICONTROL Nombre]** para su marca.

1. Arrastre y suelte o seleccione el archivo para cargar las directrices de marca y extraer automáticamente la información de marca relevante. Haga clic en **[!UICONTROL Crear marca]**.

   Comienza el proceso de extracción de información. Tenga en cuenta que puede tardar varios minutos en completarse.

   ![Carga de archivos para la extracción de directrices de marca](assets/brands_7.png)

1. El contenido y los estándares de creación visual se rellenan automáticamente. Examine las diferentes pestañas para adaptar la información según sea necesario.

1. En la ficha **[!UICONTROL Estilo de escritura]**, haga clic en ![Agregar icono](assets/do-not-localize/Smock_Add_18_N.svg) para agregar una directriz o exclusión, incluidos ejemplos.

   ![Ficha Estilo de escritura con la opción Agregar directriz](assets/brands_2.png)

1. En la ficha **[!UICONTROL Contenido visual]**, haga clic en ![Agregar icono](assets/do-not-localize/Smock_Add_18_N.svg) para agregar otra directriz o exclusión.

1. Para agregar una imagen que muestre el uso correcto, seleccione **[!UICONTROL Ejemplos]** y haga clic en **[!UICONTROL Seleccionar imagen]**. También puede añadir una imagen que muestre un uso incorrecto como ejemplo de exclusión.

   ![Pestaña de contenido visual con opciones de imagen de ejemplo](assets/brands_3.png)

1. Una vez configurada, haz clic en **[!UICONTROL Guardar]** y luego en **[!UICONTROL Publicar]** para que la guía de marca esté disponible en el asistente de IA.

1. Para modificar tu marca publicada, haz clic en **[!UICONTROL Editar marca]**.

   >[!NOTE]
   >
   >Esto crea una copia temporal en el modo de edición y reemplaza la versión activa una vez publicada.

   ![Editar opción de marca en el menú Marcas](assets/brands_4.png)

1. En tu panel de **[!UICONTROL Marcas]**, abre el menú avanzado haciendo clic en el icono de ![Más opciones](assets/do-not-localize/Smock_More_18_N.svg) para:

   * Ver marca
   * Editar
   * Duplicar
   * Publicación
   * Cancelar publicación
   * Eliminar

   ![Opciones de menú avanzadas en el panel Marcas](assets/brands_5.png)

Ahora se puede acceder a las directrices de marca desde la lista desplegable **[!UICONTROL Marca]** del menú del asistente de IA. Esto permite al asistente de IA generar contenido y recursos alineados con las especificaciones. [Más información sobre el asistente de IA](../email/generative-gs.md)

![Menú del asistente de IA con la lista desplegable de Marca](assets/brands_6.png)