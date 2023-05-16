---
audience: end-user
title: Configuración de envío de correos electrónicos
description: Obtenga más información sobre la configuración de envío de correo electrónico en la IU de la web de Campaign
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: ht
source-wordcount: '1473'
ht-degree: 100%

---


# Configuración de envío de correos electrónicos {#email-del-settings}

Esta configuración consiste en los **parámetros técnicos del envío** que se definen en la plantilla de correo electrónico. Están disponibles en el icono **Configuración del envío** al editar un envío por correo electrónico.

## Configuración de envío de correos electrónicos {#email-delivery-settings}

>[!CAUTION]
>
> Esta configuración es solo informativa. Algunos ajustes dependen de la configuración y los permisos. No deben modificarse en esta versión del producto.

## Tipología {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipología"
>abstract="La tipología permite controlar, filtrar y monitorizar la entrega de envíos."

Las tipologías son conjuntos de **reglas de tipología** que se ejecutan durante la fase de análisis de mensajes. Le permiten asegurarse de que los mensajes de correo electrónico siempre contengan determinados elementos (como un vínculo de baja o una línea de asunto) o reglas de filtrado para excluir grupos de los destinatarios deseados (como suscriptores que han cancelado la suscripción, competidoras o clientes que no sean fieles).

Al asociar una tipología a un mensaje o plantilla de mensaje, las reglas de tipología incluidas se ejecutarán para comprobar la validez del mensaje durante su preparación.

![](assets/delivery-settings-1.png)


### Parámetros de presión {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso del envío"
>abstract="El peso del envío le permite identificar los envíos de mayor prioridad dentro del marco de la administración de presión. Los mensajes con mayor peso tienen prioridad."

En esta sección, los parámetros de presión permiten definir un **umbral**. Este es el número máximo de mensajes que se pueden enviar a un perfil durante un período determinado. Una vez alcanzado este umbral, no se pueden realizar más envíos hasta el final del periodo. Este proceso permite excluir automáticamente un perfil de un envío si un mensaje supera el umbral establecido, evitando así saturar al destinatario.

Los valores de umbral pueden ser constantes o variables. Esto significa que, para un periodo determinado, los umbrales pueden variar de un perfil a otro o incluso en un mismo perfil.

En el campo **Tipo de peso**, hay tres opciones disponibles:

* **Constante**
* **Según el destinatario**
* **Definido en cada regla**

Utilice el campo **Peso del envío** para definir la prioridad de envío. Cada envío tiene un peso que representa su nivel de prioridad. De forma predeterminada, el peso de un envío se establece en 5. Las reglas de presión permiten definir el peso de los envíos a los que se aplican. El peso puede ser fijo o calcularse mediante una fórmula para adaptarse a los destinatarios. Por ejemplo, puede definir el peso de un envío en función de los intereses del destinatario.


Utilice el campo **Modo de envío** para seleccionar el modo de evaluación del destinatario. Hay tres modos disponibles:

* **Estimación de destinatarios y personalización de mensajes**
* **Estimación y aprobación de los destinatarios provisionales**
* **Evaluación de los destinatarios**

La administración de la fatiga viene con el complemento **Optimización de la campaña**. Obtenga más información sobre las reglas de presión y cómo configurar la administración de la fatiga en la [documentación de la versión 8 de Campaign](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=es){target="_blank"}.

### Configuración de la capacidad {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importancia del destinatario"
>abstract="La importancia del destinatario es una fórmula que se utiliza para determinar qué destinatarios se mantienen cuando se exceden las reglas de tipología de capacidad."

En esta sección, puede seleccionar una regla de capacidad definida en la consola de la versión 8 de Adobe Campaign. Esta regla está asociada al canal de correo electrónico.

El campo **importancia del destinatario** es una fórmula que se utiliza para determinar qué destinatarios se mantienen cuando se exceden las reglas de tipología de capacidad.

Obtenga más información sobre las reglas de coherencia y capacidad y cómo configurarlas en la [documentación de la versión 8 de Campaign](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=es){target="_blank"}.


## Audiencia {#audience}

En esta sección, puede seleccionar una **asignación de destino** entre las disponibles. Las asignaciones de destino se definen en la consola de la versión 8 de Adobe Campaign.

Obtenga más información sobre las asignaciones de destino en la [documentación de la versión 8 de Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=es){target="_blank"}.

## Envío {#delivery}

Los parámetros de envío son las configuraciones técnicas que se aplican a su envío.

* **Enrutamiento**: la cuenta externa de enrutamiento del correo electrónico integrada se proporciona de forma predeterminada. Contiene los parámetros técnicos que le permiten a la aplicación enviar correos electrónicos.

* **Prueba de envío SMTP**: esta opción se utiliza para probar el envío a través de SMTP. El envío se procesa hasta la conexión con el servidor SMTP, pero no se envía. Para cada destinatario, Campaign se conecta al servidor del proveedor SMTP, ejecuta el comando RCPT TO del servidor de correo saliente (SMTP) y cierra la conexión antes del comando DATA del SMTP.

* **CCO del correo electrónico**: esta opción se utiliza para almacenar correos electrónicos en un sistema externo como CCO, simplemente al agregar una dirección de correo electrónico a copia oculta (CCO) al destinatario del mensaje. Obtenga más información acerca de la CCO del correo electrónico en la [documentación de la versión 8 de Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=es){target="_blank"}.



### Reintentos {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Número máximo de reintentos"
>abstract="Si un mensaje falla debido a un error temporal, se realizan reintentos hasta el final de la duración del envío."

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

Obtenga más información sobre la administración de reintentos en la [documentación de la versión 8 de Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html?lang=es){target="_blank"}.

## Aprobación {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modo de aprobación"
>abstract="Los pasos de un envío pueden estar sujetos a aprobación para garantizar la monitorización y el control completo de los distintos procesos."

Si se generan advertencias durante la preparación del envío, se puede configurar el envío para definir si se debe ejecutar o no. De forma predeterminada, el usuario debe confirmar el envío de los mensajes al final de la fase de análisis: esta es la validación **manual**.

Puede seleccionar otro modo de aprobación en el campo correspondiente. Los modos disponibles son los siguientes:

* **Manual**: al final de la fase de análisis, el usuario debe confirmar el envío para iniciarlo.

* **Semiautomático**: el envío se realiza automáticamente si la fase de análisis no genera mensajes de advertencia.

* **Automático**: el envío se realiza automáticamente al final de la fase de análisis, sin importar el resultado.


## Validez {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Duración del envío"
>abstract="El campo Duración del envío permite introducir el límite de los reintentos de envío global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, luego, solo para los mensajes que devuelven un error, se realizan reintentos normales y configurables hasta que se alcanza la vigencia."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Vigencia de los recursos"
>abstract="El campo Vigencia se utiliza para los recursos cargados, como la página espejo y las imágenes. Estos recursos son válidos durante un tiempo limitado: una vez alcanzado el límite, los recursos ya no están disponibles."


El campo **Duración del envío** permite introducir el límite de los reintentos de envío global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, para los mensajes que devuelven solo un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez.

Asimismo, puede especificar fechas. Para ello, seleccione **Establecer explícitamente las fechas de validez**. En este caso, las fechas de envío y de límite de validez también permiten especificar el tiempo. El tiempo actual se utiliza de forma predeterminada, pero puede modificarse directamente en el campo de entrada.

**La vigencia de los recursos** se utiliza para los recursos cargados, principalmente para la página espejo y las imágenes. Los recursos de esta página son válidos durante un tiempo limitado (para ahorrar espacio en el disco). Después de este límite, estos recursos ya no están disponibles.

![](assets/delivery-settings-2.png)


Obtenga más información sobre el período de validez del envío en la [documentación de la versión 8 de Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=es#validity-period){target="_blank"}.

### Administración de la página espejo {#mirror}

La página espejo es una página HTML a la que se puede acceder en línea mediante un navegador web. Su contenido es idéntico al del correo electrónico. De forma predeterminada, la página espejo se genera si el vínculo se inserta en el contenido del correo.

Además del modo predeterminado, también están disponibles las siguientes opciones:


* **[!UICONTROL Forzar la generación de la página espejo]**: utilice este modo para generar la página espejo, aunque no haya ningún vínculo a la página espejo insertado en el envío.
* **[!UICONTROL No generar la página espejo]**: utilice este modo para evitar generar una página espejo, incluso si el vínculo está presente en el envío.
* **[!UICONTROL Generar una página espejo a la que se pueda acceder solo mediante el identificador de mensaje]**: cuando el vínculo de la página espejo no esté en el contenido del correo electrónico, utilice esta opción para habilitar el acceso en la ventana del registro del envío, en la consola del cliente.


### Seguimiento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Período de validez"
>abstract="Esta opción define la duración a partir de la cual se activa el seguimiento en las direcciones URL."

Los parámetros de seguimiento se definen en la sección relacionada. Las opciones posibles son las siguientes:

**Vigencia del seguimiento**: utilice esta opción para cambiar la duración por la que se activa el seguimiento en las URL.

**URL de sustitución para URL caducadas**: utilice esta opción para introducir una URL de una página web de reserva, se muestra una vez que el seguimiento ha caducado.

## Configuración de pruebas {#test-setttings}

Puede establecer los parámetros de exclusión en esta sección. Las opciones disponibles son las siguientes:

* **Mantener doble** permite autorizar varios envíos a destinatarios que cumplan varios criterios de direccionamiento.

* **Mantener las direcciones incluidas en la lista de bloqueados** permite excluir de los destinatarios los perfiles a los que ya no se dirige el envío, por ejemplo, tras una cancelación de baja (exclusión).

* **Mantener direcciones en cuarentena** permite excluir del destinatario cualquier perfil con una dirección que no responde.

También puede personalizar el nombre de los correos electrónicos de prueba.

Utilice la opción **Conservar el código de entrega para la prueba** para asociar al correo electrónico de prueba el mismo código de envío que el definido para el envío al que se refiere.

De forma predeterminada, el asunto del correo electrónico de prueba incluye el prefijo “PROOF #”, y “#” es el correo electrónico de prueba. Se puede cambiar este prefijo en el campo **Prefijo de la etiqueta**.