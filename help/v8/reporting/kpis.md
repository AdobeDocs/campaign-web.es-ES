---
title: Indicadores clave de rendimiento
description: Descubra cómo comprender los indicadores de rendimiento clave
badge: label="Beta"
exl-id: 4b182219-100b-4101-919b-b0b770dd8515
source-git-commit: 53f1cc7776d56a42b4027f73cb3399a8c630cdfa
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 73%

---

# Indicadores clave de rendimiento {#kpis}

>[!CONTEXTUALHELP]
>id="acw_homepage_kpi"
>title="Indicadores clave de rendimiento"
>abstract="Los **indicadores clave de rendimiento** le permiten comprobar la eficacia de la plataforma mediante indicadores clave de rendimiento (KPI) frecuentes."

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="KPI de spam"

Examine la página de inicio para comprobar los indicadores clave de rendimiento de su plataforma. Dichos indicadores muestran la cantidad y el porcentaje de mensajes enviados, abiertos y clicados, así como las bajas y las tasas de error.

De forma predeterminada, las métricas se calculan para los envíos realizados durante los 7 días anteriores. Puede cambiar el período en la lista desplegable de la sección superior derecha de la tarjeta. Se excluyen los mensajes enviados a perfiles de prueba.

Puede seleccionar el canal que desea mostrar. De forma predeterminada, los indicadores reflejan las métricas del canal de correo electrónico.

![](assets/kpi.png)

## Mensaje entregado {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Entregados"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todos los mensajes procesados correctamente y el porcentaje de mensajes entregados correctamente en comparación con la cantidad total de mensajes enviados."

La cantidad de mensajes enviados refleja la tasa de entregabilidad. Nunca puede ser del 100 % por los siguientes motivos: es posible que algunas direcciones o números de teléfono sean incorrectos, que los bloqueadores de correo no deseado de los proveedores de correo electrónico rechacen sus mensajes o que se produzcan problemas de entregabilidad.

Para cada canal, el indicador **Enviado** muestra los siguientes indicadores clave de rendimiento (KPI):

* Porcentaje de mensajes enviados correctamente en comparación con la cantidad total de mensajes enviados.

* Suma de todos los mensajes procesados correctamente.

En Adobe Campaign, la regla para marcar un mensaje como &quot;Enviado&quot; es:

Recuento de mensajes en los que el campo &quot;dirección semilla&quot; es igual a &quot;No&quot; y su estado es igual a &quot;Considerado por el proveedor de servicios&quot; (para SMS), &quot;Enviado&quot; (para correos electrónicos) o &quot;Recibido en el móvil&quot; (para notificaciones push).


## Total de aperturas {#ui-open-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_opens"
>title="Aperturas"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todos los mensajes abiertos y el porcentaje de mensajes abiertos en comparación con la cantidad total de mensajes entregados correctamente."

El total de aperturas se calcula realizando un seguimiento de la cantidad total de veces que se abre un mensaje, independientemente de cuántas personas destinatarias hayan generado dichas aperturas. Este indicador solo está disponible para correos electrónicos.

Para cada canal, el indicador **Aperturas** muestra los siguientes indicadores clave de rendimiento (KPI):

* Porcentaje de mensajes abiertos en comparación con el número total de mensajes enviados correctamente.

* Suma de todos los mensajes abiertos, por canal.

Adobe Campaign detecta que el mensaje se abre cuando la persona destinataria descarga las imágenes del correo electrónico. Los correos electrónicos HTML con varias partes o alternativos incluyen una imagen de 0 píxeles que permite detectar qué mensajes se han abierto. Dado que los mensajes en formato de texto no incluyen imágenes, es imposible detectar si se han abierto o no. Los valores calculados basados en las aperturas de mensajes siempre son estimaciones debido al margen del error relacionado con la visualización de la imagen.



## Tasa de clics {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clics"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las URL clicadas de los mensajes y el porcentaje de clics comparado con la cantidad total de mensajes entregados correctamente."

Puede añadir URL en el contenido del mensaje para redirigir a una página concreta. La tasa de clics mide la cantidad y el porcentaje de personas que hicieron clic en un vínculo del mensaje.

Para cada canal, el indicador **Clics** muestra los siguientes indicadores clave de rendimiento (KPI):

* Porcentaje de clics en comparación con la cantidad total de mensajes enviados correctamente.

* Cantidad de personas diferentes que han hecho clic al menos una vez en un envío. Se excluyen los vínculos de baja y los vínculos a la página espejo de correo electrónico.

Estas métricas se basan en la tabla Seguimiento consolidado (`nms:trackingStats`). Esta tabla de acumulados se utiliza por motivos de rendimiento al mostrar los informes, en lugar de la tabla Registros de seguimiento de destinatarios (`nms:trackingLogRcp`), y no se calcula en tiempo real. La tabla se genera unos minutos después de recuperar los registros de seguimiento.


## Tasas de suscripción {#ui-sub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_subscriptions"
>title="Suscripciones"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las suscripciones a un servicio y el porcentaje de suscripciones en comparación con el número total de mensajes enviados correctamente."


Los destinatarios pueden optar por recibir comunicaciones por correo electrónico y SMS.

El **Suscripciones** Este indicador muestra los siguientes KPI, para cada canal el porcentaje del número de suscripciones comparado con el número total de mensajes enviados correctamente.


>[!NOTE]
>
> Los KPI de suscripción y baja varían en función del tipo de servicio. Por ejemplo, las suscripciones por correo electrónico y las bajas de suscripción abarcan todos los servicios relacionados con el correo electrónico, ya sean resultantes de acciones manuales o formularios web. Es importante distinguir este método de la métrica de baja en el nivel de entrega, que rastrea los clics en los vínculos de baja en lugar de los usuarios reales sin suscripción.

## Tasas de baja {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Bajas"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las bajas de un servicio y el porcentaje de bajas en comparación con la cantidad total de mensajes entregados correctamente."


Las personas deben poder pedir la exclusión de los correos electrónicos y los SMS mediante un vínculo de baja específico en el contenido del correo electrónico o respondiendo DETENER a un SMS.

Para cada canal, el indicador **Bajas** muestra los siguientes indicadores clave de rendimiento (KPI):

* Porcentaje de bajas en comparación con la cantidad total de mensajes enviados correctamente.

* Suma de todos los clics hechos en un vínculo de baja, es decir, que tengan una categoría URL igual a &quot;Exclusión&quot;.


>[!NOTE]
>
> Los KPI de suscripción y baja varían en función del tipo de servicio. Por ejemplo, las suscripciones por correo electrónico y las bajas de suscripción abarcan todos los servicios relacionados con el correo electrónico, ya sean resultantes de acciones manuales o formularios web. Es importante distinguir este método de la métrica de baja en el nivel de entrega, que rastrea los clics en los vínculos de baja en lugar de los usuarios reales sin suscripción.

## Tasas de error {#ui-error-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_errors"
>title="Errores"
>abstract="Número total de errores acumulados durante los envíos y el procesamiento automático de rechazos. La tasa asociada es la proporción respecto al número de mensajes que desea enviar."

Es posible que algunos mensajes enviados por su plataforma de Adobe Campaign no lleguen al destino. Es posible que ocurra si la dirección o el teléfono tienen errores tipográficos, si la persona cambió la dirección de correo electrónico o si su buzón está lleno. Si no es posible enviar un mensaje a un perfil, el servidor remoto envía automáticamente un mensaje de error a Adobe Campaign. Este error sirve para determinar si la dirección de correo electrónico, el número de teléfono o el dispositivo deben ponerse en cuarentena.

Como consecuencia, siempre debe comprobar y actualizar la base de datos y asegurarse de que todos los perfiles estén activos y sean reales. Los errores de envío pueden ser temporales o permanentes (mensajes devueltos no entregados o rechazos permanentes), según el motivo por el que no se envió el mensaje.

Para cada canal, el indicador **Errores** muestra los siguientes indicadores clave de rendimiento (KPI):

* Porcentaje de errores en comparación con la cantidad total de mensajes que se van a enviar.

* Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos.

## Mensaje enviado {#ui-sent-kpi}

<!--DRAFT - This section requires a validation-->

>[!CONTEXTUALHELP]
>id="acw_keyindicators_sent"
>title="Enviado"
>abstract="Esta métrica muestra, para el canal de correo postal, la suma de todos los mensajes enviados y el porcentaje de mensajes enviados al proveedor, en comparación con el número total de mensajes preparados durante la fase de preparación de la entrega."

Durante la fase de preparación, se genera el archivo de extracción de correo postal, pero la información sobre los destinatarios (es decir, registros de envío) no se actualiza.  El estado de una entrega se movió de Envío pendiente a Enviado cuando el usuario de Campaign confirma la entrega de la entrega. A continuación, la entrega se establece en Finished.

Nunca puede ser el 100% de los mensajes enviados en comparación con el total de mensajes preparados, ya que algunas direcciones pueden faltar o estar incompletas.

El **Enviado** Este indicador muestra los siguientes KPI, para el canal de correo postal:

* Porcentaje del número de mensajes enviados comparado con el número total de mensajes preparados.

* Suma de todos los mensajes enviados.

