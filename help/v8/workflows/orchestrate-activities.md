---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
exl-id: 0c8e2158-518c-4620-9971-00ed2eccdd4f
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 5%

---

# Organización de actividades {#orchestrate}

Una vez que lo haya hecho [creó un flujo de trabajo](create-workflow.md), ya sea desde el menú de flujo de trabajo o dentro de una campaña, puede empezar a organizar las diferentes tareas que va a realizar. Para ello, se proporciona un lienzo visual, que le permite construir un diagrama de flujo de trabajo. Dentro de este diagrama, puede añadir varias actividades y conectarlas en un orden secuencial.

## Añadir actividades {#add}

En esta fase de la configuración, el diagrama se muestra con un icono de inicio que representa el principio del flujo de trabajo. Para añadir su primera actividad, haga clic en **+** botón conectado al icono de inicio.

Aparecerá una lista de actividades que se pueden agregar al diagrama. Las actividades disponibles dependen de su posición en el diagrama de flujo de trabajo. Por ejemplo, al añadir la primera actividad de, puede iniciar el flujo de trabajo segmentando una audiencia, dividiendo la ruta del flujo de trabajo o estableciendo un **Esperar** para retrasar la ejecución del flujo de trabajo. Por otro lado, después de un **Crear audiencia** actividad, puede refinar el segmento con actividades de segmentación, realizar una entrega a la audiencia con actividades de canal u organizar el proceso de flujo de trabajo con actividades de control de flujo.

![](assets/workflow-start.png){zoomable=&quot;yes&quot;}

Una vez que se ha agregado una actividad al diagrama, aparece un panel derecho que le permite configurar la actividad recién agregada con ajustes específicos. Encontrará información detallada sobre cómo configurar cada actividad en [esta sección](activities/about-activities.md).

![](assets/workflow-configure-activities.png){zoomable=&quot;yes&quot;}

Repita este proceso para agregar tantas actividades como desee según las tareas que desee que realice el flujo de trabajo. Tenga en cuenta que también puede insertar una nueva actividad entre dos actividades. Para ello, haga clic en el **+** en la transición entre las actividades, seleccione la actividad deseada y configúrela en el panel derecho.

Para quitar una actividad, selecciónela en el lienzo y haga clic en **Eliminar** en las propiedades de la actividad.

>[!TIP]
>
>Tiene la opción de personalizar el nombre de las transiciones entre cada actividad. Para ello, seleccione la transición y cambie su etiqueta en el panel derecho.

## Administrar actividades {#manage}

Al agregar actividades, los botones de acción están disponibles en el panel de propiedades, lo que le permite realizar varias operaciones. Puede hacer lo siguiente:

* **Eliminar** la actividad del lienzo.
* **Deshabilitar/habilitar** la actividad. Cuando se ejecuta el flujo de trabajo, las actividades desactivadas y las siguientes actividades en la misma ruta no se ejecutan y el flujo de trabajo se detiene.
* **Copiar** la actividad. A continuación, puede pegarlo en cualquier flujo de trabajo haciendo clic en **+** en una transición y seleccione &quot;Pegar 1 actividad&quot;.
* Acceda a los **Registros y tareas**.
* **Pausar/reanudar** la actividad. Cuando se ejecuta el flujo de trabajo, se detiene en la actividad pausada. No se ejecutan la tarea correspondiente ni todas las que la siguen en la misma ruta.

![](assets/activity-action.png){zoomable=&quot;yes&quot;}{width="50%"}

Varios **Segmentación** actividades, como **Combinar** o **Deduplicación**, le permite procesar la población restante e incluirla en una transición saliente adicional. Por ejemplo, si utiliza un **Split** actividad, el complemento está formado por la población que no coincide con ninguno de los subconjuntos definidos anteriormente. Para utilizar esta capacidad, active la variable **Generar complemento** opción.

![](assets/workflow-split-complement.png)

## Ejemplo {#example}

VIP A continuación, se muestra un ejemplo de flujo de trabajo diseñado para enviar un correo electrónico a todos los clientes (que no sean clientes de la red) con un correo electrónico que estén interesados en las máquinas de café.

![](assets/workflow-example.png){zoomable=&quot;yes&quot;}{zoomable=&quot;yes&quot;}

Para ello, se han añadido las actividades siguientes:

* A **[!UICONTROL Tenedor]** actividad que divide el flujo de trabajo en tres rutas (una para cada conjunto de clientes),
* **[!UICONTROL Crear audiencia]** actividades para dirigirse a los tres conjuntos de clientes:

   * Clientes con un correo electrónico,
   * Clientes que pertenecen a la audiencia preexistente &quot;Interesado en las máquinas de café&quot;,
   * VIP Clientes que pertenecen a la audiencia preexistente de &quot;recompensa o&quot;.

* A **[!UICONTROL Combinar]** actividad que agrupa a clientes con un correo electrónico y a aquellos interesados en las máquinas de café,
* A **[!UICONTROL Combinar]** VIP actividad que excluye a los clientes de la,
* Un **[!UICONTROL Envío de correo electrónico]** actividad que envía un correo electrónico a los clientes resultantes.

Una vez completado el flujo de trabajo, añada. **[!UICONTROL Fin]** actividad al final del diagrama. Esta actividad le permite marcar visualmente el final de un flujo de trabajo y no tiene impacto funcional.

Después de diseñar correctamente el diagrama de flujo de trabajo, puede ejecutar el flujo de trabajo y realizar un seguimiento del progreso de sus distintas tareas. [Obtenga información sobre cómo iniciar un flujo de trabajo y monitorizar su ejecución](start-monitor-workflows.md)
