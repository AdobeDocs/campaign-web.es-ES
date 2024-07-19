---
audience: end-user
title: Envío de un envío SMS
description: Obtenga información sobre cómo enviar SMS con Adobe Campaign Web
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 14%

---

# Previsualización y envío de un envío de SMS {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nueva métrica de cuarentenas"
>abstract="Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar."

## Previsualización del envío de SMS{#preview-sms}

Una vez definido el contenido del mensaje, puede utilizar perfiles de prueba para previsualizarlo y probarlo. Si ha incluido contenido personalizado, puede examinar cómo se muestra este en el mensaje utilizando datos de perfil de prueba. Esto le permite asegurarse de que el mensaje aparece según lo previsto y de que toda la información personalizada se presenta correctamente.

Los pasos principales para previsualizar su envío de SMS son los siguientes. Encontrará más detalles sobre cómo obtener una vista previa de los envíos en [esta sección](../preview-test/preview-content.md).

1. Desde la página de contenido de tu envío, usa **[!UICONTROL Simular contenido]** para obtener una vista previa del contenido personalizado.

   ![](assets/sms_send_1.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Añadir perfil(es) de prueba]** para seleccionar uno o varios perfiles de prueba o perfiles.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png){zoomable="yes"}
    -->

1. En el panel derecho, encontrará una vista previa del envío SMS, donde los elementos personalizados se sustituyen dinámicamente por datos del perfil seleccionado.

   ![](assets/sms_send_3.png){zoomable="yes"}

Ahora puede revisar y enviar su mensaje SMS a su público.

## Prueba del envío de SMS {#test-sms}

Con **Adobe Campaign**, tiene la capacidad de probar un mensaje antes de enviarlo a la audiencia principal, lo cual es un paso esencial para validar su campaña de correo electrónico e identificar posibles problemas.

El envío de pruebas es un paso importante para garantizar la calidad y la eficacia de su envío. Los destinatarios de la prueba pueden revisar varios elementos, como vínculos, vínculos de exclusión e imágenes, así como identificar cualquier error en la renderización, el contenido, la configuración de personalización y la configuración de SMS. Este proceso le ayuda a evaluar y optimizar exhaustivamente su SMS antes de llegar a su audiencia principal.

![](../assets/do-not-localize/book.png) Aprenda a enviar pruebas en [esta sección](../preview-test/test-deliveries.md).

![](assets/sms_send_6.png){zoomable="yes"}

## Realización de la entrega de SMS {#send-sms}

1. Después de personalizar el contenido de tu SMS, haz clic en **[!UICONTROL Revisar y enviar]** desde tu página de **[!UICONTROL Envío]**.

   ![](assets/sms_send_4.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Preparar]** y supervise el progreso y las estadísticas proporcionadas.

   Si se produce algún error, consulte el menú Registros para obtener información detallada sobre el error.

1. Envíe los mensajes haciendo clic en **[!UICONTROL Enviar]** para continuar con el proceso de envío final.

   ![](assets/sms_send_5.png){zoomable="yes"}

   Si la entrega de SMS se ha programado, haga clic en el botón **[!UICONTROL Enviar como programado]**. Obtenga más información acerca de la programación de entregas en [esta sección](../msg/gs-messages.md#schedule-the-delivery-sending).


1. Confirme la acción de envío haciendo clic en el botón **[!UICONTROL Enviar]**.

Una vez entregado el envío, puede rastrear los datos de KPI (Indicador de rendimiento clave) de su página de envío y los datos del menú **[!UICONTROL Registros]**.

Ahora puede empezar a medir el impacto del mensaje con informes integrados. [Más información](../reporting/sms-report.md)
