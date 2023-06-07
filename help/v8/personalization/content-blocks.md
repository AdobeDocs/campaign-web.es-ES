---
title: Personalización del contenido en Campaign
description: Obtenga información sobre cómo personalizar su contenido en la IU de la web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
source-git-commit: 573f0bbf396f795029c5e34b436521cb1c7b80a5
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Descripción de los bloques de contenido integrados {#ootb-content-blocks}

Descripción de los bloques de contenido integrados:

* **[!UICONTROL Habilitado por Adobe Campaign]**: inserta el logotipo “Habilitado por Adobe Campaign”.
* **[!UICONTROL Función de formateo para nombres propios]**: genera la función JavaScript **[!UICONTROL toSmartCase]**, que cambia la primera letra de cada palabra a mayúscula.
* **[!UICONTROL Saludos]**: inserta los saludos con el nombre completo del destinatario, seguidos de una coma. Ejemplo: “Hola, John Doe”.
* **[!UICONTROL Insertar logotipo]**: inserta un logotipo que se define en la configuración de la instancia.
* **[!UICONTROL Enlace a página espejo]**: inserta un enlace a la [página espejo](../content/mirror-page.md). El formato predeterminado es: “Si no puede ver este mensaje correctamente, haga clic aquí”.
* **[!UICONTROL URL de la página espejo]**: inserta la dirección URL de la página espejo, permite que los diseñadores de envío comprueben el vínculo.
* **[!UICONTROL URL de aceptación de la oferta en modo unitario]**: inserta una URL que permite establecer una oferta como **[!UICONTROL Aceptada]**. (Este bloque está disponible si el módulo Interacción está habilitado)
* **[!UICONTROL Confirmación del registro]**: inserta un vínculo que permite confirmar la suscripción.
* **[!UICONTROL Vínculo de registro]**: inserta un vínculo de suscripción. Este vínculo se define en la configuración de la instancia. El contenido predeterminado es: “Para registrarse, haga clic aquí”.
* **[!UICONTROL Vínculo de registro (con referencia)]**: inserta un vínculo de suscripción que permite identificar el visitante y el envío. Este vínculo se define en la configuración de la instancia.
* **[!UICONTROL URL de la página de registro]**: inserta una URL de suscripción.
* **[!UICONTROL Estilo de los correos electrónicos de contenido]** y **[!UICONTROL Estilo de las notificaciones]**: generan un código que da formato a un correo electrónico con estilos HTML predefinidos.
* **[!UICONTROL Vínculo de baja]**: inserta un vínculo que permite cancelar la suscripción a todos los envíos (lista de bloqueados). El contenido asociado predeterminado es el siguiente: “Usted recibe este mensaje porque ha estado en contacto con ***nombre de la organización*** o un afiliado. Para dejar de recibir mensajes de ***nombre de la organización*** haga clic aquí”.
