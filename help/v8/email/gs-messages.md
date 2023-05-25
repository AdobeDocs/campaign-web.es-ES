---
audience: end-user
title: Introducción a mensajes y envíos en la web de la versión 8 de Campaign
description: Aprenda a trabajar con envíos y a enviar mensajes con la web de Campaign
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: cd00fcf90283c99e4790789ab2375c3a1da0ce50
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 30%

---

# Introducción a los mensajes en la web de Campaign {#gs-messages}

Con Adobe Campaign, puede enviar campañas en canales múltiples, incluidos correos electrónicos, SMS y notificaciones push, y medir su eficacia mediante varios informes dedicados. Estos mensajes están diseñados y enviados por medio de envíos y pueden personalizarse para cada destinatario. Estos envíos pueden ser independientes o incluirse en el contexto de una campaña de marketing.

Adobe Campaign v8 incluye los siguientes canales de entrega:

* **Canal de correo electrónico**: las entregas de correo electrónico le permiten enviar correos electrónicos personalizados a la población objetivo. Obtenga información sobre cómo crear y enviar un correo electrónico en [esta página](../email/create-email.md).

* **Canal de SMS**: las entregas en canales móviles permiten enviar mensajes SMS personalizados a la población objetivo.  Aprenda a crear y enviar SMS en [esta página](../sms/create-sms.md).

* **Canal de aplicación móvil**: los envíos de aplicaciones móviles permiten enviar notificaciones a sistemas iOS y Android.  Obtenga información sobre cómo crear y enviar notificaciones push en [esta página](../push/gs-push.md).

## Creación de una entrega {#create-delivery}

Puede crear envíos independientes desde el **[!UICONTROL Envíos]** menú de la izquierda o cree envíos en el contexto de una campaña de marketing, desde **[!UICONTROL Campañas]** menú izquierdo.

>[!BEGINTABS]

>[!TAB Creación de un envío independiente]

Para crear un envío independiente, siga estos pasos:

1. Vaya a la **[!UICONTROL Envíos]** en el menú de navegación de la izquierda y haga clic en **[!UICONTROL Creación de envíos]** botón.

   ![](assets/create-a-delivery.png)

1. Elija un canal para la entrega. Obtenga más información acerca de los canales de envío y cómo definir un contenido de envío en estas secciones:

   * [Canal de correo electrónico](../email/create-email.md)
   * [Canal de notificaciones push](../push/gs-push.md)
   * [Canal de SMS](../sms/create-sms.md)

1. Defina la audiencia de envío para el destinatario principal y el grupo de control. Obtenga más información sobre las audiencias en [esta sección](../audience/about-audiences.md).
1. Definición del contenido del mensaje.
1. (opcional) Defina el programa de entregas. Si no se define ninguna programación, los mensajes se envían inmediatamente después de hacer clic en el **[!UICONTROL Enviar]** botón.
1. Haga clic en  **[!UICONTROL Revisar y enviar]** para comprobar su configuración.
1. Utilice el  **[!UICONTROL Simular contenido]** para probar el envío y la configuración de personalización. Obtenga más información sobre la simulación de mensajes en [esta sección](../preview-test/preview-test.md).
1. Haga clic en  **[!UICONTROL Preparar]** para calcular la población objetivo y generar los mensajes. El paso de preparación puede tardar unos minutos. Cuando la preparación haya finalizado, los mensajes estarán listos para enviarse. En caso de error, vaya a la **Registros** para comprobar las alertas y advertencias.
1. Compruebe los resultados y haga clic en  **[!UICONTROL Enviar]** para empezar a enviar mensajes.
1. Una vez enviados los mensajes, vaya a **Informes** para acceder a métricas clave. Obtenga más información acerca de los informes de envío en [esta sección](../reporting/reports.md).

>[!TAB Creación de una entrega en una campaña]

Para crear una entrega en una campaña, siga estos pasos:

1. Cree una campaña o abra una campaña existente. Más información sobre [campañas de marketing](../campaigns/gs-campaigns.md).
1. Cree un flujo de trabajo o abra uno existente.
1. Adición y configuración de un **[!UICONTROL Crear audiencia]** y haga clic en el botón `+`botón.

   ![](assets/add-delivery-in-wf.png)

   El **[!UICONTROL Crear audiencia]** la actividad se detalla en [esta sección](../workflows/targeting-activities.md).

1. Seleccione una actividad de entrega: **[!UICONTROL Correo electrónico]**, **[!UICONTROL SMS]**, **[!UICONTROL Notificación push (Android)]** o **[!UICONTROL Notificación push (iOS)]**. Obtenga más información sobre las actividades del canal de envíos en un flujo de trabajo y cómo definir un contenido de envío en esta sección [sección](../workflows/channel-activities.md).
1. Inicie el flujo de trabajo y compruebe los registros.

También puede añadir envíos en una campaña sin crear un flujo de trabajo. Para conseguirlo, vaya a la **[!UICONTROL Envíos]** de la campaña y haga clic en el icono **[!UICONTROL Creación de envíos]** botón.

![](assets/new-campaign-delivery.png)

Los pasos de configuración son similares a los de los envíos independientes.

Para obtener más información sobre cómo configurar una campaña y administrar las entregas que pertenecen a una campaña, consulte [esta sección](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Adición de personalización{#personalization}

Los mensajes enviados por Adobe Campaign se pueden personalizar de varias formas. [Obtenga más información acerca las funcionalidades de personalización](../personalization/personalize.md).

Utilice Campaign para crear contenido dinámico y enviar mensajes personalizados. Las funcionalidades de personalización se pueden combinar para mejorar sus mensajes y crear una experiencia de usuario personalizada.

Puede personalizar el contenido del mensaje haciendo lo siguiente:

* Inserción dinámica de **campos de personalización**

   Los campos de personalización se utilizan para la personalización de primer nivel de los mensajes. Puede seleccionar cualquier campo disponible en la base de datos desde el editor de personalización. Para un envío, se puede seleccionar cualquier campo relacionado con el destinatario, el mensaje o el envío. Estos atributos de personalización se pueden insertar en la línea de asunto o en el cuerpo de los mensajes. [Más información](../personalization/personalize.md)

* Inserción predefinida de los **bloques de contenido**

   Campaign incluye un conjunto de bloques de personalización que contienen una renderización específica que puede insertar en los envíos. Por ejemplo, puede añadir un logotipo, un mensaje de saludo o un enlace a la página espejo del mensaje. Los bloques de contenido están disponibles en la entrada del editor de personalización. [Más información](../personalization/personalize.md#ootb-content-blocks)

* Crear **contenido condicional**

   Configure el contenido condicional para añadir personalización dinámica basada en el perfil del destinatario, por ejemplo. Los bloques de texto o las imágenes se insertan cuando una condición en particular es verdadera. [Más información](../personalization/conditions.md)

* Añadir **ofertas personalizadas**

   Inserte ofertas personalizadas en el contenido del mensaje, según la ubicación del destinatario, el tiempo actual o la última orden de compra.


## Previsualización y prueba de entregas

Una vez definido el contenido del mensaje, puede obtener una vista previa para controlar la renderización de los mensajes y comprobar la configuración de personalización con perfiles de prueba. [Más información](../preview-test/preview-test.md)


## Registros de seguimiento y entrega{#gs-tracking-logs}

La monitorización de las entregas una vez enviadas es un paso clave para garantizar que las campañas de marketing sean eficientes y lleguen a los clientes. Puede monitorizarlas después de enviar una entrega, así como comprender cómo se administran los errores y las cuarentenas.

## Duplicación de una entrega{#delivery-duplicate}

Puede crear una copia de una entrega existente, ya sea desde la lista de entregas o desde el panel de entregas.

Para duplicar una entrega de la lista de envíos, siga estos pasos:

1. Haga clic en el botón de tres puntos de la derecha, junto al nombre de la entrega que desea duplicar.
1. Seleccionar  **[!UICONTROL Duplicar]**.
1. Confirmar duplicación: el nuevo panel de envío se abre en la pantalla central.


Para duplicar una entrega desde su panel, siga estos pasos:

1. Abra la entrega y haga clic en  **[!UICONTROL ...Más]** botón en la sección superior de la pantalla.
1. Seleccionar  **[!UICONTROL Duplicar]**.
1. Confirmar duplicación: la nueva entrega reemplaza la entrega actual en la pantalla central.

