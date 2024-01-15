---
title: Personalización del contenido en Campaign
description: Obtenga información sobre cómo personalizar su contenido en la IU de la web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
exl-id: 45cdd310-7c0c-4b57-bb7f-0576d8eca19d
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 65%

---

# Añadir bloques de contenido integrados {#ootb-content-blocks}

Adobe Campaign ofrece una lista de bloques de contenido preconfigurados. Estos bloques de contenido son dinámicos, personalizados y tienen un procesamiento específico que puede insertar en las entregas. Por ejemplo, puede añadir un logotipo, un mensaje de saludo o un enlace a una página espejo.

Para añadir un bloque de contenido a una entrega, siga estos pasos:

1. Abra una entrega y edite su contenido.

1. Busque el campo donde desea agregar un bloque de contenido y haga clic en **[!UICONTROL Abrir diálogo de personalización]** para abrir el editor de expresiones.

   ![](assets/content-block-access.png){width="800" align="center"}

1. En el editor de expresiones, busque **[!UICONTROL Bloques de contenido]** menú izquierdo.

1. Para añadir un bloque de contenido, coloque el cursor en la ubicación deseada dentro del contenido y haga clic en el botón &quot;+&quot; para insertarlo.

   ![](assets/content-blocks.png){width="800" align="center"}

Descripción de los bloques de contenido integrados:

* **[!UICONTROL Banner de exclusión predeterminado]**
* **[!UICONTROL Habilitado por Adobe Campaign]**: inserta el logotipo “Habilitado por Adobe Campaign”.
* **[!UICONTROL Función de formateo para nombres propios]**: genera la función JavaScript **[!UICONTROL toSmartCase]**, que cambia la primera letra de cada palabra a mayúscula.
* **[!UICONTROL Saludos]**: inserta los saludos con el nombre completo del destinatario, seguidos de una coma. Ejemplo: “Hola, John Doe”.
* **[!UICONTROL Insertar logotipo]**: inserta un logotipo definido en la configuración de la instancia.
* **[!UICONTROL Enlace a página espejo]**: inserta un enlace a la [página espejo](../email/mirror-page.md). El formato predeterminado es: “Si no puede ver este mensaje correctamente, haga clic aquí”.
* **[!UICONTROL URL de la página espejo]**: inserta la dirección URL de la página espejo, permite que los diseñadores de envío comprueben el vínculo.
* **[!UICONTROL Estilo de notificación]**
* **[!UICONTROL URL de aceptación de la oferta en modo unitario]**: inserta una URL que permite establecer una oferta como **[!UICONTROL Aceptada]**. (Este bloque está disponible si el módulo Interacción está habilitado)
* **[!UICONTROL Confirmación del registro]**: inserta un vínculo que permite confirmar la suscripción.
* **[!UICONTROL Vínculo de registro]**: inserta un vínculo de suscripción. Este vínculo se define en la configuración de la instancia. El contenido predeterminado es: “Para registrarse, haga clic aquí”.
* **[!UICONTROL Vínculo de registro (con referencia)]**: inserta un vínculo de suscripción que permite identificar el visitante y el envío. Este vínculo se define en la configuración de la instancia.
* **[!UICONTROL URL de la página de registro]**: inserta una URL de suscripción.
* Vínculos para compartir en redes sociales
* **[!UICONTROL Estilo de los correos electrónicos de contenido]** y **[!UICONTROL Estilo de las notificaciones]**: generan un código que da formato a un correo electrónico con estilos HTML predefinidos.
* **[!UICONTROL Vínculo de baja]**: inserta un vínculo que permite cancelar la suscripción a todos los envíos (lista de bloqueados). El contenido asociado predeterminado es el siguiente: “Usted recibe este mensaje porque ha estado en contacto con ***nombre de la organización*** o un afiliado. Para dejar de recibir mensajes de ***nombre de la organización*** haga clic aquí”.

>[!NOTE]
>
>Puede definir nuevos bloques desde la consola de Adobe Campaign v8 que le permitan optimizar la personalización de las entregas. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}.
