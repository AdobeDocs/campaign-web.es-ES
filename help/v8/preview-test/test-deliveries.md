---
audience: end-user
title: Envío de entregas de prueba
description: Obtenga información sobre cómo definir y enviar envíos de prueba
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Beta"
source-git-commit: f5e7f354735416f828d4b0e065cb8c424a9b4fc8
workflow-type: tm+mt
source-wordcount: '1145'
ht-degree: 4%

---

# Envío de entregas de prueba {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Modo de vista previa"
>abstract="Obtenga una vista previa y pruebe el mensaje incluyendo la población de prueba en el público destinatario principal."

Una vez definido el contenido del mensaje, puede previsualizarlo y probarlo enviando envíos de prueba (también conocido como. &#39;proofs&#39;) para probar perfiles. Si ha insertado contenido personalizado, puede comprobar cómo se muestra este en el mensaje con los datos del perfil de prueba.

Para detectar posibles errores en el contenido del mensaje o en la configuración de personalización, envíe mensajes de prueba a perfiles de prueba antes de enviarlos a la audiencia de destino. Se debe enviar un mensaje de prueba cada vez que se realiza un cambio para validar el contenido más reciente. El envío de envíos de prueba (anteriormente conocidos como &quot;pruebas&quot;) es un paso importante para validar la campaña e identificar posibles problemas. Los destinatarios de un mensaje de prueba pueden comprobar varios elementos, como vínculos, vínculos de exclusión, imágenes o páginas espejo, así como detectar cualquier error en la renderización, el contenido, la configuración de personalización y la configuración de envío.

## Seleccione los destinatarios de la prueba {#test-recipients}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Población de prueba"
>abstract="Seleccione un modo de población de prueba."

Según el canal que utilice, los mensajes de prueba se pueden enviar a tres tipos de destinatarios:

* [Perfiles de prueba](#test-profiles) - Enviar **prueba de correos electrónicos y SMS** a las direcciones semilla, que son destinatarios adicionales de la base de datos. Se pueden crear en la variable [!DNL Campaign] consola en la **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Direcciones semilla]** carpeta. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

* [Sustituir del destinatario principal](#substitution-profiles) - Enviar **prueba de correos electrónicos y SMS** a una dirección de correo electrónico o número de teléfono específicos mientras se suplanta a un perfil existente. Esto le permite experimentar el mensaje como lo harían los destinatarios, lo que le ofrece una representación precisa del contenido que recibirá el perfil.

* [Suscriptores](#subscribers) - Enviar **probar notificaciones push** a suscriptores ficticios añadidos a la base de datos. Al igual que los perfiles de prueba, se pueden crear en la variable [!DNL Campaign] consola en la **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Direcciones semilla]** carpeta. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

Para seleccionar los destinatarios de una entrega de prueba, siga los pasos a continuación según el tipo de perfiles que desee utilizar.

### Perfiles de prueba {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Destinatario de la prueba"
>abstract="Puede cargar un segundo archivo como &quot;destino de la prueba&quot;, si desea probar el envío antes de enviarlo al destino principal."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Cargar perfiles"
>abstract="Puede cargar un segundo archivo con perfiles adicionales si desea probar el envío con un conjunto diferente del conjunto utilizado para el destinatario principal."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="Archivo de plantilla"
>abstract="El formato del archivo debe ser el mismo que el del archivo original.<br/>Formatos de archivo compatibles: txt, csv. Tamaño máximo de archivo: 15 MB. Usar la primera línea como encabezado de columna."


Los perfiles de prueba son direcciones semilla que son destinatarios adicionales en la base de datos. Se pueden crear en la variable [!DNL Adobe Campaign] consola de cliente en **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Direcciones semilla]** carpeta. A continuación se detallan los pasos para enviar mensajes de prueba a las direcciones semilla.


1. Vaya a la pantalla de edición de contenido de su envío de correo electrónico o SMS y haga clic en **[!UICONTROL Simular contenido]** botón.

1. Haga clic en **[!UICONTROL Prueba]** botón.

   >[!NOTE]
   >
   >Si ya ha seleccionado perfiles para [previsualización del envío](preview-content.md), aparecen en el panel izquierdo.

   ![](assets/simulate-test-button-email.png)

1. Desde el **[!UICONTROL Modo]** lista desplegable, elija **[!UICONTROL Perfiles de prueba]** para dirigirse a destinatarios ficticios que recibirán el correo electrónico o el SMS de prueba.

   ![](assets/simulate-profile-mode.png)

1. Si ya ha seleccionado perfiles para [previsualización del mensaje](preview-content.md) en la pantalla de simulación de contenido, esos perfiles se preseleccionan como destinatarios de prueba. Puede borrar la selección o agregar destinatarios adicionales mediante el **[!UICONTROL Añadir perfil(es) de prueba]** botón.

   >[!NOTE]
   >
   >De forma predeterminada, la variable **[!UICONTROL Uso de perfiles de prueba]** El modo está seleccionado.

1. Para enviar también el mensaje final a los destinatarios de la entrega de prueba, seleccione la **[!UICONTROL Incluir la población de prueba en el destinatario principal]** opción.

1. Una vez seleccionados los perfiles de prueba, puede [realizar la entrega de prueba](#send-test).

### Perfiles de sustitución {#substitution-profiles}

Para enviar un correo electrónico o SMS de prueba a una dirección de correo electrónico o un número de teléfono específicos mientras se muestran datos de un perfil existente de [!DNL Adobe Campaign] base de datos, utilice perfiles de sustitución, como se detalla a continuación:

1. Antes de enviar una prueba, asegúrese de definir una audiencia objetivo para la entrega. [Más información](../audience/about-recipients.md)

1. Vaya a la pantalla de edición de contenido de su envío de correo electrónico o SMS y haga clic en **[!UICONTROL Simular contenido]** botón.

1. Haga clic en **[!UICONTROL Prueba]** botón.

   ![](assets/simulate-test-button-email.png)

1. Desde el **[!UICONTROL Modo]** lista desplegable, elija **[!UICONTROL Sustituir del destinatario principal]** para enviar una prueba a una dirección de correo electrónico o número de teléfono específicos mientras se muestran los datos de un perfil existente.

   >[!CAUTION]
   >
   >Si no ha seleccionado ningún [audiencia](../audience/about-recipients.md) para su envío, la variable **[!UICONTROL Sustituir del destinatario principal]** Esta opción aparecerá atenuada y no podrá seleccionar perfiles de sustitución.

1. Haga clic en **[!UICONTROL Añadir dirección]** y especifique la dirección de correo electrónico o el número de teléfono que recibirá el envío de prueba.

   ![](assets/simulate-add-substitution-address.png)

   >[!NOTE]
   >
   >Puede introducir cualquier dirección de correo electrónico o número de teléfono. Esto permite enviar envíos de prueba a cualquier destinatario, incluso si no son usuarios de [!DNL Adobe Campaign].

1. Seleccione el perfil del destinatario definido para la entrega que se utilizará como sustituto. También puede permitir que [!DNL Adobe Campaign] seleccione un perfil aleatorio del destinatario. Los datos de perfil del perfil seleccionado se muestran en la entrega de prueba.

1. Confirme el destinatario y repita la operación para añadir tantas direcciones de correo electrónico o números de teléfono como sea necesario.

   ![](assets/simulate-profile-substitute.png)

1. Para enviar también el mensaje final a los destinatarios de la entrega de prueba, seleccione la **[!UICONTROL Incluir la población de prueba en el destinatario principal]** opción.

1. Una vez seleccionados los perfiles de sustitución, puede [realizar la entrega de prueba](#send-test).

### Suscriptores {#subscribers}

Al trabajar con notificaciones push, los envíos de prueba solo se pueden enviar a los suscriptores de la aplicación. Para seleccionarlos, siga los pasos a continuación.

1. Vaya a la pantalla de edición de contenido del envío y haga clic en **[!UICONTROL Simular contenido]** botón.

1. Haga clic en **[!UICONTROL Prueba]** botón.

   ![](assets/simulate-test-button-push.png)

1. Si ya ha seleccionado suscriptores a [previsualización de la entrega](preview-content.md) en la pantalla de simulación de contenido, esos perfiles se preseleccionan como suscriptores de prueba.

   Puede borrar su selección y/o añadir suscriptores adicionales usando el botón dedicado.

   ![](assets/simulate-test-subscribers.png)

1. Para enviar también la notificación push final a los suscriptores de prueba, seleccione la **[!UICONTROL Incluir la población de prueba en el destinatario principal]** opción.

1. Una vez seleccionados los suscriptores, puede [realizar la entrega de prueba](#send-test).

## Realización del envío de prueba {#send-test}

Para realizar la entrega de prueba a los destinatarios seleccionados, siga los pasos a continuación.

1. Haga clic en **[!UICONTROL Enviar prueba]** botón.

1. Confirme el envío.

   ![](assets/simulate-send-test.png)

1. Envíe tantas pruebas como sea necesario hasta que haya finalizado el contenido de su envío.

Una vez finalizado, puede preparar y realizar la entrega al destinatario principal. Descubra cómo en las secciones dedicadas a continuación:

* [Envíe su correo electrónico](../monitor/prepare-send.md)
* [Envío de la notificación push](../push/send-push.md#send-push)
* [Realización de la entrega de SMS](../sms/send-sms.md#send-sms)

## Acceso a envíos de prueba enviados {#access-proofs}

Una vez enviados los envíos de prueba, puede acceder a los registros dedicados desde el **[!UICONTROL Ver registro de prueba]** botón.

Estos registros le permiten acceder a todas las pruebas enviadas para la entrega seleccionado y visualizar estadísticas específicas relacionadas con su entrega. [Obtenga información sobre cómo monitorizar los registros de envío](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

También puede acceder a las pruebas enviadas desde el [lista de envíos](../msg/gs-messages.md), como cualquier envío.

![](assets/simulate-deliveries-list.png)
