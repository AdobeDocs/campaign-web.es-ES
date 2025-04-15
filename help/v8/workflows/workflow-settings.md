---
audience: end-user
title: Configuración del flujo de trabajo
description: Aprenda a configurar los ajustes de flujo de trabajo con Adobe Campaign Web
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 17%

---

# Configuración del flujo de trabajo {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Propiedades del flujo de trabajo"
>abstract="En esta pantalla, elija la plantilla que desea utilizar para crear el flujo de trabajo y especifique una etiqueta. Expanda la **sección Opciones adicionales** para configurar más opciones, como el nombre interno del flujo de trabajo, su carpeta, zona horaria y grupo supervisor. Se recomienda muy especialmente seleccionar un grupo de supervisores para que los operadores sean advertidos si se produce un error."

Al crear una flujo de trabajo u organizar actividades flujo de trabajo en el lienzo, acceda a la configuración avanzada relacionada con el flujo de trabajo. Por ejemplo, establezca una zona horaria específica para el flujo de trabajo, administrar cómo debe comportarse el flujo de trabajo en caso de error o administrar el retraso después del cual se depura el historial de flujo de trabajo.

Estos ajustes están preconfigurados en la plantilla seleccionada al crear el flujo de trabajo, pero se pueden editar según sea necesario para este flujo de trabajo específico.

![Configuración del flujo de trabajo botón interfaz](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## Propiedades del flujo de trabajo {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propiedades del flujo de trabajo"
>abstract="En esta sección se proporcionan propiedades genéricas de flujo de trabajo a las que también se puede acceder al crear el flujo de trabajo. Puede elegir la plantilla que desea utilizar para crear el flujo de trabajo y especificar una etiqueta. Expanda la sección Opciones adicionales para configurar opciones específicas, como el flujo de trabajo que almacena la carpeta o la zona horaria."

La sección **[!UICONTROL Propiedades]** proporciona opciones genéricas que se pueden configurar al crear un flujo de trabajo. Para acceder a las propiedades de un flujo de trabajo existente, haga clic en el botón **[!UICONTROL Configuración]** disponible en la barra de acciones situada encima del lienzo del flujo de trabajo.

![Interfaz de configuración de flujo de trabajo](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}

Estas propiedades incluyen:

* La **[!UICONTROL etiqueta]** del flujo de trabajo que se muestra en la lista.
* **[!UICONTROL Nombre interno]** del flujo de trabajo.
* **[!UICONTROL Carpeta]** en la que se debe guardar el flujo de trabajo.
* La **[!UICONTROL zona horaria]** predeterminada para usar en todas las actividades del flujo de trabajo. De forma predeterminada, la zona horaria del flujo de trabajo es la definida para el operador de Campaign actual.
Los valores posibles son:
   * **Zona** horaria del servidor para utilizar la zona horaria del servidor de aplicación de Adobe Campaign.
   * **Zona horaria** del operador para utilizar la zona horaria del operador Adobe Campaign que ejecuta el flujo de trabajo, tal como se define en la perfil del operador en la consola del cliente.
   * **Zona horaria de la base de datos** para utilizar la zona horaria del servidor de base de datos.
   * Una zona horaria específica.
* Cuando un flujo de trabajo falla, los operadores pertenecientes al operador grupo seleccionados en el **[!UICONTROL campo Supervisor(es)]** son notificados por correo electrónico.
* Especifique un **[!UICONTROL Descripción]** del flujo de trabajo.

Cuando el flujo de trabajo se [asocia a un campaña](create-workflow.md), se muestra en el **[!UICONTROL campo campaña]** vinculado. Abra la campaña asociada desde ese campo.

## Configuración de segmentación {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Configuración de segmentación"
>abstract="En esta sección, puede seleccionar el dimensión de segmentación para destino perfiles en el flujo de trabajo y elegir mantener los resultados flujo de trabajo entre dos ejecuciones. Esta opción solo debe utilizarse con fines de prueba y nunca debe habilitarse en un flujo de trabajo de producción."

* **[!UICONTROL Dimensión de segmentación]**: Seleccione la dimensión de segmentación que se utilizará para segmentar perfiles, como destinatarios, beneficiarios de contratos, operadores, suscriptores y otros. [Más información sobre las dimensiones de segmentación](../audience/targeting-dimensions.md).

* **[!UICONTROL Mantener el resultado de poblaciones provisionales entre dos ejecuciones]**: De forma predeterminada, solo se conservan las tablas de trabajo de la última ejecución del flujo de trabajo. Las tablas de trabajo de ejecuciones anteriores se depuran mediante un flujo de trabajo técnico, que se ejecuta diariamente.

  Si esta opción está activada, las tablas de trabajo se conservarán incluso después de ejecutar el flujo de trabajo. Utilícelo con fines de prueba y asegúrese de que se usa **solamente** en entornos de ensayo o desarrollo. Nunca se debe comprobar en un flujo de trabajo de producción.

## Configuración de ejecución {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Configuración de ejecución"
>abstract="En esta sección, puede configurar las opciones relacionadas con la ejecución del flujo de trabajo, como el número de días que se mantiene el historial del flujo de trabajo."

* **[!UICONTROL Historial en días]**: especifica el número de días después de los cuales se debe purgar el historial. El historial contiene elementos relacionados con el flujo de trabajo, como registros, tareas y eventos (objetos técnicos vinculados a la operación de flujo de trabajo). El valor predeterminado es 30 días para plantillas de flujo de trabajo predeterminadas. La depuración del historial se realiza mediante el flujo de trabajo técnico Database cleanup, que se ejecuta a diario.

  >[!IMPORTANT]
  >
  >Si el campo Historial **[!UICONTROL en días]** se deja en blanco, su valor se considerará como &quot;1&quot;, lo que significa que el historial se purgará después de 1 día.

* **[!UICONTROL afinidad]** predeterminada: Si la instalación incluye varios servidores flujo de trabajo, utilice este campo para especificar el servidor en el que se ejecutará la flujo de trabajo. Esto fuerza la ejecución de ese flujo de trabajo en un servidor determinado. Elija un nombre de afinidad existente, pero asegúrese de no utilizar espacios ni signos de puntuación. Si utiliza servidores diferentes, especifique nombres diferentes separados por comas.

  >[!IMPORTANT]
  >
  >Si el valor definido en este campo no existe en ningún servidor, el flujo de trabajo permanecerá pendiente.

* **[!UICONTROL Guardar consultas SQL en el registro]**: marque esta opción para guardar las consultas SQL del flujo de trabajo en los registros. Esta funcionalidad se reserva únicamente a los usuarios avanzados. Se aplica a los flujos de trabajo que contienen actividades de segmentación, como **[!UICONTROL Generar audiencia]**. Cuando esta opción está habilitada, las consultas SQL enviadas a la base de datos durante la ejecución del flujo de trabajo se muestran en los registros del flujo de trabajo, lo que le permite analizarlas para optimizar consultas o diagnosticar problemas.

## Configuración de administración de errores {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Configuración de administración de errores"
>abstract="En esta sección, puede definir cómo el flujo de trabajo debe administrar errores durante su ejecución. Puede optar por poner en pausa el proceso, ignorar un determinado número de errores o detener la ejecución del flujo de trabajo."

* **[!UICONTROL Administración de errores]**: este campo permite definir las acciones que deben realizarse si una tarea de flujo de trabajo tiene errores. Hay tres opciones posibles:

   * **[!UICONTROL Suspender el proceso]**: el flujo de trabajo se pone en pausa automáticamente y su estado cambia a **[!UICONTROL Error]**. Una vez resuelto el problema, reanude el flujo de trabajo con los botones **[!UICONTROL Reanudar]**.
   * **[!UICONTROL Ignorar]**: El estado de la tarea que activó el error cambia a **[!UICONTROL Fallido]**, pero el flujo de trabajo mantiene el estado **[!UICONTROL Iniciado]**. <!-- TO ADD ONCE SCHEDULER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Anular el proceso]**: el flujo de trabajo se detiene automáticamente y su estado cambia a **[!UICONTROL Error]**. Una vez resuelto el problema, reinicie el flujo de trabajo con los botones **[!UICONTROL Start]**.

* **[!UICONTROL Errores consecutivos]**: este campo está disponible cuando se selecciona el **[!UICONTROL valor Ignorar]** en el **[!UICONTROL campo En caso de errores]** . Especifique el número de errores que se pueden omitir antes de que se detenga el proceso. Una vez alcanzado este número, el estado del flujo de trabajo cambia a **[!UICONTROL Failed]**. Si el valor de este campo es 0, el flujo de trabajo nunca se detiene, independientemente del número de errores.

## Script de inicialización {#initialization-script}

La **secuencia de comandos** de inicialización permite inicializar variables o modificar actividad propiedades. Haga clic en el **botón código** Editar y escriba el fragmento de código que desea ejecutar. Se llama al script cuando se ejecuta el flujo de trabajo. Consulte la sección relacionada con [variables de eventos](../workflows/event-variables.md).