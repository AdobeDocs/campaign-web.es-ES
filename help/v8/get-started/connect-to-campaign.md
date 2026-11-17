---
title: Conexión con la interfaz web de Adobe Campaign
description: Obtenga información sobre cómo conectarse a la interfaz de usuario de Adobe Campaign Web
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
TQID: 'https://experienceleague.adobe.com/TSbgkDH1v-9HH-szfGQx0z6-6fP8tny4s7Vx2SE8gUo'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
topic_v2:
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 7bbc2d4c383886788afc1ef83cdd27e7ec4b24ae
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 81%
---
# Conexión a Adobe Campaign {#connect-to-campaign}

[!DNL Adobe CX Enterprise] es la familia integrada de aplicaciones, productos y servicios de marketing digital de Adobe. Desde su intuitiva interfaz, puede acceder rápidamente a sus aplicaciones, funciones de productos y servicios en la nube. Obtenga información sobre cómo conectarse a [!DNL CX Enterprise] y obtener acceso a la interfaz web de Adobe Campaign en esta página.

## Iniciar sesión en [!DNL Adobe CX Enterprise] {#sign-in-to-exc}

También puede utilizar el inicio de sesión único (SSO) para conectarse a Campaign. Normalmente, [!DNL CX Enterprise] administradores conceden acceso a aplicaciones y servicios. Siga los pasos de la invitación del correo electrónico para [!DNL CX Enterprise].

Para iniciar sesión en [!DNL Adobe CX Enterprise], siga estos pasos básicos:

1. Vaya a [[!DNL Adobe CX Enterprise]](https://experience.adobe.com/){target="_blank"}.

1. Inicie sesión con su Adobe ID o Enterprise ID. Obtenga más información sobre los tipos de identidad en Adobe en [este artículo](https://helpx.adobe.com/es/enterprise/using/identity.html){target="_blank"}.

   Después de iniciar sesión en [!DNL CX Enterprise], puede acceder rápidamente a todas sus soluciones y aplicaciones.

   ![Captura de pantalla que muestra la página principal de Adobe CX Enterprise](assets/exc-home.png){zoomable="yes"}

1. Compruebe que se encuentra en la organización correcta.

   ![Captura de pantalla que muestra la selección de organizaciones en Adobe CX Enterprise](assets/exc-orgs.png){zoomable="yes"}{width="50%"}

   Obtenga más información acerca de las organizaciones en [!DNL Adobe CX Enterprise] en [este artículo](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=es){target="_blank"}.

## Acceso a Adobe Campaign {#access-to-campaign}

Para acceder a su entorno de Campaign, seleccione **Campaign** en la sección **Acceso rápido** de la página principal de [!DNL Adobe CX Enterprise].

Si ya está conectado a otra solución de [!DNL Adobe CX Enterprise], vaya al entorno de Campaign desde el conmutador de soluciones en la parte superior derecha de la pantalla.

![Captura de pantalla que muestra el conmutador de soluciones en Adobe CX Enterprise](assets/solution-switcher.png){zoomable="yes"}

Si tiene acceso a varios entornos, incluido el Panel de control de Campaign, haga clic en el botón **Iniciar** para la instancia correcta.

![Captura de pantalla que muestra el botón de inicio de Adobe Campaign](assets/launch-campaign.png){zoomable="yes"}

Ahora está conectado a Campaign. Obtenga información sobre cómo empezar a utilizar la interfaz de usuario en [esta página](user-interface.md).

### Control de acceso {#access-control}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="Permiso obligatorio"
>abstract="El administrador debe otorgarle permiso para poder crear este objeto."

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="Este público es de solo lectura"
>abstract="No tiene permisos para editar este público. Si es necesario, póngase en contacto con el administrador para que le conceda acceso."

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="Este servicio es de solo lectura"
>abstract="No tiene permisos para editar este servicio. Si es necesario, póngase en contacto con el administrador para que le conceda acceso."

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="Perfil de solo lectura de los destinatarios"
>abstract="No tiene permisos para editar este perfil. Si es necesario, póngase en contacto con el administrador para que le conceda acceso."

>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="Esta campaña es de solo lectura"
>abstract="No tiene permisos para editar esta campaña. Si es necesario, póngase en contacto con el administrador para que le conceda acceso."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="Este envío es de solo lectura"
>abstract="No tiene permisos para editar este envío. Si es necesario, póngase en contacto con el administrador para que le conceda acceso."

>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="Este flujo de trabajo es de solo lectura"
>abstract="No tiene permisos para editar este flujo de trabajo. Si es necesario, póngase en contacto con el administrador para que le conceda acceso."

El control de acceso restringe el acceso a objetos y datos de listas principales, como envíos, destinatarios o flujos de trabajo. Estas restricciones también se aplican en el árbol de navegación del Explorador. Además, necesita permisos para crear, eliminar, duplicar y editar objetos desde la interfaz de usuario.

Todos los permisos de la web de Campaign se sincronizan con los permisos de la consola del cliente de Campaign. Solo los administradores de Campaign pueden definir y modificar los permisos de usuario.

A medida que navega por la interfaz de usuario web de Campaign, puede acceder a datos, objetos y funcionalidades en función de sus permisos. Por ejemplo, si no tiene permisos de acceso a una carpeta, no podrá verla. Los permisos también afectan a la administración de objetos y datos. Sin permisos de escritura para una carpeta específica, no se puede crear un envío en dicha carpeta, aunque se pueda ver en la interfaz de usuario.

Puede aprender a [ver y administrar los permisos aquí](permissions.md).

## [!DNL Adobe CX Enterprise] navegación superior {#top-bar}

La barra superior de la interfaz le proporciona acceso rápido a las características principales de [!DNL CX Enterprise].

![Captura de pantalla que muestra la barra de navegación superior de Adobe CX Enterprise](assets/do-not-localize/unified-shell.png){zoomable="yes"}

Utilice la barra superior para:

* Compartir comentarios sobre la interfaz de usuario web de Campaign
* Cambie entre sus organizaciones.
* Cambiar entre las soluciones y aplicaciones de [!DNL Adobe CX Enterprise].
* Busque ayuda sobre [Adobe Experience League](https://experienceleague.adobe.com/docs/?lang=es){target="_blank"}.
* Vea las notificaciones del producto.
* Edite el perfil de Adobe y administre la configuración, como [actualizar su idioma preferido](#language-pref) o [cambiar entre las temáticas clara y oscura](#dark-theme).

## Navegadores admitidos {#browsers}

Adobe Campaign Web está diseñada para funcionar de forma óptima con la última versión de Google Chrome, Safari y Microsoft Edge. Es posible que tenga problemas al utilizar determinadas funciones en versiones anteriores u otros exploradores.

## Preferencias de idioma {#language-pref}

Adobe Campaign Web está disponible actualmente en los siguientes idiomas:

* Inglés (EE. UU.) - EN-US
* Francés - FR
* Alemán - DE
* Italiano - IT
* Español - ES
* Portugués (Brasil) - PTBR
* Japonés - JP
* Coreano - KR
* Chino simplificado - CHS
* Chino tradicional - CHT

Además, el formato específico de la configuración regional (como fechas, horas, calendarios, números) también puede estar disponible en las variantes de los idiomas admitidos por la interfaz de usuario:

* Inglés (Israel)
* Inglés (Reino Unido)
* Español (México)
* Español (América Latina)
* Francés (Canadá)

El idioma predeterminado de la web de Campaign viene determinado por el idioma preferido especificado en el perfil de usuario. No está relacionado con el idioma del servidor de Campaign y de la consola del cliente.

Para cambiar el idioma, haga lo siguiente:

1. Haga clic en el icono del perfil, en la parte superior derecha, y luego seleccione **Preferencias**.
1. Haga clic en el vínculo de idioma mostrado debajo de su dirección de correo electrónico.
1. Seleccione el idioma preferido y haga clic en **Guardar**. Puede seleccionar un segundo idioma en caso de que el componente que esté utilizando no se haya localizado en su primer idioma.


## Temáticas oscuras y claras {#dark-theme}

Adobe Campaign está disponible en temáticas claras y oscuras. De forma predeterminada, la interfaz de usuario está habilitada en la temática clara. Para cambiar a la temática oscura, haga clic en su icono de perfil y utilice la opción **Temática oscura** para habilitarla o deshabilitarla.

La configuración del perfil de usuario y las preferencias de cuenta se detallan en [esta sección](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=es#preferences){target="_blank"}.

Obtenga más información acerca de los componentes de la interfaz central de Experience Cloud en [esta documentación](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=es){target="_blank"}.