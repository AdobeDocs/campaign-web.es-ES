---
audience: end-user
title: Envío de un envío SMS
description: Aprenda a enviar SMS con Adobe Campaign Web
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 11%

---

# Previsualización y envío de un envío de SMS {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nueva métrica de cuarentenas"
>abstract="Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar."

## Previsualización del envío de SMS {#preview-sms}

Una vez definido el contenido del mensaje, utilice perfiles de prueba para previsualizarlo y probarlo. Si se incluye contenido personalizado, examine cómo aparece este contenido en el mensaje utilizando datos de perfil de prueba. Esto garantiza que el mensaje se muestre según lo previsto y que la información personalizada se presente correctamente.

Los pasos principales para previsualizar su envío de SMS son los siguientes. Encontrará más detalles sobre cómo obtener una vista previa de los envíos en [esta sección](../preview-test/preview-content.md).

1. Desde la página de contenido de tu envío, usa **[!UICONTROL Simular contenido]** para obtener una vista previa del contenido personalizado.

   ![Vista previa del contenido personalizado de SMS](assets/sms_send_1.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Añadir perfil(es) de prueba]** para seleccionar uno o varios perfiles de prueba o perfiles.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. En el panel derecho, vista un previsualización de la envío SMS, donde los elementos personalizados se reemplazan dinámicamente con datos del perfil seleccionado.

   ![Vista previa panel que muestra envío SMS personalizados](assets/sms_send_3.png){zoomable="yes"}

Revise y envíe su mensaje SMS a su audiencia.

## Prueba del envío de SMS {#test-sms}

Con **Adobe Campaign**, pruebe un mensaje antes de enviarlo a la audiencia principal. Este paso valida la campaña de correo electrónico e identifica posibles problemas.

El envío de pruebas es crucial para garantizar la calidad y la eficacia de su envío. Los destinatarios de la prueba revisan varios elementos, como vínculos, vínculos de exclusión e imágenes, e identifican cualquier error en la renderización, el contenido, la configuración de personalización y la configuración de SMS. Este proceso evalúa y optimiza a fondo su SMS antes de llegar a su audiencia principal.

![Icono de libro para enviar pruebas](../assets/do-not-localize/book.png) Aprenda a enviar pruebas en [esta sección](../preview-test/test-deliveries.md).

![Probando envío de SMS](assets/sms_send_6.png){zoomable="yes"}

## Realización de la entrega de SMS {#send-sms}

1. Después de personalizar su contenido de SMS, haga clic en **[!UICONTROL Revisar y enviar]** desde su **[!UICONTROL Página de entrega]** .

   ![Revisar y enviar SMS envío](assets/sms_send_4.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Preparar]** y monitor el progreso y las estadísticas proporcionadas.

   Si se producen errores, consulte el menú Registros para obtener información detallada sobre el fallo.

1. Envíe los mensajes haciendo clic en **[!UICONTROL Enviar]** para continuar con el proceso de envío final.

   ![Envío de SMS](assets/sms_send_5.png){zoomable="yes"}

   Si la entrega de SMS está programada, haga clic en el botón **[!UICONTROL Enviar como programado]**. Obtenga más información acerca de la programación de entregas en [esta sección](../msg/gs-messages.md#schedule-the-delivery-sending).

1. Confirme la acción de envío haciendo clic en el botón **[!UICONTROL Enviar]**.

Una vez entregado el envío, realice un seguimiento de los datos de KPI (indicador de rendimiento clave) de su página de envío y de los datos del menú **[!UICONTROL Registros]**.

Empiece a medir el impacto del mensaje con los informes integrados. [Más información](../reporting/sms-report.md)