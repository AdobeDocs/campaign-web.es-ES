---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 4%

---

# Iniciar y monitorizar sus flujos de trabajo {#start-monitor}

Una vez creado el flujo de trabajo y diseñado las tareas que se realizan en el lienzo, puede iniciarlo y monitorizar cómo se ejecuta.

## Inicio del flujo de trabajo {#start}

Para iniciar el flujo de trabajo, vaya al menú **[!UICONTROL Flujos de trabajo]** o a la campaña asociada y haga clic en el botón **[!UICONTROL Iniciar]** en la esquina superior derecha del lienzo.

Una vez que se esté ejecutando el flujo de trabajo, cada actividad del lienzo se ejecuta secuencialmente hasta que se llega al final del flujo de trabajo.

Puede realizar un seguimiento del progreso de los perfiles de destino en tiempo real mediante un flujo visual. Esto le permite identificar rápidamente el estado de cada actividad y el número de perfiles en transición entre ellas.

![Representación visual de la ejecución del flujo de trabajo en curso.](assets/workflow-execution.png){zoomable="yes"}

## Transiciones de flujo de trabajo {#transitions}

En los flujos de trabajo, los datos que pasan de una actividad a otra a través de transiciones se almacenan en una tabla de trabajo temporal. Estos datos se pueden mostrar para cada transición. Para mostrar los datos, seleccione una transición para abrir sus propiedades en el lado derecho de la pantalla.

* Haga clic en **[!UICONTROL Vista previa del esquema]** para mostrar el esquema de la tabla de trabajo.
* Haga clic en **[!UICONTROL Previsualizar resultados]** para ver los datos transportados en la transición seleccionada.

![Ejemplo de propiedades de transición y vista previa de datos.](assets/transition.png){zoomable="yes"}

## Monitorización de la ejecución de actividades {#activities}

Los indicadores visuales de la esquina superior derecha de cada cuadro de actividad permiten comprobar su estado de ejecución:

| Indicador visual | Descripción |
|------------------|-------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | La actividad se está ejecutando. |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | La actividad requiere su atención. Esto puede implicar confirmar el envío de una entrega o realizar la acción necesaria. |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | La actividad ha encontrado un error. Para resolver el problema, abra los registros de flujo de trabajo para obtener más información. |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | La actividad se ha ejecutado correctamente. |

## Monitorización de registros y tareas {#logs-tasks}

La monitorización de los registros y las tareas de flujo de trabajo es un paso clave para analizar los flujos de trabajo y garantizar que se ejecuten correctamente. Se puede acceder a los registros y tareas desde el icono **[!UICONTROL Registros]**, que está disponible en la barra de herramientas de acciones y en el panel de propiedades de cada actividad.

El menú **[!UICONTROL Registros y tareas]** proporciona un historial de la ejecución del flujo de trabajo, registrando todas las acciones del usuario y los errores encontrados. Este historial se guarda durante la duración especificada en el flujo de trabajo [opciones de ejecución](workflow-settings.md). Durante esta duración, todos los mensajes se guardan, incluso después de reiniciar el flujo de trabajo. Si no desea guardar los mensajes de una ejecución anterior, haga clic en el botón **[!UICONTROL Purgar historial]**.

![Ejemplo de interfaz de tareas y registros de flujo de trabajo.](assets/workflow-logs.png){zoomable="yes"}

Hay dos tipos de información disponibles:

* La pestaña **[!UICONTROL Log]** contiene el historial de ejecución de todas las actividades de flujo de trabajo. Indexa las operaciones realizadas y los errores de ejecución en orden cronológico.
* La ficha **[!UICONTROL Tareas]** detalla la secuencia de ejecución de las actividades.

En ambas pestañas, puede elegir las columnas mostradas y su orden, aplicar filtros y utilizar el campo de búsqueda para encontrar rápidamente la información deseada.

## Comandos de ejecución de flujo de trabajo {#execution-commands}

La barra de acciones de la esquina superior derecha proporciona comandos para administrar la ejecución del flujo de trabajo. Puede hacer lo siguiente:

* **[!UICONTROL Iniciar]** / **[!UICONTROL Reanudar]** la ejecución del flujo de trabajo. Si el flujo de trabajo estaba en pausa, se reanuda. De lo contrario, se inicia y se activan las actividades iniciales.
* **[!UICONTROL Pausar]** la ejecución del flujo de trabajo. A continuación, el flujo de trabajo adquiere el estado Paused. No se activan nuevas actividades hasta que se reanuda, pero las operaciones en curso no se suspenden.
* **[!UICONTROL Detener]** un flujo de trabajo que se está ejecutando. A continuación, el flujo de trabajo adquiere el estado Finished. Las operaciones en curso se interrumpen si es posible. No puede reanudar el flujo de trabajo desde el mismo punto en el que se detuvo.