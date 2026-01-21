---
audience: end-user
title: Trabajar con actividades de flujos de trabajo
description: Aprenda a trabajar con las actividades de flujo de trabajo
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 61f3a2bff32bba1e202d3e811e9f116f3987c191
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 20%

---

# Acerca de las actividades de flujo de trabajo {#workflow-activities}

Las actividades de flujo de trabajo se agrupan en tres categorías. Dependiendo del contexto, las actividades disponibles pueden diferir.

Todas las actividades se detallan en las secciones siguientes:

* [Actividades de segmentación y administración de datos](#targeting)
* [Actividades del canal](#channel)
* [Actividades de control de flujo](#flow-control)

![Resumen de actividades de flujo de trabajo](../assets/workflow-activities.png)

## Actividades de segmentación {#targeting}

Estas actividades son específicas de la segmentación. Permiten crear una o más audiencias de destino definiendo una audiencia y dividiendo o combinando estas audiencias mediante operaciones de intersección, unión o exclusión.

* [Generar audiencia](build-audience.md): defina la población objetivo. Seleccione una audiencia existente o utilice el modelador de consultas para definir su propia consulta.
* [Cambiar origen de datos](change-data-source.md): cambie el origen de datos de la tabla de trabajo del flujo de trabajo.
* [Cambiar dimensión](change-dimension.md): cambie la dimensión de segmentación al crear el flujo de trabajo.
* [Combinar](combine.md): realice la segmentación en la población entrante. Utilice una unión, una intersección o una exclusión.
* [Anulación de duplicación](deduplication.md): elimine duplicados en los resultados de las actividades entrantes.
* [Enriquecimiento](enrichment.md): defina datos adicionales para procesar en el flujo de trabajo. Configure la actividad para completar la transición de salida con datos adicionales.
* [Consulta incremental](incremental-query.md): consulte la base de datos de forma programada. Cada vez que se ejecuta esta actividad, excluye los resultados de ejecuciones anteriores, dirigiéndose únicamente a los elementos nuevos.
* [Reconciliación](reconciliation.md): defina el vínculo entre los datos de la base de datos de Adobe Campaign y los datos de una tabla de trabajo, como los datos cargados desde un archivo externo.
* [Guardar audiencia](save-audience.md): actualice una audiencia existente o cree una nueva a partir de la población calculada en sentido ascendente en un flujo de trabajo.
* [Split](split.md): Segmente la población entrante en varios subconjuntos.

## Actividades de administración de datos {#data}

Estas actividades son específicas para manipular y enriquecer datos de población.

* [Extraer archivo](extract-file.md): Exporte datos de Adobe Campaign a otro sistema como un archivo externo.
* [Cargar archivo](load-file.md): Trabaje con perfiles y datos almacenados en un archivo externo.
* [Transferir archivo](transfer-file.md): Reciba o envíe archivos, pruebe la presencia de archivos o enumere archivos en un servidor. El protocolo que se utiliza puede ser un protocolo de servidor a servidor o el protocolo HTTP.
* [JavaScript code](javascript-code.md): ejecute un fragmento de código JavaScript en el contexto de un flujo de trabajo.
* [Servicios de suscripción](subscription-services.md): suscriba o cancele la suscripción de varios perfiles a o desde un servicio en una sola acción.
* [Actualizar datos](update-data.md): realice actualizaciones masivas en los campos de la base de datos. Varias opciones permiten personalizar la actualización de datos.

## Actividades del canal {#channel}

Adobe Campaign Web le permite automatizar y ejecutar campañas de marketing en varios canales. Combine actividades de canal en el lienzo para crear flujos de trabajo entre canales que almacenen en déclencheur las acciones según el comportamiento del cliente. Las siguientes actividades de **Canal** están disponibles: notificaciones push por correo electrónico, SMS, Android y iOS. [Obtenga información sobre cómo configurar un envío en el contexto de un flujo de trabajo](channels.md).

## Actividades de control de flujo {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Actividad final"
>abstract="La actividad **Finalizar** le permite marcar de forma gráfica el final de un flujo de trabajo. Esta actividad no tiene impacto funcional y, por lo tanto, es opcional."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="Señal externa"
>abstract="marcador de posición para la sección de señal externa en los parámetros de la actividad final. Disponible solo para campañas orquestadas. DO NOT DELETE"

Las siguientes actividades son específicas para organizar y ejecutar flujos de trabajo. Su tarea principal es coordinar las otras actividades:

* [And-join](and-join.md): sincronice varias ramas de ejecución de un flujo de trabajo.
* **Fin**: marca gráficamente el final de un flujo de trabajo. Esta actividad no tiene impacto funcional y, por lo tanto, es opcional.
* [Señal externa](external-signal.md): Déclencheur la ejecución de un flujo de trabajo desde otro flujo de trabajo o una llamada de API.
* [Bifurcación](fork.md): cree transiciones salientes para iniciar varias actividades simultáneamente.
* [Programador](scheduler.md): Programe cuando se inicie el flujo de trabajo.
* [Prueba](test.md): habilita transiciones basadas en condiciones especificadas.
* [Esperar](wait.md): Pausar temporalmente la ejecución de una parte de un flujo de trabajo.