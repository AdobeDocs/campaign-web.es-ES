---
title: Indicadores clave de rendimiento
description: Descubra cómo comprender los indicadores de rendimiento clave
badge: label="Beta"
source-git-commit: e784f9aeb0805269561065c10ccbbf6756e62e44
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 98%

---

# Indicadores clave de rendimiento {#kpis}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_spam"
>title="Spam"
>abstract="KPI de spam"

Examine la página de inicio para comprobar los indicadores clave de rendimiento de su plataforma. Dichos indicadores muestran la cantidad y el porcentaje de mensajes enviados, abiertos y clicados, así como las bajas y las tasas de error.

De forma predeterminada, las métricas se calculan para los envíos realizados durante los 7 días anteriores. Puede cambiar el período en la lista desplegable de la sección superior derecha de la tarjeta. Se excluyen los mensajes enviados a perfiles de prueba.

Puede seleccionar el canal que desea mostrar. De forma predeterminada, los indicadores reflejan las métricas del canal de correo electrónico.

![](assets/kpi.png)

## Mensaje enviado {#ui-delivered-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_delivered"
>title="Entregados"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todos los mensajes procesados correctamente y el porcentaje de mensajes enviados correctamente en comparación con la cantidad total de mensajes enviados."

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
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todos los mensajes abiertos y el porcentaje de mensajes abiertos en comparación con la cantidad total de mensajes enviados correctamente."

El total de aperturas se calcula realizando un seguimiento de la cantidad total de veces que se abre un mensaje, independientemente de cuántas personas destinatarias hayan generado dichas aperturas. Este indicador solo está disponible para correos electrónicos.

Para cada canal, el indicador **Aperturas** muestra los siguientes indicadores clave de rendimiento (KPI):

* Porcentaje de mensajes abiertos en comparación con el número total de mensajes enviados correctamente.

* Suma de todos los mensajes abiertos, por canal.

Adobe Campaign detecta que el mensaje se abre cuando la persona destinataria descarga las imágenes del correo electrónico. Los correos electrónicos HTML con varias partes o alternativos incluyen una imagen de 0 píxeles que permite detectar qué mensajes se han abierto. Dado que los mensajes en formato de texto no incluyen imágenes, es imposible detectar si se han abierto o no. Los valores calculados basados en las aperturas de mensajes siempre son estimaciones debido al margen del error relacionado con la visualización de la imagen.



## Tasa de clics {#ui-click-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_clicks"
>title="Clics"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las URL clicadas de los mensajes y el porcentaje de clics comparado con la cantidad total de mensajes enviados correctamente."

Puede añadir URL en el contenido del mensaje para redirigir a una página concreta. La tasa de clics mide la cantidad y el porcentaje de personas que hicieron clic en un vínculo del mensaje.

Para cada canal, el indicador **Clics** muestra los siguientes indicadores clave de rendimiento (KPI):

* Porcentaje de clics en comparación con la cantidad total de mensajes enviados correctamente.

* Cantidad de personas diferentes que han hecho clic al menos una vez en un envío. Se excluyen los vínculos de baja y los vínculos a la página espejo de correo electrónico.

Estas métricas se basan en la tabla Seguimiento consolidado (`nms:trackingStats`). Esta tabla de acumulados se utiliza por motivos de rendimiento al mostrar los informes, en lugar de la tabla Registros de seguimiento de destinatarios (`nms:trackingLogRcp`), y no se calcula en tiempo real. La tabla se genera unos minutos después de recuperar los registros de seguimiento.


## Tasas de baja {#ui-unsub-kpi}

>[!CONTEXTUALHELP]
>id="acw_keyindicators_unsubscriptions"
>title="Bajas"
>abstract="Esta métrica muestra, para el canal seleccionado, la suma de todas las bajas de un servicio y el porcentaje de bajas en comparación con la cantidad total de mensajes enviados correctamente."

Las personas deben poder pedir la exclusión de los correos electrónicos y los SMS mediante un vínculo de baja específico en el contenido del correo electrónico o respondiendo DETENER a un SMS.

Para cada canal, el indicador **Bajas** muestra los siguientes indicadores clave de rendimiento (KPI):

* Porcentaje de bajas en comparación con la cantidad total de mensajes enviados correctamente.

* Suma de todos los clics hechos en un vínculo de baja, es decir, que tengan una categoría URL igual a &quot;Exclusión&quot;.


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
