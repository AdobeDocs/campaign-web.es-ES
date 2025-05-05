---
audience: end-user
title: Crear mensajes transaccionales
description: Aprenda a crear un mensaje transaccional en Campaign interfaz web del usuario
exl-id: 74e468f5-d9c3-4470-8ff2-68648b5f396f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1312'
ht-degree: 11%

---

# Crear mensajes transaccionales

En el mensajería transaccional, una evento activa el envío de un mensaje personalizado. Para habilitar esto, cree un plantilla de mensaje para cada tipo de evento. Estas plantillas contienen toda la información necesaria para personalizar el mensaje transaccional.

## Crear un plantilla de mensaje transaccional {#transactional-template}

En Campaign interfaz web de usuario, el primer paso en la configuración del mensajería transaccional es la creación del plantilla o la creación directa del mensaje. Es diferente a [la configuración de los mensajes transaccionales en la consola](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional) del cliente.

Se puede utilizar un plantilla de mensaje transaccional para previsualización el envío contenido recibido por el perfil antes de que llegue al audiencia final. Por ejemplo, un administrador puede configurar las plantillas, preparándolas para que las utilicen los usuarios de marketing.

Para crear una plantilla de mensaje transaccional, siga los pasos a continuación:

* En la sección **[!UICONTROL Mensajes activados]**, vaya a **[!UICONTROL Mensajes transaccionales]**. En la ficha **[!UICONTROL Plantillas]**, puede ver todas las plantillas de envío de los mensajes transaccionales. Haga clic en el botón **[!UICONTROL Crear plantilla de mensaje transaccional]** para comenzar a crear la plantilla.

  ![Captura de pantalla que muestra la sección de plantillas transaccionales en la interfaz de usuario web de Campaign.](assets/transactional-templates.png){zoomable="yes"}

* En la nueva página mostrada, elija el canal de la plantilla. Para este ejemplo, seleccione el canal **[!UICONTROL Correo electrónico]**. También puede trabajar desde otro plantilla de mensajes y seleccionarlo en el lista de plantillas.

  ![Captura de pantalla que muestra la selección de canales para las plantillas de mensajes transaccionales.](assets/transactional-template-channel.png){zoomable="yes"}

  Vuelva a hacer clic en el botón **[!UICONTROL Crear mensaje transaccional]** para validar la creación de la plantilla en el canal seleccionado.

* Acceda a la configuración de la plantilla de mensaje transaccional.

  ![Captura de pantalla que muestra la página de configuración de las plantillas de mensajes transaccionales.](assets/transactional-template-configuration.png){zoomable="yes"}

### Propiedades del mensaje transaccional {#transactional-properties}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_properties"
>title="Propiedades de la mensajería transaccional"
>abstract="Rellene este formulario para configurar las propiedades de la mensajería transaccional."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_email_properties"
>title="Propiedades de correo electrónico de la mensajería transaccional"
>abstract="Complete este formulario para configurar las propiedades del correo electrónico de mensajería transaccional."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_sms_properties"
>title="Propiedades de SMS de la mensajería transaccional"
>abstract="Rellene este formulario para configurar las propiedades del SMS de mensajería transaccional."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_push_properties"
>title="Propiedades de Push de la mensajería transaccional"
>abstract="Rellene este formulario para configurar las propiedades push de la mensajería transaccional."

La sección **[!UICONTROL Propiedades]** de un mensaje transaccional le ayuda a configurar:

* **[!UICONTROL Label]**, que es el nombre mostrado en la lista de mensajes transaccionales. Aclarar para investigación y uso futuro.
* **[!UICONTROL Internal name]**, que es un nombre único que diferencia el mensaje de otros mensajes creados.
* La **[!UICONTROL carpeta]**, donde se crea la plantilla de mensaje transaccional.
* La **[!UICONTROL carpeta de ejecución]**, donde se almacena el mensaje después de la ejecución.
* El **[!UICONTROL código de envío]**, que es un código que ayuda a reconocer el mensaje para la creación de informes, si es necesario.
* La **[!UICONTROL Descripción]**.
* La **[!UICONTROL Naturaleza]**, que es la naturaleza de su entrega, como se muestra en la enumeración *deliveryNature*. [Más información sobre las enumeraciones](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings#enumerations).

![Captura de pantalla que muestra la sección de propiedades de una plantilla de mensaje transaccional.](assets/template-properties.png){zoomable="yes"}

### Aplicación móvil {#mobile-app}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_mobileapp"
>title="Aplicación móvil de mensajería transaccional"
>abstract="En esta sección, puede seleccionar la aplicación en la que desea insertar el mensaje."

En esta sección, seleccione la aplicación en la que desea insertar el mensaje.

Al hacer clic en el icono búsqueda, acceda a la lista de aplicaciones móviles en su Adobe Campaign instancia.

![Captura de pantalla que muestra la selección de aplicaciones móviles para mensajes transaccionales.](assets/transactional-mobileapp.png){zoomable="yes"}

### Muestra de contexto {#context-sample}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_context"
>title="Contexto de la mensajería transaccional"
>abstract="La muestra de contexto le permite crear un evento de prueba para obtener una vista previa del mensaje transaccional recibido con la personalización del perfil."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_addcontext"
>title="Contexto de la mensajería transaccional"
>abstract="La muestra de contexto le permite crear un evento de prueba para obtener una vista previa del mensaje transaccional recibido con la personalización del perfil."

La muestra de contexto le permite crear un evento de prueba para obtener una vista previa del mensaje transaccional recibido con la personalización del perfil.

Este paso es opcional. Puede utilizar la plantilla sin el ejemplo de contexto, pero el inconveniente es que no puede obtener una vista previa del contenido personalizado.

En el ejemplo de configuración de la contraseña, el evento envía el nombre, los apellidos y un vínculo personalizado del usuario para restablecer su contraseña. El contexto se puede configurar como se muestra a continuación.

El contenido del contexto depende de la personalización que necesite.

![Captura de pantalla que muestra la configuración de muestra de contexto para los mensajes transaccionales.](assets/transactional-context.png){zoomable="yes"}

### Contenido de la plantilla de mensaje transaccional {#transactional-content}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_content"
>title="Contenido de la mensajería transaccional"
>abstract="Aprenda a crear el contenido de mensajería transaccional."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_personalization"
>title="Personalización de la mensajería transaccional"
>abstract="Aprenda a personalizar el mensajería transaccional contenido."

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_event_context"
>title="Contexto del evento"
>abstract="Este menú proporciona variables del evento activador que puede aprovechar para personalizar el contenido del mensaje transaccional."

Trabajar el contenido de una mensaje transaccional es similar a la creación contenido de una envío. Haga clic en **[!UICONTROL Abrir correo electrónico diseñador]** o **[!UICONTROL Editar correo electrónico cuerpo]** y seleccione una plantilla contenido o importe su código HTML.

![Captura de pantalla que muestra la creación contenido para mensaje transaccional plantillas.](assets/template-content.png){zoomable="yes"}

Para agregar personalización al contenido, haga clic en la sección donde desea agregarlo y elija el **[!UICONTROL icono de añadir Personalización]** .

![Captura de pantalla que muestra el icono personalización en el editor contenido.](assets/template-perso.png){zoomable="yes"}

Acceda a la ventana de **personalización de Editar**&#x200B;[!UICONTROL . Para agregar variables desde el evento activador, haga clic en el icono de contexto &#x200B;]&#x200B;**Evento**. Navegue por el contexto que definió para su plantilla ([obtenga más información sobre el contexto](#context-sample)) y haga clic en el **[!UICONTROL botón +]** para insertar el variable requerido.

La siguiente imagen muestra cómo añadir personalización para el nombre.

![Captura de pantalla que muestra el agregado de personalización para el nombre.](assets/template-firstname.png){zoomable="yes"}

En este ejemplo, agrega el nombre y los apellidos y personaliza el vínculo de botón **[!UICONTROL Restablecer la contraseña]**.

![Captura de pantalla que muestra la personalización del botón Restablecer contraseña.](assets/template-button.png){zoomable="yes"}

### Previsualice la plantilla

En esta fase de la creación de la plantilla, previsualice el contenido de la plantilla y compruebe la personalización.

Para ello, rellene el ejemplo de [contexto y haga clic en el **[[!UICONTROL botón]](#context-sample) Simular contenido]**.

![Captura de pantalla que muestra la vista previa de la plantilla de mensaje transaccional.](assets/template-preview.png){zoomable="yes"}

## Creación de un mensaje transaccional {#transactional-message}

Puede crear un mensaje transaccional directamente o mediante una plantilla de mensaje transaccional. [Aprenda a crear una plantilla de mensaje transaccional](#transactional-template).

Para crear un mensaje transaccional, siga los pasos a continuación:

* En la sección **[!UICONTROL Mensajes activados]**, vaya a **[!UICONTROL Mensajes transaccionales]**. En la pestaña **[!UICONTROL Examinar]**, puedes ver todos los mensajes transaccionales creados. Haga clic en el botón **[!UICONTROL Crear mensaje transaccional]** para comenzar a crear su mensaje.

  ![Captura de pantalla que muestra la sección de exploración para mensajes transaccionales.](assets/transactional-browse.png){zoomable="yes"}

* En la nueva página mostrada, elija el canal del mensaje y seleccione la plantilla con la que desee trabajar. En este ejemplo, elija [la plantilla creada anteriormente](#transactional-template).

  ![Captura de pantalla que muestra la selección de canal para los mensajes transaccionales.](assets/transactional-channel.png){zoomable="yes"}

  Vuelva a hacer clic en el botón **[!UICONTROL Crear mensaje transaccional]** para validar la creación del mensaje en el canal seleccionado.

* Acceda a la configuración de su mensaje transaccional. El mensaje hereda la configuración de la plantilla. Esta página es casi idéntica a la página de configuración de la plantilla de mensaje transaccional, excepto que también incluye la configuración de tipo de evento.

  ![Captura de pantalla que muestra la página de configuración de los mensajes transaccionales.](assets/transactional-configuration.png){zoomable="yes"}

  Rellene la configuración del mensaje como para una plantilla:
   * [Propiedades del mensaje transaccional](#transactional-properties)
   * [Muestra de contexto](#context-sample)
   * [Contenido del mensaje](#transactional-content)
y [configure el tipo de evento](#event-type) como se detalla a continuación.

* Después de [validar tu mensaje transaccional](validate-transactional.md), haz clic en el botón **[!UICONTROL Revisar y publicar]** para crear y publicar tu mensaje. Los déclencheur ahora pueden insertar el envío del mensaje transaccional.

### Acerca del tipo de evento {#event-type}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_event"
>title="Evento de mensajería transaccional"
>abstract="La configuración del tipo de evento vincula el mensaje al evento de déclencheur."

La configuración del tipo de evento vincula el mensaje al evento de déclencheur.

En la interfaz de usuario web de Campaign, seleccione un tipo de evento ya creado o cree el tipo de evento directamente en esta página de configuración.

![Captura de pantalla que muestra la configuración del tipo de evento para los mensajes transaccionales.](assets/transactional-event-type.png){zoomable="yes"}

>[!CAUTION]
>
>Si selecciona un tipo de evento que esté utilizando otro mensaje transaccional, almacenará en déclencheur ambos mensajes. Para obtener prácticas recomendadas, **vincule UN tipo de evento a UN solo mensaje transaccional.**

## Añadir ofertas a los mensajes transaccionales {#transactional-offers}

Puede incluir ofertas en los mensajes transaccionales, lo que le permite presentar propuestas relevantes a los usuarios finales, incluso cuando el mensaje se activa por evento.

Se puede acceder a esta función durante la fase de edición de contenido del mensaje transaccional. Haga clic en el botón **[!UICONTROL Configurar ofertas]** para configurarlo.

El proceso de configuración es idéntico al de configuración de ofertas para envíos estándar. [Aprenda a agregar ofertas a su mensaje](../msg/offers.md).

![Captura de pantalla que muestra la configuración de ofertas en mensajes transaccionales.](assets/transactional-offers.png){zoomable="yes"}