---
title: Introducción a los perfiles
description: Aprenda a monitor y administrar perfiles en Campaign web.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 11%

---

# Introducción a los perfiles {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfiles"
>abstract="Un perfil es un registro destinado a recibir mensajes enviados por Adobe Campaign. En esta lista, puede ver los detalles de los perfiles en función de sus permisos. Utilice las opciones de filtrado para examinar esta lista. Puede editar y actualizar un pequeño conjunto de atributos de los perfiles."

## ¿Qué es un perfil? {#what}

Un **perfil**, también conocido como &quot;destinatario&quot; en la consola del cliente, representa un registro almacenado en la base de datos Campaign. Sirve como un componente clave para [crear audiencias para las entregas](create-audience.md) y [agregar datos personalización](../personalization/personalize.md) a su contenido. Adobe Campaign permite una gestión fluida de los perfiles, incluida la creación de nuevas entradas y el acceso a una vista completa de los atributos de todos los perfiles y las suscripciones de servicios, a través de la interfaz de Campaign Web usuario.

Además, **[!UICONTROL prueba perfiles]**, identificados como &quot;perfiles semilla&quot; en la consola del cliente, permiten direccionamiento de destinatarios adicionales que no coinciden con los criterios de direccionamiento de un envío determinado. Estos perfiles contienen información de contacto ficticia o información de contacto controlada por el remitente. Los perfiles de prueba son prueba destinatarios utilizados para prueba mensajes mediante el envío de pruebas. [Aprenda a trabajar con perfiles prueba](test-profiles.md)

Tanto los perfiles como los perfiles prueba son útiles para probar los envíos antes de que alcancen el audiencia previsto. Esto permite obtener una vista previa de la contenido y el personalización de mensajes, enviar pruebas para pruebas y validación, evaluar correo electrónico renderizar en varias plataformas y dispositivos, y probar páginas de destino. [Obtenga información sobre cómo previsualización y prueba entregas](../preview-test/preview-test.md)

➡️ [Descubra esta funcionalidad en vídeo](#video)

## Acceder a la lista de perfiles {#access}

Los perfiles son accesibles y editables en Adobe Campaign Web desde la **[!UICONTROL entrada Gestión de]** clientes > **Perfiles** en la parte izquierda navegación carril. También se puede acceder a ellos en el **[!UICONTROL vista Explorer]** , desde el **[!UICONTROL nodo Profiles &amp; Targets]** > **[!UICONTROL Recipients]** . Desde allí, examinar, crear y administrar carpetas o subcarpetas, así como comprobar los permisos asociados. [Aprenda a crear carpetas](../get-started/permissions.md#folders).

>[!NOTE]
>
>En función de sus permisos, es posible que no tenga acceso a la lista completa de perfiles almacenados en la base de datos. [Más información sobre los permisos](../get-started/permissions.md)

Filtrar los **[!UICONTROL perfiles]** lista utilizando el campo de búsqueda o los filtros disponibles en el **botón de filtros** de Mostrar. Restrinja los resultados a una carpeta[&#128279;](../get-started/permissions.md#folders) específica [mediante el lista desplegable o agregue reglas mediante el modelador](../query/query-modeler-overview.md) consulta.

![Filtros disponibles en los perfiles lista](assets/profiles-list-filters.png){zoomable="yes"}

Para acceder a los detalles de una perfil, haga clic en su nombre desde el lista. Se abre una vista detallada de la perfil, que permite explorar sus atributos y los servicios a los que perfil suscrito. [Obtén información sobre cómo explorar los detalles de los perfiles](create-profile.md)

Para eliminar un perfil, seleccione la opción correspondiente en el **[!UICONTROL menú Más acciones]** .

## Vídeos explicativos {#video}

Aprenda a acceder, administrar y explorar perfiles utilizando la interfaz de Campaign Web usuario.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)