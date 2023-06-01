---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con la web de Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: c842829915784654b7130563d36dea188e84ff3d
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 4%

---


# Creación de un flujo de trabajo {#create}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propiedades del flujo de trabajo"
>abstract="Por determinar"

## Creación del flujo de trabajo {#create-workflow}

El primer paso para crear el flujo de trabajo en Campaign v8 Web es crearlo como un flujo de trabajo independiente o directamente dentro de una campaña y definir sus propiedades generales. Para ello, siga estos pasos:

1. Comience por decidir si desea crear un flujo de trabajo independiente o integrarlo directamente en una campaña:

   * **Flujo de trabajo independiente**: vaya al menú Flujos de trabajo y haga clic en el botón Crear flujo de trabajo en la esquina superior derecha.
   * **Flujo de trabajo de campaña:** Vaya al menú Campaigns y abra la campaña donde desee crear un nuevo flujo de trabajo. Haga clic en el botón Create workflow en la esquina superior derecha de la pestaña Workflows.

   Aparecerá el cuadro de diálogo Propiedades del flujo de trabajo.

   ![](assets/workflow-create.png)

1. Seleccione la plantilla que desea utilizar para crear el flujo de trabajo y proporcione una etiqueta para él.

   Las plantillas de flujo de trabajo contienen actividades preconfiguradas y configuraciones de propiedad generales que se pueden reutilizar para crear nuevos flujos de trabajo. Se crean desde la consola del cliente. [Aprenda a trabajar con plantillas](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. Expanda la sección Opciones adicionales si desea configurar opciones específicas para el flujo de trabajo, como la carpeta de almacenamiento y la zona horaria. [Obtenga información sobre cómo configurar las propiedades del flujo de trabajo](workflow-settings.md)

1. Haga clic en el botón Create workflow para confirmar la creación del flujo de trabajo.

Con el flujo de trabajo creado, ahora puede empezar a organizar las distintas tareas que realizará mediante un lienzo visual dedicado. [Obtenga información sobre cómo organizar actividades de flujo de trabajo](#build)

## Organización de las actividades del flujo de trabajo {#build}

Una vez que lo haya hecho [creó un flujo de trabajo](create-workflow.md), ya sea desde el menú de flujo de trabajo o dentro de una campaña, puede empezar a organizar las diferentes tareas que va a realizar. Para ello, se proporciona un lienzo visual, que le permite construir un diagrama de flujo de trabajo. Dentro de este diagrama, puede añadir varias actividades y conectarlas en un orden secuencial.

En esta fase de la configuración, el diagrama se muestra con un icono de inicio que representa el principio del flujo de trabajo. Para añadir la primera actividad, haga clic en el botón + conectado al icono de inicio.

Aparecerá una lista de actividades que se pueden agregar al diagrama. Las actividades disponibles dependen de su posición en el diagrama de flujo de trabajo. Por ejemplo, al añadir la primera actividad de, puede iniciar el flujo de trabajo segmentando una audiencia, dividiendo la ruta del flujo de trabajo o configurando una actividad de espera para retrasar la ejecución del flujo de trabajo. Por otro lado, después de una actividad Generar audiencia, puede refinar el objetivo con actividades de objetivo, enviar una entrega a la audiencia con actividades de canal u organizar el proceso de flujo de trabajo con actividades de control de flujo.

![](assets/workflow-start.png)

Una vez que se ha agregado una actividad al diagrama, aparece un panel derecho que le permite configurar la actividad recién agregada con ajustes específicos. Encontrará información detallada sobre cómo configurar cada actividad en [esta sección](activities/about-activities.md).

![](assets/workflow-configure-activities.png)

Repita este proceso y agregue tantas actividades como desee según las tareas que desee que realice el flujo de trabajo. Tenga en cuenta que también puede insertar una nueva actividad entre dos actividades. Para ello, haga clic en el botón + de la transición entre las actividades, seleccione la actividad deseada y configúrela en el panel derecho.

Para quitar una actividad, selecciónela en el lienzo y haga clic en el icono Eliminar en las propiedades de la actividad.

>[!TIP]
>
>Tiene la opción de personalizar el nombre de las transiciones entre cada actividad. Para ello, seleccione la transición y cambie su etiqueta en el panel derecho.

Una vez completado el flujo de trabajo, añada una actividad End al final del diagrama. Esta actividad le permite marcar visualmente el final de un flujo de trabajo y no tiene impacto funcional.

Después de diseñar correctamente el diagrama de flujo de trabajo, puede ejecutar el flujo de trabajo y realizar un seguimiento del progreso de sus distintas tareas. [Obtenga información sobre cómo iniciar un flujo de trabajo y monitorizar su ejecución](start-monitor-workflows.md)
