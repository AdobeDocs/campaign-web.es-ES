---
audience: end-user
title: Seguimiento de mensajes
description: Aprenda a añadir vínculos y rastrear mensajes enviados
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
badge: label="Alpha" type="Informative"
source-git-commit: 15c37b0651b1d15dd80571c504aaca59d848b619
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---

# Adición de vínculos y seguimiento de mensajes {#tracking}

Utilice el Diseñador de correo electrónico para añadir vínculos al contenido y realizar un seguimiento de los mensajes enviados para controlar el comportamiento de los destinatarios.

## Insertar vínculos {#insert-links}

Al diseñar un mensaje, puede agregar vínculos al contenido.

>[!NOTE]
>
>Cuando el seguimiento está habilitado, se realiza el seguimiento de todos los vínculos incluidos en el contenido del mensaje.

Para insertar vínculos en el contenido del correo electrónico, siga los pasos a continuación:

1. Seleccione un elemento y haga clic en **[!UICONTROL Insertar vínculo]** de la barra de herramientas contextual.

   ![](assets/message-tracking-insert-link.png)

1. Agregue un **[!UICONTROL Etiqueta]** y **[!UICONTROL Vínculo]**.

1. Guarde los cambios.

1. Una vez creado el vínculo, puede modificarlo desde el **[!UICONTROL Configuración de componentes]** a la derecha.

   * Puede editar el vínculo y cambiar su **[!UICONTROL Target]**.
   * Puede elegir subrayar el vínculo o no marcando la opción correspondiente.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>Los mensajes de correo electrónico de tipo de marketing deben incluir un vínculo de no participación, que no es necesario para los mensajes transaccionales. La categoría del mensaje (**[!UICONTROL Marketing]** o **[!UICONTROL Transaccional]**) se define en el nivel de superficie del canal (es decir, en el valor preestablecido de mensaje) y al crear el mensaje.

Se debe añadir un vínculo específico a la página espejo en todos los mensajes de correo electrónico. Obtenga más información sobre la página espejo en [esta sección](mirror-page.md).

## Administrar seguimiento {#manage-tracking}

La variable [Diseñador de correo electrónico](create-email-content.md) le permite administrar las direcciones URL rastreadas, como editar el tipo de seguimiento para cada vínculo.

1. Haga clic en el **[!UICONTROL Vínculos]** del panel izquierdo para mostrar la lista de todas las direcciones URL del contenido que se va a rastrear.

   Esta lista permite tener una vista centralizada y localizar cada URL en el contenido del correo electrónico.

1. Para editar un vínculo, haga clic en el icono de lápiz correspondiente.

   ![](assets/message-tracking-edit-links.png)

1. Puede modificar el **[!UICONTROL Tipo de seguimiento]** si es necesario:

   ![](assets/message-tracking-edit-a-link.png)

   Para cada URL rastreada, puede establecer el modo de seguimiento en uno de estos valores:

   * **[!UICONTROL Seguimiento]**: Activa el seguimiento en esta dirección URL.
   * **[!UICONTROL Exclusión]**: Considera esta URL como una URL de exclusión o de baja.
   * **[!UICONTROL Página espejo]**: Considera que esta URL es una URL de página espejo.
   * **[!UICONTROL Nunca]**: Nunca activa el seguimiento de esta dirección URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Agregue un **[!UICONTROL Categoría]** al vínculo para agrupar los vínculos rastreados y hacer clic en **[!UICONTROL Guardar]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. Después de realizar la entrega, acceda al informe de entrega. En el **[!UICONTROL Seguimiento]** , el **[!UICONTROL URL y flujos de clics]** muestra las direcciones URL de su envío más visitadas. [Más información](../reporting/reports.md)
