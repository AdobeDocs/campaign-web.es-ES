---
audience: end-user
title: Uso de la actividad de flujo de trabajo Consulta incremental
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Consulta incremental
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 13%

---

# Consulta incremental {#incremental-query}

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Consulta incremental"
>abstract="La actividad de **Consulta incremental** es una actividad de **Segmentación** que permite consultar la base de datos utilizando el modelador de consultas. Cada vez que se ejecuta esta actividad, se excluyen los resultados de las ejecuciones anteriores. Esto permite buscar solo elementos nuevos."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Historial de consultas incrementales"
>abstract="Historial de consultas incrementales"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Datos procesados de consulta incremental"
>abstract="Datos procesados de consulta incremental"

La actividad **Incremental query** es una actividad **Segmentación** que le permite consultar la base de datos de forma programada. Cada vez que se ejecuta esta actividad, se excluyen los resultados de las ejecuciones anteriores. Esto permite dirigirse únicamente a los elementos nuevos.

>[!NOTE]
>
>Aunque la consola del cliente de Campaign integra la actividad **[!UICONTROL Incremental query]** con un programador integrado, la interfaz de usuario web de Campaign trata esta funcionalidad por separado. Para programar ejecuciones de consultas incrementales, agregue una actividad **[!UICONTROL Scheduler]** en el flujo de trabajo antes de la actividad **[!UICONTROL Incremental query]**. [Aprenda a configurar una actividad de Planificador](scheduler.md)

La actividad **[!UICONTROL Incremental query]** se puede usar para varios propósitos:

* Segmentación de individuos para definir el destinatario de un mensaje, la audiencia u otras operaciones.
* Exportación de datos. Por ejemplo, utilice la actividad para exportar con regularidad nuevos registros en los archivos. Esto resulta útil para los informes externos o las herramientas de inteligencia empresarial.

La población objetivo de ejecuciones anteriores se almacena en el flujo de trabajo. Dos flujos de trabajo iniciados desde la misma plantilla no comparten el mismo registro. Sin embargo, dos tareas basadas en la misma consulta incremental en el mismo flujo de trabajo utilizan el mismo registro.

Si el resultado de una consulta incremental es igual a 0 durante una de sus ejecuciones, el flujo de trabajo se detiene hasta la siguiente ejecución programada de la consulta. Las transiciones y actividades que siguen a la consulta incremental no se procesan antes de la siguiente ejecución.

## Configuración de la actividad Consulta incremental {#incremental-query-configuration}

Siga estos pasos para configurar la actividad **Incremental query**:

[Descripción: captura de pantalla que muestra la interfaz de configuración para la actividad Consulta incremental en Adobe Campaign.]\
![](../assets/incremental-query.png)

1. Agregue una actividad **Incremental query** a su flujo de trabajo.

1. En la sección **[!UICONTROL Audiencia]**, elija la **Dimensión de segmentación** y luego haga clic en **[!UICONTROL Continuar]**.

   La dimensión de segmentación define la población objetivo de la operación, como destinatarios, beneficiarios de contratos, operadores o suscriptores. De forma predeterminada, el público destinatario se selecciona entre los destinatarios. [Más información sobre las dimensiones de segmentación](../../audience/about-recipients.md#targeting-dimensions)

1. Utilice el modelador de consultas para definir la consulta, de forma similar a como crea una audiencia al diseñar un nuevo correo electrónico. [Aprenda a trabajar con el modelador de consultas](../../query/query-modeler-overview.md)

1. En la sección **[!UICONTROL Datos procesados]**, seleccione el modo incremental que desea utilizar:

   * **[!UICONTROL Excluir resultados de ejecuciones anteriores]**: Cada vez que se ejecuta la actividad, se excluyen los resultados de las ejecuciones anteriores.

     Los registros ya segmentados en ejecuciones anteriores se pueden registrar durante un número máximo de días desde el día en que fueron segmentados. Utilice el campo **[!UICONTROL Historial en días]** para establecer este valor. Si este valor es cero, los destinatarios nunca se eliminan del registro.

   * **[!UICONTROL Usar un campo de fecha]**: esta opción excluye los resultados de ejecuciones anteriores en función de un campo de fecha específico. Elija el campo de fecha deseado de la lista de atributos disponibles para la dimensión de segmentación seleccionada. En ejecuciones posteriores del flujo de trabajo, solo se recuperan los datos modificados o creados después de la última fecha de ejecución.

     Después de la primera ejecución del flujo de trabajo, está disponible el campo **[!UICONTROL Última fecha de ejecución]**. Especifica la fecha utilizada para la siguiente ejecución y se actualiza automáticamente cada vez que se ejecuta el flujo de trabajo. Puede anular manualmente este valor para adaptarlo a sus necesidades.

   >[!NOTE]
   >
   >El modo **[!UICONTROL Usar un campo de fecha]** proporciona más flexibilidad según el campo de fecha seleccionado. Por ejemplo, si el campo especificado corresponde a una fecha de modificación, el modo de campo de fecha recupera los datos actualizados recientemente. El otro modo excluye las grabaciones ya segmentadas en una ejecución anterior, incluso si se han modificado desde la última ejecución del flujo de trabajo.

## Ejemplo {#incremental-query-example}

En el siguiente ejemplo se muestra la configuración de un flujo de trabajo que filtra perfiles en la base de datos de Adobe Campaign cada semana. Se dirige a las personas suscritas al servicio Yoga Newsletter y les envía un correo electrónico de bienvenida.

![Captura de pantalla de un ejemplo de configuración de flujo de trabajo para filtrar perfiles suscritos al servicio Yoga Newsletter.](../assets/incremental-query-example.png)

El flujo de trabajo incluye los siguientes elementos:

* Una actividad **[!UICONTROL Scheduler]** que ejecuta el flujo de trabajo todos los lunes a las 6 a. m.
* Una actividad **[!UICONTROL Incremental query]**, que identifica a todos los suscriptores actuales durante la primera ejecución y solo a los nuevos suscriptores durante las ejecuciones posteriores.
* Una actividad **[!UICONTROL Email delivery]**.