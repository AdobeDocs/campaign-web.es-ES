---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Obtenga información sobre cómo crear un flujo de trabajo con Adobe Campaign Web
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 18%

---

# Creación del flujo de trabajo {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Lista de flujos de trabajo de la campaña"
>abstract="La pestaña **Flujos de trabajo** enumera todos los flujos de trabajo vinculados a la campaña actual. Haga clic en el nombre de un flujo de trabajo para editarlo. Utilice el botón **Crear flujo de trabajo** para añadir un nuevo flujo de trabajo para esta campaña."

Puede crear flujos de trabajo independientes o flujos de trabajo dentro de una campaña. El primer paso es seleccionar una plantilla y definir sus propiedades generales. A continuación, configure las opciones adicionales que sean necesarias.

Para ello, siga estos pasos:

1. Para crear un **flujo de trabajo independiente**, vaya al menú **Flujos de trabajo**. Para crear un **flujo de trabajo de campaña**, vaya al menú **Campañas** y abra la campaña para la que desea crear un nuevo flujo de trabajo.

1. Haga clic en el botón **[!UICONTROL Crear flujo de trabajo]** en la esquina superior derecha de la pantalla.

   ![Captura de pantalla que muestra el botón Crear flujo de trabajo en la esquina superior derecha de la pantalla.](assets/workflow-create.png){zoomable="yes"}

1. En el cuadro de diálogo **Propiedades** del flujo de trabajo, seleccione la plantilla que desea utilizar para crear el flujo de trabajo (también puede utilizar la plantilla integrada predeterminada). [Más información sobre las plantillas de flujo de trabajo](#workflow-templates).

1. Introduzca una etiqueta para el flujo de trabajo. Además, agregue una descripción al flujo de trabajo en el campo específico de la sección **[!UICONTROL Opciones adicionales]** de la pantalla.

1. Expanda la sección **[!UICONTROL Opciones adicionales]** para configurar opciones adicionales para el flujo de trabajo. Aprenda a configurar las propiedades del flujo de trabajo en [esta página](workflow-settings.md#properties).

   ![Captura de pantalla que muestra la sección Opciones adicionales para configurar las opciones del flujo de trabajo.](assets/workflow-additional-options.png){zoomable="yes"}

1. Haga clic en el botón **[!UICONTROL Crear flujo de trabajo]** para confirmar la creación del flujo de trabajo.

El flujo de trabajo se habrá creado y estará disponible en la lista de flujos de trabajo. Puede acceder a su lienzo visual y empezar a añadir, configurar y organizar las tareas que va a realizar. [Aprenda a organizar actividades de flujo de trabajo](orchestrate-activities.md).

## Trabajo con plantillas de flujo de trabajo {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Plantillas de flujo de trabajo"
>abstract="Las plantillas de flujo de trabajo contienen ajustes y actividades preconfiguradas que se pueden reutilizar para crear nuevos flujos de trabajo."

>[!CONTEXTUALHELP]
>id="acw_workflow_template_creation_properties"
>title="Propiedades del flujo de trabajo"
>abstract="Las plantillas de flujo de trabajo contienen ajustes y actividades preconfiguradas que se pueden reutilizar para crear nuevos flujos de trabajo. En esta pantalla, introduzca la etiqueta de la plantilla de flujo de trabajo y configure sus opciones, como el nombre interno, la carpeta y las carpetas de ejecución, la zona horaria y el grupo del supervisor."

Las plantillas de flujo de trabajo contienen ajustes y actividades preconfiguradas que se pueden reutilizar para crear nuevos flujos de trabajo. La plantilla del flujo de trabajo se selecciona en las propiedades del flujo de trabajo al crearlo. De forma predeterminada, se proporciona una plantilla vacía.

Puede crear una plantilla a partir de un flujo de trabajo existente o crear una nueva plantilla desde cero. Ambos métodos se detallan a continuación.

>[!BEGINTABS]

>[!TAB Crear una plantilla a partir de un flujo de trabajo existente]

Para crear una plantilla de flujo de trabajo a partir de un flujo de trabajo existente, siga estos pasos:

1. Abra el menú **Flujos de trabajo** y vaya al flujo de trabajo para guardarlo como plantilla.
1. Haga clic en los tres puntos a la derecha del nombre del flujo de trabajo y elija **Copiar como plantilla**.

   ![Captura de pantalla que muestra la opción Copiar como plantilla en el menú de flujo de trabajo.](assets/wf-copy-as-template.png){zoomable="yes"}

1. En la ventana emergente, confirme la creación de la plantilla.
1. En el lienzo de la plantilla de flujo de trabajo, compruebe, añada y configure las actividades según sea necesario.
1. Vaya a la configuración, en el botón **Configuración**, para cambiar el nombre de la plantilla de flujo de trabajo e introduzca una descripción.
1. Seleccione la **carpeta** y la **carpeta de ejecución** de la plantilla. La carpeta es la ubicación donde se guarda la plantilla de flujo de trabajo. La carpeta de ejecución es la carpeta en la que se guardan los flujos de trabajo creados basándose en esta plantilla.

   ![Captura de pantalla que muestra la configuración de la carpeta y la carpeta de ejecución en la plantilla de flujo de trabajo.](assets/wf-settings-template.png){zoomable="yes"}

   Las demás propiedades son comunes en los flujos de trabajo. Obtenga más información en [esta página](workflow-settings.md#properties).

1. Guarde los cambios.

La plantilla de flujo de trabajo ya está disponible en la lista de plantillas. Puede crear un flujo de trabajo basado en esta plantilla. Este flujo de trabajo se preconfigura con la configuración y las actividades definidas en la plantilla.

>[!TAB Crear una plantilla desde cero]

Para crear una plantilla de flujo de trabajo desde cero, siga estos pasos:

1. Abra el menú **Flujos de trabajo** y vaya a la pestaña **Plantillas**. Puede ver la lista de plantillas de flujo de trabajo disponibles.
1. Haga clic en el botón **[!UICONTROL Crear plantilla]** en la esquina superior derecha de la pantalla.
1. Introduzca la etiqueta y abra las opciones adicionales para introducir una descripción de la plantilla de flujo de trabajo.
1. Seleccione la carpeta y la carpeta de ejecución de la plantilla. La carpeta es la ubicación donde se guarda la plantilla de flujo de trabajo. La carpeta de ejecución es la carpeta en la que se guardan los flujos de trabajo creados basándose en esta plantilla.

   ![Captura de pantalla que muestra la creación de una nueva plantilla de flujo de trabajo con la configuración de carpeta y carpeta de ejecución.](assets/new-wf-template.png){zoomable="yes"}

   Las demás propiedades son comunes en los flujos de trabajo. Obtenga más información en [esta página](workflow-settings.md#properties).

1. Haga clic en el botón **Crear** para confirmar la configuración.
1. En el lienzo de la plantilla de flujo de trabajo, añada y configure las actividades según sea necesario.

   ![Captura de pantalla que muestra el lienzo de la plantilla de flujo de trabajo para agregar y configurar actividades.](assets/wf-template-activities.png){zoomable="yes"}

1. Guarde los cambios.

La plantilla de flujo de trabajo ya está disponible en la lista de plantillas. Puede crear un flujo de trabajo basado en esta plantilla. Este flujo de trabajo se preconfigura con la configuración y las actividades definidas en la plantilla.

>[!ENDTABS]