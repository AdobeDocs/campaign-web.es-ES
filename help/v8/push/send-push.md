---
audience: end-user
title: Envío de una entrega de notificaciones push
description: Obtenga información sobre cómo enviar una entrega de notificaciones push con Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 2%

---

# Previsualizar y enviar un envío push {#send-push-delivery}

## Previsualización del envío de notificaciones push {#preview-push}

Una vez definido el contenido del mensaje, puede utilizar los suscriptores de prueba para previsualizar y probar el mensaje. Si ha incluido contenido personalizado, puede examinar cómo se muestra este en el mensaje utilizando datos de perfil de prueba. Esto le permite asegurarse de que el mensaje se está representando correctamente y de que los elementos personalizados se están incorporando correctamente.

Los pasos principales para previsualizar la notificación push son los siguientes. Encontrará más detalles sobre cómo obtener una vista previa de los envíos en [esta sección](../preview-test/preview-content.md).

1. Desde la página de contenido de tu envío, usa **[!UICONTROL Simular contenido]** para obtener una vista previa del contenido personalizado.

   ![](assets/push_send_1.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Agregar suscriptores]** para seleccionar uno o varios perfiles y obtener una vista previa de sus datos en el contenido de las notificaciones push.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. En el panel derecho, encontrará una vista previa de la notificación push, donde los elementos personalizados se sustituyen dinámicamente por datos del perfil seleccionado.

   ![](assets/push_send_7.png){zoomable="yes"}

Ahora puede revisar y enviar la notificación push a su audiencia.

## Prueba de la entrega de notificaciones push {#test-push}

Con **Adobe Campaign**, tiene la capacidad de enviar pruebas antes de enviarlas a su audiencia principal. Este paso es importante para validar el envío e identificar cualquier problema.

Los perfiles de prueba son los destinatarios de prueba. Pueden revisar y validar componentes y configuraciones como vínculos, imágenes y personalización, lo que garantiza un rendimiento óptimo y detecta errores. Este proceso le ayuda a refinar y optimizar sus notificaciones push antes de llegar a su audiencia principal. [Aprenda a enviar pruebas](../preview-test/test-deliveries.md#subscribers)

![](assets/push_send_6.png){zoomable="yes"}

## Realización del envío de notificaciones push {#send-push}

1. Después de personalizar el contenido de las notificaciones push, haga clic en **[!UICONTROL Revisar y enviar]** desde la página de **[!UICONTROL Envío]**.

   ![](assets/push_send_2.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Preparar]** y supervise el progreso y las estadísticas proporcionadas.

   Si se produce algún error, consulte el menú Registros para obtener información detallada sobre el error.

   ![](assets/push_send_3.png){zoomable="yes"}

1. Envíe los mensajes haciendo clic en **[!UICONTROL Enviar]** para continuar con el proceso de envío final.

1. Confirme la acción de envío haciendo clic en **[!UICONTROL Enviar]**.

   Si la entrega de inserción se ha programado, haga clic en el botón **[!UICONTROL Enviar como programado]**. Obtenga más información acerca de la programación de entregas en [esta sección](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![](assets/push_send_4.png){zoomable="yes"}

Una vez entregado el envío, puede rastrear los datos de KPI (Indicador de rendimiento clave) de su página de envío y los datos del menú **[!UICONTROL Registros]**.

Ahora puede empezar a medir el impacto del mensaje con informes integrados. [Más información](../reporting/push-report.md)
