---
audience: end-user
title: Alertas de envío
description: Aprenda a trabajar con las alertas de entrega.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 26%

---

# Criterios de alertas de envío {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Panel de criterios de alertas de envío"
>abstract="La interfaz de usuario web de Campaign proporciona criterios de alertas predefinidos (envíos con bajo rendimiento, envíos cuya preparación ha fallado...) que puede añadir a su panel. También puede crear sus propios criterios para adaptarlos a sus necesidades."

La interfaz de usuario web de Campaign proporciona criterios de alerta predefinidos (entregas con bajo rendimiento, entregas cuya preparación ha fallado...) que puede añadir a su panel. También puede crear sus propios criterios para adaptarlos a sus necesidades.

Se puede acceder a los criterios de alerta desde el menú **Alerta de entrega** del panel de navegación izquierdo, en la pestaña **Criterios**.

![](assets/alerting-criteria-list.png)

## Criterios de alerta predefinidos {#ootb-criteria}

Los criterios de alerta predefinidos están disponibles en la interfaz de usuario web de Campaign. Estos criterios abarcan una serie de escenarios, que se enumeran a continuación:

* **Entregas con error**: Cualquier entrega programada dentro de un intervalo definido, con un estado erróneo.
* **Envíos con error de preparación**: Cualquier envío modificado dentro de un intervalo definido, para el cual el paso de preparación (cálculo del objetivo y generación de contenido) ha fallado.
* **Envío con una proporción de errores incorrecta para los rechazos leves**: Cualquier envío programado dentro de un intervalo definido, con un estado al menos En curso, con una proporción de errores de rechazos leves mayor que un porcentaje definido.
* **Envío con una proporción de errores incorrecta para los rechazos graves**: Cualquier envío programado dentro de un intervalo definido, con un estado al menos En curso, con una proporción de errores de rechazos graves mayor que un porcentaje definido.
* **Envíos con inicio largo pendiente**: Cualquier envío programado dentro de un intervalo definido, con un estado de Inicio pendiente durante más de una duración definida; el estado de Inicio pendiente significa que el sistema aún no ha tenido en cuenta los mensajes.
* **Envíos con bajo rendimiento**: Cualquier envío se inició durante más tiempo que una duración definida, con menos de un porcentaje definido de mensajes procesados, con un rendimiento inferior a un valor definido.
* **Envíos en curso**: Cualquier envío programado dentro de un intervalo definido, con el estado En curso.

>[!NOTE]
>
>Los valores predeterminados se aplican a todos los parámetros para los criterios anteriores. Estos valores se pueden personalizar en la sección **Parámetros de criterios** de los paneles de alertas de envío donde se utilizan. [Aprenda a trabajar con paneles](../msg/delivery-alerting-dashboards.md)

## Crear un criterio de alerta {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Crear criterios de alertas de envío"
>abstract="Además de los criterios de alertas predefinidos proporcionados por Adobe Campaign, puede crear sus propios criterios para adaptarlos a sus necesidades."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicadores para añadir en alertas"
>abstract="Seleccione los indicadores que se mostrarán como columnas en la sección “Detalles” de las alertas de correo electrónico."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Tipo de alerta"
>abstract="Especifique el **Tipo de alerta** para el criterio, es decir, la etiqueta y el color que se muestran junto al criterio de envío en la sección “Resumen” de las alertas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Frecuencia del criterio"
>abstract="Controle la frecuencia de alertas por día para cada envío que cumpla el criterio."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Crear un criterio de alerta"
>abstract="Para crear sus propios filtros de envío, cree un nuevo filtro predefinido en la consola Campaign v8 desde el nodo **Administración** > **Configuración** > **Filtros predefinidos**."

Para crear un nuevo criterio, siga estos pasos:

1. Vaya al menú **Delivery Àlerting** en el panel de navegación izquierdo y seleccione la pestaña **Criterios**.
1. Haga clic en el botón **Crear criterios de alerta de envío**.
1. Proporcione una etiqueta para el criterio. El nombre interno se rellena automáticamente y es de solo lectura.
1. El filtro de **envío aplicado según estos criterios** le permite restringir el ámbito del criterio al aplicarle un filtro predefinido.

   En el ejemplo siguiente, se ha seleccionado el filtro **Deliveries in progress (criptInProgressDeliveries)**, lo que significa que el criterio solo tiene en cuenta las entregas con el estado &quot;En curso&quot;.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Si ninguno de los filtros predefinidos se adapta a sus necesidades, puede ponerse en contacto con el administrador para crear su propio filtro.  Encontrará información detallada sobre cómo crear filtros predefinidos en la consola de Campaign en la [documentación de Adobe Campaign v8 (consola)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Esta operación solo deben realizarla usuarios avanzados.

1. En la sección **Indicadores que se agregarán en las alertas**, elija los indicadores que se mostrarán como columnas en la sección &quot;Detalles&quot; de las alertas de correo electrónico.

1. Especifique el **Tipo de alerta** para el criterio, es decir, la etiqueta y el color que se muestran junto al criterio de envío en la sección “Resumen” de las alertas.

1. La sección **Frecuencia de criterios** le permite controlar la frecuencia de alertas por día para cada envío que cumpla con el criterio:

   * **Este criterio de entrega se repetirá en cada notificación**: muestra una entrega que cumple el criterio en cada alerta de correo electrónico del día.
   * **Este criterio de entrega se envía solamente en la primera aparición del día**: muestra una entrega que cumple el criterio solo en el primer informe del día, no se repite en las alertas de correo electrónico posteriores.
