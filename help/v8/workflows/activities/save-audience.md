---
audience: end-user
title: Uso de la actividad de flujo de trabajo Guardar audiencia
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: 75c612d50d2d4a675829a412e2c4f55ed1cb817c
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 16%

---

# Guardado de público {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Guardar un público"
>abstract="Utilice esta actividad para actualizar un público existente o crear uno nuevo a partir de la población calculada en sentido ascendente en un flujo de trabajo. Los públicos creados se añaden a la lista de públicos y están disponibles en el menú **Públicos**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Generar transición de salida"
>abstract="Utilice esta opción si desea añadir una transición después de la actividad **Guardado de público**."

La actividad **Guardar audiencia** es una actividad de **segmentación**. Esta actividad le permite actualizar una audiencia existente o crear una nueva a partir de la población calculada en sentido ascendente en un flujo de trabajo. Las audiencias creadas se agregan a la lista de audiencias de aplicación y están disponibles a través del menú **Audiencias**.

Esta actividad se utiliza esencialmente para mantener los grupos de población calculados en el mismo flujo de trabajo, convirtiéndolos en audiencias reutilizables. Conéctelo a otras actividades de segmentación, como una **audiencia de compilación** o una actividad **Combinar**.

## Configuración de la actividad Guardar audiencia{#save-audience-configuration}

Siga estos pasos para configurar la actividad **Guardar audiencia**:

![](../assets/workflow-save-audience.png)

1. Agregue una actividad **Guardar audiencia** a su flujo de trabajo.

1. En la lista desplegable **Modo**, seleccione la acción que desee llevar a cabo:

   * **Crear o actualizar una audiencia existente**: defina una **etiqueta de audiencia**. Si la audiencia ya existe, se actualiza; de lo contrario, se crea una nueva.

   * **Actualizar una audiencia existente**: elija la **audiencia** que desee actualizar entre la lista de audiencias existentes.

1. Seleccione el **modo de actualización** que se aplicará a las audiencias existentes:

   * **Reemplazar contenido de audiencia por nuevos datos**: se reemplaza todo el contenido de audiencia. Se pierden los datos antiguos. Solo se conservan los datos de la transición entrante de la actividad Guardar audiencia. Esta opción borra el tipo de audiencia y la dimensión de segmentación de la audiencia actualizada.

   * **Audiencia completa con nuevos datos**: el contenido de audiencia anterior se conserva y los datos de la transición de entrada de la actividad Guardar audiencia se agregan a ella.

1. Marque la opción **Generar una transición saliente** si desea agregar una transición después de la actividad **Guardar audiencia**.

El contenido de la audiencia guardada está disponible en la vista de detalles de la audiencia, a la que se puede acceder desde el menú **Audiencias**. Las columnas disponibles en esta vista corresponden a las columnas de la transición entrante de la actividad **Guardar audiencia** del flujo de trabajo.


## Ejemplo{#save-audience-example}

El siguiente ejemplo ilustra una actualización de audiencia simple desde la segmentación. Se agrega un planificador para ejecutar el flujo de trabajo una vez al mes. Una consulta recupera todos los perfiles suscritos a las diferentes aplicaciones disponibles. La actividad **Guardar audiencia** actualiza la audiencia eliminando perfiles que se han dado de baja del servicio desde la última ejecución del flujo de trabajo y agregando los perfiles recién suscritos.
