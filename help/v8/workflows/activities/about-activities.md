---
audience: end-user
title: Trabajar con actividades de flujos de trabajo
description: Aprenda a trabajar con las actividades de flujo de trabajo
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: a0086f41463524cf2bebef6bda31bb079b28259d
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 30%

---


# Acerca de las actividades de flujo de trabajo {#workflow-activities}

Las actividades de flujo de trabajo se agrupan en tres categorías. Dependiendo del contexto, las actividades disponibles pueden diferir.

Todas las actividades se detallan en las secciones siguientes:

* [Actividades de segmentación y administración de datos](#targeting)
* [Actividades del canal](#channel)
* [Actividades de control de flujo](#flow-control)

![](../assets/workflow-activities.png)

## Actividades de segmentación {#targeting}

Estas actividades son específicas de la segmentación. Le permiten crear uno o más públicos destinatarios al definir públicos y dividirlos o combinarlos mediante operaciones de intersección, unión o exclusión.

* [Crear audiencia](build-audience.md): Defina la población objetivo. Puede seleccionar una audiencia existente o utilizar el modelador de consultas para definir su propia consulta.
* [Cambiar fuente de datos](change-data-source.md): cambie la fuente de datos de la tabla de trabajo del flujo de trabajo.&quot;
* [Cambiar dimensión](change-dimension.md): cambie la dimensión de segmentación a medida que vaya creando el flujo de trabajo.
* [Combinar](combine.md): realice la segmentación en la población entrante. Puede utilizar una unión, una intersección o una exclusión.
* [Deduplicación](deduplication.md): elimine duplicados en los resultados de las actividades entrantes.
* [Enriquecimiento](enrichment.md): Defina datos adicionales para procesarlos en el flujo de trabajo. Con esta actividad, puede aprovechar la transición entrante y configurar la actividad para completar la transición saliente con datos adicionales.
* [Consulta incremental](incremental-query.md): consulte la base de datos de forma programada. Cada vez que se ejecuta esta actividad, se excluyen los resultados de las ejecuciones anteriores. Esto permite buscar solo elementos nuevos.
* [Reconciliación](reconciliation.md): Defina el vínculo entre los datos de la base de datos de Adobe Campaign y los datos de una tabla de trabajo, por ejemplo, los datos cargados desde un archivo externo.
* [Guardar audiencia](save-audience.md): actualice una audiencia existente o cree una nueva a partir de la población calculada en sentido ascendente en un flujo de trabajo.
* [Split](split.md): Segmente la población entrante en varios subconjuntos.

## Actividades de administración de datos {#data}

Estas actividades son específicas para manipular y enriquecer datos de población.

* [Extraer archivo](extract-file.md): exporte datos de Adobe Campaign a otro sistema como archivo externo.
* [Cargar archivo](load-file.md): trabaje con perfiles y datos almacenados en un archivo externo.
* [Transferir archivo](transfer-file.md): Reciba o envíe archivos, pruebe la presencia de archivos o enumere archivos en un servidor. El protocolo utilizado puede ser el protocolo servidor a servidor o el protocolo HTTP.
* [Código JavaScript](javascript-code.md): ejecute un fragmento de código JavaScript en el contexto de un flujo de trabajo.
* [Servicios de suscripción](subscription-services.md): suscriba o cancele la suscripción de varios perfiles a un servicio o desde él en una sola acción.
* [Actualización de datos](update-data.md): realice actualizaciones masivas de los campos de la base de datos. Varias opciones permiten personalizar la actualización de datos.

## Actividades del canal {#channel}

Adobe Campaign Web le permite automatizar y ejecutar campañas de marketing en varios canales. Puede combinar actividades de canal en el lienzo para crear flujos de trabajo entre canales que puedan almacenar en déclencheur acciones basadas en el comportamiento del cliente. Lo siguiente **Canal** Hay actividades disponibles: notificaciones push por correo electrónico, SMS, Android y iOS. [Obtenga información sobre cómo configurar una entrega en el contexto de un flujo de trabajo](channels.md).

## Actividades de control de flujo {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Actividad final"
>abstract="La actividad **Finalizar** le permite marcar de forma gráfica el final de un flujo de trabajo. Esta actividad no tiene impacto funcional y, por lo tanto, es opcional."

Las siguientes actividades son específicas para organizar y ejecutar flujos de trabajo. Su tarea principal es coordinar las otras actividades:

* [And-join](and-join.md): sincronice varias ramas de ejecución de un flujo de trabajo.
* **Fin**: Marca gráfica del final de un flujo de trabajo. Esta actividad no tiene impacto funcional y, por lo tanto, es opcional
* [Señal externa](external-signal.md): Déclencheur la ejecución de un flujo de trabajo desde otro flujo de trabajo o una llamada de API.
* [Tenedor](fork.md): cree transiciones salientes para el inicio de varias actividades al mismo tiempo.
* [Planificador](scheduler.md): programe cuándo se inicia el flujo de trabajo.
* [Prueba](test.md): habilite transiciones basadas en condiciones especificadas.
* [Esperar](wait.md): Pause momentáneamente la ejecución de una parte de un flujo de trabajo.
