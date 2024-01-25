---
title: Introducción a los perfiles
description: Obtenga información sobre cómo monitorizar y administrar perfiles en Campaign Web.
badge: label="Disponibilidad limitada"
source-git-commit: 22b183a739dd92d7c4245fb4694034a247511d75
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 33%

---

# Introducción a los perfiles {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Vista 360 de sus perfiles"
>abstract="Cree nuevos perfiles y monitorícelos con potentes informes y herramientas. Acceda a los atributos, interacciones y registros de sus perfiles. Utilice las opciones de filtrado para examinar la lista de perfiles y editar y actualizar su perfil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=es" text="Consulte las notas de la versión"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Vista 360 de sus perfiles"
>abstract="Cree nuevos perfiles y monitorícelos con potentes informes y herramientas. Acceda a los atributos, interacciones y registros de sus perfiles. Utilice las opciones de filtrado para examinar la lista de perfiles y editar y actualizar su perfil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=es" text="Consulte las notas de la versión"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfiles"
>abstract="Un perfil es una persona que está destinada a recibir mensajes enviados por Adobe Campaign. En esta lista, puede ver los detalles de los perfiles en función de sus permisos. Utilice las opciones de filtrado para examinar esta lista. Puede editar y actualizar un pequeño conjunto de atributos de los perfiles."

## ¿Qué es un perfil? {#what}

Un perfil en Adobe Campaign Web es una persona almacenada en la base de datos y que sirve como componente clave para [crear audiencias](create-audience.md) para entregas y [añadir personalización](../personalization/personalize.md) datos en el contenido.

Adobe Campaign le permite crear y supervisar sus perfiles directamente desde la interfaz de. Desde aquí puede crear perfiles, acceder a una vista detallada de los mismos y editarlos.

En la base de datos se almacenan otros tipos de perfiles, como **[!UICONTROL Perfiles de prueba]**, diseñadas para probar los envíos antes de enviarlos a la audiencia final. [Aprenda a trabajar con perfiles de prueba](test-profiles.md)

## Acceso a la lista de perfiles {#access}

Los perfiles son accesibles y editables en Adobe Campaign Web desde el **[!UICONTROL Administración de clientes]** > **Perfiles** en el carril de navegación izquierdo.

También puede acceder a ellas a través del **[!UICONTROL Explorer]** vista, desde el **[!UICONTROL Perfiles y objetivos]** > **[!UICONTROL Destinatarios]** nodo. Desde allí puede examinar, crear y administrar carpetas o subcarpetas, así como comprobar los permisos asociados. [Obtenga información sobre cómo crear carpetas](../get-started/permissions.md#folders)

>[!NOTE]
>
>Según los permisos, es posible que no tenga acceso a la lista completa de perfiles almacenados en la base de datos. [Más información sobre los permisos](../get-started/permissions.md).

Puede filtrar la variable **[!UICONTROL Perfiles]** mediante el campo de búsqueda o filtros disponibles en la lista **Mostrar filtros** botón. Puede restringir los resultados a un específico [carpeta](../get-started/permissions.md#folders) mediante la lista desplegable o agregue reglas utilizando la variable [modelador de consultas](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png)

Para acceder a los detalles de un perfil, haga clic en su nombre en la lista. Se abre una vista detallada del perfil, que le permite explorar sus atributos y los servicios a los que se suscribió. [Obtenga información sobre cómo explorar los detalles de los perfiles](create-profile.md)

Para eliminar un perfil, seleccione la opción correspondiente en la **[!UICONTROL Más acciones]** menú.
