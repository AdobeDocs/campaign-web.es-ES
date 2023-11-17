---
audience: end-user
title: Uso de la actividad de flujo de trabajo Guardar audiencia
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
badge: label="Beta"
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: 091775bae73595cb209199b062508931dd3ea315
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 16%

---

# Guardado de público {#save-audience}


>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Guardar un público"
>abstract="Utilice esta actividad para actualizar un público existente o crear uno nuevo a partir de la población calculada en sentido ascendente en un flujo de trabajo. Los públicos creados se añaden a la lista de públicos y están disponibles en el menú **Públicos**."


El **Guardar audiencia** la actividad es una **Segmentación** actividad. Esta actividad le permite actualizar una audiencia existente o crear una nueva a partir de la población calculada en sentido ascendente en un flujo de trabajo. Las audiencias creadas se añaden a la lista de audiencias de aplicación y están disponibles a través del **Audiencias** menú.

Esta actividad se utiliza esencialmente para mantener los grupos de población calculados en el mismo flujo de trabajo, convirtiéndolos en audiencias reutilizables. Conéctelo a otras actividades de segmentación, como una **Crear audiencia** o una **Combinar** actividad.

## Configuración de la actividad Guardar audiencia{#save-audience-configuration}

Siga estos pasos para configurar el **Guardar audiencia** actividad:

![](../assets/workflow-save-audience.png)

1. Añadir un **Guardar audiencia** a su flujo de trabajo.

1. En el **Modo** , seleccione la acción que desee llevar a cabo:

   * **Crear o actualizar una audiencia existente**: defina un **Etiqueta de audiencia**. Si la audiencia ya existe, se actualiza; de lo contrario, se crea una nueva.

   * **Actualizar una audiencia existente**: elija el **Audiencia** desea actualizar entre la lista de audiencias existentes.

1. Seleccione el **Modo de actualización** que se aplicará a las audiencias existentes:

   * **Reemplazar contenido de audiencia por nuevos datos**: todo el contenido de la audiencia se sustituye. Se pierden los datos antiguos. Solo se conservan los datos de la transición de entrada de la actividad Guardar audiencia. Esta opción borra el tipo de audiencia y la dimensión de segmentación de la audiencia actualizada.

   * **Audiencia completa con nuevos datos**: el contenido de audiencia anterior se conserva y se añaden a él los datos de la transición de entrada de la actividad guardar audiencia.

1. Compruebe la **Generación de una transición saliente** si desea añadir una transición después de la variable **Guardar audiencia** actividad.

El contenido de la audiencia guardada está disponible en la vista de detalles de la audiencia, a la que se puede acceder desde el **Audiencias** menú. Las columnas disponibles en esta vista corresponden a las columnas de la transición entrante del flujo de trabajo **Guardar audiencia** actividad.


## Ejemplo{#save-audience-example}

El siguiente ejemplo ilustra una actualización de audiencia simple desde la segmentación. Se agrega un planificador para ejecutar el flujo de trabajo una vez al mes. Una consulta recupera todos los perfiles suscritos a los diferentes servicios de aplicaciones disponibles. El **Guardar audiencia** la actividad actualiza la audiencia eliminando perfiles que han dejado de suscribirse al servicio desde la última ejecución del flujo de trabajo y añadiendo los perfiles recién suscritos.
