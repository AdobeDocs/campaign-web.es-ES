---
audience: end-user
title: Administración de plantillas de campaña con Adobe Campaign Web
description: Obtenga información sobre cómo administrar plantillas de campaña con Adobe Campaign Web
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 47%

---


# Administración de plantillas de campaña{#manage-campaign-templates}

Todas las campañas de marketing se basan en una plantilla que almacena las características y capacidades principales. Campaign incluye un conjunto de plantillas integradas para ayudarle a empezar. Puede crear y configurar las plantillas de campañas y luego crear campañas a partir de estas plantillas.

## Creación de una plantilla de campaña

Para crear una plantilla de campaña, siga estos pasos:

Abra el explorador de Campaign y vaya a Resources > Templates > Campaign templates.
Haga clic en New en la barra de herramientas situada encima de la lista de plantillas.


También puede duplicar la plantilla integrada para reutilizar y adaptar su configuración. Para ello, haga clic con el botón derecho en la plantilla y seleccione Duplicate.

Introduzca la etiqueta de la nueva plantilla de campaña.

Haga clic en Save y vuelva a abrir la plantilla.

En la pestaña Edit, defina las propiedades de la plantilla.

Seleccione el vínculo Advanced campaign parameters... para añadir un flujo de trabajo a la plantilla de campaña.



Cambie el valor de Targeting and workflows a Yes. y confirme. Aprenda a añadir funcionalidades en esta sección.

La pestaña Targeting and workflows se añade a la plantilla. Haga clic en Add a workflow... , introduzca una Label y haga clic en Ok.

Cree su flujo de trabajo según sus necesidades.



Haga clic en Guardar. La plantilla ya está lista para utilizarse para crear una nueva campaña.

Las distintas pestañas y subpestañas de la plantilla de campaña permiten acceder a su configuración, tal y como se describe en Configuración general.

Seleccione módulos El vínculo Advanced campaign parameters... permite habilitar y deshabilitar los trabajos de las campañas en función de esta plantilla. Seleccione las funciones que desee habilitar en las campañas creadas en función de esta plantilla.



Si no se selecciona una funcionalidad, los elementos correspondientes del proceso (menús, iconos, opciones, pestañas, subpestañas, etc.) no aparecen en la interfaz de la plantilla ni en las campañas basadas en esta plantilla. Las pestañas a la izquierda de los detalles de la campaña y las pestañas disponibles coinciden con las funcionalidades seleccionadas en la plantilla. Por ejemplo, si la funcionalidad Gastos y objetivos no está habilitada, la pestaña Presupuesto correspondiente no se muestra en las campañas basadas en esta plantilla.

Además, los accesos directos a las ventanas de configuración se añaden al panel de campañas. Cuando una funcionalidad está habilitada, un vínculo directo le permite acceder a ella desde el panel de campañas.

Ejemplos de configuración Por ejemplo, con la siguiente configuración:



El panel de campañas muestra:



Tenga en cuenta que falta la pestaña Targeting and workflows.

Estas son las funcionalidades disponibles:



Tenga en cuenta que falta la pestaña Presupuesto.

La configuración avanzada de la campaña también refleja esta configuración.



Tenga en cuenta que la pestaña Aprobaciones no está disponible.

Con esta configuración:


El panel de campañas muestra:



Tenga en cuenta que la pestaña Targeting and workflows está disponible, pero falta el vínculo Add a document.

Estas son las funcionalidades disponibles:



Tenga en cuenta que la pestaña Presupuesto está disponible.

La configuración avanzada de la campaña también refleja esta configuración.



Tenga en cuenta que la pestaña Aprobaciones está disponible, pero las pestañas Control de población y Direcciones semilla no están habilitadas.

Tipología de módulos Grupo de control

Cuando se selecciona este módulo, se añade una pestaña adicional a la configuración avanzada de la plantilla y a las campañas basadas en esta plantilla. La configuración se puede definir mediante la plantilla o bien por separado para cada campaña. Obtenga más información sobre los grupos de control en esta sección.



Direcciones semilla

Cuando se selecciona este módulo, se añade una pestaña adicional a la configuración avanzada de la plantilla y a las campañas basadas en esta plantilla. La configuración se puede definir mediante la plantilla o por separado para cada campaña.



Documentos

Cuando se selecciona este módulo, se añade una pestaña adicional a la pestaña Edit de la plantilla y a las campañas basadas en esta plantilla. Los documentos adjuntos se pueden agregar desde la plantilla o bien por separado para cada campaña. Obtenga más información sobre los documentos en esta sección.



Descripción del envío

Cuando se selecciona este módulo, se añade una pestaña adicional de Delivery outlines a la pestaña de Documents para definir los esquemas de entrega de la campaña. Obtenga más información sobre los esquemas de entrega en esta sección.



Establecimiento de objetivos y flujos de trabajo

Al seleccionar el módulo de Targeting and workflows, se añade una pestaña para permitirle crear uno o más flujos de trabajo para las campañas basadas en esta plantilla. Los flujos de trabajo también se pueden configurar por separado para cada campaña basada en esta plantilla. Obtenga más información sobre los flujos de trabajo de campañas en esta sección.



Cuando este módulo está habilitado, se añade una pestaña Jobs a la configuración avanzada de la campaña para definir la secuencia de ejecución del proceso.

Aprobaciones

Si activa las Aprobaciones, puede seleccionar los procesos de aprobación y los operadores asignados al proceso de aprobación. Obtenga más información sobre aprobaciones en esta sección.



Puede elegir si desea habilitar o no la aprobación del proceso mediante la pestaña Approvals de la sección de configuración avanzada de plantillas.

Gastos y objetivos

Cuando se selecciona este módulo, se añade una pestaña de Budget a los detalles de la plantilla y a las campañas basadas en esta plantilla, de modo que se pueda seleccionar el presupuesto asociado.



Propiedades de plantilla


Cuando crea una plantilla de campaña, debe introducir la siguiente información:

Introduzca la etiqueta de la plantilla: la etiqueta es obligatoria y es la etiqueta predeterminada para todas las campañas basadas en esta plantilla.
Seleccione la naturaleza de la campaña en la lista desplegable. Los valores disponibles en esta lista son los guardados en la enumeración natureOp.
Obtenga información sobre cómo acceder y configurar las enumeraciones en esta página.

Seleccione el tipo de campaña: única, recurrente o periódica. De manera predeterminada, las plantillas de campaña se aplican a las campañas únicas. Las campañas recurrentes y periódicas se detallan en esta sección.

Especifique la duración de la campaña, es decir, el número de días durante los que se desarrolla la campaña. Al crear una campaña basada en esta plantilla, las fechas de inicio y finalización de la campaña se rellenan automáticamente.

Si la campaña es recurrente, debe especificar las fechas de inicio y finalización de la campaña directamente en la plantilla.

Especifique el programa relacionado de la plantilla: las campañas basadas en esta plantilla están vinculadas al programa seleccionado.

