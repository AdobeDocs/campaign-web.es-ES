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
>abstract="La interfaz de usuario web de Campaign proporciona criterios de alerta predefinidos (envíos con bajo rendimiento, envíos cuya preparación ha fallado...) que puede añadir a su panel. También puede crear sus propios criterios para adaptarlos a sus necesidades."

La interfaz de usuario web de Campaign proporciona criterios de alerta predefinidos (entregas con bajo rendimiento, entregas cuya preparación ha fallado...) que puede añadir a su panel. También puede crear sus propios criterios para adaptarlos a sus necesidades.

Los criterios de alerta son accesibles desde el **Alerta de envío** menú en el panel de navegación izquierdo, bajo el **Criterios** pestaña.

![](assets/alerting-criteria-list.png)

## Criterios de alerta predefinidos {#ootb-criteria}

Los criterios de alerta predefinidos están disponibles en la interfaz de usuario web de Campaign. Estos criterios abarcan una serie de escenarios, que se enumeran a continuación:

* **Error de envíos**: Cualquier envío programado dentro de un intervalo definido, con un estado erróneo.
* **Envíos con error de preparación**: Cualquier entrega modificada dentro de un intervalo definido, para el cual el paso de preparación (cálculo del objetivo y generación de contenido) ha fallado.
* **Envío con una proporción de errores incorrecta para devoluciones suaves**: Cualquier entrega programada dentro de un intervalo definido, con un estado al menos En curso, con una proporción de errores de devolución suave mayor que un porcentaje definido.
* **Envío con una proporción de errores incorrecta para devoluciones graves**: Cualquier entrega programada dentro de un intervalo definido, con un estado al menos En curso, con una proporción de errores de devolución dura mayor que un porcentaje definido.
* **Envíos con inicio largo pendiente**: cualquier entrega programada dentro de un intervalo definido, con un estado Start pending por más tiempo que una duración definida; el estado Start pending significa que el sistema aún no ha tenido en cuenta los mensajes.
* **Envíos con bajo rendimiento**: Cualquier envío que se inicie durante más tiempo del definido, con menos de un porcentaje definido de mensajes procesados, con un rendimiento inferior a un valor definido.
* **Entregas en curso**: Cualquier entrega programada dentro de un intervalo definido, con el estado En curso.

>[!NOTE]
>
>Los valores predeterminados se aplican a todos los parámetros para los criterios anteriores. Estos valores se pueden personalizar en la variable **Parámetros de criterio** de los paneles de alertas de envío donde se utilizan. [Aprenda a trabajar con paneles](../msg/delivery-alerting-dashboards.md)

## Crear un criterio de alerta {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Crear criterios de alertas de envío"
>abstract="Además de los criterios de alerta predefinidos proporcionados por Adobe Campaign, puede crear sus propios criterios para adaptarlos a sus necesidades."

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
>title="Frecuencia de criterios"
>abstract="Controle la frecuencia de alertas por día para cada envío que cumpla el criterio."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Crear un criterio de alerta"
>abstract="Para crear sus propios filtros de envío, cree un nuevo filtro predefinido en la consola Campaign v8 desde el nodo **Administración** > **Configuración** > **Filtros predefinidos**."

Para crear un nuevo criterio, siga estos pasos:

1. Vaya a **Alerta de envío** en el panel de navegación izquierdo y seleccione la opción **Criterios** pestaña.
1. Haga clic en **Crear criterios de alerta de envío** botón.
1. Proporcione una etiqueta para el criterio. El nombre interno se rellena automáticamente y es de solo lectura.
1. El **Filtro de envío aplicado según estos criterios** permite refinar el ámbito del criterio al aplicarle un filtro predefinido.

   En el ejemplo siguiente, la variable **Envíos en curso (criptInProgressDeliveries)** se ha seleccionado, lo que significa que el criterio solo tiene en cuenta las entregas con el estado &quot;En curso&quot;.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Si ninguno de los filtros predefinidos se adapta a sus necesidades, puede ponerse en contacto con el administrador para crear su propio filtro.  Encontrará información detallada sobre cómo crear filtros predefinidos en la consola de Campaign en la [Documentación de Adobe Campaign v8 (consola)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Esta operación solo deben realizarla usuarios avanzados.

1. En el **Indicadores para añadir en alertas** , elija los indicadores que se mostrarán como columnas en la sección &quot;Detalles&quot; de las alertas de correo electrónico.

1. Especifique el **Tipo de alerta** para el criterio, es decir, la etiqueta y el color que se muestran junto al criterio de envío en la sección “Resumen” de las alertas.

1. El **Frecuencia de criterios** Esta sección permite controlar la frecuencia de alertas por día para cada entrega que cumpla los criterios:

   * **Este criterio de entrega se repite en cada notificación**: muestra una entrega que cumple el criterio en cada alerta de correo electrónico del día.
   * **Este criterio de entrega solo se envía en la primera aparición del día**: muestra una entrega que cumple el criterio solo en el primer informe del día, no se repite en las alertas de correo electrónico posteriores.
