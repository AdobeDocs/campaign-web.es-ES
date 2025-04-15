---
title: Indicadores clave de rendimiento
description: Aprenda a comprender los indicadores clave de rendimiento
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

Examine la página de inicio para comprobar los indicadores clave de rendimiento de su plataforma. Estos indicadores muestran el número y el porcentaje de mensajes entregados, abiertos, en los que se hizo clic, las bajas de suscripción y las tasas de error.

Las métricas se calculan para los envíos realizados durante los siete días anteriores de forma predeterminada. Puede cambiar el período desde la lista desplegable en la sección superior derecha del tarjeta. Se excluyen los mensajes enviados a perfiles de prueba.

Puede seleccionar el canal que desea mostrar. De forma predeterminada, los indicadores reflejan las métricas del canal de correo electrónico.

![Captura de pantalla que muestra el KPI tarjeta con métricas para el canal correo electrónico.](assets/kpi.png){zoomable="yes"}

## Mensaje entregado {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Entregados"
>abstract="Este Métrica muestra, para el canal seleccionado, la suma de todos los mensajes procesados con éxito y el porcentaje de mensajes entregados con éxito en comparación con el número total de mensajes enviados."

La cantidad de mensajes enviados refleja la tasa de entregabilidad. Nunca puede ser 100% por las siguientes razones: algunas direcciones o números de teléfono pueden estar equivocados, los bloqueadores de spam en correo electrónico proveedores pueden rechazar sus mensajes o pueden ocurrir problemas de entrega.

El **indicador Entregado** muestra los siguientes KPI para cada canal:

* Porcentaje del número de mensajes enviados con éxito en comparación con el número total de mensajes enviados.

* Suma de todos los mensajes procesados correctamente.

En Adobe Campaign, la regla para marcar un mensaje como &quot;Enviado&quot; es:

Recuento de mensajes para los que el campo &quot;dirección semilla&quot; es igual a &quot;No&quot; y con un estado igual a &quot;Tomado en cuenta por el proveedor de servicio&quot; (para SMS), &quot;Enviado&quot; (para correos electrónicos) o &quot;Recibido en el móvil&quot; (para notificaciones push).

## Total de aperturas {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Aperturas"
>abstract="Este Métrica muestra, para el canal seleccionado, la suma de todos los mensajes abiertos y el porcentaje de mensajes abiertos en comparación con el número total de mensajes entregados con éxito."

Las aperturas totales se calculan seguimiento el número total de veces que se abre un mensaje, independientemente de cuántos destinatarios individuales generen esas aperturas. Este indicador solo está disponible para correos electrónicos.

El **indicador de aperturas** muestra los siguientes KPI para cada canal:

* Porcentaje del número de mensajes abiertos en comparación con el número total de mensajes entregados correctamente.

* Suma de todos los mensajes abiertos, por canal.

Adobe Campaign detecta que el mensaje se abre cuando la persona destinataria descarga las imágenes del correo electrónico. Los correos electrónicos HTML y Multipart/Alternative incluyen una imagen de 0 píxeles, que le permite detectar mensajes que se han abierto. Dado que los mensajes en formato de texto no incluyen ninguna imagen, es imposible detectar si se han abierto. Los valores calculados en función de las aperturas de mensajes son siempre estimaciones debido al margen de error vinculado a la visualización de la imagen.

## Tasa de clics {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clics"
>abstract="Este Métrica muestra, para el canal seleccionado, la suma de todas las URL en los mensajes donde se hizo clic y el porcentaje de clics en comparación con el número total de mensajes enviados con éxito."

añadir URL del mensaje contenido para redirección destinatarios a un Página concreto. La tasa de pulsaciones mide el número y el porcentaje de destinatarios que hicieron clic en un vincular del mensaje.

El **indicador de clics** muestra los siguientes KPI para cada canal:

* Porcentaje de clics en comparación con la cantidad total de mensajes enviados correctamente.

* Número de personas diferentes que hicieron clic al menos una vez al envío. Se excluyen los enlaces para darse de baja y los vínculos a las página espejo de correo electrónico.

Estas métricas se basan en la tabla seguimiento consolidada (`nms:trackingStats`). Esta tabla agregado se utiliza por motivos de rendimiento al mostrar informes, en lugar de la tabla Destinatario registros de seguimiento (`nms:trackingLogRcp`). No se calcula en tiempo real. La tabla se genera unos minutos después de recuperar los registros de seguimiento.

## Tasas de suscripción {#ui-sub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Suscripciones"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las suscripciones a un servicio y el porcentaje de suscripciones en comparación con la cantidad total de mensajes entregados correctamente."

Los destinatarios pueden adhesión a las comunicaciones por correo electrónico y SMS.

El **indicador de suscripciones** muestra los siguientes KPI para cada canal:

* Porcentaje del número de suscripciones comparados con el número total de mensajes enviados correctamente.

>[!NOTE]
>
> Los KPI de suscripción y baja varían según el tipo de servicio. Por instancia, correo electrónico suscripciones y bajas abarcan todos los servicios relacionados con el correo electrónico, ya sean el resultado de acciones manuales o formularios web. Es importante distinguir este enfoque del Métrica de baja de nivel envío, que rastrea baja vincular clics en lugar de usuarios reales no suscritos.

## Tasas de baja {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Bajas"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las bajas de un servicio y el porcentaje de bajas en comparación con la cantidad total de mensajes entregados correctamente."

Los destinatarios deben poder exclusión desde correo electrónico y SMS a través de un vincular de baja dedicado en el contenido de correo electrónico o respondiendo STOP a un SMS.

El **indicador de bajas de** suscripción muestra los siguientes KPI para cada canal:

* Porcentaje de bajas en comparación con la cantidad total de mensajes enviados correctamente.

* Suma de todos los clics a un vincular baja, es decir, con un categoría URL igual a &quot;Exclusión&quot;.

>[!NOTE]
>
> Los KPI de suscripción y baja varían según el tipo de servicio. Por instancia, correo electrónico suscripciones y bajas abarcan todos los servicios relacionados con el correo electrónico, ya sean el resultado de acciones manuales o formularios web. Es importante distinguir este enfoque del Métrica de baja de nivel envío, que rastrea baja vincular clics en lugar de usuarios reales no suscritos.

## Tasas de error {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Errores"
>abstract="Número total de errores acumulados durante los envíos y el procesamiento automático de rechazos. La tasa asociada es la proporción respecto al número de mensajes que desea enviar."

Es posible que algunos mensajes enviados por su plataforma de Adobe Campaign no lleguen al destino. Puede suceder cuando la dirección usuario o el teléfono tiene errores tipográficos, si el destinatario cambió su dirección correo electrónico o si su buzón está lleno. Si no es posible enviar un mensaje a un perfil, el servidor remoto envía automáticamente un mensaje de error a Adobe Campaign. Este error se califica para determinar si la dirección correo electrónico, el número de teléfono o el dispositivos deben ponerse en cuarentena.

Revise y actualice su base de datos regularmente, y asegúrese de que todos los perfiles estén activos y sean reales. Los errores de envío pueden ser temporales o permanentes (rebote leve o grave), dependiendo de la razón por la cual no se entregó el mensaje.

El **indicador de errores** muestra los siguientes KPI para cada canal:

* Porcentaje de errores en comparación con la cantidad total de mensajes que se van a enviar.

* Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos.

## Mensaje enviado {#ui-sent-kpi}

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Enviado"
>abstract="Este Métrica muestra, para el canal correo directo, la suma de todos los mensajes enviados y el porcentaje de mensajes enviados al proveedor, en comparación con el número total de mensajes preparados durante la fase de preparación del envío."

Durante la fase de preparación, se genera el correo directo extracción archivo, pero no se actualiza la información relativa a los destinatarios (registros de envío). El estado de una envío pasa de Pendiente de envío a Enviado cuando el usuario Campaign confirma el envío del envío. A continuación, la envío se establece en Terminado.

Nunca puede ser el 100% de los mensajes enviados en comparación con el total de mensajes preparados, ya que algunas direcciones pueden faltar o estar incompletas.

El **indicador de enviados** muestra los siguientes KPI para el canal correo postal:

* Porcentaje del número de mensajes enviados en comparación con el número total de mensajes preparados.

* Suma de todos los mensajes enviados.