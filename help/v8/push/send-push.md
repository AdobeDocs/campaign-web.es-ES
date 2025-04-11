---
audience: end-user
title: Envío de una entrega de notificaciones push
description: Obtenga información sobre cómo enviar una entrega de notificaciones push con Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---

# Previsualizar y enviar un envío push {#send-push-delivery}

## Previsualización del envío de notificaciones push {#preview-push}

Una vez definido el contenido del mensaje, utilice los suscriptores de prueba para previsualizar y probar el mensaje. Si se incluye contenido personalizado, examine cómo se muestra este contenido en el mensaje mediante los datos de perfil de prueba. Esto garantiza que el mensaje se represente correctamente y que los elementos personalizados se incorporen correctamente.

Los pasos principales para previsualizar la notificación push son los siguientes. Encontrará más detalles sobre cómo obtener una vista previa de los envíos en [esta sección](../preview-test/preview-content.md).

1. Desde la página de contenido de tu envío, usa **[!UICONTROL Simular contenido]** para obtener una vista previa del contenido personalizado.

   ![Vista previa del contenido personalizado en la página de contenido de envío](assets/push_send_1.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Agregar suscriptores]** para seleccionar uno o varios perfiles y obtener una vista previa de sus datos en el contenido de las notificaciones push.

   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. En el panel derecho, busque una vista previa de la notificación push, donde los elementos personalizados se sustituyen dinámicamente por datos del perfil seleccionado.

   ![El panel de vista previa muestra elementos personalizados reemplazados con datos de perfil](assets/push_send_7.png){zoomable="yes"}

Revise y envíe la notificación push a su audiencia.

## Prueba de la entrega de notificaciones push {#test-push}

Con **Adobe Campaign**, envíe pruebas antes de enviarlas a la audiencia principal. Este paso valida la entrega e identifica cualquier problema.

Los perfiles de prueba actúan como destinatarios de prueba. Revisan y validan componentes y configuraciones como vínculos, imágenes y personalización, lo que garantiza un rendimiento óptimo y detecta errores. Este proceso perfecciona y optimiza las notificaciones push antes de llegar a la audiencia principal. [Aprenda a enviar pruebas](../preview-test/test-deliveries.md#subscribers).

![Probando envío de notificaciones push con destinatarios de prueba](assets/push_send_6.png){zoomable="yes"}

## Realización del envío de notificaciones push {#send-push}

1. Después de personalizar el contenido de las notificaciones push, haga clic en **[!UICONTROL Revisar y enviar]** desde la página de **[!UICONTROL Envío]**.

   ![Botón Revisar y enviar en la página de envío](assets/push_send_2.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Preparar]** y supervise el progreso y las estadísticas proporcionadas.

   Si se producen errores, consulte el menú Registros para obtener información detallada sobre el error.

   ![Supervisión del progreso y las estadísticas de preparación](assets/push_send_3.png){zoomable="yes"}

1. Envíe los mensajes haciendo clic en **[!UICONTROL Enviar]** para continuar con el proceso de envío final.

1. Confirme la acción de envío haciendo clic en **[!UICONTROL Enviar]**.

   Si la entrega de inserción está programada, haga clic en el botón **[!UICONTROL Enviar como programado]**. Obtenga más información acerca de la programación de entregas en [esta sección](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![Botón Enviar como programado para la entrega de inserción programada](assets/push_send_4.png){zoomable="yes"}

Una vez entregado el envío, realice un seguimiento de los datos de Indicador de rendimiento clave (KPI) de su página de envío y de los datos del menú **[!UICONTROL Registros]**.

Empiece a medir el impacto del mensaje con los informes integrados. [Más información](../reporting/push-report.md).