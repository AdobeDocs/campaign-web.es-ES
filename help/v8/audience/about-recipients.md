---
title: Introducción a los perfiles
description: Obtenga información sobre cómo monitorizar y administrar perfiles en Campaign Web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: 5a4bf85a1f70a0282405aededfb31038f9db17a8
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 12%

---

# Introducción a los perfiles {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfiles"
>abstract="Un perfil es un registro que está destinado a recibir mensajes enviados por Adobe Campaign. En esta lista, puede ver los detalles de los perfiles en función de sus permisos. Utilice las opciones de filtrado para examinar esta lista. Puede editar y actualizar un pequeño conjunto de atributos de los perfiles."

## ¿Qué es un perfil? {#what}

A **perfil**, también conocido como &quot;destinatario&quot; en la consola del cliente, representa un registro almacenado en la base de datos de Campaign, que sirve como componente clave para [crear audiencias](create-audience.md) para entregas y [añadir personalización](../personalization/personalize.md) datos en el contenido. Adobe Campaign le permite administrar perfiles sin problemas, desde la creación de nuevas entradas al acceso a una vista completa de todos los atributos y suscripciones a servicios de los perfiles, todo a través de la interfaz de usuario web de Campaign.

Además, **[!UICONTROL perfiles de prueba]**, identificados como &quot;perfiles semilla&quot; en la consola del cliente, le permiten dirigirse a destinatarios adicionales que no coinciden con los criterios de objetivo de una entrega determinada. Estos perfiles contienen información de contacto ficticia o información de contacto controlada por el remitente. Los perfiles de prueba son destinatarios de prueba: se utilizan para probar los mensajes enviando pruebas. [Aprenda a trabajar con perfiles de prueba](test-profiles.md)

Tanto los perfiles como los perfiles de prueba se pueden utilizar para probar los envíos antes de que lleguen a la audiencia deseada. Al hacerlo, puede obtener una vista previa del contenido y la personalización del mensaje, enviar pruebas para pruebas y validación, evaluar el procesamiento de correos electrónicos en varias plataformas y dispositivos y probar las páginas de aterrizaje. [Obtenga información sobre cómo previsualizar y probar entregas](../preview-test/preview-test.md)

➡️ [Descubra esta función en vídeo](#video)

## Acceso a la lista de perfiles {#access}

Los perfiles son accesibles y editables en Adobe Campaign Web desde el **[!UICONTROL Administración de clientes]** > **Perfiles** en el carril de navegación izquierdo. También puede acceder a ellas desde el **[!UICONTROL Explorer]** vista, desde el **[!UICONTROL Perfiles y objetivos]** > **[!UICONTROL Destinatarios]** nodo. Desde allí puede examinar, crear y administrar carpetas o subcarpetas, así como comprobar los permisos asociados. [Obtenga información sobre cómo crear carpetas](../get-started/permissions.md#folders)

>[!NOTE]
>
>Según los permisos, es posible que no tenga acceso a la lista completa de perfiles almacenados en la base de datos. [Más información sobre los permisos](../get-started/permissions.md).

Puede filtrar la variable **[!UICONTROL Perfiles]** mediante el campo de búsqueda o filtros disponibles en la lista **Mostrar filtros** botón. Puede restringir los resultados a un específico [carpeta](../get-started/permissions.md#folders) mediante la lista desplegable o agregue reglas utilizando la variable [modelador de consultas](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable="yes"}

Para acceder a los detalles de un perfil, haga clic en su nombre en la lista. Se abre una vista detallada del perfil, que le permite explorar sus atributos y los servicios a los que se suscribió. [Obtenga información sobre cómo explorar los detalles de los perfiles](create-profile.md)

Para eliminar un perfil, seleccione la opción correspondiente en la **[!UICONTROL Más acciones]** menú.

## Vídeos explicativos {#video}

Obtenga información sobre cómo acceder, administrar y explorar perfiles mediante la interfaz de usuario web de Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)
