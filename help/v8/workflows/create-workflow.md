---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Obtenga información sobre cómo crear un flujo de trabajo con Adobe Campaign Web
badge: label="Beta"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 9272419162d95859147949717e294aa7ae24fc71
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 21%

---


# Creación del flujo de trabajo {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propiedades del flujo de trabajo"
>abstract="En esta pantalla, elija la plantilla que desea utilizar para crear el flujo de trabajo y especifique una etiqueta. Expanda la sección OPCIONES ADICIONALES para configurar más opciones, como el nombre interno del flujo de trabajo, su carpeta, zona horaria y grupo de supervisores. Se recomienda encarecidamente seleccionar un grupo de supervisores para que los operadores sean alertados si se produce un error."


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Lista de flujos de trabajo de la campaña"
>abstract="La pestaña **Flujos de trabajo** enumera todos los flujos de trabajo vinculados a la campaña actual. Haga clic en el nombre de un flujo de trabajo para editarlo. Utilice el botón **Crear flujo de trabajo** para añadir un nuevo flujo de trabajo para esta campaña."


Puede crear flujos de trabajo independientes o flujos de trabajo dentro de una campaña. El primer paso es seleccionar una plantilla y definir sus propiedades generales. A continuación, puede configurar ajustes adicionales según sea necesario.

Para ello, siga estos pasos:

1. Para crear un **Flujo de trabajo independiente**, vaya a **Flujos de trabajo** menú.

   Para crear un **Flujo de trabajo de campaña**, vaya a **Campañas** y abra la campaña para la que desea crear un nuevo flujo de trabajo.

1. Haga clic en **[!UICONTROL Crear flujo de trabajo]** en la esquina superior derecha de la pantalla.

   ![](assets/workflow-create.png)

1. En flujo de trabajo **Propiedades** , seleccione la plantilla que desea utilizar para crear el flujo de trabajo (también puede utilizar la plantilla integrada predeterminada). Obtenga más información sobre las plantillas en [la sección siguiente](#work-with-workflow-templates-workflow-templates).

1. Introduzca una etiqueta para el flujo de trabajo. Además, le recomendamos encarecidamente que añada una descripción al flujo de trabajo, en el campo dedicado del **[!UICONTROL Opciones adicionales]** de la pantalla.

1. Expanda el **[!UICONTROL Opciones adicionales]** para definir más configuraciones para el flujo de trabajo. Obtenga información sobre cómo configurar las propiedades del flujo de trabajo en [esta página](workflow-settings.md#properties)

   ![](assets/workflow-additional-options.png)

1. Haga clic en **[!UICONTROL Crear flujo de trabajo]** para confirmar la creación del flujo de trabajo.

El flujo de trabajo se habrá creado y estará disponible en la lista de flujos de trabajo. Ahora puede acceder a su lienzo visual y empezar a agregar, configurar y organizar las tareas que va a realizar. Obtenga información sobre cómo organizar actividades de flujo de trabajo en [esta página](orchestrate-activities.md).

## Trabajo con plantillas de flujo de trabajo {#workflow-templates}


>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Plantillas de flujo de trabajo"
>abstract="Las plantillas de flujo de trabajo contienen ajustes y actividades preconfiguradas que se pueden reutilizar para crear nuevos flujos de trabajo."

Las plantillas de flujo de trabajo contienen ajustes y actividades preconfiguradas que se pueden reutilizar para crear nuevos flujos de trabajo. Puede seleccionar la plantilla del flujo de trabajo en las propiedades del flujo de trabajo al crear un flujo de trabajo. De forma predeterminada, se proporciona una plantilla vacía.

Puede crear una plantilla a partir de un flujo de trabajo existente o crear una nueva plantilla desde cero. Ambos métodos se detallan a continuación.


>[!BEGINTABS]

>[!TAB Creación de una plantilla a partir de un flujo de trabajo existente]

Para crear una plantilla de flujo de trabajo a partir de un flujo de trabajo existente, siga estos pasos:

1. Abra para abrir **Flujos de trabajo** y vaya al flujo de trabajo para guardarlo como plantilla.
1. Haga clic en los tres puntos a la derecha del nombre del flujo de trabajo y seleccione **Copiar como plantilla**.

   ![](assets/wf-copy-as-template.png)

1. En la ventana emergente, confirme la creación de la plantilla.
1. En el lienzo de la plantilla de flujo de trabajo, compruebe, añada y configure las actividades según sea necesario.
1. Vaya a la configuración, desde el **Configuración** para cambiar el nombre de la plantilla de flujo de trabajo e introduzca una descripción.
1. Seleccione el **carpeta** y **carpeta de ejecución** de la plantilla. La carpeta es la ubicación donde se guarda la plantilla de flujo de trabajo. La carpeta de ejecución es la carpeta en la que se guardan los flujos de trabajo creados basándose en esta plantilla.

   ![](assets/wf-settings-template.png)

   Las demás propiedades son comunes en los flujos de trabajo. Obtenga más información en [esta página](workflow-settings.md#properties)

1. Guarde los cambios.

La plantilla de flujo de trabajo ya está disponible en la lista de plantillas. Puede crear un flujo de trabajo basado en esta plantilla. Este flujo de trabajo se preconfigura con la configuración y las actividades definidas en la plantilla.


>[!TAB Creación de una plantilla desde cero]


Para crear una plantilla de flujo de trabajo desde cero, siga estos pasos:

1. Abra para abrir **Flujos de trabajo** y vaya al menú **Plantillas** pestaña. Puede ver la lista de plantillas de flujo de trabajo disponibles.
1. Haga clic en **[!UICONTROL Crear plantilla]** en la esquina superior derecha de la pantalla.
1. Introduzca la etiqueta y abra las opciones adicionales para introducir una descripción de la plantilla de flujo de trabajo.
1. Seleccione la carpeta y la carpeta de ejecución de la plantilla. La carpeta es la ubicación donde se guarda la plantilla de flujo de trabajo. La carpeta de ejecución es la carpeta en la que se guardan los flujos de trabajo creados basándose en esta plantilla.

   ![](assets/new-wf-template.png)

   Las demás propiedades son comunes en los flujos de trabajo. Obtenga más información en [esta página](workflow-settings.md#properties)

1. Haga clic en **Crear** para confirmar la configuración.
1. En el lienzo de la plantilla de flujo de trabajo, añada y configure las actividades según sea necesario.

   ![](assets/wf-template-activities.png)

1. Guarde los cambios.

La plantilla de flujo de trabajo ya está disponible en la lista de plantillas. Puede crear un flujo de trabajo basado en esta plantilla. Este flujo de trabajo se preconfigura con la configuración y las actividades definidas en la plantilla.

>[!ENDTABS]
