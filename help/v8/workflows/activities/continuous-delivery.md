---
audience: end-user
title: Uso de una actividad de flujo de trabajo Entrega continua
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Entrega continua
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 4%

---

# Envío continuo {#continuous-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Actividad de envío continuo"
>abstract="Ahora puede agregar nuevos destinatarios a una entrega existente. Este tipo de entrega evita tener que crear una nueva cada vez, lo que lo hace más eficiente para alertas de bajo volumen o notificaciones enviadas según sea necesario."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

La actividad **Envío continuo** le permite agregar nuevos destinatarios a un envío existente. Este tipo de entrega evita tener que crear una nueva cada vez, lo que lo hace más eficiente para alertas de bajo volumen o notificaciones enviadas según sea necesario.

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
* [Actividades de correo electrónico, SMS, push, correo directo](channels.md)
* [Plantillas de envíos](../../msg/delivery-template.md)
