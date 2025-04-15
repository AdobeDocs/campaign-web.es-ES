---
audience: end-user
title: Trabajar con servicios de suscripción
description: Aprenda a acceder, crear y administrar servicios de suscripción en Adobe Campaign Web
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 25%

---

# Crear y administrar servicios de suscripción {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Crear y administrar servicios"
>abstract="Utilice Adobe Campaign para crear y monitor sus servicios, como boletines informativos, y para verificar las suscripciones o bajas de suscripción a estos servicios. Las suscripciones solo se aplican al envío de correo electrónico y SMS."

Utilice Adobe Campaign Web para administrar y crear sus servicios, como boletines informativos, y para verificar las suscripciones o bajas a estos servicios.

Se pueden definir varios servicios en paralelo, por ejemplo: boletines informativos para categorías específicas de productos, temáticas o áreas de un sitio web, suscripciones a varios tipos de mensajes de alerta y notificaciones en tiempo real.

>[!NOTE]
>
>Las suscripciones solo se aplican al envío de correo electrónico y SMS.

## Acceso a los servicios de suscripción {#access-services}

Para acceder a los servicios de suscripción disponibles para su plataforma, seguir los pasos que se indican a continuación.

1. Examinar al menú Servicios ]**de**[!UICONTROL  suscripción situado a la izquierda navegación carril, en **[!UICONTROL Gestión de]** clientes.

   ![Captura de pantalla que muestra el menú Servicios de suscripción a la izquierda navegación carril en Gestión de clientes](assets/service-list.png){zoomable="yes"}

1. Se muestra el lista de todos los servicios de suscripción existentes. Puede búsqueda los servicios y filtrar por canal, carpeta o agregar reglas con el modelador](../query/query-modeler-overview.md) consulta[.

   ![Captura de pantalla que muestra el lista de los servicios de suscripción con filtros para canal, carpeta y reglas](assets/service-filters.png){zoomable="yes"}

1. Para editar un servicio existente, haga clic en su nombre.

1. Eliminar o duplicado cualquier servicio mediante el icono de tres puntos junto al nombre del servicio.<!--so all subscribers are unsubscribed - need to mention?-->

## Creación de su primer servicio de suscripción {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Definir las propiedades del servicio"
>abstract="Introduzca la etiqueta del servicio de suscripción y defina opciones adicionales, como el período de validez del servicio."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Selección de un mensaje de confirmación"
>abstract="Cuando un usuario se suscribe o cancela la suscripción a un servicio, puede enviar un mensaje de confirmación. Seleccione las plantillas que usará en ese mensaje."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Página de aterrizaje predeterminada"
>abstract="Seleccione las páginas de aterrizaje predeterminadas asociadas a este servicio."

Para crear una servicio de suscripción, seguir los pasos que se describen a continuación.

1. Seleccione el **[!UICONTROL Crear servicio de suscripción]** botón.

   ![Captura de pantalla que muestra el botón de servicio de suscripción de Crear](assets/service-create-button.png){zoomable="yes"}

1. Seleccione un canal: **[!UICONTROL correo electrónico]** o **[!UICONTROL SMS]**.

1. En las propiedades del servicio, introduzca una etiqueta y defina **[!UICONTROL las opciones]** adicionales necesarias.

   ![Captura de pantalla que muestra la sección de propiedades del servicio con etiqueta y opciones adicionales](assets/service-create-properties.png){zoomable="yes"}

1. De forma predeterminada, los servicios se almacenan en la **[!UICONTROL carpeta Servicios y Suscripciones]** . Puede cambiarla desplazándose a la ubicación deseada. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders)

1. De forma predeterminada, las suscripciones son ilimitadas.

   Deshabilite la **[!UICONTROL opción Período]** de validez ilimitado para definir una duración de validez para el servicio. Una vez finalizado el periodo de validez:
   * Ya ningún perfil puede suscribirse a este servicio.
   * Todos los suscriptores de este servicio son dados de baja automáticamente.

   ![Captura de pantalla que muestra la configuración del período de validez de un servicio de suscripción](assets/service-create-validity-period.png){zoomable="yes"}

1. Cuando un usuario se suscribe o cancela la suscripción a un servicio, puede enviar un mensaje de confirmación. Seleccione las plantillas que se usarán para ese mensaje según su caso de uso. Estas plantillas deben configurarse con el **[!UICONTROL asignación de destino de]** suscripciones. [Más información](#create-confirmation-message)

   ![Captura de pantalla que muestra el mensaje de confirmación plantilla selección](assets/service-create-confirmation-msg.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Guardar y revisar]**. El nuevo servicio se añade al lista de servicios ]**de**[!UICONTROL  suscripción.

1. Seleccione la suscripción predeterminada y baja páginas de destino asociadas con este servicio.

   >[!AVAILABILITY]
   >
   >Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

   ![Captura de pantalla que muestra la configuración de página de aterrizaje predeterminada para un servicio de suscripción](assets/service-create-default-lp.png){zoomable="yes"}

   Una vez hecho esto, al [insertar un vincular](../email/message-tracking.md) en un correo electrónico, seleccione **[!UICONTROL vincular]** de suscripción o **[!UICONTROL vincular]** de cancelación de suscripción. Al hacer clic en ese vincular, los usuarios serán dirigidos a la suscripción o baja página de aterrizaje a los que se hace referencia en el servicio. <!--After submitting the form, they will be subscribed to / unsubscribed from the service.-->

   ![Captura de pantalla que muestra la configuración de la suscripción y vincular baja](assets/service-create-default-lp-link.png){zoomable="yes"}

1. Guardar y revise los cambios.

Ahora puede hacer lo siguiente:

* Agregue manualmente suscriptores a este servicio y cancelar la suscripción perfiles. [Más información](../audience/manage-subscribers.md)

* Invite a sus clientes a suscribirse a este servicio a través de una página de aterrizaje. [Más información](../landing-pages/lp-use-cases.md#lp-subscription)

* Enviar mensajes a los suscriptores de este servicio. [Descubra cómo](../msg/send-to-subscribers.md)

## Creación de un mensaje de confirmación {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Selección de la plantilla de envíos de suscripciones"
>abstract="Para enviar mensajes de confirmación a los usuarios que se suscriben al servicio, debe seleccionar una plantilla de envíos específica basada en la asignación de destino **[!UICONTROL Suscripciones]**, sin un destino definido."

>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="Selección de la plantilla de envíos de cancelación de suscripciones"
>abstract="Para enviar mensajes de confirmación a los usuarios que cancelan la suscripción al servicio, debe seleccionar una plantilla de envíos específica basada en la asignación de destino **[!UICONTROL Suscripciones]**, sin un destino definido."

Para enviar mensajes de confirmación a los usuarios que se suscriben o cancelar la suscripción de su servicio, cree un plantilla de envíos con el **[!UICONTROL asignación de destino de]** suscripciones, sin un destino definido. Siga estos pasos:

1. Crear un plantilla de envíos para la confirmación de la suscripción. [Aprenda a crear una plantilla](../msg/delivery-template.md)

1. No seleccione un audiencia para este envío. En su lugar, acceda al Configuración de envío ****, vaya al [pestaña de audiencias](../advanced-settings/delivery-settings.md#audience) y seleccione el **[!UICONTROL asignación de destino Suscripciones]** en el lista.

   ![Captura de pantalla que muestra la selección asignación de destino para un plantilla de envíos](assets/service-confirmation-template-mapping.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si no selecciona el **[!UICONTROL asignación de destino Suscripciones]** , sus suscriptores no recibirán el mensaje de confirmación. Obtenga más información sobre destino asignaciones en [esta sección](../audience/targeting-dimensions.md).

1. Editar el contenido de la plantilla de envíos, guárdelo y ciérrelo.

   ![Captura de pantalla que muestra el editor de contenido para una plantilla de envíos](assets/service-confirmation-template.png){zoomable="yes"}

   >[!NOTE]
   >
   >Obtén más información sobre envío canales y cómo definir envío contenido en las [secciones canal](../email/create-email.md) correo electrónico y [SMS canal](../sms/create-sms.md) .

1. Repita los pasos anteriores para crear un plantilla de envíos para la confirmación del baja.

Ahora puede seleccionar estos mensajes al [crear un servicio de suscripción](#create-service). Los usuarios que se suscriban o cancelar la suscripción de ese servicio recibirán los mensajes de confirmación seleccionados.

## Monitorizar los servicios de suscripción {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Recuento de suscriptores"
>abstract="Haga clic en **Calcular** para obtener el número total de suscriptores para este servicio."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers_report"
>title="Número total de suscriptores"
>abstract="El indicador clave de rendimiento (KPI) proporciona una vista completa de la base de suscriptores, mostrando el recuento total de personas que se han suscrito a este servicio."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Número de suscripciones para el periodo"
>abstract="Utilice la lista desplegable para cambiar el intervalo de tiempo y ver el número de suscripciones y sus bajas durante el periodo seleccionado."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Evolución general de suscripciones"
>abstract="Este gráfico muestra el desglose por periodo, incluyendo suscripciones, bajas, la evolución en números y el porcentaje de fidelidad."

Para medir la eficacia de sus servicios de suscripción para canales de SMS y correo electrónico, acceda a los registros e informes de un servicio determinado.

1. Seleccione un servicio existente en la **[!UICONTROL lista Servicios]** de suscripción. Haga clic en **[!UICONTROL Calcular]** para obtener el número total de suscriptores.

   ![Captura de pantalla que muestra el cálculo del número total de suscriptores](assets/service-logs-subscribers-count.png){zoomable="yes"}

1. En el panel servicio, seleccione **[!UICONTROL Registros para vista el lista de suscriptores]** a este servicio.

   Puede verificar el número total de suscriptores, el nombre y la dirección de cada destinatario, y cuándo se suscribieron o cancelaron la suscripción. También puede filtrarlos.

   ![Captura de pantalla que muestra la sección de registros con detalles del suscriptor](assets/service-logs.png){zoomable="yes"}

1. En el panel de servicio, seleccione **[!UICONTROL Informes]**. Consulte los siguientes indicadores:

   * Se muestra el **[!UICONTROL número total de suscriptores]** .

   * Ver el número de suscripciones y bajas de suscripción durante un período seleccionado. Utilice la lista desplegable para cambiar el intervalo de tiempo.

     ![Captura de pantalla que muestra la sección de informes con datos de suscripción y baja](assets/service-reports.png){zoomable="yes"}

   * El **[!UICONTROL gráfico Evolución general de las]** suscripciones muestra el desglose por período, incluidas las suscripciones, las bajas, la evolución en números y el porcentaje de fidelidad.<!--what is Registered?-->

1. Utilice el **[!UICONTROL botón Recarga]** para recuperar los valores más recientes de la ejecución y programación del flujo de trabajo de seguimiento.