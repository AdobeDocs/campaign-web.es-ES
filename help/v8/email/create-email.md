---
audience: end-user
title: Enviar su primer correo electrónico
description: Obtenga información sobre cómo enviar el primer correo electrónico con la interfaz de usuario web de Campaign
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 56%

---


# Creación de su primer correo electrónico {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Empezar con correos electrónicos"
>abstract="Puede crear un envío de correo electrónico independiente o crear un correo electrónico en el contexto de un flujo de trabajo de campaña. Obtenga información sobre cómo crear el envío, seleccionar el público y diseñar el contenido del correo electrónico."

Aprenda a crear su primer correo electrónico de destino. En este caso de uso, se programa el envío de un correo electrónico a los miembros socios plata y oro en una fecha específica.

En función de una [plantilla de diseño](../email/create-email-templates.md) predefinida, el correo electrónico también incluye contenido personalizado basado en atributos de perfil del cliente.

➡️ [Descubra esta funcionalidad en vídeo](#video)

## Creación del envío de correo electrónico {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Selección de una plantilla de correo electrónico"
>abstract="Una plantilla de correo electrónico es una configuración de envío específica que contiene configuraciones predefinidas, como reglas de tipología, parámetros de personalización o enrutamiento. Las plantillas se definen en la consola del cliente de Campaign."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Definición de las propiedades del correo electrónico"
>abstract="Las propiedades son los parámetros de envío comunes que le ayudan a nombrar y clasificar el envío. La configuración adicional es opcional. Si el envío se basa en un esquema ampliado definido en la consola de la versión 8 de Adobe Campaign, algunas **Opciones personalizadas** están disponibles."

Puede crear un envío de correo electrónico independiente o crear un correo electrónico en el contexto de un flujo de trabajo de campaña. Los pasos siguientes detallan el procedimiento para un envío de correo electrónico independiente (único). Obtenga más información acerca de los pasos de creación de entregas en Adobe Campaign en [esta página](../msg/gs-deliveries.md).

Para crear un nuevo envío de correo electrónico independiente, siga los pasos a continuación.

1. Vaya al menú **[!UICONTROL Envíos]** en el carril izquierdo y haga clic en el botón **[!UICONTROL Crear envío]**.

   ![](../msg/assets/create-a-delivery.png)

1. Seleccione **[!UICONTROL Correo electrónico]** como canal y elija una plantilla de envíos de correo electrónico en la lista.

   >[!NOTE]
   >
   >Las plantillas son ajustes de envío preconfigurados que se guardan para utilizarlos en el futuro. [Más información](../msg/delivery-template.md)

   ![](assets/channel-template.png){zoomable="yes"}

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.
1. Introduzca una etiqueta para el envío y configure las opciones adicionales según sus necesidades:

   * **[!UICONTROL Nombre interno]**: asigne un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene la entrega en una carpeta específica.
   * **[!UICONTROL Código de envío]**: utilice este campo para organizar los envíos según sus propias convenciones de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para la entrega.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza del correo electrónico con fines de clasificación.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Si ha ampliado el esquema con campos personalizados específicos, puede acceder a ellos en la sección **[!UICONTROL Opciones personalizadas]**.

   ![](assets/email-properties.png){zoomable="yes"}

1. Además, se puede acceder a la configuración avanzada, como las reglas de tipología y las asignaciones de destino, a través del botón **[!UICONTROL Settings]** ubicado en la parte superior derecha de la pantalla. Estos ajustes están preconfigurados en la plantilla seleccionada, pero se pueden editar según sea necesario para este correo electrónico específico. [Más información](../advanced-settings/delivery-settings.md)

## Definición del público {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Seleccione un público para el envío"
>abstract="Seleccione el mejor público para el mensaje de marketing. Puede elegir un público existente (ya definido en una instancia de la versión 8 de Campaign o Adobe Experience Platform), crear un nuevo público con el modelador de consultas o cargar un archivo que contenga el público. Los grupos de control no están habilitados para la opción **Seleccionar del archivo** y viceversa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html?lang=es" text="Selección de los públicos principales"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=es" text="Establecer un grupo de control"

En este caso de uso, envía el correo electrónico a una audiencia existente.

Encontrará instrucciones adicionales sobre cómo trabajar con públicos en [esta sección](../audience/about-recipients.md).

1. Para seleccionar el público del correo electrónico, haga clic en el botón **[!UICONTROL Seleccionar público]** y elija un público existente en la lista.

   En este ejemplo, queremos utilizar un público existente dirigido a clientes que pertenezcan a los niveles de puntos de lealtad de oro y plata.

   ![](assets/create-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >Las audiencias disponibles en la lista proceden de la instancia de Campaign v8 o de Adobe Experience Platform si se ha configurado la integración de destino y Source en la instancia. Esta integración le permite enviar segmentos de Experience Platform a Adobe Campaign y enviar registros de envío y seguimiento de Campaign a Adobe Experience Platform. Aprenda a trabajar con Campaign y Adobe Experience Platform en la [documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. Una vez seleccionado el público, puede refinar aún más el objetivo mediante la aplicación de reglas adicionales.

   ![](assets/audience-selected.png){zoomable="yes"}

1. También puede establecer un grupo de control para analizar el comportamiento de los destinatarios de correo electrónico en comparación con los que no son los destinatarios. [Aprenda a trabajar con grupos de control](../audience/control-group.md)

## Definición del contenido del correo electrónico {#create-content}

Para empezar a crear el contenido del correo electrónico, siga los pasos a continuación. En este caso de uso, utiliza un correo electrónico predefinido [plantilla de envío](../msg/delivery-template.md) para diseñar su correo electrónico.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. En el panel de envío de correo electrónico, haga clic en el botón **[!UICONTROL Editar contenido]**.

   ![](assets/email-edit-content.png){zoomable="yes"}

   Esto le lleva a una interfaz específica en la que puede configurar el contenido del correo electrónico y acceder al Designer de correo electrónico. [Más información](edit-content.md)

   ![](assets/edit-content.png){zoomable="yes"}

1. Escriba la línea de asunto del correo electrónico y personalícela con el Editor de expresiones. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

   ![](assets/subject-line.png){zoomable="yes"}

1. Para diseñar el contenido del correo electrónico, haga clic en el botón **[!UICONTROL Editar cuerpo del correo electrónico]**.

   Elija el método que desee utilizar para crear el contenido del correo electrónico. En este ejemplo, use [una plantilla de contenido predefinida](create-email-templates.md).

   ![](assets/select-template.png){zoomable="yes"}

1. Una vez seleccionada la plantilla, se mostrará en [Email Designer](create-email-content.md), donde podrá realizar los cambios necesarios y agregar personalización.

   Por ejemplo, para personalizar el título del correo electrónico, seleccione el bloque de componentes y haga clic en **[!UICONTROL Añadir personalización]**.

   ![](assets/add-perso.png){zoomable="yes"}

1. Una vez que esté satisfecho con el contenido, guárdelo y cierre el diseño. Haga clic en **[!UICONTROL Guardar]** para volver a la pantalla de creación del correo electrónico.

   ![](assets/save-content.png){zoomable="yes"}

## Programación del envío {#schedule}

Cuando se realiza una entrega en el contexto de un flujo de trabajo, se debe utilizar la actividad **Planificador**. Obtenga más información en [esta página](../workflows/activities/scheduler.md). Los pasos siguientes solo se aplican a envíos independientes.

1. Vaya a la sección **[!UICONTROL Programar]** de las propiedades de entrega.

1. Utilice la opción **[!UICONTROL Habilitar programación]** para activarla.

1. Establezca la fecha y la hora deseadas para el envío.

   ![](assets/schedule.png){zoomable="yes"}

Una vez realizada la entrega, el envío real comienza en la fecha de contacto definida.

Obtenga más información acerca de la programación de entregas en [esta sección](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## Previsualización de un correo electrónico y envío de pruebas {#preview-test}

Antes de enviar el correo electrónico, puede obtener una vista previa y probarlo para asegurarse de que cumpla con sus expectativas.

En este caso de uso, puede previsualizar el correo electrónico y enviar pruebas a direcciones de correo electrónico específicas al suplantar algunos de los perfiles de destino.

Encontrará información adicional sobre cómo obtener una vista previa de un correo electrónico y enviar pruebas en [esta sección](../preview-test/preview-test.md).

1. Para revisar su correo electrónico, haga clic en **[!UICONTROL Revisar y enviar]**. Se muestra una vista previa del correo electrónico, junto con todas las propiedades, público y programación configuradas. Puede editar cualquiera de estos elementos haciendo clic en el botón modificar.

1. Para obtener una vista previa del correo electrónico y enviar pruebas, haga clic en el botón **[!UICONTROL Simular contenido]**.

   ![](assets/review-email.png){zoomable="yes"}

1. En el lado izquierdo, seleccione los perfiles que desee utilizar para previsualizar el correo electrónico.

   El panel derecho muestra una vista previa del correo electrónico en función del perfil seleccionado. Si ha añadido varios perfiles, puede alternarlos para previsualizar el correo electrónico correspondiente.

   ![](assets/preview.png){zoomable="yes"}

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Para enviar pruebas, haga clic en el botón **[!UICONTROL Enviar pruebas]** y luego elija el modo que desee utilizar.

   En este ejemplo, use el modo **[!UICONTROL Sustituir del destinatario principal]**, que envía pruebas a direcciones de correo electrónico específicas mientras suplanta algunos de los perfiles a los que apunta el correo electrónico.

   ![](assets/proof-mode.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Agregar dirección]** y especifique las direcciones de correo electrónico que recibirán las pruebas.

   Para cada dirección de correo electrónico, seleccione el perfil que desea suplantar. También puede permitir que Adobe Campaign seleccione un perfil aleatorio de destinatario.

   ![](assets/proof-test-profile.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Enviar revisión]** y confirme el envío.

   Las pruebas se envían a las direcciones de correo electrónico especificadas utilizando el perfil seleccionado con el prefijo **[Proof x]**.

   ![](assets/proof-sent.png){zoomable="yes"}

   Puede comprobar el estado del envío y acceder a las pruebas enviadas en cualquier momento haciendo clic en el botón **[!UICONTROL Ver pruebas]** en la pantalla Simular contenido.

## Envío y supervisión del correo electrónico {#prepare-send}

Después de revisar y probar el correo electrónico, puede prepararlo y enviarlo.

1. Para prepararlo, haga clic en **[!UICONTROL Preparación]**. [Aprenda a preparar un correo electrónico](../monitor/prepare-send.md)

   ![](assets/preparation.png){zoomable="yes"}

1. Una vez que el correo electrónico esté listo para enviarse, haga clic en el botón **[!UICONTROL Enviar]** (o **[!UICONTROL Enviar como está programado]** si ha programado su envío) y confirme el envío.

1. Durante el proceso de envío, puede realizar un seguimiento del progreso y ver las estadísticas en tiempo real directamente en esta pantalla.

   ![](assets/sending-email.png){zoomable="yes"}

   <!--
    ![](assets/sent-email.png){zoomable="yes"}-->

   También puede acceder a la información detallada sobre la entrega haciendo clic en el botón **[!UICONTROL Registros]**. [Obtenga información sobre cómo monitorizar los registros de envío](../monitor/delivery-logs.md)

1. Una vez enviado el correo electrónico, puede acceder a los informes específicos para un análisis más detallado haciendo clic en el botón **[!UICONTROL Informes]**.

![](assets/reports.png){zoomable="yes"}

## Vídeos explicativos {#video}

Obtenga información sobre cómo crear un envío de correo electrónico desde cero, definir el público, diseñar el contenido, simular la previsualización y enviar una prueba.

>[!VIDEO](https://video.tv.adobe.com/v/3425866/?quality=12)
