---
audience: end-user
title: Uso de la actividad de flujo de trabajo Consulta incremental
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Consulta incremental
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 23%

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

La actividad **Incremental query** es una actividad **Segmentación** que le permite consultar la base de datos de forma programada. Cada vez que se ejecuta esta actividad, se excluyen los resultados de las ejecuciones anteriores. Esto permite buscar solo elementos nuevos.

>[!NOTE]
>
>Aunque la consola del cliente de Campaign integra la actividad **[!UICONTROL Incremental query]** con un programador integrado, la interfaz de usuario web de Campaign trata esta funcionalidad por separado. Para programar ejecuciones de consultas incrementales, debe agregar una actividad **[!UICONTROL Scheduler]** en el flujo de trabajo antes de la actividad **[!UICONTROL Incremental query]**. [Aprenda a configurar una actividad de Planificador](scheduler.md)

La actividad **[!UICONTROL Incremental query]** se puede usar para varios tipos de usos:

* Segmentación de individuos para definir el destinatario de un mensaje, la audiencia, etc.
* Exportación de datos. Por ejemplo, puede utilizar la actividad para exportar con regularidad nuevos registros en los archivos. Puede resultar útil si desea utilizar los datos de registro en herramientas externas de sistema de informes o BI.

La población objetivo de ejecuciones anteriores se almacena en el flujo de trabajo. Esto significa que dos flujos de trabajo iniciados desde la misma plantilla no comparten el mismo registro. Sin embargo, dos tareas basadas en la misma consulta incremental en el mismo flujo de trabajo utilizan el mismo registro.

Si el resultado de una consulta incremental es igual a 0 durante una de sus ejecuciones, el flujo de trabajo se detiene hasta la siguiente ejecución programada de la consulta. Por lo tanto, las transiciones y actividades que siguen a la consulta incremental no se procesan antes de la siguiente ejecución.

## Configuración de la actividad Consulta incremental {#incremental-query-configuration}

Siga estos pasos para configurar la actividad **Incremental query**:

![](../assets/incremental-query.png)

1. Agregue una actividad **Incremental query** a su flujo de trabajo.

1. En la sección **[!UICONTROL Audiencia]**, elija la **Dimensión de segmentación** y luego haga clic en **[!UICONTROL Continuar]**.

   La dimensión de segmentación permite definir la población a la que se dirige la operación: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. De forma predeterminada, el público destinatario se selecciona entre los destinatarios. [Más información sobre las dimensiones de segmentación](../../audience/about-recipients.md#targeting-dimensions)

1. Utilice el modelador de consultas para definir la consulta, del mismo modo que crea una audiencia al diseñar un nuevo correo electrónico. [Aprenda a trabajar con el modelador de consultas](../../query/query-modeler-overview.md)

1. En la sección **[!UICONTROL Datos procesados]**, seleccione el modo incremental que desea utilizar:

   * **[!UICONTROL Excluir resultados de ejecuciones anteriores]**: Cada vez que se ejecuta la actividad, se excluyen los resultados de las ejecuciones anteriores.

     Los registros ya segmentados en ejecuciones anteriores se pueden registrar un número máximo de días desde el día en que fueron segmentados. Para ello, use el campo **[!UICONTROL Historial en días]**. Si este valor es cero, los destinatarios nunca se eliminan del registro.

   * **[!UICONTROL Usar un campo de fecha]**: esta opción le permite excluir los resultados de ejecuciones anteriores en función de un campo de fecha específico. Para ello, elija el campo de fecha deseado de la lista de atributos disponibles para la dimensión de segmentación seleccionada. En las siguientes ejecuciones del flujo de trabajo, solo se recuperan los datos que se han modificado o creado después de la última fecha de ejecución.

     Después de la primera ejecución del flujo de trabajo, está disponible el campo **[!UICONTROL Última fecha de ejecución]**. Especifica la fecha que se utiliza para la siguiente ejecución y se actualiza automáticamente cada vez que se ejecuta el flujo de trabajo. Todavía tiene la posibilidad de anular este valor introduciendo manualmente uno nuevo para que se ajuste a sus necesidades.

   >[!NOTE]
   >
   >El modo **[!UICONTROL Usar un campo de fecha]** permite una mayor flexibilidad según el campo de fecha seleccionado. Por ejemplo, si el campo especificado corresponde a una fecha de modificación, el modo de campo de fecha permite recuperar datos que se han actualizado recientemente, mientras que el otro modo excluye simplemente las grabaciones que ya estaban segmentadas en una ejecución anterior, incluso si se han modificado desde la última ejecución del flujo de trabajo.

## Ejemplo {#incremental-query-example}

El siguiente ejemplo muestra la configuración de un flujo de trabajo que filtra cada semana los perfiles de la base de datos de Adobe Campaign suscritos al servicio Yoga Newsletter para enviarles un correo electrónico de bienvenida.

![](../assets/incremental-query-example.png)

El flujo de trabajo se compone de los siguientes elementos:

* Una actividad **[!UICONTROL Scheduler]** para ejecutar el flujo de trabajo todos los lunes a las 6 a. m.
* Una actividad **[!UICONTROL Incremental query]**, que identifica a todos los suscriptores actuales durante la primera ejecución y luego solo a los nuevos suscriptores de esa semana durante las siguientes ejecuciones.
* Una actividad **[!UICONTROL Email delivery]**.
