---
audience: end-user
title: Uso de una actividad de flujo de trabajo de envío
description: Obtenga información sobre cómo añadir una actividad de flujo de trabajo de entrega (correo electrónico, push, SMS, correo directo)
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 40%

---

# Actividades de correo electrónico, SMS, push, correo directo {#channel}

Adobe Campaign Web le permite automatizar y ejecutar campañas de marketing por correo electrónico, SMS, correo directo y canales push. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que desencadenan acciones basadas en el comportamiento y los datos del cliente.

Por ejemplo, cree una campaña de correo electrónico de bienvenida que incluya una serie de mensajes en diferentes canales, como correo electrónico, SMS, push y correo directo. También puede enviar un correo electrónico de seguimiento después de que un cliente complete una compra o enviar un mensaje de cumpleaños personalizado a un cliente a través de SMS.

Mediante actividades de canal, cree campañas completas y personalizadas que involucren a los clientes en varios puntos de contacto e impulsen las conversiones.

>[!NOTE]
>
>También puede crear una entrega de una sola toma fuera del contexto de un flujo de trabajo de la campaña. Obtenga más información en estas secciones:
>* [Crear envío de correo electrónico independiente](../../email/create-email.md)
>* [Crear envío de SMS independiente](../../sms/create-sms.md)
>* [Crear envío push independiente](../../push/create-push.md)
>* [Crear envío de correo postal independiente](../../direct-mail/create-direct-mail.md)

## Requisitos previos {#channel-activity-prereq}

Comience a crear su flujo de trabajo con las actividades relevantes:

* Antes de insertar una actividad de canal, defina la audiencia. La audiencia es el destinatario principal del envío: los perfiles que reciben los mensajes. Al enviar mensajes en el contexto de un flujo de trabajo de campaña, la audiencia del mensaje no se define en la actividad del canal sino dentro de una actividad dedicada, como:

   * Una actividad **Generar audiencia**. [Más información](build-audience.md).

     ![Captura de pantalla que muestra la adición de una entrega en un flujo de trabajo](../../msg/assets/add-delivery-in-wf.png)

   * Una actividad **Load file** seguida de una actividad **Reconciliation**. [Más información](load-file.md).

     ![Captura de pantalla que muestra los criterios de reconciliación](../assets/workflow-reconciliation-criteria.png) del flujo de trabajo

* Para realizar una entrega recurrente, inicie el flujo de trabajo con una actividad **Scheduler**. Utilice una actividad **Scheduler** para realizar envíos únicos con una sola toma a fin de establecer la fecha de contacto de ese envío. Esa fecha de contacto también se puede establecer en la configuración de envío. Consulte [esta sección](scheduler.md).

## Configuración de la actividad de canal {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="Actividad de Correo electrónico"
>abstract="La actividad Correo electrónico facilita el envío de correos electrónicos dentro del flujo de trabajo, lo que permite mensajes únicos y recurrentes. Automatiza el proceso de envío de correos electrónicos a un destinatario calculado dentro del mismo flujo de trabajo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que desencadenan acciones basadas en el comportamiento y los datos del cliente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="Actividad de SMS"
>abstract="La actividad de SMS facilita el envío de SMS dentro del flujo de trabajo, lo que permite mensajes únicos y recurrentes. Automatiza el proceso de envío de SMS a un destinatario calculado dentro del mismo flujo de trabajo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que desencadenan acciones basadas en el comportamiento y los datos del cliente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="Actividad Push de iOS"
>abstract="La actividad Push de iOS optimiza el proceso de envío de notificaciones Push de iOS como parte del flujo de trabajo. Permite enviar mensajes únicos y recurrentes, automatizando el envío de notificaciones push de iOS a un destinatario predefinido dentro del mismo flujo de trabajo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que desencadenan acciones basadas en el comportamiento y los datos del cliente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Actividad de mensajería Push de Android"
>abstract="La actividad Push de Android optimiza el proceso de envío de notificaciones Push de Android como parte del flujo de trabajo. Permite enviar mensajes únicos y recurrentes, automatizando el envío de notificaciones push de Android a un destinatario predefinido dentro del mismo flujo de trabajo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que desencadenan acciones basadas en el comportamiento y los datos del cliente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="Actividad de correo directo"
>abstract="La actividad de correo directo facilita el envío de correo directo dentro del flujo de trabajo, lo que permite mensajes únicos y recurrentes. Automatiza el proceso de generación del archivo de extracción requerido por los proveedores de correo directo. Puede combinar actividades del canal en el lienzo del flujo de trabajo para crear flujos de trabajo entre canales que desencadenan acciones basadas en el comportamiento y los datos del cliente."

Para configurar una entrega en el contexto de un flujo de trabajo, siga los pasos a continuación:

1. Agregue una actividad de canal: **[!UICONTROL Correo electrónico]**, **[!UICONTROL SMS]**, **[!UICONTROL Notificación push (Android)]**, **[!UICONTROL Notificación push (iOS)]** o **[!UICONTROL Correo directo]**.

1. Seleccione **Tipo de entrega**: individual o recurrente.

   * Una **entrega única** es una entrega con una sola toma que se realiza una sola vez, como un correo electrónico de Black Friday.
   * Se realiza **una entrega recurrente** varias veces según su frecuencia de ejecución definida en una [actividad de planificador](scheduler.md). Cada vez que se ejecuta el flujo de trabajo, la audiencia se vuelve a calcular y se realiza la entrega a la audiencia actualizada con el contenido actualizado. Puede ser un boletín semanal o un correo electrónico de cumpleaños recurrente.

1. Seleccione una **Plantilla** de envío. Las plantillas son ajustes de envío preconfigurados específicos de un canal. Hay disponible una plantilla integrada para cada canal que se rellena previamente de forma predeterminada. [Más información](../../msg/delivery-template.md)

   ![Captura de pantalla que muestra la actividad de envío en un flujo de trabajo](../assets/delivery-activity-in-wf.png)

   Seleccione la plantilla en el panel izquierdo de la configuración de la actividad del canal. Si la audiencia seleccionada anteriormente no es compatible con el canal, no puede seleccionar una plantilla. Para resolver esto, actualice la actividad **Generar público destinatario** para seleccionar un público destinatario con la asignación de destino correcta. Obtenga más información acerca de las asignaciones de destino en [esta sección](../../audience/targeting-dimensions.md).

1. Haga clic en **Crear envío**. Defina la configuración del mensaje y su contenido del mismo modo que crea un envío independiente. Prueba y simulación del contenido. [Más información](../../msg/gs-messages.md)

1. Vuelva al flujo de trabajo. Para continuar con su flujo de trabajo, active la opción **Generar una transición saliente** para agregar una transición después de la actividad del canal.

1. Haga clic en **Iniciar** para iniciar el flujo de trabajo.

   De forma predeterminada, iniciar un flujo de trabajo déclencheur la fase de preparación del mensaje sin enviar inmediatamente el mensaje.

1. Abra la actividad del canal para confirmar el envío desde el botón **Revisar y enviar**.

1. En el panel de control de envíos, haga clic en **Enviar**.

## Ejemplos {#cross-channel-workflow-sample}

Este es un ejemplo de flujo de trabajo en canales múltiples con segmentación y dos envíos. El flujo de trabajo está dirigido a todos los clientes que viven en París y están interesados en las máquinas de café. Entre esta población, se envía un correo electrónico a los clientes normales y un SMS a los clientes de VIP.

![Captura de pantalla que muestra un ejemplo de flujo de trabajo en canales múltiples](../assets/workflow-channel-example.png)

También puede crear un flujo de trabajo recurrente para enviar un SMS personalizado todos los primeros días del mes a las 20:00 a todos los clientes que viven en París.

![Captura de pantalla que muestra un ejemplo de flujo de trabajo recurrente](../assets/workflow-channel-example2.png)

<!--
description, which use case you can perform (common other activities that you can link before or after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending of an email in a workflow. 
-->

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->