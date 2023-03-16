---
audience: end-user
title: Configuración de entrega de correo electrónico
description: Obtenga más información sobre la configuración de envío de correo electrónico en la interfaz de usuario web de Campaign
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 45%

---

# Configuración de entrega de correo electrónico {#email-del-settings}

![Versión alfa](../assets/do-not-localize/badge.png)

Esta configuración es **parámetros técnicos de entrega** que se definen en la plantilla de correo electrónico. Están disponibles en el **Configuración de la entrega** icono disponible al editar una entrega por correo electrónico.

## Configuración de entrega de correo electrónico {#email-delivery-settings}

>[!CAUTION]
>
> Estos ajustes solo se describen para su información. Algunos dependen de la configuración y los permisos. No deben modificarse en esta versión del producto.

## Tipología {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipología"
>abstract="La tipología permite controlar, filtrar y monitorizar los envíos."

Las tipologías son conjuntos de **reglas de tipología** que se ejecutan durante la fase de análisis de mensajes. Le permiten asegurarse de que los mensajes de correo electrónico siempre contengan determinados elementos (como un vínculo de baja o una línea de asunto) o reglas de filtrado para excluir grupos de los destinatarios deseados (como suscriptores que se han dado de baja, competidoras o clientes que no sean fieles).

Al asociar una tipología con un mensaje o una plantilla de mensaje, las reglas de tipología incluidas en la tipología se ejecutan para comprobar la validez del mensaje durante la preparación.

![](assets/delivery-settings-1.png)


### Parámetros de presión {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso del envío"
>abstract="El peso de la entrega le permite identificar las entregas de mayor prioridad dentro del marco de la gestión de presión. Los mensajes con mayor peso son prioritarios."

En esta sección, los parámetros de presión permiten definir una **umbral**. Es el número máximo de mensajes que se pueden enviar a un perfil durante un periodo determinado. Una vez alcanzado este umbral, no se pueden realizar más entregas hasta el final del periodo. Este proceso permite excluir automáticamente un perfil de una entrega si un mensaje supera el umbral establecido, evitando así saturar al destinatario.

Los valores de umbral pueden ser constantes o variables. Esto significa que, para un periodo determinado, los umbrales pueden variar de un perfil a otro o incluso en un mismo perfil.

En el **Tipo de peso** , hay tres opciones disponibles:

* **Constante**
* **Depende del destinatario**
* **Definido en cada regla**

Utilice la variable **Peso de la entrega** para definir la prioridad de entrega. Cada envío tiene un peso que representa su nivel de prioridad. De forma predeterminada, el peso de una entrega se establece en 5. Las reglas de presión permiten definir el peso de los envíos a los que se aplican. El peso puede ser fijo o calcularse mediante una fórmula para adaptarse a los destinatarios. Por ejemplo, puede definir el peso de una entrega en función de los intereses del destinatario.


Utilice la variable **Modo de envío** para seleccionar el modo de evaluación de destino. Hay tres modos disponibles:

* **Estimación de objetivos y personalización de mensajes**
* **Estimación y aprobación del público objetivo provisional**
* **Evaluación del público objetivo**

La gestión de la fatiga viene con la **Campaign Optimization (Optimización de la campaña)** complemento. Obtenga más información sobre las reglas de presión y cómo configurar la gestión de la fatiga en [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=es){target="_blank"}.

### Configuración de capacidad {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importancia del destinatario"
>abstract="La importancia del destinatario es una fórmula que se utiliza para determinar qué destinatarios se mantienen cuando se exceden las reglas de tipología de capacidad."

En esta sección, puede seleccionar una regla de capacidad definida en la consola de Adobe Campaign v8. Esta regla está asociada al canal de correo electrónico.

La variable **importancia del destinatario** field es una fórmula utilizada para determinar qué destinatarios se mantienen cuando se exceden las reglas de tipología de capacidad.

Obtenga más información sobre las reglas de coherencia y capacidad y cómo configurarlas en [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## Audiencia {#audience}

En esta sección, puede seleccionar un **asignación de destino** entre los disponibles. Las asignaciones de destino se definen en la consola Adobe Campaign v8.

Obtenga más información sobre las asignaciones de destino en [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Envío {#delivery}

Los parámetros de envío son configuraciones técnicas que se aplican a su envío.

* **Enrutamiento**: la cuenta externa de enrutamiento de correo electrónico integrada se proporciona de forma predeterminada. Contiene los parámetros técnicos que permiten a la aplicación enviar correos electrónicos.

* **Prueba de entrega SMTP**: esta opción se utiliza para probar el envío a través de SMTP. La entrega se procesa hasta la conexión con el servidor SMTP, pero no se envía. Para cada destinatario de la entrega, Campaign se conecta al servidor del proveedor SMTP, ejecuta el comando RCPT TO del servidor de correo saliente (SMTP) y cierra la conexión antes del comando DATA del SMTP.

* **Email BCC**: esta opción se utiliza para almacenar correos electrónicos en un sistema externo a través de CCO simplemente añadiendo una dirección de correo electrónico CCO al destino del mensaje. Obtenga más información sobre Email BCC en [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### Reintentos {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Número máximo de reintentos"
>abstract="Si un mensaje falla debido a un error temporal, los reintentos se realizan hasta el final de la duración de la entrega."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Obtenga más información sobre la administración de reintentos en [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Aprobación {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modo de aprobación"
>abstract="Cada paso de un envío puede estar sujeto a aprobación para garantizar una monitorización y un control completos de los distintos procesos."

Si se generan advertencias durante la preparación del envío, se puede configurar el envío para definir si se debe ejecutar o no. De forma predeterminada, el usuario debe confirmar la entrega de los mensajes al final de la fase de análisis: esta es la validación **manual**.

Puede seleccionar otro modo de aprobación en el campo correspondiente. Los modos disponibles son:

* **Manual**: al final de la fase de análisis, el usuario debe confirmar la entrega para iniciarlo.

* **Semiautomático**: El envío comienza automáticamente si la fase de análisis no genera mensajes de advertencia.

* **Automático**: El envío comienza automáticamente al final de la fase de análisis, independientemente de su resultado.


## Validez {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Duración del envío"
>abstract="El campo Duración del envío permite introducir el límite de los reintentos de envío global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, solo para los mensajes que devuelven un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Vigencia de recursos"
>abstract="El campo Límite de validez se utiliza para los recursos cargados, principalmente para la página espejo y las imágenes. Los recursos de esta página son válidos durante un tiempo limitado."


El campo **Duración de la entrega** permite introducir el límite de los reintentos de entrega global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, para los mensajes que devuelven solo un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez.

Asimismo, puede especificar fechas. Para ello, seleccione **Establecer explícitamente las fechas de validez**. En este caso, las fechas de entrega y de límite de validez también permiten especificar el tiempo. El tiempo actual se utiliza de forma predeterminada, pero puede modificarse directamente en el campo de entrada.

**Límite de validez de los recursos** se utiliza para los recursos cargados, principalmente para la página espejo y las imágenes. Los recursos de esta página son válidos durante un tiempo limitado (para ahorrar espacio en el disco).

![](assets/delivery-settings-2.png)


Obtenga más información sobre el periodo de validez de la entrega en [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Administración de página espejo {#mirror}

La página espejo es una página HTML accesible en línea mediante un navegador web. Su contenido es idéntico al del correo electrónico. De forma predeterminada, la página espejo se genera si el vínculo se inserta en el contenido del correo.

Además del modo predeterminado, también están disponibles las siguientes opciones:

* **[!UICONTROL Forzar la generación de la página espejo]**: incluso si no se inserta ningún vínculo a la página espejo en la entrega, se crea la página espejo.
* **[!UICONTROL Do not generate the mirror page]**: no se genera ninguna página espejo, aunque el vínculo esté presente en la entrega.
* **[!UICONTROL Generates a mirror page accessible using only the message identifier]**: esta opción permite acceder al contenido de la página duplicada, con información de personalización, en la ventana del “log” de envío. Para ello, tras finalizar la entrega, haga clic en la pestaña **[!UICONTROL Delivery]** y seleccione la línea del destinatario cuya página duplicada desee ver. Haga clic en el vínculo **[!UICONTROL Display the mirror page for this message...]**.


### Seguimiento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Período de validez"
>abstract="Esta opción define la duración durante la cual se activa el seguimiento en las direcciones URL."

Los parámetros de seguimiento se definen en la sección relacionada. Las opciones posibles son:

**Límite de validez de seguimiento**: utilice esta opción para cambiar la duración durante la cual se activa el seguimiento en las direcciones URL.

**URL de sustitución para URL caducadas**: utilice esta opción para introducir una URL a una página web de reserva: se muestra una vez que el seguimiento ha caducado.

## Configuración de la prueba {#test-setttings}

Puede establecer los parámetros de exclusión en esta sección. Las opciones disponibles son:

* **Mantener doble** permite autorizar varios envíos a destinatarios que cumplan varios criterios de objetivo.

* **Mantener direcciones incluida en la lista de bloqueados** permite evitar en el objetivo cualquier perfil que ya no vaya a ser objetivo del envío, como por ejemplo, tras una baja (exclusión).

* **Mantener direcciones en cuarentena** permite evitar que el destinatario tenga perfiles con una dirección que no responde.

También puede personalizar el nombre de los correos electrónicos de prueba.

Utilice la variable **Mantener el código de entrega de la prueba** para asociar al correo electrónico de prueba el mismo código de entrega que el definido para la entrega con el que se relaciona.

De forma predeterminada, el asunto del correo electrónico de prueba lleva el prefijo &quot;PROOF #&quot;, donde # es el número del correo electrónico de prueba. Se puede cambiar este prefijo en el campo **Label prefix**.