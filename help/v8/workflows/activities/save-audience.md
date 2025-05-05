---
audience: end-user
title: Utilice el Guardar audiencia flujo de trabajo actividad
description: Aprenda a utilizar la actividad de flujo de trabajo Tenedor
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 12%

---

# Guardado de público {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Guardar un público"
>abstract="Utilice esta actividad para actualizar un público existente o crear uno nuevo a partir de la población calculada en sentido ascendente en un flujo de trabajo. Los públicos creados se añaden a la lista de públicos y están disponibles en el menú **Públicos**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Generar transición de salida"
>abstract="Utilice esta opción si desea agregar un transición después del **actividad audiencia** Guardar."

El **Guardar audiencia** actividad es un **actividad de segmentación** . Este actividad permite actualizar un audiencia existente o crear un nuevo audiencia a partir de la población calculada en una secuencia flujo de trabajo. Las audiencias creadas se añaden a la lista de aplicación audiencias y están disponibles a través del **menú Audiences** .

Este actividad se utiliza principalmente para retener los grupos de población calculados de la misma flujo de trabajo convirtiéndolos en audiencias reutilizables. Conéctelo a otras actividades direccionamiento, como un **audiencia** de compilación o una **combinación** de actividad.

## Configurar el Guardar audiencia actividad {#save-audience-configuration}

Siga estos pasos para configurar el **Guardar audiencia** actividad:

![Descripción: configuración de flujo de trabajo para Guardar audiencia actividad](../assets/workflow-save-audience.png)

1. añadir una **Guardar audiencia** actividad a su flujo de trabajo.

1. In the **Mode** drop-down, select the action you want to perform:

   * **Crear o actualice un audiencia** existente: Defina una etiqueta **de** audiencia. Si la audiencia ya existe, se actualiza; De lo contrario, se crea una nueva audiencia.

   * **Actualizar un audiencia** existente: elija la **audiencia** que desea actualizar desde el lista de audiencias existentes.

1. Seleccione el modo **de** actualización aplicable a las audiencias existentes:

   * **Reemplazar audiencia contenido con datos** nuevos: se reemplazan todos los datos audiencia contenido y los datos antiguos se pierden. Solo se conservan los datos del transición entrante del actividad de Guardar **audiencia** . Esta opción borra el tipo de audiencia y el dimensión de segmentación del audiencia actualizado.

   * **Todas las aplicaciones audiencia con datos** nuevos: se conserva el contenido de audiencia antiguo y se le agregan los datos del transición entrante del actividad de **audiencia** de Guardar.

1. Marque la **opción Generar un transición** saliente si desea agregar un transición después del actividad de audiencia **&#x200B;**&#x200B;Guardar.

El contenido del audiencia guardado está disponible en la vista detallada del audiencia, al que se puede acceder desde el **menú Audiences** . Las columnas disponibles en este vista corresponden a las columnas del transición entrante del Guardar del flujo de trabajo **actividad de audiencia** .

## Ejemplo {#save-audience-example}

The following example illustrates a simple audience update from targeting. Una planificador ejecuta la flujo de trabajo una vez al mes. Una consulta recupera todos los perfiles suscritos a las diferentes aplicaciones disponibles. El **Guardar audiencia** actividad actualiza el audiencia eliminando los perfiles que se han dado de baja del servicio desde la última flujo de trabajo de ejecución y agregando perfiles recién suscritos.