---
audience: end-user
title: Utilice el consulta incremental flujo de trabajo actividad
description: Aprenda a utilizar la actividad de flujo de trabajo de consulta incremental
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

La **actividad de consulta** incremental es una **actividad de objetivo** que permite consulta la base de datos de forma programada. Cada vez que se ejecuta esta actividad, se excluyen los resultados de las ejecuciones anteriores. Esto permite destino solo elementos nuevos.

>[!NOTE]
>
>Mientras que la consola del cliente Campaign integra el **[!UICONTROL actividad de consulta]** incremental con un planificador integrado, la interfaz del usuario web de Campaign trata esta funcionalidad por separado. Para programar consulta incremental ejecuciones, añada un **[!UICONTROL actividad del programador]** en el flujo de trabajo antes del **[!UICONTROL actividad de consulta]** incremental. [Aprenda a configurar una actividad del programador](scheduler.md)

La **[!UICONTROL actividad de consulta]** incremental puede utilizarse para diversos propósitos:

* Segmentar a los individuos para definir el destino de un mensaje, audiencia u otras operaciones.
* Exportación de datos. Por ejemplo, utilice el actividad para exportar regularmente nuevos registros en archivos. Esto resulta útil para herramientas inteligencia empresarial o sistema de informes externas.

La población ya objeto de ejecuciones anteriores se almacena en el flujo de trabajo. Dos flujos de trabajo iniciados desde la misma plantilla no comparten el mismo registro. Sin embargo, dos tareas basadas en el mismo consulta incremental en el mismo flujo de trabajo utilizar el mismo registro.

Si el resultado de una consulta incremental es igual a 0 durante una de sus ejecuciones, la flujo de trabajo se detiene hasta la siguiente ejecución programada del consulta. Las transiciones y actividades que seguir el consulta incremental no se procesan antes de la siguiente ejecución.

## Configurar el actividad de consulta incremental {#incremental-query-configuration}

Siga estos pasos para configurar el **actividad de consulta** incremental:

[Descripción: captura de pantalla que muestra la interfaz de configuración para el actividad de consulta incremental en Adobe Campaign.]\
![](../assets/incremental-query.png)

1. añadir un **actividad de consulta** incremental en su flujo de trabajo.

1. En la **[!UICONTROL sección Audiencia]**, selecciona el dimensión **Segmentación** y haz clic en **[!UICONTROL Continuar]**.

   El dimensión de segmentación define la población objetivo de la operación, como destinatarios, beneficiarios del contrato, operadores o suscriptores. De forma predeterminada, el público destinatario se selecciona entre los destinatarios. [Más información sobre direccionamiento dimensiones](../../audience/about-recipients.md#targeting-dimensions)

1. Utilice el modelador de consulta para definir su consulta, de forma similar a como se crea una audiencia al diseñar una nueva correo electrónico. [Aprenda a trabajar con el consulta modelador](../../query/query-modeler-overview.md)

1. En la **[!UICONTROL sección Datos procesados]** , seleccione el modo incremental que desea utilizar:

   * **[!UICONTROL Excluir resultados de ejecución anterior]**: Cada vez que se ejecuta el actividad, se excluyen los resultados de las ejecuciones anteriores.

     Los registros ya seleccionados en ejecuciones anteriores pueden registrarse durante un número máximo de días desde el día en que fueron seleccionados. Utilice el **[!UICONTROL campo Historial en días]** para establecer este valor. Si este valor es cero, los destinatarios nunca se eliminan del registro.

   * **[!UICONTROL Utilizar un campo]** de fecha: esta opción excluye los resultados de ejecuciones anteriores basadas en un campo de fecha específico. Elija el campo de fecha deseado entre los lista de atributos disponibles para el dimensión de segmentación seleccionado. En las ejecuciones posteriores del flujo de trabajo, solo se recuperarán los datos modificados o creados después de la última fecha de ejecución.

     Tras la primera ejecución del flujo de trabajo, aparecerá disponible el **[!UICONTROL campo Fecha de la última ejecución]** . Especifica la fecha utilizada para la siguiente ejecución y se actualiza automáticamente cada vez que se ejecuta el flujo de trabajo. Puede anular manualmente este valor para ajustarlo a sus necesidades.

   >[!NOTE]
   >
   >El **[!UICONTROL modo Usar un campo]** de fecha proporciona más flexibilidad en función del campo de fecha seleccionado. Por ejemplo, si el campo especificado corresponde a una fecha de modificación, el modo de campo de fecha recupera los datos actualizados recientemente. El otro modo excluye las grabaciones ya segmentadas en una ejecución anterior, igualado si han sido modificadas desde la última ejecución del flujo de trabajo.

## Ejemplo {#incremental-query-example}

En el ejemplo siguiente se muestra la configuración de una flujo de trabajo que filtros perfiles en la base de datos de Adobe Campaign cada semana. Se dirige a las personas suscritas al servicio de Newsletter de Yoga y les envía un correo electrónico de bienvenida.

![Captura de pantalla de un ejemplo flujo de trabajo configuración para filtrar perfiles suscritos al servicio Yoga Newsletter.](../assets/incremental-query-example.png)

La flujo de trabajo incluye los siguientes elementos:

* Un **[!UICONTROL actividad programador]** que ejecuta el flujo de trabajo todos los lunes a las 6 a. m.
* Un **[!UICONTROL actividad de consulta]** incremental, dirigido a todos los suscriptores actuales durante la primera ejecución y solo a los nuevos suscriptores durante las ejecuciones posteriores.
* Un **[!UICONTROL correo electrónico envío]** actividad.