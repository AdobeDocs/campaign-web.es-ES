---
audience: end-user
title: Introducción a los mensajes de LINE
description: Obtenga información sobre cómo crear y enviar mensajes de LINE con la interfaz de usuario web de Adobe Campaign
feature: Line App
topic: Content Management
role: User
level: Beginner
source-git-commit: 1c4cdd5164d0cf572e9b88881bbe240b06308866
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 12%
---
# Introducción a los mensajes de LINE {#get-started-line}

LINE es una aplicación gratuita de mensajería instantánea, llamadas de voz y vídeo disponible en todos los sistemas operativos móviles y en PC. Puede utilizar Adobe Campaign para enviar mensajes de LINE. Utilice LINE en envíos independientes o en flujos de trabajo, junto con sus otros canales.

![Ejemplo de mensaje de LINE recibido en un dispositivo móvil](assets/line-message.png)

* **[!UICONTROL Envíos]**: cree un envío LINE independiente desde el menú de **[!UICONTROL Envíos]** en el carril izquierdo, similar a SMS o push. [Más información](send-line.md).

* **[!UICONTROL Flujos de trabajo]**: en el lienzo del flujo de trabajo, agregue una actividad de canal **[!UICONTROL LINE]**, elija una plantilla de envío y defina el contenido y la configuración en el panel de envío. Obtenga más información acerca de las actividades de canal en [esta sección](../workflows/activities/channels.md).

  >[!NOTE]
  >
  >En la actividad **[!UICONTROL Generar audiencia]** que alimenta su actividad de canal **[!UICONTROL LINE]**, cambie la dimensión de segmentación a **[!UICONTROL Suscripciones de visitantes]**. Asegúrese de habilitar **[!UICONTROL Mostrar todos los esquemas]** en el panel lateral. El selector de plantillas de envío solo está disponible una vez que se ha establecido esta dimensión de segmentación.
