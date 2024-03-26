---
audience: end-user
title: Previsualización y envío de una entrega de correo directo
description: Obtenga información sobre cómo obtener una vista previa y enviar un envío de correo directo con Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 3%

---

# Previsualización y envío de una entrega de correo directo {#send-direct-mail}

Una vez configurado el archivo de extracción para la entrega de correo postal, puede utilizar perfiles de prueba para previsualizarlo. Si ha incluido contenido personalizado, puede examinar cómo se muestra este contenido en las columnas utilizando datos de perfil de prueba. Esto le permite asegurarse de que el contenido del archivo se está representando correctamente y de que los elementos personalizados se están incorporando correctamente.

Cuando el archivo de extracción esté listo, puede realizar la entrega de correo postal para generar el archivo y compartirlo con su proveedor de correo postal. [Obtenga información sobre cómo realizar envíos de correo directo](#dm-send)

## Previsualización del archivo de extracción {#preview-dm}

Los pasos principales para previsualizar el archivo de extracción son los siguientes. Encontrará más detalles sobre cómo previsualizar las entregas en [esta sección](../preview-test/preview-content.md).

1. En la página de contenido de la entrega, utilice **[!UICONTROL Simular contenido]** para previsualizar el contenido personalizado.

   ![](assets/dm-simulate.png){zoomable=&quot;yes&quot;}

1. Clic **[!UICONTROL Añadir perfil(es) de prueba]** para seleccionar uno o varios perfiles para previsualizar sus datos en el contenido del archivo de extracción.

1. En el panel derecho, encontrará una vista previa del archivo de extracción, donde los elementos personalizados se sustituyen dinámicamente por datos del perfil seleccionado.

   ![](assets/dm-preview-right.png){zoomable=&quot;yes&quot;}

## Envío de pruebas {#test-dm}

Uso de **Adobe Campaign**, tiene la capacidad de enviar pruebas antes de enviarlas a su audiencia principal. Este paso es importante para validar el envío e identificar cualquier problema. Los destinatarios de la prueba pueden revisar elementos como la configuración de personalización, lo que garantiza un rendimiento óptimo y detecta errores. Este proceso le ayuda a refinar y optimizar su archivo de extracción antes de llegar a su audiencia principal.

Para las entregas de correo postal, la entrega de pruebas genera una muestra del archivo de extracción utilizando datos de los perfiles de prueba seleccionados. Para acceder a él, siga estos pasos:

1. En la pantalla de simular contenido, haga clic en **[!UICONTROL Enviar prueba]** y siga los mismos pasos que para cualquier tipo de entrega para enviar una prueba. [Obtenga información sobre cómo enviar pruebas](../preview-test/test-deliveries.md)

1. Una vez enviada la prueba, puede acceder a ella desde el **[!UICONTROL Ver pruebas]** o en la lista de envíos. [Obtenga información sobre cómo acceder a las pruebas enviadas](../preview-test/test-deliveries.md#access-test-deliveries)

1. En el panel de envío de prueba, haga clic en **[!UICONTROL Previsualizar archivo]** para acceder a una previsualización del archivo de extracción.

   ![](assets/dm-proof.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >En el archivo de vista previa solo se muestran las 100 primeras líneas.

## Realización de la entrega de correo directo {#send-dm}

Una vez que el correo postal esté listo para enviarse a sus clientes, puede realizar la entrega para iniciar la extracción de datos en el archivo de extracción especificado. Para ello, siga estos pasos:

1. Después de diseñar el contenido del archivo de extracción, haga clic en **[!UICONTROL Revisar y enviar]** de su **[!UICONTROL Envío]** página.

   ![](assets/dm-review-send.png){zoomable=&quot;yes&quot;}

1. Clic **[!UICONTROL Preparar]** y supervisar el progreso y las estadísticas proporcionadas.

   Si se produce algún error, consulte la **[!UICONTROL Registros]** para obtener información detallada sobre el error.

   ![](assets/dm-prepare.png){zoomable=&quot;yes&quot;}

1. Envíe los mensajes haciendo clic en **[!UICONTROL Enviar]** para continuar con el proceso de envío final.

1. Confirme la acción de envío haciendo clic en **[!UICONTROL Enviar]**.

   Si la entrega de correo postal se ha programado, haga clic en el **[!UICONTROL Enviar como está programado]** botón. Obtenga más información sobre la programación de entregas en [esta sección](../msg/gs-messages.md#schedule-the-delivery-sending).

Una vez realizado el envío, el archivo de extracción se genera automáticamente y se exporta a la ubicación especificada en la **[!UICONTROL Enrutamiento]** cuenta externa seleccionada en la plantilla de envíos [configuración avanzada](../advanced-settings/delivery-settings.md).

Puede realizar un seguimiento de los datos de KPI (Indicador de rendimiento clave) desde la página de envío y desde los datos de **[!UICONTROL Registros]** menú.

También puede empezar a medir el impacto del mensaje con informes integrados. [Más información](../reporting/direct-mail.md)
