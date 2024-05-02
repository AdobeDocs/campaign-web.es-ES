---
audience: end-user
title: Seguimiento de mensajes
description: Obtenga información sobre cómo añadir vínculos y rastrear los mensajes enviados
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: a95a70aa56061106a920584a3501cd4b1434ec8a
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 66%

---

# Adición de vínculos y seguimiento de mensajes {#tracking}

Utilice el Diseñador de correo electrónico para añadir vínculos al contenido y realizar un seguimiento de los mensajes enviados para controlar el comportamiento de los destinatarios.

## Inserción de vínculos {#insert-links}

Al diseñar un mensaje, puede agregar vínculos al contenido.

>[!NOTE]
>
>Cuando el seguimiento está habilitado, se realiza el seguimiento de todos los vínculos incluidos en el contenido del mensaje.

Para insertar vínculos en el contenido del correo electrónico, siga los pasos a continuación:

1. Seleccione un elemento y haga clic en **[!UICONTROL Insertar vínculo]** en la barra de herramientas contextual.

1. Elija el tipo de vínculo que desea crear:

   ![](assets/message-tracking-insert-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL Vínculo externo]**: inserte un vínculo a una dirección URL externa.

     >[!AVAILABILITY]
     >
     >Las siguientes capacidades (vínculo a **[!UICONTROL Página de aterrizaje]**, **[!UICONTROL Vínculo de suscripción]** y **[!UICONTROL Vínculo de baja]**) están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se pueden implementar en ningún otro entorno.

   * **[!UICONTROL Página de aterrizaje]**: inserte un vínculo a una página de aterrizaje. Si selecciona una página de aterrizaje dinámica (con la variable **[!UICONTROL Servicio desde URL]** opción seleccionada), puede seleccionar cualquier servicio de la lista. [Más información](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL Vínculo de suscripción]**: Inserte un vínculo a un servicio de suscripción. Cuando los usuarios hacen clic en el vínculo, se les dirige a la página de aterrizaje de suscripción a la que se hace referencia en el servicio seleccionado. [Más información](../audience/manage-services.md#create-service)

     ![](assets/service-create-default-lp-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL Vínculo de baja]**: Inserte un vínculo a un servicio de baja. Cuando los suscriptores hacen clic en el vínculo, se les dirige a la página de aterrizaje de baja a la que se hace referencia en el servicio seleccionado. [Más información](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. Introduzca la dirección URL deseada en el campo correspondiente o seleccione una página de aterrizaje o un servicio y defina la configuración y los estilos del vínculo.

1. Agregue una **[!UICONTROL Etiqueta]** y un **[!UICONTROL Vínculo]**.

1. Guarde los cambios.

1. Una vez creado el vínculo, aún puede modificarlo desde la pestaña **[!UICONTROL Configuración]**.

   * Puede editar el vínculo y cambiar su **[!UICONTROL Destinatario]**.
   * Puede elegir subrayar el vínculo o no marcando la opción correspondiente.

   ![](assets/message-tracking-link-settings.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>Los mensajes de correo electrónico de tipo marketing deben incluir un vínculo de no participación, que no es necesario para los mensajes transaccionales. La categoría del mensaje (**[!UICONTROL Marketing]** o **[!UICONTROL Transaccional]**) se define en el nivel de superficie de canal y durante la creación del mensaje.

Se debe añadir un vínculo específico a la página espejo en todos los correos electrónicos. Obtenga más información sobre la página espejo en [esta sección](mirror-page.md).

## Administrar seguimiento {#manage-tracking}

El [Diseñador de correo electrónico](create-email-content.md) le permite administrar las direcciones URL rastreadas, como editar el tipo de seguimiento para cada vínculo.

1. Haga clic en el icono **[!UICONTROL Vínculos]** del panel izquierdo para mostrar la lista de todas las direcciones URL del contenido que se va a rastrear.

   Esta lista permite tener una vista centralizada y localizar cada URL en el contenido del correo electrónico.

1. Para editar un vínculo, haga clic en el icono de lápiz correspondiente.

   ![](assets/message-tracking-edit-links.png){zoomable=&quot;yes&quot;}

1. Puede modificar el **[!UICONTROL Tipo de seguimiento]** si es necesario:

   ![](assets/message-tracking-edit-a-link.png){zoomable=&quot;yes&quot;}

   Para cada URL individual, puede definir el modo de seguimiento en uno de estos valores:

   * **[!UICONTROL Habilitado]**: activa el seguimiento en esta dirección URL.
   * **[!UICONTROL Exclusión]**: considera esta URL como una de exclusión o de baja.
   * **[!UICONTROL Página espejo]**: considera esta URL como una de página espejo.
   * **[!UICONTROL Nunca]**: nunca se activa el seguimiento de esta URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Agregue una **[!UICONTROL Categoría]** a su vínculo para agrupar los vínculos rastreados y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/message-tracking-edit-a-link_2.png){zoomable=&quot;yes&quot;}

1. Después de realizar el envío, puede acceder al informe. En el menú **[!UICONTROL Seguimiento]**, las **[!UICONTROL URL y flujos de clics]** muestran las direcciones URL de su envío más visitadas. [Más información](../reporting/gs-reports.md)
