---
audience: end-user
title: Envío de un mensaje de LINE
description: Obtenga información sobre cómo crear y enviar una entrega LINE en la interfaz de usuario web de Adobe Campaign
feature: Line App
topic: Content Management
role: User
level: Beginner
source-git-commit: 1c4cdd5164d0cf572e9b88881bbe240b06308866
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%
---

# Envío de un mensaje de LINE {#send-line}

Puede crear y enviar mensajes de LINE a sus suscriptores mediante contenido de texto, imagen o vídeo. Los envíos de LINE se pueden crear como envíos independientes o añadir a un flujo de trabajo.

Esta página muestra cómo crear una entrega de LINE independiente, pero se aplican los mismos pasos al configurar una actividad de canal de LINE en un flujo de trabajo.

>[!IMPORTANT]
>
>Actualmente, la vista previa del mensaje no es compatible con los envíos de LINE. Revise cuidadosamente el contenido en el editor antes de enviarlo, ya que no puede obtener una vista previa del mensaje procesado.

## Creación de una entrega de LINE {#create-line-delivery}

1. Vaya al menú **[!UICONTROL Envíos]** y haga clic en **[!UICONTROL Crear envío]**.

1. Elija **[!UICONTROL LINE]** y seleccione una plantilla de entrega, como la plantilla predeterminada **[!UICONTROL LINE V2 delivery]**. [Más información sobre las plantillas](../msg/delivery-template.md).

   ![Plantilla de creación de mensaje Line](assets/line-message2.png)

1. Haga clic en **[!UICONTROL Crear entrega]** para confirmar y mostrar la pantalla de configuración de la entrega.

1. Escriba una **[!UICONTROL Etiqueta]** para la entrega y defina opciones adicionales o personalizadas, si es necesario. [Más información](../push/create-push.md#configure-push-settings).

   ![Propiedades del mensaje de línea](assets/line-message3.png)

## Selección del público {#audience}

1. Haga clic en **[!UICONTROL Seleccionar audiencia]** para segmentar una audiencia existente o generar una. El objetivo de los envíos de LINE se basa en **[!UICONTROL suscripciones de visitantes]**. [Más información sobre las audiencias](../audience/about-recipients.md).

1. Active la opción **[!UICONTROL Habilitar grupo de control]** para establecer un grupo de control y medir el impacto de su envío. Los mensajes no se envían a ese grupo de control, por lo que puede comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo recibieron. [Más información](../audience/control-group.md)

## Definición del contenido {#content}

Haga clic en **[!UICONTROL Editar contenido]**.

![Botón de contenido de edición de mensaje en línea](assets/line-message4.png)

Se muestra el editor de contenido LINE.

![Pantalla de contenido de edición de mensajes Line](assets/line-message5.png)

Una entrega LINE puede contener hasta cinco mensajes. Haga clic en **[!UICONTROL Agregar mensaje]** para agregar otro mensaje a la entrega o en **[!UICONTROL Quitar mensaje]** para eliminar uno.

Cuando esté disponible, puede utilizar el editor de personalización para insertar contenido dinámico. [Más información](../personalization/personalize.md).

Cada mensaje utiliza uno de los siguientes tipos.

>[!NOTE]
>
>Solo se admiten direcciones URL de imagen y vídeo. La carga de un archivo local no está disponible, lo que coincide con el comportamiento de la consola del cliente.

### Mensaje de texto {#text-message}

Un mensaje de texto es un mensaje simple enviado en forma de texto. Simplemente escriba el mensaje en el campo relacionado y utilice campos de personalización, si es necesario.

![Texto de edición de mensaje en línea](assets/line-message6.png)

### Mensaje de imagen {#image-message}

Un mensaje de imagen permite enviar una imagen, dividida de forma opcional en regiones en las que se puede hacer clic, cada una de las cuales se vincula a una dirección URL diferente.

![Imagen de contenido de edición de mensaje en línea](assets/line-message7.png)

* **[!UICONTROL Imagen personalizada]**: defina la imagen dinámicamente por destinatario.
* **[!UICONTROL URL de imagen]**: proporcione la URL de su imagen. El tamaño recomendado es de 1040 x 1040 px. Habilite **[!UICONTROL Definir imágenes por tamaño de pantalla del dispositivo]** para proporcionar distintas resoluciones de imagen optimizadas para diferentes tamaños de pantalla.
* **[!UICONTROL Texto alternativo]**: texto alternativo obligatorio que se muestra si la imagen no se puede cargar.
* **[!UICONTROL Vínculos]**: elija un diseño para dividir la imagen en una o varias regiones en las que se puede hacer clic y, a continuación, asigne una dirección URL a cada región.

### Mensaje de vídeo {#video-message}

Un mensaje de vídeo permite enviar un vídeo a los destinatarios.

![Vídeo de contenido de edición de mensajes Line](assets/line-message8.png)

* **[!UICONTROL URL del vídeo]**: la URL del vídeo. Solo se admite el formato MP4.
* **[!UICONTROL URL de imagen de vista previa]**: la URL de una imagen mostrada antes de que se reproduzca el vídeo.

## Programar y enviar {#schedule-send}

1. Después de definir el contenido, haga clic en **Guardar** y luego haga clic en el icono Atrás para volver a la pantalla de configuración de la entrega.

1. Habilitar **[!UICONTROL Habilitar la programación]** para enviar en una fecha y hora específicas. [Más información](../msg/gs-deliveries.md#gs-schedule).

   ![Programación de mensajes de línea](assets/line-message9.png)

1. Una vez que el contenido esté listo, haz clic en **[!UICONTROL Revisar y enviar]**. Esto abre el panel de envío.

   ![Panel de mensajes de línea](assets/line-message10.png)

1. Haga clic en **[!UICONTROL Preparar]** y confirme. Si hay errores, corríjalos y haga clic de nuevo en **[!UICONTROL Preparar]**.

1. Haga clic en **[!UICONTROL Enviar]**. A continuación, puede rastrear los resultados de los puntos de entrada de la entrega **[!UICONTROL Informes]** y **[!UICONTROL Registros]**.
