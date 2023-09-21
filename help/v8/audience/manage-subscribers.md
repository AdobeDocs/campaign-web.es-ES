---
audience: end-user
title: Administración de los suscriptores de un servicio
description: Obtenga información sobre cómo administrar y entregar a los suscriptores de un servicio en Adobe Campaign Web
badge: label="Beta"
source-git-commit: 6406be82c2bad9346f6743e18535fdfe132b2bd0
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---


# Administración de los suscriptores de un servicio {#manage-subscribers}

Una vez que [creó un servicio](manage-services.md#create-service), puede añadir suscriptores, cancelar la suscripción de destinatarios y enviar mensajes a los suscriptores de ese servicio.

La administración de los suscriptores se detalla en esta página. Para aprender a enviar mensajes a los suscriptores, consulte [esta sección](../content/send-to-subscribers.md).

## Añadir suscriptores a su servicio {#add-subscribers}

Para añadir suscriptores manualmente, siga los pasos a continuación.

1. Seleccione un servicio existente del **[!UICONTROL Servicios de suscripción]** lista.

1. Seleccione el **[!UICONTROL Suscriptores]** y haga clic en **[!UICONTROL Añadir perfiles]**.

   ![](assets/service-subscribers-tab.png)

1. Seleccione los perfiles que desee añadir en la lista y haga clic en **[!UICONTROL Confirmar]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Clic **[!UICONTROL Enviar]**.<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> Los destinatarios seleccionados recibirán la suscripción [mensaje de confirmación](manage-services.md#create-confirmation-message) que seleccionó al [creación del servicio](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

Los perfiles añadidos se muestran en la variable **[!UICONTROL Suscriptores]** lista. Ahora están suscritos a su servicio.

## Eliminación de suscriptores del servicio {#remove-subscribers}

### Cancelar la suscripción manual de destinatarios {#manual-unsubscription}

Una vez que [suscriptores añadidos](#add-subscribers) Al servicio, puede cancelar manualmente la suscripción de cada uno de ellos. Siga estos pasos.

1. Seleccione un servicio existente del **[!UICONTROL Servicios de suscripción]** lista.

1. Haga clic en el icono de tres puntos junto al nombre del destinatario deseado y seleccione **[!UICONTROL Eliminar]**.

   ![](assets/service-subscribers-delete.png)

1. Confirme la eliminación y haga clic en **[!UICONTROL Enviar]**. El destinatario seleccionado recibirá la baja [mensaje de confirmación](manage-services.md#create-confirmation-message) que seleccionó al [creación del servicio](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

El destinatario se elimina del **[!UICONTROL Suscriptores]** y ya no está suscrito a su servicio.

### Cancelar automáticamente la suscripción de destinatarios {#automatic-unsubscription}

Un servicio de suscripción puede tener una duración limitada. La suscripción de los destinatarios se cancela automáticamente cuando caduca el periodo de validez.

Este periodo se especifica cuando [creación del servicio](manage-services.md#create-service). Desde el **[!UICONTROL Opciones adicionales]**, deshabilite la **[!UICONTROL Período de validez ilimitado]** y defina un periodo de validez del servicio.

![](assets/service-create-validity-period.png)

Una vez que caduca la duración especificada, se cancela la suscripción de forma automática a todos los suscriptores de ese servicio.
