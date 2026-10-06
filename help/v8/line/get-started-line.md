---
audience: end-user
title: Introducción a los mensajes de LINE
description: Obtenga información sobre cómo crear y enviar mensajes de LINE con la interfaz de usuario web de Adobe Campaign
feature: Line App
topic: Content Management
role: User
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
subfeature_v2:
  - id: d9d413df-4e9e-4906-bbbc-28c06c2ccf59
    internal-label: LINE App
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
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
