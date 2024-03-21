---
audience: end-user
title: Uso de una actividad de flujo de trabajo de envío
description: Obtenga información sobre cómo añadir una actividad de flujo de trabajo de entrega (correo electrónico, push, SMS, correo directo)
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: 6df7a483ea178abade4bb15256dbd120d556085e
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 51%

---

# Actividades de correo electrónico, SMS, push, correo directo {#channel}

Adobe Campaign Web le permite automatizar y ejecutar campañas de marketing por correo electrónico, SMS, correo directo y canales push. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que puedan activar acciones basadas en el comportamiento y los datos del cliente.

Por ejemplo, puede crear una campaña de correo electrónico de bienvenida que incluya una serie de mensajes en diferentes canales, como correo electrónico, SMS, push y correo directo. También puede enviar un correo electrónico de seguimiento a los clientes después de que hayan completado una compra o enviarles un mensaje de cumpleaños personalizado a través de SMS.

Mediante las actividades del canal, puede crear campañas completas y personalizadas que atraigan a los clientes en varios touchpoints e impulsen las conversiones.

>[!NOTE]
>
>También puede crear una entrega con una sola toma, fuera del contexto de un flujo de trabajo de la campaña. Obtenga más información en estas secciones:
>* [Creación de envíos de correo electrónico independientes](../../email/create-email.md)
>* [Creación de envíos de SMS independientes](../../sms/create-sms.md)
>* [Crear envío push independiente](../../push/create-push.md)
>* [Creación de envíos de correo directo independientes](../../direct-mail/create-direct-mail.md)

## Requisitos previos {#channel-activity-prereq}

Comience a crear su flujo de trabajo con las actividades relevantes:

* Antes de insertar una actividad de canal, debe definir la audiencia. La audiencia es el destinatario principal del envío: los perfiles que reciben los mensajes. Al enviar mensajes en el contexto de un flujo de trabajo de campaña, la audiencia del mensaje no se define en la actividad del canal, sino dentro de una actividad dedicada, como:

   * A **Crear audiencia** actividad. [Más información](build-audience.md).

     ![](../../msg/assets/add-delivery-in-wf.png)

   * A **Cargar archivo** actividad seguida de un **Reconciliación** actividad. [Más información](load-file.md).

     ![](../assets/workflow-reconciliation-criteria.png)

* Para realizar una entrega recurrente, inicie el flujo de trabajo con una **Planificador** actividad. También puede utilizar un **Planificador** actividad para envíos únicos de una sola toma para establecer la fecha de contacto de ese envío. Esa fecha de contacto también se puede establecer en la configuración de envío. Consulte [esta sección](scheduler.md).

## Configuración de la actividad de canal {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="Actividad de correo electrónico"
>abstract="La actividad Correo electrónico facilita el envío de correos electrónicos dentro del flujo de trabajo, lo que permite mensajes únicos y recurrentes. Sirve para automatizar el proceso de envío de correos electrónicos a un destinatario calculado dentro del mismo flujo de trabajo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que puedan activar acciones basadas en el comportamiento y los datos del cliente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="Actividad de SMS"
>abstract="La actividad de SMS facilita el envío de SMS dentro del flujo de trabajo, lo que permite mensajes únicos y recurrentes. Sirve para automatizar el proceso de envío de SMS a un destinatario calculado dentro del mismo flujo de trabajo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que puedan activar acciones basadas en el comportamiento y los datos del cliente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Actividad de push iOS"
>abstract="La actividad Push de iOS optimiza el proceso de envío de notificaciones Push de iOS como parte del flujo de trabajo. Permite la entrega de mensajes recurrentes y únicos, lo que automatiza el envío de notificaciones Push de iOS a un destino predefinido dentro del mismo flujo de trabajo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que puedan activar acciones basadas en el comportamiento y los datos del cliente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Actividad de mensajería push de Android"
>abstract="La actividad Push de Android optimiza el proceso de envío de notificaciones Push de Android como parte del flujo de trabajo. Permite enviar mensajes recurrentes y únicos, lo que automatiza el envío de notificaciones Push de Android a un destino predefinido dentro del mismo flujo de trabajo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que puedan activar acciones basadas en el comportamiento y los datos del cliente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="Actividad de correo directo"
>abstract="La actividad de correo postal facilita el envío de correo postal dentro del flujo de trabajo, lo que permite mensajes únicos y recurrentes. Sirve para automatizar el proceso de generación del archivo de extracción requerido por los proveedores de correo postal. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que puedan activar acciones basadas en el comportamiento y los datos del cliente."

Para configurar una entrega en el contexto de un flujo de trabajo, siga los pasos a continuación:

1. Añada una actividad de canal: **[!UICONTROL Correo electrónico]**, **[!UICONTROL SMS]**, **[!UICONTROL Notificación push (Android)]**, **[!UICONTROL Notificación push (iOS)]** o **[!UICONTROL Correo directo]**.

1. Seleccione el **Tipo de envío**: único o recurrente.

   * A **Entrega única** es una entrega de una sola toma que se envía una sola vez, por ejemplo, un correo electrónico de Black Friday.
   * A **Envío recurrente** se envía varias veces en función de su frecuencia de ejecución definida en una [actividad del planificador](scheduler.md). Cada vez que se ejecuta el flujo de trabajo, la audiencia se recalcula y la entrega se envía a la audiencia actualizada, con el contenido actualizado. Puede ser un boletín semanal o un correo electrónico de cumpleaños recurrente, por ejemplo.

1. Seleccione una **Plantilla** de envío. Las plantillas son opciones de envío preconfigurados específicos de un canal. Hay disponible una plantilla integrada para cada canal, que se rellena previamente de forma predeterminada. [Más información](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)

   Puede seleccionar la plantilla en el panel izquierdo de configuración de actividad de canal. Si el público seleccionado anteriormente no es compatible con el canal, no se puede seleccionar una plantilla. Para resolver esto, actualice la actividad **Generar público destinatario** para seleccionar un público destinatario con la asignación de destino correcta. Obtenga más información sobre las asignaciones de destino en [esta sección](../../audience/targeting-dimensions.md)

1. Haga clic en **Crear envío**. A continuación, puede definir la configuración del mensaje y el contenido del mismo modo que crea un envío independiente. También puede probar y simular el contenido. [Más información](../../msg/gs-messages.md)

1. Vuelva al flujo de trabajo. Si desea continuar con el flujo de trabajo, cambie el **Generación de una transición saliente** para añadir una transición después de la actividad del canal.

1. Haga clic en **Iniciar** para iniciar el flujo de trabajo.

   De forma predeterminada, el inicio de un flujo de trabajo activa la fase de preparación de mensajes, sin enviarlos inmediatamente.

1. Abra la actividad de canal para confirmar el envío desde el **Revisar y enviar** botón.

1. En el panel de envíos, haga clic en **Enviar**.

## Ejemplos {#cross-channel-workflow-sample}

Este es un ejemplo de flujo de trabajo en canales múltiples con una segmentación y dos envíos. El flujo de trabajo está dirigido a todos los clientes que residen en París y que están interesados en las máquinas de café. Se envía un correo electrónico a los clientes habituales y un SMS a los clientes VIP de esta población.

![](../assets/workflow-channel-example.png)

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->

También puede crear un flujo de trabajo recurrente para enviar un SMS personalizado todos los primeros días del mes a las 20:00 a todos los clientes que viven en París.

![](../assets/workflow-channel-example2.png)

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
