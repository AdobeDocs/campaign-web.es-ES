---
audience: end-user
title: Alertas de envío
description: Aprenda a trabajar con las alertas de entrega.
hidefromtoc: true
hide: true
robots: noindex
googlebot: noindex
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: 19a7540af7502709b7eafdace038b5958e077173
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 24%

---

# Criterios de alertas de envío {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Panel de criterios de alertas de envío"
>abstract="La interfaz de usuario web de Campaign proporciona criterios de alertas predefinidos (envíos con bajo rendimiento, envíos cuya preparación ha fallado...) que puede añadir a su panel. También puede crear sus propios criterios para adaptarlos a sus necesidades."

La interfaz de usuario web de Campaign proporciona criterios de alerta predefinidos, como envíos con bajo rendimiento o envíos cuya preparación ha fallado, que puede añadir al panel. También puede crear sus propios criterios para adaptarlos a sus necesidades.

Se puede acceder a los criterios de alerta desde el menú **Alerta de entrega** del panel de navegación izquierdo, en la pestaña **Criterios**.

![Lista de criterios de alerta mostrados en el menú Alerta de entrega](assets/alerting-criteria-list.png)

## Criterios de alerta predefinidos {#ootb-criteria}

Los criterios de alerta predefinidos están disponibles en la interfaz de usuario web de Campaign. Estos criterios abarcan una serie de escenarios, que se enumeran a continuación:

* **Entregas con error**: Cualquier entrega programada dentro de un intervalo definido, con un estado erróneo.
* **Envíos con error de preparación**: Cualquier envío modificado dentro de un intervalo definido, para el cual el paso de preparación (cálculo del objetivo y generación de contenido) ha fallado.
* **Envío con una proporción de errores incorrecta para los rechazos leves**: Cualquier envío programado dentro de un intervalo definido, con un estado de al menos &quot;En curso&quot; y una proporción de errores de rechazos leves mayor que un porcentaje definido.
* **Envío con una proporción de errores incorrecta para los rechazos graves**: Cualquier envío programado dentro de un intervalo definido, con un estado de al menos &quot;En curso&quot; y una proporción de errores de rechazos graves mayor que un porcentaje definido.
* **Envíos con inicio largo pendiente**: Cualquier envío programado dentro de un intervalo definido, con un estado de &quot;Inicio pendiente&quot; durante más de una duración definida. El estado &quot;Inicio pendiente&quot; significa que el sistema aún no ha tenido en cuenta los mensajes.
* **Envíos con bajo rendimiento**: Cualquier envío se inició durante más tiempo que una duración definida, con menos de un porcentaje definido de mensajes procesados y un rendimiento inferior a un valor definido.
* **Envíos en curso**: Cualquier envío programado dentro de un intervalo definido, con el estado &quot;En curso&quot;.

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

Para crear un nuevo criterio, siga estos pasos:

1. Vaya al menú **Alerta de entrega** en el panel de navegación izquierdo y seleccione la pestaña **Criterios**.
1. Haga clic en el botón **Crear criterios de alerta de envío**.
1. Proporcione una etiqueta para el criterio. El nombre interno se rellena automáticamente y es de solo lectura.
1. Use el filtro de **envío aplicado por estos criterios** para restringir el ámbito del criterio al aplicarle un filtro predefinido.

   En el ejemplo siguiente, se ha seleccionado el filtro **Deliveries in progress (criptInProgressDeliveries)**, lo que significa que el criterio solo tiene en cuenta las entregas con el estado &quot;En curso&quot;.

   ![Ejemplo de propiedades de criterios de alerta con el filtro seleccionado](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Si ninguno de los filtros predefinidos se ajusta a sus necesidades, puede crear los suyos propios en el menú **Administración de clientes** > **Filtros predefinidos**. [Más información](../get-started/predefined-filters.md)
   >
   >Esta operación solo deben realizarla usuarios avanzados.

1. En la sección **Indicadores que se agregarán en las alertas**, elija los indicadores que se mostrarán como columnas en la sección &quot;Detalles&quot; de las alertas de correo electrónico.

1. Especifique el **Tipo de alerta** para el criterio, es decir, la etiqueta y el color que se muestran junto al criterio de envío en la sección “Resumen” de las alertas.

1. Utilice la sección **Frecuencia de criterios** para controlar la frecuencia de alertas por día para cada envío que cumpla el criterio:

   * **Este criterio de entrega se repetirá en cada notificación**: muestra una entrega que cumple el criterio en cada alerta de correo electrónico del día.
   * **Este criterio de entrega se envía solamente en la primera ocurrencia del día**: muestra una entrega que cumple el criterio solo en el primer informe del día, sin repetirlo en las alertas de correo electrónico posteriores.