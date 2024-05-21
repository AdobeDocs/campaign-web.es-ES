---
title: Campos personalizados
description: Obtenga información sobre cómo configurar campos personalizados
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 4%

---

# Configuración de los campos personalizados {#custom-fields}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Campos personalizados"
>abstract="Los campos personalizados son atributos adicionales añadidos a los esquemas predeterminados a través de la consola de Adobe Campaign. Ahora están disponibles en la interfaz de usuario web."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"



Los campos personalizados son atributos adicionales añadidos a los esquemas predeterminados a través de la consola de Adobe Campaign. Obtenga más información en la [Documentación de Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"}

Estos campos personalizados se muestran en varias pantallas, por ejemplo, los detalles de un perfil o un perfil de prueba.

En la interfaz de usuario web, no se pueden crear campos personalizados, pero se puede modificar la forma en que se muestran. Las modificaciones se aplican a todos los usuarios de Campaign.

>[!NOTE]
>
>Debe tener derechos de administrador para modificar los campos personalizados.

Los campos personalizados están disponibles en los siguientes esquemas:

* Destinatarios (nms)
* Campañas (nms)
* Envíos (nms)
* Direcciones semilla (nms)

Para configurar los campos personalizados, siga estos pasos:

1. En **Administration**, haga clic en **Esquemas**.

   ![](assets/custom-fields.png){zoomable="yes"}

1. Busque el esquema deseado, por ejemplo, la variable **Destinatarios (nms)** esquema.

   ![](assets/custom-fields2.png){zoomable="yes"}

1. Haga clic en **Más acciones** y seleccione **Editar detalles personalizados**.

   ![](assets/custom-fields3.png){zoomable="yes"}

   El **Editar detalles personalizados** La pantalla muestra todos los campos personalizados y su tipo.

   ![](assets/custom-fields4.png){zoomable="yes"}

   Esta pantalla le permite realizar las siguientes acciones:

   * cambie el orden de los diferentes campos mediante las flechas arriba y abajo.
   * haga que el campo sea obligatorio: marque la **Obligatorio** cuadro.
   * hacer visible u ocultar el campo: haga clic en el icono **Visible** botón.
   * añada una condición de visibilidad: haga clic en **Visible si** y escriba la expresión xtk utilizando las funciones xtk disponibles.

1. Vaya a la pantalla que muestra el campo personalizado. En nuestro ejemplo, es la pantalla de detalles del perfil.

   ![](assets/custom-fields5.png){zoomable="yes"}
