---
audience: end-user
title: Enviar su primer correo electrónico
description: Obtenga información sobre cómo enviar su primer correo electrónico con la IU de la web de Campaign
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
badge: label="Beta"
source-git-commit: 883463ef70bfd908ae0ec66863fa61ec2334442b
workflow-type: tm+mt
source-wordcount: '1350'
ht-degree: 62%

---


# Enviar su primer correo electrónico {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_card2"
>title="Generación de IA para contenido de correo electrónico"
>abstract="Nuestra tecnología de IA general utiliza algoritmos avanzados para generar contenido altamente atractivo y personalizado. Aumente las tasas de apertura, las tasas de clics y las conversiones con la generación inteligente de contenido de Gen AI. Manténgase a la cabeza de la competencia y eleve su juego de marketing por correo electrónico con Gen AI en el contenido del correo electrónico."

Aprenda a crear su primer correo electrónico de destino. En este caso de uso, se programa el envío de un correo electrónico a los miembros socios plata y oro en una fecha específica.

Basado en un [plantilla de diseño](../content/email-templates.md), el correo electrónico también incluye contenido personalizado basado en atributos de perfil del cliente.

## Creación de la entrega de correo electrónico {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Selección de una plantilla de correo electrónico"
>abstract="Una plantilla de correo electrónico es una configuración de envío específica que contiene configuraciones predefinidas, como reglas de tipología, parámetros de personalización o enrutamiento. Las plantillas se definen en la consola del cliente de Campaign."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Defina las propiedades de correo electrónico"
>abstract="Las propiedades son los parámetros de envío comunes que le ayudan a nombrar y clasificar el envío. La configuración adicional es opcional. Si el envío se basa en un esquema ampliado definido en la consola de la versión 8 de Adobe Campaign, algunas **Opciones personalizadas** están disponibles."

Puede crear una entrega de correo electrónico independiente o crear un correo electrónico en el contexto de un flujo de trabajo de la campaña. Los pasos siguientes detallan el procedimiento para un envío de correo electrónico independiente (único). Si está trabajando en el contexto de un flujo de trabajo de campaña, los pasos de creación se detallan en [esta sección](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Para crear un nuevo envío de correo electrónico independiente, siga los pasos a continuación.

1. Vaya a la **[!UICONTROL Envíos]** en el carril izquierdo y haga clic en el botón  **[!UICONTROL Creación de envíos]** botón.

   ![](assets/delivery-list.png)

1. Seleccionar **[!UICONTROL Correo electrónico]** como canal y seleccione una plantilla de envíos de correo electrónico de la lista.

   >[!NOTE]
   >
   >Las plantillas son ajustes de envío preconfigurados que se guardan para utilizarlos en el futuro. [Más información](../msg/delivery-template.md)

   ![](assets/channel-template.png)

1. Haga clic en el botón **[!UICONTROL Crear envío]** para confirmar.
1. Introduzca una etiqueta para el envío y configure las opciones adicionales según sus necesidades:

   * **[!UICONTROL Nombre interno]**: asigne un identificador único a la entrega.
   * **[!UICONTROL Carpeta]**: almacene la entrega en una carpeta específica.
   * **[!UICONTROL Código de envío]**: utilice este campo para organizar los envíos en función de su propia convención de nombres.
   * **[!UICONTROL Descripción]**: especifique una descripción para la entrega.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza del correo electrónico con fines de clasificación.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Si ha ampliado el esquema con campos personalizados específicos, puede acceder a ellos en la sección **[!UICONTROL Opciones personalizadas]**.

   ![](assets/email-properties.png)

1. Además, se puede acceder a la configuración avanzada, como reglas de tipología y asignaciones de destino, a través del **[!UICONTROL Configuración]** situado en la parte superior derecha de la pantalla. Estos ajustes están preconfigurados en la plantilla seleccionada, pero se pueden editar según sea necesario para este correo electrónico específico.

## Definición de la audiencia {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Seleccione una audiencia para el envío"
>abstract="Seleccione la mejor audiencia para el mensaje de marketing. Puede elegir una audiencia existente (ya definida en una instancia de Campaign v8 o de Adobe Experience Platform), crear una nueva audiencia con el generador de reglas o cargar un archivo que contenga la audiencia. Los grupos de control no están habilitados para **Seleccionar del archivo** y viceversa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html" text="Audiencias de destino"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/control-group.html" text="Establecer un grupo de control"

En este caso de uso, envíe el correo electrónico a una audiencia existente.

Encontrará instrucciones adicionales sobre cómo trabajar con audiencias en [esta sección](../audience/about-audiences.md).

1. Para seleccionar la audiencia del correo electrónico, haga clic en el botón **[!UICONTROL Seleccionar audiencia]** y elija una audiencia existente en la lista.

   En este ejemplo, queremos utilizar una audiencia existente dirigida a clientes que pertenezcan a los niveles de puntos de lealtad de oro y plata.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Las audiencias disponibles en la lista proceden de la instancia de Campaign v8 o de Adobe Experience Platform si se ha configurado la integración destino/origen en la instancia. Esta integración le permite enviar segmentos de Experience Platform a Adobe Campaign y enviar registros de envío y seguimiento de Campaign a Adobe Experience Platform. Descubra cómo trabajar con Campaign y Adobe Experience Platform en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. Una vez seleccionada la audiencia, puede refinar aún más el objetivo mediante la aplicación de reglas adicionales.

   ![](assets/audience-selected.png)

1. También puede establecer un grupo de control para analizar el comportamiento de los destinatarios de correo electrónico en comparación con los que no son los destinatarios. [Aprenda a trabajar con grupos de control](../audience/control-group.md)

## Definición del contenido del correo electrónico {#create-content}

Para empezar a crear el contenido del correo electrónico, siga los pasos a continuación. En este caso de uso, se utiliza un correo electrónico predefinido [plantilla de envíos](../msg/delivery-template.md) para diseñar el correo electrónico.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../content/edit-content.md).-->

1. En el panel de envío de correo electrónico, haga clic en **[!UICONTROL Editar contenido]** botón.

   ![](assets/email-edit-content.png)

   Esto le lleva a una interfaz dedicada en la que puede configurar el contenido del correo electrónico y acceder al Diseñador de correo electrónico. [Más información](../content/edit-content.md)

   ![](assets/edit-content.png)

1. Escriba la línea de asunto del correo electrónico y personalícela con el Editor de expresiones. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Para diseñar el contenido del correo electrónico, haga clic en el botón **[!UICONTROL Editar cuerpo del correo electrónico]**.

   Elija el método que desee utilizar para crear el contenido del correo electrónico. En este ejemplo, utilice un [plantilla de contenido predefinida](../msg/delivery-template.md).

   ![](assets/select-template.png)

1. Una vez seleccionada la plantilla, se muestra en el [Diseñador de correo electrónico](../content/create-email-content.md), donde puede realizar las ediciones necesarias y agregar personalización.

   Por ejemplo, para personalizar el título del correo electrónico, seleccione el bloque de componentes y haga clic en **[!UICONTROL Añadir personalización]**.

   ![](assets/add-perso.png)

1. Una vez que esté satisfecho con el contenido, guárdelo y cierre el diseño. Haga clic en **[!UICONTROL Guardar]** para volver a la pantalla de creación del correo electrónico.

   ![](assets/save-content.png)

## Programación del envío {#schedule}

Para programar el envío del correo electrónico, siga los pasos a continuación.

Las instrucciones adicionales sobre cómo programar la entrega de envíos se detallan en [esta sección](../msg/gs-messages.md#gs-schedule).

1. Vaya a la **[!UICONTROL Programación]** sección.

1. Utilice el **[!UICONTROL Habilitar programación]** para activarlo.

1. Establezca la fecha y la hora deseadas para el envío.

   ![](assets/schedule.png)

Una vez que realice esto, el envío real comenzará en la fecha de contacto que haya definido.

## Vista previa y prueba del correo electrónico {#preview-test}

Antes de enviar el correo electrónico, puede obtener una vista previa y probarlo para asegurarse de que cumpla con sus expectativas.

En este caso de uso, se obtiene una vista previa del correo electrónico y se envían versiones de prueba a direcciones de correo electrónico específicas para suplantar algunos de los perfiles de destino.

Encontrará información adicional sobre cómo previsualizar y probar correos electrónicos en [esta sección](../preview-test/preview-test.md).

1. Para revisar su correo electrónico, haga clic en **[!UICONTROL Revisar y enviar]**. Se muestra una vista previa del correo electrónico, junto con todas las propiedades, audiencia y programación configuradas. Puede editar cualquiera de estos elementos haciendo clic en el botón modificar.

1. Para obtener una vista previa del correo electrónico y enviar versiones de prueba, haga clic en el botón **[!UICONTROL Simular contenido]**.

   ![](assets/review-email.png)

1. En el lado izquierdo, seleccione los perfiles que desee utilizar para previsualizar el correo electrónico.

   El panel derecho muestra una vista previa del correo electrónico en función del perfil seleccionado. Si ha añadido varios perfiles, puede alternarlos para previsualizar el correo electrónico correspondiente.

   ![](assets/preview.png)

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Para enviar versiones de prueba de su correo electrónico, haga clic en el botón **[!UICONTROL Prueba]**, y a continuación, seleccione el modo que desee utilizar.

   En este ejemplo, utilice el modo **[!UICONTROL Sustituir desde el destinatario principal]**, que envía versiones de prueba a direcciones de correo electrónico específicas al suplantar algunos de los perfiles a los que se dirige el correo electrónico.

   ![](assets/proof-mode.png)

1. Haga clic en **[!UICONTROL Añadir dirección]** y especifique las direcciones de correo electrónico que recibirán las versiones de prueba.

   Para cada dirección de correo electrónico, seleccione el perfil que desea suplantar. También puede permitir que Adobe Campaign seleccione un perfil aleatorio de destinatario.

   ![](assets/proof-test-profile.png)

1. Haga clic en **[!UICONTROL Enviar correo electrónico de prueba]** y confirme el envío.

   Las versiones de prueba se envían a las direcciones de correo electrónico especificadas mediante el perfil seleccionado con el prefijo **[Prueba x]**.

   ![](assets/proof-sent.png)

   Puede comprobar el estado del envío y acceder a los correos electrónicos de prueba enviados en cualquier momento haciendo clic en el botón **[!UICONTROL Ver registro de correos electrónicos de prueba]** en la pantalla Simular contenido.

## Envío y supervisión del correo electrónico {#prepare-send}

Después de revisar y probar el correo electrónico, puede prepararlo y enviarlo.

1. Para prepararlo, haga clic en **[!UICONTROL Preparación]**. [Aprenda a preparar un correo electrónico](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Una vez que el correo electrónico esté listo para enviarse, haga clic en el botón **[!UICONTROL Enviar]** (o **[!UICONTROL Enviar como está programado]** si ha programado su envío) y confirme el envío.

1. Durante el proceso de envío, puede realizar un seguimiento del progreso y ver las estadísticas en tiempo real directamente en esta pantalla.

   ![](assets/sent-mail.png)

   También puede acceder a la información detallada sobre la entrega haciendo clic en el botón **[!UICONTROL Registros]**. [Obtenga información sobre cómo monitorizar los registros de envío](../monitor/delivery-logs.md)

1. Una vez enviado el correo electrónico, puede acceder a los informes específicos para un análisis más detallado haciendo clic en el botón **[!UICONTROL Informes]**.

![](assets/reports.png)
