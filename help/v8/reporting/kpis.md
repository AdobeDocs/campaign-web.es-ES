---
title: Indicadores clave de rendimiento
description: Descubra cómo comprender los indicadores de rendimiento clave
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 27%

---

# Indicadores clave de rendimiento {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Indicadores clave de rendimiento"
>abstract="Los **indicadores clave de rendimiento** le permiten comprobar la eficacia de la plataforma mediante indicadores clave de rendimiento (KPI) frecuentes."

<!-- à enlever? -->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="KPI de spam"

Examine la página de inicio para comprobar los indicadores clave de rendimiento de su plataforma. Estos indicadores muestran el número y el porcentaje de mensajes enviados, abiertos, pulsados, cancelaciones de suscripción y tasas de error.

De forma predeterminada, las métricas se calculan para las entregas realizadas durante los siete días anteriores. Puede cambiar el periodo en la lista desplegable de la sección superior derecha de la tarjeta. Se excluyen los mensajes enviados a perfiles de prueba.

Puede seleccionar el canal que desea mostrar. De forma predeterminada, los indicadores reflejan las métricas del canal de correo electrónico.

![Captura de pantalla que muestra la tarjeta KPI con métricas para el canal de correo electrónico.](assets/kpi.png){zoomable="yes"}

## Mensaje entregado {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Entregados"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todos los mensajes procesados correctamente y el porcentaje de mensajes enviados correctamente comparado con el número total de mensajes enviados."

La cantidad de mensajes enviados refleja la tasa de entregabilidad. Nunca puede ser del 100% por las siguientes razones: algunas direcciones o números de teléfono pueden estar equivocados, los bloqueadores de correo no deseado en los proveedores de correo electrónico pueden rechazar sus mensajes o pueden ocurrir problemas de envío.

El indicador **Delivered** muestra los siguientes KPI para cada canal:

* Porcentaje del número de mensajes enviados correctamente comparado con el número total de mensajes enviados.

* Suma de todos los mensajes procesados correctamente.

En Adobe Campaign, la regla para marcar un mensaje como &quot;Enviado&quot; es:

Recuento de mensajes para los que el campo &quot;Dirección semilla&quot; es igual a &quot;No&quot; y con un estado igual a &quot;Tenido en cuenta por el proveedor de servicios&quot; (para SMS), &quot;Enviado&quot; (para correos electrónicos) o &quot;Recibido en el móvil&quot; (para notificaciones push).

## Total de aperturas {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Aperturas"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todos los mensajes abiertos y el porcentaje de mensajes abiertos en comparación con el número total de mensajes enviados correctamente."

El total de aperturas se calcula realizando un seguimiento de la cantidad total de veces que se abre un mensaje, independientemente de cuántos destinatarios individuales generen dichas aperturas. Este indicador solo está disponible para correos electrónicos.

El indicador **Abre** muestra los siguientes KPI para cada canal:

* Porcentaje del número de mensajes abiertos en comparación con el número total de mensajes enviados correctamente.

* Suma de todos los mensajes abiertos, por canal.

Adobe Campaign detecta que el mensaje se abre cuando la persona destinataria descarga las imágenes del correo electrónico. Los correos electrónicos HTML y multiparte/alternativos incluyen una imagen de 0 píxeles, que permite detectar qué mensajes se han abierto. Dado que los mensajes en formato de texto no incluyen imágenes, es imposible detectar si se han abierto. Los valores calculados basados en las aperturas de mensajes siempre son estimaciones debido al margen de error vinculado a la visualización de la imagen.

## Tasa de clics {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clics"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las direcciones URL en las que se hizo clic en los mensajes y el porcentaje de clics comparado con el número total de mensajes enviados correctamente."

Añada direcciones URL en el contenido del mensaje para redirigir a los destinatarios a una página concreta. La tasa de clics mide el número y el porcentaje de destinatarios que hicieron clic en un vínculo del mensaje.

El indicador **Clics** muestra los siguientes KPI para cada canal:

* Porcentaje de clics en comparación con la cantidad total de mensajes enviados correctamente.

* Número de personas distintas que hicieron clic al menos una vez en una entrega. Se excluyen los vínculos de baja y los vínculos a la página espejo de correo electrónico.

Estas métricas se basan en la tabla Consolidated tracking (`nms:trackingStats`). Esta tabla de acumulados se utiliza por motivos de rendimiento al mostrar los informes, en lugar de la tabla Recipient tracking logs (`nms:trackingLogRcp`). No se calcula en tiempo real. La tabla se genera unos minutos después de recuperar los registros de seguimiento.

## Tasas de suscripción {#ui-sub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Suscripciones"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las suscripciones a un servicio y el porcentaje de suscripciones en comparación con la cantidad total de mensajes entregados correctamente."

Los destinatarios pueden suscribirse a las comunicaciones por correo electrónico y SMS.

El indicador **Suscripciones** muestra los siguientes KPI para cada canal:

* Porcentaje del número de suscripciones comparado con el número total de mensajes enviados correctamente.

>[!NOTE]
>
> Los KPI de suscripción y baja varían en función del tipo de servicio. Por ejemplo, las suscripciones por correo electrónico y las bajas de suscripción abarcan todos los servicios relacionados con el correo electrónico, ya sean resultantes de acciones manuales o formularios web. Es importante distinguir este método de la métrica de baja en el nivel de entrega, que rastrea los clics en los vínculos de baja en lugar de los usuarios reales sin suscripción.

## Tasas de baja {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Bajas"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las bajas de un servicio y el porcentaje de bajas en comparación con la cantidad total de mensajes entregados correctamente."

Los destinatarios deben poder desactivar el correo electrónico y los SMS mediante un vínculo de baja dedicado en el contenido del correo electrónico o respondiendo DETENER a un SMS.

El indicador **Cancelaciones de suscripciones** muestra los siguientes KPI para cada canal:

* Porcentaje de bajas en comparación con la cantidad total de mensajes enviados correctamente.

* Suma de todos los clics a un vínculo de baja, es decir, con una categoría URL igual a &quot;Exclusión&quot;.

>[!NOTE]
>
> Los KPI de suscripción y baja varían en función del tipo de servicio. Por ejemplo, las suscripciones por correo electrónico y las bajas de suscripción abarcan todos los servicios relacionados con el correo electrónico, ya sean resultantes de acciones manuales o formularios web. Es importante distinguir este método de la métrica de baja en el nivel de entrega, que rastrea los clics en los vínculos de baja en lugar de los usuarios reales sin suscripción.

## Tasas de error {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Errores"
>abstract="Número total de errores acumulados durante los envíos y el procesamiento automático de rechazos. La tasa asociada es la proporción respecto al número de mensajes que desea enviar."

Es posible que algunos mensajes enviados por su plataforma de Adobe Campaign no lleguen al destino. Puede ocurrir cuando la dirección de usuario o el teléfono tienen errores tipográficos, si el destinatario cambió su dirección de correo electrónico o si el buzón está lleno. Si no es posible enviar un mensaje a un perfil, el servidor remoto envía automáticamente un mensaje de error a Adobe Campaign. Este error sirve para determinar si la dirección de correo electrónico, el número de teléfono o el dispositivo deben ponerse en cuarentena.

Compruebe y actualice la base de datos regularmente y asegúrese de que todos los perfiles estén activos y sean reales. Los errores de envío pueden ser temporales o permanentes (mensajes devueltos no entregados o rechazados), según el motivo por el que no se entregó el mensaje.

El indicador **Errores** muestra los siguientes KPI para cada canal:

* Porcentaje de errores en comparación con la cantidad total de mensajes que se van a enviar.

* Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos.

## Mensaje enviado {#ui-sent-kpi}

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Enviado"
>abstract="Esta métrica muestra, para el canal de correo postal, la suma de todos los mensajes enviados y el porcentaje de mensajes enviados al proveedor, en comparación con el número total de mensajes preparados durante la fase de preparación de la entrega."

Durante la fase de preparación, se genera el archivo de extracción de correo postal, pero la información sobre los destinatarios (registros de envío) no se actualiza. El estado de una entrega pasa de Pending delivery a Sent cuando el usuario de Campaign confirma la entrega. A continuación, la entrega se establece en Finished.

Nunca puede ser el 100% de los mensajes enviados en comparación con el total de mensajes preparados, ya que algunas direcciones pueden faltar o estar incompletas.

El indicador **Enviado** muestra los siguientes KPI para el canal de correo postal:

* Porcentaje del número de mensajes enviados comparado con el número total de mensajes preparados.

* Suma de todos los mensajes enviados.