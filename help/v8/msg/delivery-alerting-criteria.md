---
audience: end-user
title: Alertas de envío
description: Aprenda a trabajar con las alertas de entrega.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 21%

---

# Criterios de alertas de envío {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Panel de criterios de alertas de envío"
>abstract="La interfaz de usuario web de Campaign proporciona criterios de alertas predefinidos (envíos con bajo rendimiento, envíos cuya preparación ha fallado...) que puede añadir a su panel. También puede crear sus propios criterios para adaptarlos a sus necesidades."

Campaign interfaz web del usuario proporciona criterios de alerta predefinidos, como envíos con bajo rendimiento o envíos cuya preparación falló, que puede agregar a su panel. También puede crear sus propios criterios para adaptarlos a sus necesidades.

Se puede acceder a los criterios de alerta desde el **menú Alertas de** envío en el panel navegación izquierdo, en el **pestaña Criterios** .

![Lista de criterios de alerta mostrados en el menú Alertas de envío](assets/alerting-criteria-list.png)

## Criterios de alerta predefinidos {#ootb-criteria}

Los criterios de alerta predefinidos están disponibles en Campaign interfaz Web del usuario. Estos criterios cubren una serie de escenarios, que se enumeran a continuación:

* **Envíos fallidos**: cualquier envío programado dentro de un intervalo definido, con un estado erróneo.
* **Envíos con preparación fallida**: Cualquier envío modificado dentro de un rango definido, para el cual el paso de preparación (cálculo destino y generación contenido) ha fallado.
* **Envío con una proporción de errores incorrecta para los rechazos leves**: Cualquier envío programado dentro de un intervalo definido, con un estado de al menos &quot;En curso&quot; y una proporción de errores de rechazos leves mayor que un porcentaje definido.
* **Entrega con relación de error incorrecta para rebotes duros**: Cualquier envío programado dentro de un rango definido, con un estado de al menos &quot;En progreso&quot; y un índice de error de rebote duro mayor que un porcentaje definido.
* **Entregas con inicio pendientes** largos: Cualquier envío programado dentro de un rango definido, con un estado &quot;Inicio pendiente&quot; por más de una duración definida. El estado &quot;Inicio pendiente&quot; significa que el sistema aún no ha tomado en cuenta los mensajes.
* **Entregas con bajo rendimiento**: cualquier envío iniciado durante más de una duración definida, con menos de un porcentaje definido de mensajes procesados y un rendimiento inferior a un valor definido.
* **Entregas en curso**: Cualquier envío programada dentro de un rango definido, con el estado &quot;En progreso&quot;.

>[!NOTE]
>
>Los valores predeterminados se aplican a todos los parámetros para los criterios anteriores. Estos valores pueden personalizarse en la **sección Parámetros** de criterios de la envío alertando a los tableros donde se estén utilizando. [Aprenda a trabajar con paneles](../msg/delivery-alerting-dashboards.md)

## Crear un criterio de alerta {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Crear criterios de alertas de envío"
>abstract="Además de los criterios de alertas predefinidos proporcionados por Adobe Campaign, puede crear sus propios criterios para adaptarlos a sus necesidades."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicadores para añadir en alertas"
>abstract="Seleccione los indicadores que se mostrarán como columnas en la sección &quot;Detalles&quot; de las alertas de correo electrónico."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Tipo de alerta"
>abstract="Especifique el tipo **de** alerta para el criterio, es decir, la etiqueta y el color que se mostrarán junto al criterio envío en la sección &quot;Resumen&quot; de las alertas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Frecuencia del criterio"
>abstract="Controle la frecuencia de alertas por día para cada envío que cumpla el criterio."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Crear un criterio de alerta"
>abstract="Para crear sus propios filtros de envío, cree un nuevo filtro predefinido en la consola Campaign v8 desde el nodo **Administración** > **Configuración** > **Filtros predefinidos**."

Para crear un nuevo criterio, seguir estos pasos:

1. Vaya al menú **Alerta de entrega** en el panel de navegación izquierdo y seleccione la pestaña **Criterios**.
1. Haga clic en el botón **Crear criterios de alerta de envío**.
1. Proporcione una etiqueta para el criterio. El nombre interno se rellena automáticamente y es de solo lectura.
1. Utilice el **filtro de envío aplicado por este criterio** para restringir el ámbito del criterio aplicándole un filtro predefinido.

   En el siguiente ejemplo, se ha seleccionado el **filtro Entregas en curso (critInProgressDeliveries),** lo que significa que el criterio solo tiene en cuenta cuenta entregas con el estado &quot;En progreso&quot;.

   ![Ejemplo de propiedades de criterios de alerta con el filtro seleccionado](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Si ninguna de las filtros predefinidos se ajusta a sus necesidades, póngase en contacto con el administrador para crear su propio filtro. Encontrará información detallada sobre cómo crear filtros predefinidos en la consola Campaign en la documentación](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"} de la [Adobe Campaign v8 (consola).
   >
   >Esta operación solo deben realizarla usuarios avanzados.

1. En la **sección Indicadores para agregar alertas** , elija los indicadores que desea mostrar como columnas en la sección &quot;Detalles&quot; de las alertas correo electrónico.

1. Especifique el **Tipo de alerta** para el criterio, es decir, la etiqueta y el color que se muestran junto al criterio de envío en la sección “Resumen” de las alertas.

1. Utilice la sección **Frecuencia de criterios** para controlar la frecuencia de alertas por día para cada envío que cumpla el criterio:

   * **Este criterio de entrega se repetirá en cada notificación**: muestra una entrega que cumple el criterio en cada alerta de correo electrónico del día.
   * **Este criterio de entrega se envía solamente en la primera ocurrencia del día**: muestra una entrega que cumple el criterio solo en el primer informe del día, sin repetirlo en las alertas de correo electrónico posteriores.