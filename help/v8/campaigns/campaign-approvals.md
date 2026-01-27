---
audience: end-user
title: Configuración y administración del proceso de aprobación
description: Obtenga información sobre cómo administrar las aprobaciones de campañas de marketing en Campaign Web
feature: Approvals, Campaigns
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 4%

---

# Administrar el proceso de aprobación {#campaign-approvals}

>[!IMPORTANT]
>
>Las aprobaciones solo están disponibles para las entregas creados dentro de una campaña. Esto no se aplica a los envíos independientes o a los envíos creados en flujos de trabajo fuera de un contexto de campaña.

El proceso de aprobación ayuda a coordinar varias partes interesadas y garantiza el control de calidad antes de realizar las entregas. Utilice aprobaciones cuando su organización requiera que equipos diferentes lo validen, como administradores de marketing que revisan contenido o analistas de datos que validan audiencias de destino.

Cuando las aprobaciones están habilitadas, debe enviar el contenido o el destino para la aprobación. Los revisores designados reciben notificaciones por correo electrónico que solicitan validación y pueden aprobarlas o rechazarlas directamente desde la interfaz de usuario web. No se pueden realizar envíos hasta que se hayan concedido todas las aprobaciones necesarias. Puede activar:

* **Aprobación de contenido**: valide el contenido, el diseño y la personalización del mensaje
* **Aprobación de destino**: valide la audiencia y los criterios de segmentación
* **Confirmación de envío**: se requiere una confirmación final antes de enviar

## Configuración de la aprobación {#configure-approvals}

La configuración de aprobación se hereda de la plantilla de campaña y se puede modificar para campañas individuales. Siga estos pasos para configurar las opciones de aprobación:

1. Abra su campaña o plantilla de campaña o cree una nueva desde el menú **[!UICONTROL Campañas]**.

1. Haga clic en el botón **[!UICONTROL Configuración]** en la parte superior derecha del panel de campañas.

1. En la sección **[!UICONTROL Aprobaciones]**, configure las siguientes opciones:

   ![Captura de pantalla que muestra la configuración de aprobación de la campaña](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL Habilitar aprobación de contenido]**: cuando está habilitado, el contenido de la entrega debe aprobarse antes de enviarlo. Haga clic en el icono de la carpeta en el campo **[!UICONTROL Revisor]** para seleccionar un operador o grupo de operadores.

   * **[!UICONTROL Habilitar aprobación de destino]**: cuando está habilitada, la audiencia de destino de envío debe aprobarse. Haga clic en el icono de la carpeta en el campo **[!UICONTROL Revisor]** para seleccionar un operador o grupo de operadores.

   * **[!UICONTROL Confirmar la entrega antes de enviarla]**: requiere una confirmación manual final antes de enviarla, incluso después de completar todas las demás aprobaciones.

>[!NOTE]
>
>* Si no se especifica ningún revisor, el propietario de la campaña se asigna como revisor.
>* Los revisores necesitan los permisos adecuados para aprobar los envíos. Solo los usuarios identificados en la lista de revisores pueden aprobar.

## Enviar para aprobación {#submit-approval}

Después de crear la entrega, siga estos pasos para enviar contenido y destinatario para su aprobación.

>[!NOTE]
>Las aprobaciones están disponibles tanto en los envíos del flujo de trabajo de la campaña como en los envíos independientes de la campaña.

1. En el panel de envío, haga clic en el botón **[!UICONTROL Enviar contenido]**. Los revisores designados pueden aprobarlo o rechazarlo. Consulte esta [sección](#approve-reject).

   ![Captura de pantalla que muestra el botón Enviar contenido](assets/approvals2.png){zoomable="yes"}

   El estado de aprobación cambia a pendiente en la sección **[!UICONTROL Properties]** del panel de envío. Consulte esta [sección](#rack-approvals).

1. Una vez aprobado el contenido, haga clic en el botón **[!UICONTROL Preparar]** para preparar el objetivo de la entrega. El sistema prepara la audiencia y los criterios de segmentación.

1. Haga clic en el botón **[!UICONTROL Enviar destino]**. Los revisores designados pueden aprobarlo o rechazarlo. Consulte esta [sección](#approve-reject).

   ![Captura de pantalla que muestra el botón Enviar destino](assets/approvals5.png){zoomable="yes"}

   El estado de aprobación cambia a pending. Consulte esta [sección](#rack-approvals).

1. Una vez aprobado el objetivo, la preparación se reanuda y se puede realizar el envío.

>[!NOTE]
>Si se rechaza una aprobación, el propietario de la entrega debe realizar todos los cambios necesarios en el contenido o el destino según los comentarios del revisor y volver a enviar para su aprobación.

## Aprobar o rechazar {#approve-reject}

Los revisores designados pueden aprobar o rechazar el contenido y los envíos de destino. Consulte esta [sección](#submit-approval).

>[!NOTE]
>Para que se envíe la notificación por correo electrónico, la dirección del revisor debe configurarse en la instancia de.

1. Cuando reciba el correo electrónico de notificación, abra la entrega que requiera aprobación directamente desde la interfaz de usuario web.

1. Revise el contenido o la información de destino.

1. Haga clic en el botón **[!UICONTROL Aprobar contenido]** o **[!UICONTROL Aprobar destino]**.

   ![Captura de pantalla que muestra el botón Aprobar contenido en el panel de envío](assets/approvals3.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Aprobar]** o **[!UICONTROL Rechazar]**.

1. Opcionalmente, agregue **[!UICONTROL Comment]** para explicar su decisión.

   ![Captura de pantalla que muestra el diálogo de aprobación con los botones Aprobar, Rechazar y el campo Comentario](assets/approvals4.png){zoomable="yes"}

1. Confirme su decisión. El estado de aprobación se actualiza inmediatamente en el panel de envío. Consulte esta [sección](#rack-approvals).

## Seguimiento del estado de aprobación {#track-approvals}

El estado de aprobación es visible en la sección **[!UICONTROL Propiedades]** del panel de envío. El estado muestra qué aprobaciones están esperando y su estado actual:

![Captura de pantalla que muestra el estado de aprobación](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL En edición]**: el contenido o el destino aún no se ha enviado para su aprobación
* **[!UICONTROL Aprobación pendiente]**: el contenido o el destino está a la espera de revisión
* **[!UICONTROL Aprobado]**: el revisor ha aprobado el contenido o el destino
* **[!UICONTROL Rechazado]**: el revisor ha rechazado el contenido o el destino

La sección de aprobación muestra todas las aprobaciones y actualizaciones habilitadas en tiempo real a medida que los revisores validan o rechazan cada paso.

## Temas relacionados {#related}

* [Creación de campañas](create-campaigns.md)
* [Administración de campañas](manage-campaigns.md)
