---
audience: end-user
title: Introducción a los canales externos personalizados
description: Obtenga información sobre cómo crear y enviar envíos de canales externos personalizados con Adobe Campaign Web
source-git-commit: 7438ce1805cde00cf5b76f05d72bd19d2ef2343a
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# Introducción a los canales externos personalizados {#gs-custom-channel}

Puede, directamente desde la interfaz de usuario web de Adobe Campaign, organizar y ejecutar envíos basados en canales externos personalizados integrados con terceros. La creación del canal externo personalizado se realiza en la consola del cliente.

Puede configurar envíos externos de canal personalizado en flujos de trabajo o como envíos independientes, definir la audiencia y generar archivos de exportación personalizables con todos los datos de contacto y personalización necesarios.

>[!NOTE]
>
>Los informes no están disponibles en la interfaz de usuario web para las entregas externas del canal personalizado. Debe navegar a la consola del cliente para acceder a los informes.

Los pasos siguientes detallan el procedimiento para un envío independiente (de una sola toma). La mayoría de los pasos son similares a los envíos del centro de llamadas. Para obtener más información, consulte esta [página](../call-center/create-call-center.md).

Para crear y enviar un nuevo envío externo personalizado independiente, siga estos pasos principales:

1. Crear el canal externo personalizado, [leer más](#create-channel)
1. Cree la entrega [leer más](#create-delivery)
1. Defina la audiencia, [leer más](#select-audience)
1. Editar el contenido, [leer más](#edit-content)
1. Previsualice y envíe el envío, [leer más](#preview-send)

## Creación del canal externo personalizado{#create-channel}

En primer lugar, debe configurar el canal externo personalizado. Estos son los pasos principales que se deben seguir en la consola del cliente:

1. Configure el esquema para añadir el nuevo canal a la lista de canales disponibles.
1. Cree una nueva cuenta externa de enrutamiento.
1. Cree una nueva plantilla de envío asociada al nuevo canal.

Para obtener más información, consulte la [documentación de la consola del cliente](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html)

## Creación del envío{#create-delivery}

Siga estos pasos para crear la entrega y configurar sus propiedades:

1. Seleccione el menú **[!UICONTROL Envíos]** y haga clic en el botón **[!UICONTROL Crear envío]**.

1. Elija el canal externo personalizado que desee, seleccione la plantilla asociada y haga clic en **[!UICONTROL Crear envío]** para confirmar.

   ![Captura de pantalla que muestra la creación de un envío personalizado](assets/cus-create.png){zoomable="yes"}


1. En **[!UICONTROL Propiedades]**, escriba una **[!UICONTROL Etiqueta]** para la entrega.

   ![Captura de pantalla que muestra la configuración de propiedades de un envío personalizado](assets/cus-properties.png){zoomable="yes"}

Para obtener más información sobre la creación de envíos, consulte la [documentación](../call-center/create-call-center.md#create-delivery) del centro de llamadas.

## Definición del público{#select-audience}

Ahora, debe definir la audiencia a la que se dirige el archivo de extracción.

1. En la sección **[!UICONTROL Audiencia]** de la página de entrega, haga clic en **[!UICONTROL Seleccionar audiencia]**.

1. Elija una audiencia existente o cree la suya propia.

   ![Captura de pantalla que muestra la selección de audiencias para una entrega personalizada](assets/cc-audience2.png){zoomable="yes"}

Para obtener más información sobre la definición de audiencia, consulte la [documentación](../call-center/create-call-center.md#select-audience) del centro de llamadas.

## Edición del contenido{#edit-content}

Ahora, vamos a editar el contenido del archivo de extracción que se generará con la entrega del canal personalizado.

1. En la página de envío, haga clic en el botón **[!UICONTROL Editar contenido]**.

1. Especifique un **[!UICONTROL nombre de archivo]**, seleccione un **[!UICONTROL formato de archivo]** y agregue tantas columnas como sea necesario para el archivo de extracción.

   ![Captura de pantalla que muestra las opciones de configuración de atributos para el archivo de extracción.](assets/cc-content-attributes.png)

Para obtener más información sobre la edición de contenido, consulte la [documentación](../call-center/create-call-center.md#edit-content) del centro de llamadas.

## Previsualización y envío de la entrega{#preview-send}

Cuando el contenido de la entrega está listo, puede previsualizarlo con perfiles de prueba y enviar pruebas. A continuación, puede realizar la entrega para generar el archivo de extracción.

1. En la página de contenido de la entrega, haga clic en el botón **[!UICONTROL Simular contenido]** y seleccione perfiles de prueba.

   ![Captura de pantalla que muestra la opción de simular contenido en la página de contenido de envío](assets/cus-simulate.png){zoomable="yes"}

1. En la página de entrega, haga clic en **[!UICONTROL Revisar y enviar]** y luego en **[!UICONTROL Preparar]**. A continuación, confirme.

   ![Captura de pantalla que muestra la opción de preparación y el menú de registros](assets/cus-prepare.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Enviar]** para continuar con el proceso de envío final y confirme.

Para obtener más información sobre la vista previa y el envío, consulte la [documentación](../call-center/create-call-center.md#preview-send) del centro de llamadas.
