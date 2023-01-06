---
audience: end-user
title: Configuración avanzada
description: Documentación web de Campaign v8
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 3c7aa37bb74349e88176f1fc75a26bc52e34c628
workflow-type: tm+mt
source-wordcount: '1077'
ht-degree: 47%

---

# Configuración avanzada {#advanced-settings}

>[!NOTE]
>
>Esta documentación está en construcción y se actualiza con frecuencia. La versión final de este contenido estará lista en enero de 2023.

Estos ajustes son parámetros técnicos de envío definidos en la plantilla de correo electrónico. Si desea modificar cualquiera de ellos para un envío específico, tenga cuidado.

## Configuración de entrega de correo electrónico {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

Todos los parámetros técnicos de envío de la plantilla.

>[!NOTE]
>
> Cambie solo los parámetros, no cree aquí. Según los permisos.

>[!NOTE]
>
> Los practicantes no deben modificarlo, tenga cuidado. Compruebe y cambie solo la regla de tipología.

## Tipología {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipología"
>abstract="La tipología permite controlar, filtrar y monitorizar los envíos."

Las tipologías son conjuntos de reglas de tipología que se ejecutan durante la fase de análisis de mensajes. Le permiten asegurarse de que los mensajes de correo electrónico siempre contengan determinados elementos (como un vínculo de baja o una línea de asunto) o reglas de filtrado para excluir grupos de los destinatarios deseados (como suscriptores que se han dado de baja, competidoras o clientes que no sean fieles).

Al asociar una tipología con una plantilla de mensaje o un mensaje, las reglas de tipología incluidas en ella se ejecutarán para comprobar la validez del mensaje.

### Parámetros de presión {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso del envío"
>abstract="El peso de la entrega le permite identificar las entregas de mayor prioridad dentro del marco de la gestión de presión. Los mensajes con mayor peso son prioritarios."

En esta sección, los parámetros de presión permiten definir un umbral. Es el número máximo de mensajes que se pueden enviar a un perfil durante un periodo determinado. Una vez alcanzado este umbral, no se pueden realizar más entregas hasta el final del periodo. Este proceso permite excluir automáticamente un perfil de una entrega si un mensaje supera el umbral establecido, evitando así saturar al destinatario.

Los valores de umbral pueden ser constantes o variables. Esto significa que, para un periodo determinado, los umbrales pueden variar de un perfil a otro o incluso en un mismo perfil.

En el **Tipo de peso** , hay tres opciones disponibles: (falta la fórmula en función de la opción.)

La variable **Peso de la entrega** field : Cada envío tiene un peso que representa su nivel de prioridad. De forma predeterminada, el peso de una entrega se establece en 5. Las reglas de presión permiten definir el peso de los envíos a los que se aplican. El peso se puede establecer o calcular mediante una fórmula para adaptarse a los destinatarios. Por ejemplo, puede definir el peso de una entrega en función de los intereses del destinatario.

La variable **Modo de envío** campo. ??

### Configuración de capacidad {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importancia del destinatario"
>abstract="La importancia del destinatario es una fórmula que se utiliza para determinar qué destinatarios se mantienen cuando se exceden las reglas de tipología de capacidad."

En esta sección, puede seleccionar una regla de capacidad definida en la consola de Adobe Campaign v8. Esta regla está asociada al canal de correo electrónico.

La variable **importancia del destinatario** field es una fórmula utilizada para determinar qué destinatarios se mantienen cuando se exceden las reglas de tipología de capacidad.

## Audiencia {#audience}

En esta sección, puede elegir una **asignación de destino** definida en la consola de Adobe Campaign v8. La creación de la asignación de destino es necesaria en el caso de que se utilice una tabla de destinatarios distinta de la proporcionada por Adobe Campaign.

## Envío {#delivery}

**Enrutamiento** selección: seleccione la cuenta externa....

**Prueba de entrega SMTP**: utilice esta opción para probar el envío a través de SMTP. La entrega se procesa hasta la conexión con el servidor SMTP, pero no se envía. Para cada destinatario de la entrega, Campaign se conecta al servidor del proveedor SMTP, ejecuta el comando RCPT TO del servidor de correo saliente (SMTP) y cierra la conexión antes del comando DATA del SMTP.

**Email BCC**: utilice esta opción para almacenar correos electrónicos en un sistema externo a través de CCO simplemente añadiendo una dirección de correo electrónico CCO al destino del mensaje.

### Reintentos {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Número máximo de reintentos"
>abstract="Si un mensaje falla debido a un error temporal, los reintentos se realizan durante la duración del envío."

Para los mensajes que no se hayan enviado temporalmente debido a un error leve o ignorado, se realiza un reintento automático. De manera predeterminada, se programan cinco reintentos para el primer día de la entrega con un intervalo mínimo de una hora distribuidos durante las 24 horas del día. Después de ello, se programa un reintento por día hasta la fecha límite de entrega, que se define en la pestaña Validez .

## Aprobación {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Aprobación mode"
>abstract="Cada paso de una entrega puede estar sujeto a aprobación para garantizar una monitorización y un control completos de los distintos procesos."

**Manual**: al final de la fase de análisis, el usuario debe confirmar la entrega para iniciarlo.

**Semiautomático**: El envío comienza automáticamente si la fase de análisis no genera mensajes de advertencia.

**Automatic**: la entrega comienza automáticamente al final de la fase de análisis, independientemente de su resultado.


## Validez {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Duración del envío"
>abstract="El campo Duración de la entrega permite introducir el límite de los reintentos de entrega global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, para los mensajes que devuelven solo un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Vigencia de recursos"
>abstract="El campo Límite de validez se utiliza para los recursos cargados, principalmente para la página espejo y las imágenes. Los recursos de esta página son válidos durante un tiempo limitado."


El campo **Duración de la entrega** permite introducir el límite de los reintentos de entrega global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, para los mensajes que devuelven solo un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez.

Asimismo, puede especificar fechas. Para ello, seleccione **Establecer explícitamente las fechas de validez**. En este caso, las fechas de entrega y de límite de validez también permiten especificar el tiempo. El tiempo actual se utiliza de forma predeterminada, pero puede modificarse directamente en el campo de entrada.

**Límite de validez de los recursos** se utiliza para los recursos cargados, principalmente para la página espejo y las imágenes. Los recursos de esta página son válidos durante un tiempo limitado (para ahorrar espacio en el disco).

### Administración de página espejo {#mirror}

**Administración de páginas espejo** contiene cuatro opciones :


### Seguimiento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Período de validez"
>abstract="Esta opción define la duración durante la cual se activará el seguimiento en las direcciones URL."

**Límite de validez de seguimiento**: Esta opción define la duración durante la cual se activará el seguimiento en las direcciones URL.

**URL de sustitución para URL caducadas**: TBC


## Configuración de la prueba {#test-setttings}

**Mantener doble** permite autorizar varios envíos a destinatarios que cumplan varios criterios de objetivo.

**Mantener direcciones incluidas en la lista de bloqueados**

**Mantener direcciones en cuarentena** permite evitar que el destinatario tenga perfiles con una dirección que no responde.

**Mantener el código de entrega de la prueba** permite dar a la prueba el mismo código de entrega que el definido para la entrega con el que se relaciona.

De forma predeterminada, el asunto de la prueba lleva el prefijo &quot;Proof #&quot;, donde # es el número de la prueba. Se puede cambiar este prefijo en el campo **Label prefix**.