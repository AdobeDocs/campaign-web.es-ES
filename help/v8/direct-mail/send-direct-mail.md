---
audience: end-user
title: Previsualización y envío de una entrega de correo directo
description: Obtenga información sobre cómo obtener una vista previa y enviar un envío de correo directo con Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 1%

---

# Previsualización y envío de una entrega de correo directo {#send-direct-mail}

Una vez configurado el archivo de extracción para la entrega de correo postal, utilice perfiles de prueba para previsualizarlo. Si se incluye contenido personalizado, examine cómo aparece este contenido en las columnas mediante los datos del perfil de prueba. Esto garantiza que el contenido del archivo se represente correctamente y que los elementos personalizados se incorporen correctamente.

Cuando el archivo de extracción esté listo, realice la entrega de correo postal para generar el archivo y compartirlo con su proveedor de correo postal. [Aprenda a realizar su envío de correo postal](#dm-send)

## Previsualización del archivo de extracción {#preview-dm}

Los pasos principales para previsualizar el archivo de extracción son los siguientes. Encontrará más detalles sobre cómo obtener una vista previa de los envíos en [esta sección](../preview-test/preview-content.md).

1. Desde la página de contenido de tu envío, usa **[!UICONTROL Simular contenido]** para obtener una vista previa del contenido personalizado.

   ![Captura de pantalla que muestra la opción de simular contenido en la página de contenido de envío](assets/dm-simulate.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Agregar perfiles de prueba]** para seleccionar uno o varios perfiles y previsualizar sus datos en el contenido del archivo de extracción.

1. En el panel derecho, vea una vista previa del archivo de extracción, donde los elementos personalizados se sustituyen dinámicamente por datos del perfil seleccionado.

   ![Captura de pantalla que muestra la vista previa del archivo de extracción en el panel derecho](assets/dm-preview-right.png){zoomable="yes"}

## Envío de pruebas {#test-dm}

Con **Adobe Campaign**, envíe pruebas antes de enviarlas a la audiencia principal. Este paso valida la entrega e identifica cualquier problema. Los destinatarios de la prueba revisan elementos como la configuración de personalización, lo que garantiza un rendimiento óptimo y detecta errores. Este proceso perfecciona y optimiza el archivo de extracción antes de llegar a la audiencia principal.

Para las entregas de correo postal, la entrega de pruebas genera una muestra del archivo de extracción utilizando datos de los perfiles de prueba seleccionados. Para acceder a él, siga estos pasos:

1. En la pantalla de simular contenido, haga clic en el botón **[!UICONTROL Enviar prueba]** y siga los mismos pasos que para cualquier tipo de entrega para enviar una prueba. [Aprenda a enviar pruebas](../preview-test/test-deliveries.md)

1. Una vez enviada la prueba, acceda a ella desde el botón **[!UICONTROL Ver pruebas]** o desde la lista de envíos. [Obtenga información sobre cómo acceder a las pruebas enviadas](../preview-test/test-deliveries.md#access-test-deliveries)

1. En el panel de envío de prueba, haga clic en el botón **[!UICONTROL Vista previa del archivo]** para acceder a una vista previa del archivo de extracción.

   ![Captura de pantalla que muestra la opción de vista previa del archivo en el panel de envío de prueba](assets/dm-proof.png){zoomable="yes"}

   >[!NOTE]
   >
   >En el archivo de vista previa solo se muestran las 100 primeras líneas.

## Realización de la entrega de correo directo {#send-dm}

Una vez que el correo postal esté listo para enviarse a los clientes, realice la entrega para iniciar la extracción de datos en el archivo de extracción especificado. Para ello, siga estos pasos:

1. Después de diseñar el contenido del archivo de extracción, haga clic en **[!UICONTROL Revisar y enviar]** desde la página de **[!UICONTROL Envío]**.

   ![Captura de pantalla que muestra la opción de revisión y envío en la página de envío](assets/dm-review-send.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Preparar]** y supervise el progreso y las estadísticas proporcionadas.

   Si se produce algún error, consulte el menú **[!UICONTROL Registros]** para obtener información detallada sobre el error.

   ![Captura de pantalla que muestra la opción de preparación y el menú de registros](assets/dm-prepare.png){zoomable="yes"}

1. Envíe los mensajes haciendo clic en **[!UICONTROL Enviar]** para continuar con el proceso de envío final.

1. Confirme la acción de envío haciendo clic en **[!UICONTROL Enviar]**.

   Si la entrega de correo postal está programada, haga clic en el botón **[!UICONTROL Enviar como programado]**. Obtenga más información acerca de la programación de entregas en [esta sección](../msg/gs-messages.md#schedule-the-delivery-sending).

Una vez entregado el envío, el archivo de extracción se genera automáticamente y se exporta a la ubicación especificada en la cuenta externa **[!UICONTROL Routing]** seleccionada en la [configuración avanzada](../advanced-settings/delivery-settings.md) de la plantilla de envío.

Rastree los datos de KPI (indicador de rendimiento clave) de su página de entrega y los datos del menú **[!UICONTROL Registros]**.

Empiece a medir el impacto del mensaje con los informes integrados. [Más información](../reporting/direct-mail.md)