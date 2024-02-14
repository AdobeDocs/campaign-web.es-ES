---
audience: end-user
title: Configuración de envío
description: Obtenga más información sobre la configuración de envíos en Campaign Web
feature: Email
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: a516a5aba56dbbff213d9a61b47144d6b4d801ff
workflow-type: tm+mt
source-wordcount: '2417'
ht-degree: 61%

---


# Configuración de envío de correos electrónicos {#email-del-settings}

La configuración de envío de correo electrónico es **parámetros técnicos de envío** que se definen en la plantilla de correo electrónico. Se pueden sobrecargar para cada envío.

Esta configuración está disponible en **Configuración** botón disponible al editar una entrega por correo electrónico o una plantilla de envíos por correo electrónico.

## Configuración de envío de correos electrónicos {#email-delivery-settings}

>[!CAUTION]
>
>Esta configuración es solo informativa. Algunos ajustes dependen de la configuración y los permisos. No deben modificarse en esta versión del producto.

## Configuración de tipología {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipología"
>abstract="Las reglas de tipología permiten a los especialistas en marketing estandarizar las prácticas comerciales en todos los envíos. Una tipología es una colección de reglas de tipología que le permiten controlar, filtrar y priorizar la entrega de envíos. Los perfiles que coinciden con los criterios dentro de las reglas de tipología quedan excluidos de los públicos de envío en la fase de preparación. Las tipologías y reglas de tipología se crean en la consola del cliente de Campaign."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Configuración de tipología para el envío"
>abstract="Las reglas de tipología permiten a los especialistas en marketing estandarizar las prácticas comerciales en todos los envíos. Una tipología es una colección de reglas de tipología que le permiten controlar, filtrar y priorizar la entrega de envíos. Los perfiles que coinciden con los criterios dentro de las reglas de tipología quedan excluidos de los públicos de envío en la fase de preparación. Las tipologías y reglas de tipología se crean en la consola del cliente de Campaign."


Las tipologías son conjuntos de **reglas de tipología** que se ejecutan durante la fase de preparación para aplicar fácilmente varias reglas de filtrado a una entrega a la vez. Permiten a los especialistas en marketing estandarizar las prácticas comerciales en todas las entregas, ya que les permiten controlar, filtrar y priorizar la entrega de entregas.

Al asociar una tipología con una plantilla de mensaje o un mensaje, las reglas de tipología incluidas en ella se ejecutan para comprobar la validez de la entrega durante la preparación del mensaje. Los perfiles que coinciden con los criterios dentro de una regla de tipología se excluyen de las audiencias de envío.

Las tipologías le permiten asegurarse de que los correos electrónicos siempre contengan determinados elementos (como un vínculo de baja o una línea de asunto) o reglas de filtrado para excluir grupos de los destinatarios deseados (como suscriptores que se han dado de baja, competidores o clientes que no sean fieles).

![](assets/delivery-settings-typology.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>Las tipologías y reglas de tipología se crean en la consola del cliente de Campaign. Obtenga más información acerca de las reglas de presión y cómo configurar la administración de la fatiga en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html?lang=es){target="_blank"}.

### Parámetros de presión {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Parámetros de presión del envío"
>abstract="Los pesos del envío le permiten identificar los envíos de mayor prioridad dentro del marco de la administración de la fatiga. Los mensajes con mayor peso tienen prioridad."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Peso del envío"
>abstract="El peso del envío le permite identificar los envíos de mayor prioridad dentro del marco de la administración de presión. Los mensajes con mayor peso tienen prioridad."

En esta sección, los parámetros de presión permiten definir una **umbral** para configurar las reglas de gestión de fatiga, que es el número máximo de mensajes que se pueden enviar a un perfil durante un periodo determinado.

Una vez alcanzado este umbral, no se pueden realizar más envíos hasta el final del periodo. Este proceso permite excluir automáticamente un perfil de un envío si un mensaje supera el umbral establecido, evitando así saturar al destinatario.

Los valores de umbral pueden ser constantes o variables. Esto significa que, para un periodo determinado, los umbrales pueden variar de un perfil a otro o incluso en un mismo perfil.

En el campo **[!UICONTROL Tipo de peso]**, hay tres opciones disponibles:

* **[!UICONTROL Constante]**
* **[!UICONTROL Según el destinatario]**
* **[!UICONTROL Definido en cada regla]**

Utilice el campo **[!UICONTROL Peso del envío]** para definir la prioridad de envío. Cada envío tiene un peso que representa su nivel de prioridad. De forma predeterminada, el peso de un envío se establece en 5. Las reglas de presión permiten definir el peso de los envíos a los que se aplican. El peso puede ser fijo o calcularse mediante una fórmula para adaptarse a los destinatarios. Por ejemplo, puede definir el peso de un envío en función de los intereses del destinatario.

Utilice el campo **[!UICONTROL Modo de envío]** para seleccionar el modo de evaluación del destinatario. Hay tres modos disponibles:

* **[!UICONTROL Estimación de destinatarios y personalización de mensajes]**
* **[!UICONTROL Estimación y aprobación de los destinatarios provisionales]**
* **[!UICONTROL Evaluación de los destinatarios]**

>[!NOTE]
>
>La administración de la fatiga se configura en la consola del cliente de Campaign. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=es){target="_blank"}.

### Configuración de la capacidad {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Configuración de la capacidad del envío"
>abstract="Antes de enviar mensajes, utilice reglas de capacidad para asegurarse de que su organización pueda procesar el envío, los mensajes entrantes que puede generar el envío y el número de llamadas que se realizan para ponerse en contacto con los suscriptores, por ejemplo. Las reglas de capacidad se definen en la consola de la versión 8 de Adobe Campaign. En esta pantalla, seleccione una regla asociada al canal de correo electrónico."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Importancia del destinatario"
>abstract="La importancia del destinatario es una fórmula que se utiliza para determinar qué destinatarios se mantienen cuando se exceden las reglas de tipología de capacidad."


En esta sección, puede seleccionar una regla de capacidad definida en la consola de Adobe Campaign v8. Esta regla está asociada al canal de correo electrónico.

El **[!UICONTROL Importancia del destinatario]** field es una fórmula que se utiliza para determinar qué destinatarios se conservan cuando se exceden las reglas de tipología de capacidad.

>[!NOTE]
>
>Las reglas de tipología se configuran en la consola del cliente de Campaign. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=es){target="_blank"}.

## Configuración del público {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Configuración del público del envío"
>abstract="Seleccione una **asignación de destino** entre las disponibles. Las asignaciones de destino se definen en la consola de la versión 8 de Adobe Campaign. También puede definir los parámetros de exclusión del envío. "

En esta sección, puede seleccionar una **asignación de destino** entre las disponibles. Las asignaciones de destino se definen en la consola de la versión 8 de Adobe Campaign. La asignación de destino es el tipo de datos que administra una operación. Permite definir la población objetivo: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc.

Obtenga más información sobre las asignaciones de destino en [esta sección](../audience/targeting-dimensions.md).

En el **[!UICONTROL Exclusión]** , puede seleccionar excluir los destinatarios que ya no desean que se les contacte o que están en cuarentena. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

## Envío {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Configuración del envío"
>abstract="Los parámetros de envío son las configuraciones técnicas que se aplican a su envío. Puede cambiar los modos de entrega y rutina, activar el CCO del correo electrónico, enviar mediante olas y también elegir el formato de los mensajes de correo electrónico enviados. Estas opciones están restringidas únicamente a usuarios expertos."

**[!UICONTROL Envío]** Los parámetros de son ajustes técnicos que se aplican a su envío.

![](assets/delivery-settings-delivery.png){zoomable=&quot;yes&quot;}

El correo electrónico integrado **[!UICONTROL Enrutamiento]** La cuenta externa de se proporciona de forma predeterminada. Contiene los parámetros técnicos que le permiten a la aplicación enviar correos electrónicos.

Puede definir la variable **[!UICONTROL Enviando]** configuración siguiente.

* **[!UICONTROL Prioridad de envío]**: Utilice esta opción para cambiar el orden de envío de los envíos estableciendo su nivel de prioridad: normal, alto o bajo.

* **[!UICONTROL Cantidad de lotes de mensajes]**: utilice esta opción para definir el número de mensajes agrupados dentro del mismo paquete de envío XML. Si el parámetro se establece en 0, los mensajes se agrupan automáticamente. El tamaño del paquete se define mediante el cálculo `<delivery size>/1024`, con un mínimo de 8 y un máximo de 256 mensajes por paquete.

  >[!IMPORTANT]
  >
  >Cuando se crea la entrega duplicando una existente, este parámetro se restablece.

* **[!UICONTROL Probar envío SMTP]**: Esta opción se utiliza para probar el envío a través de SMTP. La entrega se procesa hasta la conexión con el servidor SMTP, pero no se envía: para cada destinatario de la entrega, Campaign se conecta al servidor del proveedor SMTP, ejecuta el comando SMTP RCPT TO y cierra la conexión antes del comando SMTP DATA.

* **[!UICONTROL Correo electrónico CCO]**: Esta opción se utiliza para almacenar correos electrónicos en un sistema externo como CCO simplemente añadiendo una dirección de correo electrónico CCO al objetivo del mensaje. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/email-bcc.html){target="_blank"}.

En el **[!UICONTROL Definición de ola]** , seleccione la **[!UICONTROL Envío mediante múltiples olas]** opción para aumentar progresivamente el volumen enviado mediante olas. Esto evitará que sus mensajes se marquen como correo no deseado o para limitar el número de mensajes por día. Mediante las oleadas puede dividir los envíos en varios lotes en lugar de enviar volúmenes altos de mensajes al mismo tiempo. [Más información](send-using-waves.md)

También puede cambiar el **[!UICONTROL Formatos de correo]** de los mensajes de correo electrónico enviados como se detalla a continuación.

* **[!UICONTROL Usar preferencias del destinatario]** (modo predeterminado)

  El formato de mensaje se define según los datos almacenados en el perfil de destinatario. Si un destinatario desea recibir mensajes en un formato determinado, este es el formato enviado. Si el campo no está rellenado, se envía un mensaje multipart-alternative (consulte a continuación).

* **[!UICONTROL Permitir que el cliente de correo del destinatario elija el formato más adecuado]**

  El mensaje contiene ambos formatos: texto y HTML. El formato que se muestra al recibirlo depende de la configuración del software de correo del destinatario (multipart-alternative).

  >[!IMPORTANT]
  >
  >Esta opción incluye ambas versiones del documento. Por lo tanto, esto afecta a la tasa de entrega ya que el tamaño del mensaje es mayor.

* **[!UICONTROL Enviar todos los mensajes en formato de texto]**

  El mensaje se envía en formato de texto. El formato de HTML no se envía, pero se utiliza solo para la página espejo cuando el destinatario hace clic en el mensaje.

## Análisis web {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Configuración de análisis web del envío"
>abstract="Seleccione una cuenta de análisis web. Esta cuenta se configura en la consola del cliente de Campaign. También puede definir las etiquetas compartidas con la herramienta de análisis que está utilizando."

En esta sección, puede seleccionar una cuenta de análisis web. Esta cuenta se configura en la consola del cliente de Campaign.

También puede definir las etiquetas compartidas con la herramienta de análisis que está utilizando.

>[!NOTE]
>
>Las funcionalidades de Web Analytics se configuran en la consola del cliente de Campaign. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html#external-account-ac){target="_blank"}.

## Reintentos {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Número máximo de reintentos"
>abstract="Si un mensaje falla debido a un error temporal, se realizan reintentos hasta el final de la duración del envío."

<!--Currently not visible in UI > ??-->

Los mensajes no enviados temporalmente debido a un error leve o ignorado están sujetos a un reintento automático. De manera predeterminada, se programan cinco reintentos para el primer día del envío con un intervalo mínimo de una hora distribuidos durante las 24 horas del día.

## Aprobación {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Modo de aprobación del envío"
>abstract="Seleccione el modo de aprobación. Si se generan advertencias durante la preparación del envío, se puede configurar el envío para definir si se debe ejecutar o no."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Modo de aprobación de los envíos"
>abstract="Seleccione el modo de aprobación de los envíos basados en esta plantilla. Si se generan advertencias durante la preparación del envío, se puede configurar el envío para definir si se debe ejecutar o no."

Si se generan advertencias durante la preparación del envío, se puede configurar el envío para definir si se debe ejecutar o no. De forma predeterminada, el usuario debe confirmar el envío de los mensajes al final de la fase de análisis: esta es la validación **manual**.

Puede seleccionar otro modo de aprobación en el campo correspondiente. Los modos disponibles son los siguientes:

* ****[!UICONTROL Manual]****: al final de la fase de análisis, el usuario debe confirmar el envío para iniciarlo.

* **[!UICONTROL Semiautomático]**: el envío se realiza automáticamente si la fase de análisis no genera mensajes de advertencia.

* **[!UICONTROL Automático]**: el envío se realiza automáticamente al final de la fase de análisis, sin importar el resultado.

## Validez {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Validez de la configuración"
>abstract="El campo **Duración del envío** permite introducir el límite de los reintentos de envío global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, para los mensajes que devuelven solo un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez.<br>El campo **Vigencia de los recursos** se utiliza para los recursos cargados, como la página espejo y las imágenes. Una vez alcanzado el límite, los recursos ya no están disponibles."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Vigencia de los recursos"
>abstract="El campo **Vigencia de los recursos** se utiliza para los recursos cargados, principalmente para la página espejo y las imágenes. Estos recursos son válidos durante un tiempo limitado: una vez alcanzado el límite, los recursos ya no están disponibles."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Duración del envío"
>abstract="El campo **Duración del envío** permite introducir el límite de los reintentos de envío global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, para los mensajes que devuelven solo un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez."

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### Período de validez {#validity-period}

El campo **[!UICONTROL Duración del envío]** permite introducir el límite de los reintentos de envío global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, para los mensajes que devuelven solo un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez.

Asimismo, puede especificar fechas. Para ello, seleccione **[!UICONTROL Establecer explícitamente las fechas de validez]**. En este caso, las fechas de envío y de límite de validez también permiten especificar el tiempo. El tiempo actual se utiliza de forma predeterminada, pero puede modificarse directamente en el campo de entrada.

**[!UICONTROL Vigencia de recursos]** se utiliza para los recursos cargados, principalmente para la página espejo y las imágenes. Los recursos de esta página son válidos durante un tiempo limitado (para ahorrar espacio en el disco). Después de este límite, estos recursos ya no están disponibles.

![](assets/delivery-settings-validity.png){zoomable=&quot;yes&quot;}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

Obtenga más información sobre el periodo de validez de envíos en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=es#validity-period){target="_blank"}.

### Administración de la página espejo {#mirror}

La página espejo es una página HTML a la que se puede acceder en línea mediante un navegador web. Su contenido es idéntico al del correo electrónico. De forma predeterminada, la página espejo se genera si el vínculo se inserta en el contenido del correo.

Además del modo predeterminado, también están disponibles las siguientes opciones:

* **[!UICONTROL Forzar la generación de la página espejo]**: Utilice este modo para generar la página espejo aunque no se inserte ningún vínculo a la página espejo en la entrega.
* **[!UICONTROL No generar la página espejo]**: Utilice este modo para evitar generar una página espejo, incluso si el vínculo está presente en la entrega.
* **[!UICONTROL Genera una página espejo accesible solo mediante el identificador del mensaje]**: Cuando el vínculo de página espejo no está presente en el contenido del correo electrónico, utilice esta opción para habilitar el acceso al contenido de la página espejo, en la ventana del registro de envío, desde la consola del cliente.


### Seguimiento {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Período de validez"
>abstract="El período de vigencia establece la duración durante la cual se activa el seguimiento en las direcciones URL de los mensajes."

**[!UICONTROL Seguimiento]** Los parámetros de se definen en la sección relacionada. Las opciones posibles son las siguientes:

**[!UICONTROL Vigencia de seguimiento]**: utilice esta opción para cambiar la duración durante la cual se activa el seguimiento en las direcciones URL.

**[!UICONTROL URL de sustitución para URL caducadas]**: utilice esta opción para introducir una URL a una página web de reserva: se muestra una vez que ha caducado el seguimiento.

## Configuración de prueba {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Defina la configuración de prueba del envío"
>abstract="Seleccione los parámetros de exclusión y personalice la etiqueta de las pruebas."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

Puede establecer los parámetros de exclusión en esta sección. Las opciones disponibles son las siguientes:

* ****[!UICONTROL Mantener dobles]**** permite autorizar varios envíos a destinatarios que cumplan varios criterios de objetivo.

* **[!UICONTROL Mantener las direcciones incluidas en la lista de bloqueados]** permite excluir de los destinatarios los perfiles a los que ya no se dirige el envío, por ejemplo, tras una cancelación de baja (exclusión).

* **[!UICONTROL Mantener direcciones en cuarentena]** permite excluir del destinatario cualquier perfil con una dirección que no responde.

También puede personalizar la etiqueta de las pruebas:

* Utilice el **[!UICONTROL Mantener el código de envío de la prueba]** para asociar a la prueba el mismo código de envío que el definido para la entrega con el que se relaciona.

* De forma predeterminada, el asunto de la prueba lleva el prefijo &quot;PROOF #&quot;, donde # es el número de la prueba. Se puede cambiar este prefijo en el campo **[!UICONTROL Prefijo de la etiqueta]**.