---
audience: end-user
title: Uso de la actividad de flujo de trabajo Guardar audiencia
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
badge: label="Beta"
source-git-commit: bbb22de6ff1398dbb1431f51a55350d206b4690a
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 13%

---


# Guardado de audiencia {#save-audience}

<!--
>[!CONTEXTUALHELP]
>id="???"
>title="Save audience activity"
>abstract="The Save audience activity allows you to..."
-->

El **Guardar audiencia** la actividad es una **Segmentación** actividad. Esta actividad le permite actualizar una audiencia existente o crear una nueva a partir de la población calculada en sentido ascendente en un flujo de trabajo. Las audiencias creadas se añaden a la lista de audiencias de aplicación y están disponibles a través del **Audiencias** menú.

Esta actividad se utiliza esencialmente para mantener los grupos de población calculados en el mismo flujo de trabajo, convirtiéndolos en audiencias reutilizables. Conéctelo a otras actividades de segmentación, como una **Crear audiencia** o una **Combinar** actividad.

## Configuración

Siga estos pasos para configurar el **Guardar audiencia** actividad:

1. Añadir un **Guardar audiencia** a su flujo de trabajo.

   ![](../assets/workflow-save-audience.png)

1. En el **Modo** , seleccione la acción que desee llevar a cabo:

   * **Crear o actualizar una audiencia existente**: defina un **Etiqueta de audiencia**. Si la audiencia ya existe, se actualiza; de lo contrario, se crea una nueva.

   * **Actualizar una audiencia existente**: elija el **Audiencia** desea actualizar entre la lista de audiencias existentes.

1. Seleccione el **Modo de actualización** que se aplicará a las audiencias existentes:

   * **Reemplazar contenido de audiencia por nuevos datos**: todo el contenido de la audiencia se sustituye. Se pierden los datos antiguos. Solo se conservan los datos de la transición de entrada de la actividad Guardar audiencia. Esta opción borra el tipo de audiencia y la dimensión de segmentación de la audiencia actualizada.

   * **Audiencia completa con nuevos datos**: el contenido de audiencia anterior se conserva y se añaden a él los datos de la transición de entrada de la actividad guardar audiencia.

1. Seleccione la opción **Generate complement** si desea utilizar la población restante. A continuación, se agregará una transición adicional a la actividad.

El contenido de la audiencia guardada está disponible en la vista de detalles de la audiencia, a la que se puede acceder desde el **Audiencias** menú. Las columnas disponibles en esta vista corresponden a las columnas de la transición entrante del flujo de trabajo **Guardar audiencia** actividad.


## Ejemplo



