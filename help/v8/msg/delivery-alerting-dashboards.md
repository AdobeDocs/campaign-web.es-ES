---
audience: end-user
title: Alertas de envío
description: Aprenda a trabajar con envío alertas.
exl-id: b91ef82b-f3e9-4704-87a2-0e3f75104572
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 22%

---

# Paneles de alertas de envío {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Paneles de alertas de envío"
>abstract="Las alertas de envío son un sistema de administración de alertas que permite a grupos de usuarios recibir automáticamente notificaciones por correo electrónico con información sobre la ejecución de sus envíos. Los paneles de alertas de envío le permiten especificar quién recibirá alertas por correo electrónico, elegir y configurar los criterios de alerta que se utilizarán para enviar esas alertas y acceder al historial de todas las notificaciones enviadas."

Los paneles de alertas de entrega le permiten especificar quién recibirá correo electrónico alertas, elegir y configurar los criterios de alerta que se utilizarán para enviar esas alertas y acceder al historial de todas las notificaciones enviadas. Se puede acceder a ellas desde el **menú Alerta de** envío en el panel navegación izquierdo, en el **pestaña Paneles** .

![Captura de pantalla que muestra el lista de los paneles de alerta en el menú Alertas de envío.](assets/alerting-dashboard-list.png)

## Crear un panel de envíos {#dashboards}

>[!CONTEXTUALHELP]
>id="acw_delery_alerting_dashboard_create"
>title="Crear panel de alertas de envío"
>abstract="La creación de un panel de alertas de envío permite especificar quién recibirá alertas por correo electrónico, elegir y configurar los criterios de alerta que se utilizarán para enviar esas alertas y acceder al historial de todas las notificaciones enviadas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Parámetros generales de alertas de envío"
>abstract="Especifique las propiedades generales del panel de alertas de envío. El campo **Seleccionar grupo de alertas** permite especificar el **grupo de operadores** que recibirá las alertas enviadas por este panel."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Criterios de alertas de envío"
>abstract="En esta sección, añada los criterios que desee utilizar para enviar alertas desde este panel. Elija entre los criterios predefinidos o cree sus propios criterios para adaptarlos a necesidades específicas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Parámetros de criterios"
>abstract="Los criterios tienen valores de parámetros predeterminados que definen cómo se deben aplicar. Puede cambiar estos valores para adaptarlos a sus necesidades desde esta sección."

Para crear una panel de envío, seguir estos pasos:

1. Navegue hasta el **menú Alerta de** envío en el panel de navegación izquierdo y haga clic en **Crear envío panel**.

   ![Captura de pantalla que muestra la opción Crear envío panel en el menú Alerta de envío.](assets/alerting-dashboard.png)

1. Asigne un nombre a su panel en el **campo Etiquetar** . El **campo Nombre** interno se rellena automáticamente y es de solo lectura.

1. En el **campo Seleccione alerta grupo** , especifique el **operador grupo** para recibir las alertas enviadas por este panel. Todos los miembros del operador seleccionado grupo recibirán las alertas.

   Obtenga más información sobre los permisos y los grupos de operadores en la documentación de [Adobe Campaign v8 (consola)](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. En la **sección Criterios** de alerta de entrega, agregue los criterios que desee usar para enviar alertas. Elija entre criterios predefinidos o cree sus propios criterios para alinearse con necesidades específicas. [Aprenda a trabajar con criterios](../msg/delivery-alerting-criteria.md)

1. Los criterios tienen valores de parámetro predeterminados que definen cómo deben aplicarse. Puede cambiar estos valores para adaptarlos a sus necesidades desde la **sección Parámetros** de criterios.

   ![Captura de pantalla que muestra la sección Parámetros de criterios en la panel envío.](assets/alerting-criteria-parameters.png)

   Por ejemplo, de forma predeterminada, el **parámetro Delivery destino minimum size** criteria está establecido en 50, lo que significa que se incluirá un envío en el alerta enviado por este panel solo si tiene como destino al menos 50 perfiles. Puede cambiar este parámetro si desea incluir entregas direccionamiento menos de 50 perfiles.

   Expanda la sección siguiente para obtener más información sobre cada parámetro de criterio:

   +++Parámetros de criterios disponibles

   * **Envío destino tamaño** mínimo: Por ejemplo, si introduce 100 en este campo, se envía un notificación solo para envíos con un destino igual o superior a 100 destinatarios. Este parámetro se aplica a todos los criterios.
   * **Período de monitoreo antes y después de la fecha de contacto (en horas):** Número de horas antes y después de la hora actual. Solo se tienen en cuenta cuenta las entregas que tienen una fecha de contacto en este intervalo de tiempo. Este parámetro se aplica a todos los criterios. De forma predeterminada, el valor de este campo está establecido en 24 horas.
   * **Proporción máxima de errores** de devolución leve: se envía un notificación para todas las entregas con una proporción de errores de devolución leve superior al valor especificado. De forma predeterminada, el valor de este campo se establece en 0,05 (5%).
   * **Proporción máxima de errores** de devolución dura: se envía un notificación para todas las entregas con una proporción de errores de devolución mayor que el valor especificado. De forma predeterminada, el valor de este campo se establece en 0,05 (5%).
   * **Tiempo mínimo umbral para envío en estado &quot;Inicio pendiente&quot; (en minutos):** Se envía un notificación para todos los envíos con un estado Inicio pendiente durante un período superior al especificado en este campo, Inicio estado pendiente significa que el sistema aún no ha tenido en cuenta cuenta los mensajes.
   * **Tiempo mínimo requerido para el cálculo del rendimiento (en minutos):** Solo se toman en cuenta los envíos iniciados (con estado En curso) durante más de la duración especificada para el criterio Entregas con bajo rendimiento.
   * **Porcentaje máximo de mensajes procesados para el cálculo del rendimiento**: solo se tienen en cuenta cuenta los envíos con un porcentaje de mensajes procesados inferior al porcentaje especificado para el criterio Envíos con bajo rendimiento.
   * **Rendimiento mínimo esperado (en mensajes enviados por hora):** solo se tienen en cuenta cuenta los envíos con un rendimiento inferior al valor especificado para el criterio Envíos con bajo rendimiento.
   * **Proporción mínima procesada requerida para el criterio** &quot;Entregas en curso&quot;: solo se toman en cuenta los envíos con un porcentaje de mensajes procesados superior al porcentaje especificado.

   +++

1. De forma predeterminada, los tableros de alertas están deshabilitados, lo que significa que no se envían correo electrónico alertas vinculadas a este panel. Para habilitar el panel inmediatamente, active la **opción Habilitado** en la **sección General** , junto al campo alerta grupo selección.

   También puede guardar el panel y habilitarlo más tarde.

   ![Captura de pantalla que muestra la opción de alternancia Habilitado en la configuración envío panel.](assets/alerting-dashboard-enable.png)

1. Para guardar el panel de alertas, haga clic en el **botón Guardar** .

La panel alerta se abre con datos en blanco. Cuando esté listo para activarlo y enviar notificaciones, haga clic en el **botón Configuración** y cambie la **opción Habilitado** si no lo ha hecho anteriormente.

Ahora, cada vez que una envío cumple los criterios definidos en este panel, se envía un notificación de alerta al operador especificado grupo.

## Administrar paneles de alertas

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Alertas de envío enviadas"
>abstract="Esta sección le permite visualizar información relacionada con las últimas alertas enviadas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Historial de alertas de envío"
>abstract="El panel **Historial** contiene todas las alertas enviadas desde este panel. Haga clic en un elemento para acceder a las alertas correspondientes enviadas en ese momento concreto."

Se puede acceder a todos los paneles de alerta creados desde el **menú Alertas de** envío, en la **pestaña Tableros** .

![Captura de pantalla que muestra el lista de los paneles de alerta en el menú Alertas de envío.](assets/alerting-dashboard-list.png)

Puede duplicado o eliminar un panel mediante el botón de acciones **&#x200B;**&#x200B;Más junto al nombre.

Para acceder a una vista detallada de una panel, haga clic en su nombre en la lista. Desde esta pantalla, puede visualizar los últimos alerta enviados. Todas las alertas enviadas aparecen en el panel izquierdo. Haga clic en un elemento para acceder a las alertas correspondientes enviadas en ese momento concreto.

![Captura de pantalla que muestra el vista detallado de un panel de alerta.](assets/alerting-dashboard-details.png)

Para editar el panel, haga clic en el **botón Configuración** situado en la esquina superior derecha y realice los cambios deseados.