---
title: Introducción a los perfiles
description: Obtenga información sobre cómo monitorizar y administrar perfiles en Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 14%

---

# Introducción a los perfiles {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfiles"
>abstract="Un perfil es un registro que está destinado a recibir mensajes enviados por Adobe Campaign. En esta lista, puede ver los detalles de los perfiles en función de sus permisos. Utilice las opciones de filtrado para examinar esta lista. Puede editar y actualizar un pequeño conjunto de atributos de los perfiles."

## ¿Qué es un perfil? {#what}

Un **perfil**, también conocido como &quot;destinatario&quot; en la consola del cliente, representa un registro almacenado en la base de datos de Campaign. Sirve como un componente clave para [crear audiencias](create-audience.md) para entregas y [agregar datos de personalización](../personalization/personalize.md) al contenido. Adobe Campaign permite una administración perfecta de los perfiles, incluida la creación de nuevas entradas y el acceso a una vista completa de los atributos de todos los perfiles y las suscripciones a servicios, a través de la interfaz de usuario web de Campaign.

Además, los **[!UICONTROL perfiles de prueba]**, identificados como &quot;perfiles semilla&quot; en la consola del cliente, permiten segmentar destinatarios adicionales que no coinciden con los criterios de segmentación de una entrega determinada. Estos perfiles contienen información ficticia de contacto o información de contacto controlada por el remitente. Los perfiles de prueba son destinatarios de prueba que se utilizan para probar mensajes mediante el envío de pruebas. [Aprenda a trabajar con perfiles de prueba](test-profiles.md)

Tanto los perfiles como los perfiles de prueba son útiles para probar los envíos antes de que lleguen a la audiencia deseada. Esto permite obtener una vista previa del contenido y la personalización de los mensajes, enviar pruebas para pruebas y validación, evaluar el procesamiento de los correos electrónicos en varias plataformas y dispositivos y probar las páginas de aterrizaje. [Obtenga información sobre cómo previsualizar y probar envíos](../preview-test/preview-test.md)

➡️ [Descubra esta funcionalidad en vídeo](#video)

## Acceso a la lista de perfiles {#access}

Los perfiles son accesibles y editables en Adobe Campaign Web desde la entrada **[!UICONTROL Administración de clientes]** > **Perfiles** en el carril de navegación izquierdo. También se puede acceder a ellos desde la vista **[!UICONTROL Explorer]**, desde el nodo **[!UICONTROL Profiles &amp; Targets]** > **[!UICONTROL Recipients]**. A partir de ahí, examine, cree y administre carpetas o subcarpetas, así como permisos asociados. [Más información sobre cómo crear carpetas](../get-started/permissions.md#folders).

>[!NOTE]
>
>Según los permisos, es posible que no tenga acceso a la lista completa de perfiles almacenados en la base de datos. [Más información sobre los permisos](../get-started/permissions.md)

Filtre la lista **[!UICONTROL Perfiles]** mediante el campo de búsqueda o los filtros disponibles con el botón **Mostrar filtros**. Restrinja los resultados a una [carpeta](../get-started/permissions.md#folders) específica mediante la lista desplegable o agregue reglas mediante el [modelador de consultas](../query/query-modeler-overview.md).

![Filtros disponibles en la lista de perfiles](assets/profiles-list-filters.png){zoomable="yes"}

Para acceder a los detalles de un perfil, haga clic en su nombre en la lista. Se abre una vista detallada del perfil, que permite explorar sus atributos y los servicios a los que se suscribió el perfil. [Aprenda a explorar los detalles de los perfiles](create-profile.md)

Para eliminar un perfil, seleccione la opción correspondiente en el menú **[!UICONTROL Más acciones]**.

## Vídeos explicativos {#video}

Obtenga información sobre cómo acceder, administrar y explorar perfiles mediante la interfaz de usuario web de Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3448367?captions=spa&quality=12)