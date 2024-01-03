---
title: Monitorización y administración de perfiles
description: Obtenga información sobre cómo monitorizar y administrar perfiles en Campaign Web.
badge: label="Disponibilidad limitada"
source-git-commit: a53f33360f0dc7ca80b235bd5814fd3ccc0ff698
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 9%

---

# Monitorización y administración de perfiles {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Vista 360 de sus perfiles"
>abstract="Cree nuevos perfiles y monitorícelos con potentes informes y herramientas. Acceda a los atributos, interacciones y registros de sus perfiles. Utilice las opciones de filtrado para examinar la lista de perfiles, editar y actualizar su perfil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Consulte las notas de la versión"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfiles"
>abstract="Un perfil es una persona que está destinada a recibir mensajes enviados por Adobe Campaign. Desde esta lista, puede ver los detalles de los perfiles en función de sus permisos. Utilice las opciones de filtrado para examinar esta lista. Puede editar y actualizar un pequeño conjunto de atributos de sus perfiles."

## Introducción a los perfiles {#gs}

Un perfil en Adobe Campaign Web es una persona almacenada en la base de datos, que sirve como componente clave para crear audiencias para envíos y agregar datos de personalización al contenido. En la base de datos se almacenan varios tipos de perfiles, como perfiles de prueba, que están diseñados para probar los envíos antes de enviarlos a la audiencia final. [Aprenda a trabajar con perfiles de prueba](test-profiles.md)

Los perfiles solo se pueden agregar desde la consola del cliente de Campaign. Sin embargo, se puede acceder a ellas desde Adobe Campaign Web desde el **Perfiles** en el carril de navegación izquierdo. También puede acceder a ellas desde el **Explorer** , donde puede examinar, crear carpetas y subcarpetas y comprobar los permisos asociados.

Puede filtrar la lista de perfiles mediante el campo de búsqueda o los filtros disponibles en el **Mostrar filtros** botón.

![](assets/profiles-list.png)

>[!NOTE]
>
>Según los permisos, es posible que no tenga acceso a la lista completa de perfiles almacenados en la base de datos. Puede obtener más información sobre permisos en [esta sección](../get-started/permissions.md).

## Acceso y edición de atributos de perfiles {#access}

Para acceder a los detalles de un perfil, haga clic en su nombre en la lista de perfiles.

![](assets/profiles-details.png)

Desde esta pantalla, puede acceder a información detallada sobre el perfil:

* El **[!UICONTROL Detalles]** permite examinar los atributos del perfil. Para editar un atributo, realice cambios en el campo deseado y haga clic en **[!UICONTROL Guardar]** botón.
* El **[!UICONTROL Suscripciones]** proporciona información sobre los servicios a los que está suscrito el perfil. [Descubra cómo trabajar con servicios de suscripción](manage-services.md)
* El **[!UICONTROL Registros]** El botón situado en la esquina superior derecha de la pantalla le permite ver un historial de las interacciones del perfil a través del envío, la exclusión y los registros de seguimiento, así como las propuestas presentadas al perfil.
