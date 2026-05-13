---
audience: end-user
title: Uso de una actividad de flujo de trabajo Entrega continua
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Entrega continua
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
TQID: https://experienceleague.adobe.com/uWGhvUmHdS0ixFI4d-uEPgpxSnZoOwNRMbn8aZfqA98
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 242
ht-degree: 24%

---

# Envío continuo {#continuous-delivery}

La actividad **Envío continuo** le permite agregar nuevos destinatarios a un envío existente. Este tipo de envío evita tener que crear uno nuevo cada vez, lo que resulta más eficaz para las alertas de bajo volumen o las notificaciones enviadas cuando es necesario.

Un envío continuo crea una sola instancia de envío. Todos los registros de envío (broadLog) y los registros de seguimiento hacen referencia a este envío, lo que simplifica la monitorización y la creación de informes.

## Configuración de la actividad Entrega continua {#configure}

1. Agregue una actividad **Envío continuo** a su lienzo de flujo de trabajo.

   ![Captura de pantalla que muestra la actividad de entrega continua](../assets/continuous-delivery.png){zoomable="yes"}

1. Escriba una **[!UICONTROL etiqueta]** personalizada para la actividad (opcional). De forma predeterminada, tiene la etiqueta &quot;Envío continuo&quot;.

1. Junto al campo **[!UICONTROL Plantilla]**, haga clic en el icono de búsqueda para seleccionar una plantilla de envío. Solo se pueden seleccionar plantillas (no envíos estándar). La plantilla define el canal de entrega, el contenido y la configuración.

1. En **[!UICONTROL Opciones de segmentación]**, elija cómo se define la población objetivo:

   * **[!UICONTROL Especificado por los eventos entrantes]**: el destino proviene de la transición entrante (de actividades de flujo ascendente como Generar audiencia o Consulta incremental). Esta es la opción más común.

   * **[!UICONTROL Especificado en la plantilla de envíos]**: el destino se define en la propia plantilla.

   * **[!UICONTROL Archivo especificado en el evento de entrada]**: el destino se proporciona a través de un archivo pasado a través del flujo de trabajo.

La actividad envío continuo genera automáticamente una transición saliente para continuar el flujo de trabajo.

## Temas relacionados {#related}

* [Acerca de las actividades de flujo de trabajo](about-activities.md)
* [Envío automatizado](automated-delivery.md)
* [Actividades de correo electrónico, SMS, push, correo directo](channels.md)
* [Plantillas de envíos](../../msg/delivery-template.md)
