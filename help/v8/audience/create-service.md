---
audience: end-user
title: Trabajo con servicios de suscripción
description: Obtenga información sobre cómo crear y administrar servicios en Adobe Campaign Web
badge: label="Beta"
source-git-commit: 47c00b3520ea38d4afa173f8a221ae5e127dd7a9
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 5%

---


# Trabajo con servicios de suscripción {#create-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Crear y administrar sus servicios"
>abstract="Utilice Adobe Campaign para crear y supervisar sus servicios, como los boletines informativos, y para comprobar las suscripciones o bajas de suscripción a estos servicios. Las suscripciones solo se aplican al envío de correo electrónico y SMS."

Utilice la web de Adobe Campaign para administrar y crear sus servicios, como boletines informativos, y para comprobar las suscripciones o cancelaciones de suscripción a estos servicios.

>[!NOTE]
>
>Las suscripciones solo se aplican al envío de correo electrónico y SMS.

Se pueden definir varios servicios en paralelo, por ejemplo: boletines para categorías de productos específicas, temas o áreas de un sitio web, suscripciones a varios tipos de mensajes de alerta y notificaciones en tiempo real.

Para obtener más información sobre la administración de suscripciones y bajas, consulte la [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/subscriptions.html){target="_blank"}.

## Acceso a servicios de suscripción {#access-services}

Para acceder a los servicios de suscripción disponibles para su plataforma, siga los pasos a continuación.

1. Vaya a la **[!UICONTROL Servicios de suscripción]** en el carril de navegación izquierdo.

   ![](assets/service-list.png)

1. Se muestra la lista de todos los servicios de suscripción existentes. Puede buscar en los servicios y filtrar por el canal, la carpeta o utilizar filtros avanzados.

   ![](assets/service-filters.png)

1. Para editar un servicio existente, haga clic en su nombre.

1. Puede eliminar o duplicar cualquier servicio mediante el icono de tres puntos situado junto al nombre de este servicio.

## Creación de su primer servicio de suscripción {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Defina las propiedades del servicio"
>abstract="Introduzca la etiqueta del servicio de suscripción y defina opciones adicionales, como un periodo de validez del servicio."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Seleccionar un mensaje de confirmación"
>abstract="Cuando un usuario se suscribe o cancela la suscripción a un servicio, puede enviar un mensaje de confirmación. Seleccione las plantillas que desea utilizar para ese mensaje."

Para crear un servicio de suscripción, siga los pasos a continuación.

1. Seleccione el **[!UICONTROL Crear servicio de suscripción]** botón.

   ![](assets/service-create-button.png)

1. Seleccione un canal: **[!UICONTROL Correo electrónico]** o **[!UICONTROL SMS]**.

1. En las propiedades del servicio, introduzca una etiqueta y defina las opciones adicionales que desee.

   ![](assets/service-create-properties.png)

1. De forma predeterminada, las suscripciones son ilimitadas. Puede desactivar las **[!UICONTROL Período de validez ilimitado]** para definir una duración de validez del servicio. En el ejemplo siguiente, después de 20 días, ya no podrá suscribirse a este servicio.

   ![](assets/service-create-validity-period.png)

1. Cuando un usuario se suscribe o cancela la suscripción a un servicio, puede enviar un mensaje de confirmación. Seleccione las plantillas que desea utilizar para ese mensaje según el caso de uso. Estas plantillas deben configurarse con la variable **[!UICONTROL Suscripciones]** asignación de destino. [Más información](#create-confirmation-message)

   ![](assets/service-create-confirmation-msg.png)

1. Clic **[!UICONTROL Guardar y revisar]**. El nuevo servicio se agrega al **[!UICONTROL Servicios de suscripción]** lista.

## Crear un mensaje de confirmación {#create-confirmation-message}

Para enviar un mensaje de confirmación a los usuarios que se suscriben o cancelan la suscripción a su servicio, debe crear una plantilla de envío con el **[!UICONTROL Suscripciones]** asignación de destino, sin un destino definido. Para ello, siga los pasos a continuación.

1. Cree una plantilla de envío para la confirmación de suscripción. [Descubra cómo](../msg/delivery-template.md)

1. No seleccione una audiencia para este envío. En su lugar, acceda al **[!UICONTROL Configuración de envío]**, vaya a la [Audiencia](../advanced-settings/delivery-settings.md#audience) y seleccione la pestaña **[!UICONTROL Suscripciones]** asignación de destino de la lista.

   ![](assets/service-confirmation-template-mapping.png)

   >[!NOTE]
   >
   >Si no selecciona la variable  **[!UICONTROL Suscripciones]** asignación de destino, los suscriptores no recibirán el mensaje de confirmación. Las asignaciones de destino se definen en la consola de la versión 8 de Campaign. Obtenga más información sobre la [Documentación de Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=es){target="_blank"}.

1. Edite el contenido de la plantilla de envíos, guárdelo y ciérrelo.

   ![](assets/service-confirmation-template.png)

   >[!NOTE]
   >
   >Obtenga más información acerca de los canales de envío y cómo definir un contenido de envío en la [Canal de correo electrónico](../email/create-email.md) y [Canal de SMS](../sms/create-sms.md) secciones.

1. Repita los pasos anteriores para crear una plantilla de envíos para la confirmación de baja.

Ahora puede seleccionar estos mensajes cuando [creación de un servicio de suscripción](#create-service). Los usuarios que se suscriban o cancelen su suscripción a ese servicio reciben el mensaje de confirmación seleccionado.

## Añadir suscriptores a su servicio {#add-subscribers}

Una vez creado un servicio, puede añadir manualmente suscriptores. Siga estos pasos.

1. Seleccione un servicio existente del **[!UICONTROL Servicios de suscripción]** lista.

1. Seleccione el **[!UICONTROL Suscriptores]** y haga clic en **[!UICONTROL Añadir perfiles]**.

   ![](assets/service-subscribers-tab.png)

1. Seleccione los perfiles que desee añadir en la lista y haga clic en **[!UICONTROL Confirmar]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Clic **[!UICONTROL Enviar]**. Los destinatarios seleccionados recibirán la suscripción [mensaje de confirmación](#create-confirmation-message) que seleccionó al [creación del servicio](#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

Los perfiles añadidos se muestran en la variable **[!UICONTROL Suscriptores]** lista. Ahora están suscritos a su servicio.

## Eliminación de suscriptores del servicio {#remove-subscribers}

Una vez añadidos los suscriptores al servicio, puede eliminarlos. Siga estos pasos.

1. Seleccione un servicio existente del **[!UICONTROL Servicios de suscripción]** lista.

1. Haga clic en el icono de tres puntos junto al nombre del destinatario deseado y seleccione **[!UICONTROL Eliminar]**.

   ![](assets/service-subscribers-delete.png)

1. Confirme la eliminación y haga clic en **[!UICONTROL Enviar]**. Los destinatarios seleccionados recibirán la baja [mensaje de confirmación](#create-confirmation-message) que seleccionó al [creación del servicio](#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

El destinatario se elimina del **[!UICONTROL Suscriptores]** y ya no está suscrito a su servicio.

## Registros e informes del servicio de suscripción {#logs-and-reports}

Para medir la eficacia de los servicios de suscripción para canales de correo electrónico y SMS, puede acceder a los registros e informes de un servicio determinado.

1. Seleccione un servicio existente del **[!UICONTROL Servicios de suscripción]** lista. Clic **[!UICONTROL Calcular]** el obtiene el número total de suscriptores.

   ![](assets/service-logs-reports-buttons.png)

1. En el panel de servicios, seleccione **[!UICONTROL Registros]** para ver la lista de suscriptores de este servicio. Puede comprobar el número total de suscriptores, el nombre y la dirección de cada destinatario y cuándo se suscribieron o cancelaron la suscripción. También puede filtrar por ellos.

   ![](assets/service-logs.png)

1. En el panel de servicios, seleccione **[!UICONTROL Informes]**. Compruebe las luces testigo siguientes:

   * El **[!UICONTROL Número total de suscriptores]** se muestra.

   * Puede ver el número de suscripciones y bajas de suscripción durante un periodo seleccionado. Utilice la lista desplegable para cambiar el intervalo de tiempo.

     ![](assets/service-reports.png)

   * El **[!UICONTROL Evolución general de las suscripciones]** El gráfico muestra el desglose por periodo, incluidas las suscripciones, las bajas, la evolución en los números y el porcentaje de fidelidad.<!--what is Registered?-->

   * Utilice el **[!UICONTROL Recargar]** para recuperar los últimos valores de la ejecución y programación del flujo de trabajo de seguimiento.

## Envío a los suscriptores de un servicio

Una vez que [creó un servicio de suscripción](#create-service), puede dirigirse a sus suscriptores en una entrega. Siga estos pasos.

1. [Crear una audiencia](../audience/create-audience.md) incluidos los suscriptores del servicio que ha creado:

   * En el **[!UICONTROL Crear audiencia]** actividad, muestre los atributos avanzados y seleccione **[!UICONTROL Destinatario]** > **[!UICONTROL Suscripciones]** > **[!UICONTROL Servicio]**.

   * En este ejemplo, seleccione los usuarios suscritos al servicio que tiene el **Newsletter de Luma** etiqueta.

   ![](assets/service-audience-subscribers.png)

1. [Creación de una entrega](../msg/gs-messages.md) y seleccione la audiencia que ha creado anteriormente.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Edite el contenido del mensaje como desee y realice la entrega.

   ![](assets/service-delivery-ready.png)

Su envío se realiza únicamente a los suscriptores de ese servicio.







