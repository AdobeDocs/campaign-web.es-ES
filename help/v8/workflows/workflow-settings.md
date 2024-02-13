---
audience: end-user
title: Configuración del flujo de trabajo
description: Obtenga información sobre cómo configurar los ajustes del flujo de trabajo con Adobe Campaign Web
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 28%

---


# Configuración del flujo de trabajo {#workflow-settings}

Al organizar actividades de flujo de trabajo en el lienzo, puede acceder a la configuración avanzada relacionada con el flujo de trabajo. Por ejemplo, puede establecer una zona horaria específica para el flujo de trabajo, administrar cómo debe comportarse el flujo de trabajo en caso de error o administrar el retraso tras el cual debe purgarse el historial del flujo de trabajo.

Estos ajustes están preconfigurados en la plantilla seleccionada al crear el flujo de trabajo, pero se pueden editar según sea necesario para este flujo de trabajo específico.

Para ello, haga clic en el **[!UICONTROL Configuración]** disponible en la barra de acciones sobre el lienzo del flujo de trabajo.

![](assets/workflow-settings-button.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}

## Propiedades del flujo de trabajo {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propiedades del flujo de trabajo"
>abstract="En esta sección se proporcionan propiedades genéricas de flujo de trabajo a las que también se puede acceder al crear el flujo de trabajo. Puede elegir la plantilla que desea utilizar para crear el flujo de trabajo y especificar una etiqueta. Expanda la sección Opciones adicionales para configurar ajustes específicos, como el flujo de trabajo que almacena la carpeta o la zona horaria."

El **[!UICONTROL Propiedades]** proporciona una configuración genérica a la que también se puede acceder al crear el flujo de trabajo.

![](assets/workflow-settings.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}


Estas propiedades son:

* El **[!UICONTROL Etiqueta]** del flujo de trabajo que se muestra en la lista.
* El **[!UICONTROL Nombre interno]** del flujo de trabajo.
* El **[!UICONTROL Carpeta]** donde se debe guardar el flujo de trabajo.
* El valor predeterminado **[!UICONTROL Timezone]** para usar en todas las actividades del flujo de trabajo. De forma predeterminada, el huso horario del flujo de trabajo es el definido para el operador de Campaign actual.
Los valores posibles son:
   * **Zona horaria del servidor** para utilizar la zona horaria del servidor de aplicaciones de Adobe Campaign
   * **Zona horaria del operador** to utiliza el huso horario del operador de Adobe Campaign que ejecuta el flujo de trabajo, tal como se define en el perfil del operador, en la consola del cliente
   * **Zona horaria de la base de datos** para utilizar la zona horaria del servidor de la base de datos
   * Una zona horaria específica
* Cuando falla un flujo de trabajo, los operadores que pertenecen al grupo de operadores seleccionado en la **[!UICONTROL Supervisor(s)]** se notifican por correo electrónico.
* También puede introducir una **[!UICONTROL Descripción]** del flujo de trabajo.

Cuando el flujo de trabajo es [asociado a una campaña](create-workflow.md), se muestra en la **[!UICONTROL Campaña vinculada]** field. Puede abrir la campaña asociada desde ese campo.


## Configuración de segmentación  {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Configuración de segmentación"
>abstract="En esta sección, puede seleccionar la dimensión de segmentación para segmentar los perfiles en el flujo de trabajo y elegir mantener los resultados del flujo de trabajo entre dos ejecuciones. Esta opción solo debe utilizarse con fines de prueba y nunca debe habilitarse en un flujo de trabajo de producción."

* **[!UICONTROL Dimensión de segmentación]**: Seleccione la dimensión de segmentación que se utilizará para segmentar los perfiles: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. [Más información sobre las dimensiones de segmentación](../audience/targeting-dimensions.md)

* **[!UICONTROL Mantener el resultado de poblaciones provisionales entre dos ejecuciones]**: De forma predeterminada, solo se conservan las tablas de trabajo de la última ejecución del flujo de trabajo. Las tablas de trabajo de ejecuciones anteriores se depuran mediante un flujo de trabajo técnico, que se ejecuta diariamente.

  Si esta opción está activada, las tablas de trabajo se conservarán incluso después de ejecutar el flujo de trabajo. Puede utilizarlo con fines de prueba y, por lo tanto, debe utilizarlo **solamente** en entornos de ensayo o desarrollo. Nunca se debe comprobar en un flujo de trabajo de producción.

## Configuración de ejecución  {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Configuración de ejecución"
>abstract="En esta sección, puede configurar las opciones relacionadas con la ejecución del flujo de trabajo, como el número de días que se mantiene el historial del flujo de trabajo."

* **[!UICONTROL Historial en días]**: especifica el número de días después de los cuales se debe purgar el historial. El historial contiene elementos relacionados con el flujo de trabajo: registros, tareas, eventos (objetos técnicos vinculados a la operación de flujo de trabajo). El valor predeterminado es de 30 días para las plantillas de flujo de trabajo predeterminadas. La depuración del historial se realiza mediante el flujo de trabajo de limpieza de la base de datos técnico, que se ejecuta de forma predeterminada todos los días.

  >[!IMPORTANT]
  >
  >Si el campo **[!UICONTROL Historial en días]** se deja en blanco, su valor se considerará “1”, lo que significa que el historial se purgará después de un día.

* **[!UICONTROL Afinidad predeterminada]**: Si la instalación incluye varios servidores de flujo de trabajo, utilice este campo para especificar el servidor en el que se ejecutará el flujo de trabajo. Esto fuerza la ejecución de ese flujo de trabajo en un servidor concreto. Puede elegir cualquier nombre de afinidad existente, pero asegúrese de no utilizar espacios ni signos de puntuación. Si utiliza servidores diferentes, especifique nombres diferentes separados por comas.

  >[!IMPORTANT]
  >
  >Si el valor definido en este campo no existe en ningún servidor, el flujo de trabajo permanece pendiente.


* **[!UICONTROL Guardar consultas SQL en el registro]**: Marque esta opción para guardar las consultas SQL del flujo de trabajo en los registros. Esta funcionalidad se reserva únicamente a los usuarios avanzados. Se aplica a flujos de trabajo que contienen actividades de segmentación como **[!UICONTROL Crear audiencia]**. Cuando esta opción está habilitada, las consultas SQL enviadas a la base de datos durante la ejecución del flujo de trabajo se muestran en los registros del flujo de trabajo, lo que le permite analizarlas para optimizar consultas o diagnosticar problemas.

## Configuración de administración de errores  {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Configuración de administración de errores"
>abstract="En esta sección, puede definir cómo el flujo de trabajo debe administrar errores durante su ejecución. Puede optar por poner en pausa el proceso, ignorar un determinado número de errores o detener la ejecución del flujo de trabajo."

* **[!UICONTROL Administración de errores]**: Este campo permite definir las acciones que se deben realizar si una tarea de flujo de trabajo presenta errores. Hay tres opciones posibles:

   * **[!UICONTROL Suspender el proceso]**: el flujo de trabajo se pone en pausa automáticamente y su estado cambia a **[!UICONTROL Error]**. Una vez resuelto el problema, reanude el flujo de trabajo con la variable **[!UICONTROL Reanudar]** botones.
   * **[!UICONTROL Ignorar]**: el estado de la tarea que activó el error cambia a **[!UICONTROL Error]**, pero el flujo de trabajo mantiene el **[!UICONTROL Iniciado]** estado. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Anular el proceso]**: el flujo de trabajo se detiene automáticamente y su estado cambia a **[!UICONTROL Error]**. Una vez resuelto el problema, reinicie el flujo de trabajo con la variable **[!UICONTROL Inicio]** botones.

* **[!UICONTROL Consecutive errors]**: este campo está disponible cuando la variable **[!UICONTROL Ignorar]** El valor está seleccionado en **[!UICONTROL En caso de errores]** field. Puede especificar el número de errores que se pueden omitir antes de que se detenga el proceso. Una vez alcanzado este número, el estado del flujo de trabajo cambia a **[!UICONTROL Failed]**. Si el valor de este campo es 0, el flujo de trabajo nunca se detiene, independientemente del número de errores.
