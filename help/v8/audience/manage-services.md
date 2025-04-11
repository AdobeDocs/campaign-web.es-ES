---
audience: end-user
title: Trabajar con servicios de suscripción
description: Obtenga información sobre cómo acceder, crear y administrar servicios de suscripción en Adobe Campaign Web
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
>abstract="Utilice Adobe Campaign para crear y supervisar sus servicios, como los boletines informativos, y para comprobar las suscripciones o bajas de suscripción a estos servicios. Las suscripciones solo se aplican al envío de correo electrónico y SMS."

Utilice Adobe Campaign Web para administrar y crear sus servicios, como los boletines informativos, y para comprobar las suscripciones o cancelaciones de suscripción a estos servicios.

Se pueden definir varios servicios en paralelo, por ejemplo: boletines informativos para categorías de productos específicas, temas o áreas de un sitio web, suscripciones a varios tipos de mensajes de alerta y notificaciones en tiempo real.

>[!NOTE]
>
>Las suscripciones solo se aplican al envío de correo electrónico y SMS.

## Acceso a servicios de suscripción {#access-services}

Para acceder a los servicios de suscripción disponibles para su plataforma, siga los pasos a continuación.

1. Vaya al menú **[!UICONTROL Servicios de suscripción]** en el carril de navegación izquierdo, en **[!UICONTROL Administración de clientes]**.

   ![Captura de pantalla que muestra el menú Servicios de suscripción en el carril de navegación izquierdo bajo Administración de clientes](assets/service-list.png){zoomable="yes"}

1. Se muestra la lista de todos los servicios de suscripción existentes. Puede buscar en los servicios y filtrar por canal, carpeta o agregar reglas mediante [query modeler](../query/query-modeler-overview.md).

   ![Captura de pantalla que muestra la lista de servicios de suscripción con filtros para canal, carpeta y reglas](assets/service-filters.png){zoomable="yes"}

1. Para editar un servicio existente, haga clic en su nombre.

1. Elimine o duplique cualquier servicio mediante el icono de tres puntos situado junto al nombre del servicio.<!--so all subscribers are unsubscribed - need to mention?-->

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

Para crear un servicio de suscripción, siga los pasos a continuación.

1. Seleccione el botón **[!UICONTROL Crear servicio de suscripción]**.

   ![Captura de pantalla que muestra el botón Crear servicio de suscripción](assets/service-create-button.png){zoomable="yes"}

1. Seleccione un canal: **[!UICONTROL Correo electrónico]** o **[!UICONTROL SMS]**.

1. En las propiedades del servicio, escriba una etiqueta y defina **[!UICONTROL Opciones adicionales]** según sea necesario.

   ![Captura de pantalla que muestra la sección de propiedades del servicio con etiqueta y opciones adicionales](assets/service-create-properties.png){zoomable="yes"}

1. De manera predeterminada, los servicios se almacenan en la carpeta **[!UICONTROL Services and Subscriptions]**. Puede cambiarlo navegando a la ubicación deseada. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders)

1. De forma predeterminada, las suscripciones son ilimitadas.

   Deshabilite la opción **[!UICONTROL Período de validez ilimitado]** para definir una duración de validez del servicio. Una vez finalizado el periodo de validez:
   * Ya ningún perfil puede suscribirse a este servicio.
   * Todos los suscriptores de este servicio cancelan su suscripción automáticamente.

   ![Captura de pantalla que muestra la configuración del período de validez de un servicio de suscripción](assets/service-create-validity-period.png){zoomable="yes"}

1. Cuando un usuario se suscribe o cancela la suscripción a un servicio, puede enviar un mensaje de confirmación. Seleccione las plantillas que desea utilizar para ese mensaje según el caso de uso. Estas plantillas deben configurarse con la asignación de destino **[!UICONTROL Subscriptions]**. [Más información](#create-confirmation-message)

   ![Captura de pantalla que muestra la selección de la plantilla del mensaje de confirmación](assets/service-create-confirmation-msg.png){zoomable="yes"}

1. Haz clic en **[!UICONTROL Guardar y revisar]**. El nuevo servicio se agrega a la lista **[!UICONTROL Servicios de suscripción]**.

1. Seleccione las páginas de aterrizaje predeterminadas de suscripción y de cancelación de suscripción asociadas a este servicio.

   >[!AVAILABILITY]
   >
   >Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

   ![Captura de pantalla que muestra la configuración predeterminada de la página de aterrizaje para un servicio de suscripción](assets/service-create-default-lp.png){zoomable="yes"}

   Una vez finalizado, cuando [inserte un vínculo](../email/message-tracking.md) en un correo electrónico, seleccione **[!UICONTROL Vínculo de suscripción]** o **[!UICONTROL Vínculo de baja]**. Al hacer clic en ese vínculo, se dirige a los usuarios a la página de aterrizaje de suscripción o de cancelación de suscripción a la que se hace referencia en el servicio. <!--After submitting the form, they will be subscribed to / unsubscribed from the service.-->

   ![Captura de pantalla que muestra la configuración de suscripción y vínculo de baja](assets/service-create-default-lp-link.png){zoomable="yes"}

1. Guarde y revise los cambios.

Ahora puede hacer lo siguiente:

* Añadir manualmente suscriptores a este servicio y cancelar la suscripción de perfiles. [Más información](../audience/manage-subscribers.md)

* Invite a sus clientes a suscribirse a este servicio a través de una página de aterrizaje. [Más información](../landing-pages/lp-use-cases.md#lp-subscription)

* Envíe mensajes a los suscriptores de este servicio. [Descubra cómo](../msg/send-to-subscribers.md)

## Creación de un mensaje de confirmación {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Selección de la plantilla de envíos de suscripciones"
>abstract="Para enviar mensajes de confirmación a los usuarios que se suscriben al servicio, debe seleccionar una plantilla de envíos específica basada en la asignación de destino **[!UICONTROL Suscripciones]**, sin un destino definido."

>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="Selección de la plantilla de envíos de cancelación de suscripciones"
>abstract="Para enviar mensajes de confirmación a los usuarios que cancelan la suscripción al servicio, debe seleccionar una plantilla de envíos específica basada en la asignación de destino **[!UICONTROL Suscripciones]**, sin un destino definido."

Para enviar mensajes de confirmación a los usuarios que se suscriben o cancelan la suscripción a su servicio, cree una plantilla de envío con la asignación de destino **[!UICONTROL Suscripciones]**, sin un destino definido. Siga estos pasos:

1. Cree una plantilla de envío para la confirmación de suscripción. [Aprenda a crear una plantilla](../msg/delivery-template.md)

1. No seleccione una audiencia para este envío. En su lugar, accede a la entrega **[!UICONTROL Settings]**, ve a la pestaña [Audience](../advanced-settings/delivery-settings.md#audience) y selecciona la asignación de destino **[!UICONTROL Subscriptions]** de la lista.

   ![Captura de pantalla que muestra la selección de asignación de destino para una plantilla de envíos](assets/service-confirmation-template-mapping.png){zoomable="yes"}

   >[!NOTE]
   >
   >Si no selecciona la asignación de destino **[!UICONTROL Suscripciones]**, los suscriptores no recibirán el mensaje de confirmación. Obtenga más información acerca de las asignaciones de destino en [esta sección](../audience/targeting-dimensions.md).

1. Edite el contenido de la plantilla de envíos, guárdelo y ciérrelo.

   ![Captura de pantalla que muestra el editor de contenido para una plantilla de envíos](assets/service-confirmation-template.png){zoomable="yes"}

   >[!NOTE]
   >
   >Obtenga más información acerca de los canales de envío y cómo definir el contenido de envío en las secciones [Canal de correo electrónico](../email/create-email.md) y [Canal de SMS](../sms/create-sms.md).

1. Repita los pasos anteriores para crear una plantilla de envíos para la confirmación de baja.

Ahora puede seleccionar estos mensajes al [crear un servicio de suscripción](#create-service). Los usuarios que se suscriban o cancelen su suscripción a ese servicio recibirán los mensajes de confirmación seleccionados.

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
>abstract="Este gráfico muestra el desglose por periodo, incluidas las suscripciones, las bajas de suscripción, la evolución en números y el porcentaje de fidelidad."

Para medir la eficacia de sus servicios de suscripción para canales de correo electrónico y SMS, acceda a los registros e informes de un servicio determinado.

1. Seleccione un servicio existente de la lista **[!UICONTROL Servicios de suscripción]**. Haga clic en **[!UICONTROL Calcular]** para obtener el número total de suscriptores.

   ![Captura de pantalla que muestra el número total de suscriptores](assets/service-logs-subscribers-count.png){zoomable="yes"}

1. En el panel del servicio, seleccione **[!UICONTROL Registros]** para ver la lista de suscriptores con este servicio.

   Puede comprobar el número total de suscriptores, el nombre y la dirección de cada destinatario y cuándo se han suscrito o cancelado la suscripción. También puede filtrarlos.

   ![Captura de pantalla que muestra la sección de registros con detalles del suscriptor](assets/service-logs.png){zoomable="yes"}

1. En el panel de servicios, seleccione **[!UICONTROL Informes]**. Compruebe las luces testigo siguientes:

   * Se muestra **[!UICONTROL Número total de suscriptores]**.

   * Ver el número de suscripciones y bajas de suscripción durante un periodo seleccionado. Utilice la lista desplegable para cambiar el intervalo de tiempo.

     ![Captura de pantalla que muestra la sección de informes con datos de suscripción y baja](assets/service-reports.png){zoomable="yes"}

   * El gráfico **[!UICONTROL Evolución general de las suscripciones]** muestra el desglose por período, incluidas las suscripciones, las bajas de suscripción, la evolución en números y el porcentaje de lealtad.<!--what is Registered?-->

1. Utilice el botón **[!UICONTROL Recargar]** para recuperar los valores más recientes de la ejecución y programación del flujo de trabajo de seguimiento.