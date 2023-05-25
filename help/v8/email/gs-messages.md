---
audience: end-user
title: Introducción a mensajes y envíos en la web de la versión 8 de Campaign
description: Aprenda a trabajar con envíos y a enviar mensajes con la web de Campaign
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 14e9ef2a45a1c7a2c8e089c536abd950cdb1b0a3
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 38%

---

# Introducción a los mensajes en la web de Campaign {#gs-messages}

Con Adobe Campaign, puede enviar campañas en canales múltiples, incluidos correos electrónicos, SMS y notificaciones push, y medir su eficacia mediante varios informes dedicados. Estos mensajes están diseñados y enviados por medio de envíos y pueden personalizarse para cada destinatario. Estos envíos pueden ser independientes o incluirse en el contexto de una campaña de marketing.

Adobe Campaign v8 incluye los siguientes canales de entrega:

* **Canal de correo electrónico**: las entregas de correo electrónico le permiten enviar correos electrónicos personalizados a la población objetivo. Obtenga información sobre cómo crear y enviar un correo electrónico en [esta página](../email/create-email.md).

* **Canal de SMS**: las entregas en canales móviles permiten enviar mensajes SMS personalizados a la población objetivo.  Aprenda a crear y enviar SMS en [esta página](../sms/create-sms.md).

* **Canal de aplicación móvil**: los envíos de aplicaciones móviles permiten enviar notificaciones a sistemas iOS y Android.  Obtenga información sobre cómo crear y enviar notificaciones push en [esta página](../push/gs-push.md).

## Creación de una entrega

Puede crear envíos independientes desde el **Envío** menú principal o cree envíos en el contexto de una campaña de marketing.

>[!BEGINTABS]

>[!TAB Creación de un envío independiente]

Para crear un envío independiente, siga estos pasos:

1. Vaya a la **[!UICONTROL Envíos]** en el menú de navegación de la izquierda y haga clic en **[!UICONTROL Creación de envíos]** botón.
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
1. Una vez enviados los mensajes, vaya a la sección Informes para acceder a las métricas clave. Obtenga más información acerca de los informes de envío en [esta sección](../reporting/reports.md).

>[!TAB Creación de una entrega en una campaña]

Para crear una entrega en una campaña, siga estos pasos:

1. Cree una campaña o abra una campaña existente.

Para obtener más información sobre cómo configurar una campaña, consulte

>[!ENDTABS]


## Elija cómo enviar los mensajes{#gs-send-msg}

Una vez creado el mensaje y diseñado y probado su contenido, puede elegir cómo desea enviarlo.

Campaign ofrece un conjunto de funcionalidades para lo siguiente:

* Enviar mensajes manualmente al destinatario principal

* Enviar mensajes asociados a una [campaña de marketing](../campaigns/gs-campaigns.md)

* Enviar mensajes a través de un [flujo de trabajo](../workflows/channel-activities.md)


## Adición de personalización{#personalization}

Los mensajes enviados por Adobe Campaign se pueden personalizar de varias formas


## Registros de seguimiento y entrega{#gs-tracking-logs}

La monitorización de las entregas una vez enviadas es un paso clave para garantizar que las campañas de marketing sean eficientes y lleguen a los clientes. Puede monitorizarlas después de enviar una entrega, así como comprender cómo se administran los errores y las cuarentenas.
