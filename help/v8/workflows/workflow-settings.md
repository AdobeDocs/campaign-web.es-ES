---
audience: end-user
title: Creación de flujos de trabajo con la web de Adobe Campaign
description: Aprenda a crear flujos de trabajo con Adobe Campaign Web
badge: label="Alpha" type="Positive"
source-git-commit: 60cd0ed8dcbe3e6003c1cde674fe3441d6d88869
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Configuración de los ajustes del flujo de trabajo {#workflow-settings}

contenido TBD

definir la configuración disponible en el botón del lienzo del flujo de trabajo
<!--à reformuler-->

## Propiedades del flujo de trabajo {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propiedades del flujo de trabajo"
>abstract="Por determinar"

(= igual que al crear el flujo de trabajo ? para comprobar)

* Etiqueta
* Opciones adicionales
* Nombre interno
* Carpeta
* Campaña vinculada > puede cambiarla. Si es así, el flujo de trabajo desaparecerá de la campaña actual y aparecerá en la nueva campaña vinculada
* Zona horaria: defina un huso horario específico para utilizarlo de forma predeterminada en todas las actividades del flujo de trabajo. De forma predeterminada, el uso horario del flujo de trabajo es la definida para el operador de Campaign actual.
* Supervisor: Cuando un flujo de trabajo presenta un error, se notifica por correo electrónico a los operadores que pertenecen al grupo de supervisión del flujo de trabajo, siempre que su dirección de correo electrónico aparezca en su perfil. Este grupo está seleccionado en el campo **[!UICONTROL Supervisor(s)]** de las propiedades del flujo de trabajo.
* descripción

## Configuración de segmentación

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Configuración de segmentación"
>abstract="Por determinar"

* dimensión de segmentación:

   Durante las operaciones de segmentación de datos, la clave de establecimiento de objetivos se asigna a una dimensión de filtrado. La dimensión objetivo permite definir la población objetivo de la operación: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. La dimensión de filtrado permite seleccionar la población en función de determinados criterios: titulares de contrato, suscriptores a boletines, etc.

* conservar resultados: La variable **Mantener el resultado de las poblaciones provisionales entre dos ejecuciones** mantiene las tablas temporales entre dos ejecuciones de un flujo de trabajo.  Está disponible en la pestaña **[!UICONTROL General]** de las propiedades del flujo de trabajo y se puede utilizar para fines de desarrollo y prueba para controlar los datos y comprobar los resultados. Puede utilizar esta opción en entornos de desarrollo, pero nunca en entornos de producción. Si mantiene las tablas temporales, el tamaño de la base de datos puede aumentar significativamente y finalmente alcanzar el límite de tamaño. Además, ralentiza la copia de seguridad.

   Solo se conservan las tablas de trabajo de la última ejecución del flujo de trabajo. El flujo de trabajo **[!UICONTROL cleanup]**, que se ejecuta diariamente, depura todas las tablas de trabajo de ejecuciones previas.

   >[!CAUTION]
   >
   >Esta opción debe **never** esté marcado en un **producción** flujo de trabajo. Esta opción se utiliza para analizar los resultados y está diseñada únicamente para fines de prueba y, por lo tanto, solo debe usarse en entornos de ensayo o desarrollo.

## Configuración de ejecución del flujo de trabajo

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Configuración de ejecución"
>abstract="Por determinar"

* Historial en días: Las tablas de trabajo de la base de datos mantienen un historial de ejecuciones (tareas, eventos, registros). Aquí puede definir el número de días que desea archivar para este flujo de trabajo: una vez al día, el proceso de limpieza elimina los archivos más antiguos. Si el valor de este campo es cero, el archivo no se elimina nunca.

   especifica el número de días después de los cuales se debe purgar el historial. El historial contiene elementos relacionados con el flujo de trabajo: registros, tareas, eventos (objetos técnicos vinculados a la operación del flujo de trabajo), así como archivos descargados por el **[!UICONTROL Transferir archivo]** actividad. El valor predeterminado es de 30 días para las plantillas de flujo de trabajo integradas.

   La depuración del historial se realiza mediante el flujo de trabajo técnico Database cleanup , que se ejecuta de forma predeterminada todos los días

   >[!IMPORTANT]
   >
   >Si la variable **[!UICONTROL Historial en días]** se deja en blanco, su valor se considerará &quot;1&quot;, lo que significa que el historial se purgará después de 1 día.

* afinidad predeterminada: este campo permite forzar un flujo de trabajo o una actividad de flujo de trabajo para que se ejecute en un equipo en particular.   Si su instalación incluye varios servidores de flujo de trabajo, utilice este campo para elegir el equipo en el que desea ejecutar el flujo de trabajo. Si el valor introducido en este campo no existe en ningún servidor, el flujo de trabajo se mantiene pendiente.

* guardar consultas sql en el registro: permite guardar las consultas SQL del flujo de trabajo en los registros. (¿dónde acceder a los registros sql?)

   Esta funcionalidad se reserva únicamente a los usuarios avanzados. Afecta a los flujos de trabajo que incluyen actividades de objetivos (consulta, unión, intersección, etc.). Cuando se activa esta opción, las consultas SQL enviadas a la base de datos durante la ejecución del flujo de trabajo se muestran en Adobe Campaign: esto significa que puede revisarlas para optimizar consultas o diagnosticar problemas.

   Las consultas se muestran en una pestaña **[!UICONTROL SQL logs]** que se añade al flujo de trabajo (excepto a los flujos de trabajo de la campaña) y a la actividad **[!UICONTROL Properties]** cuando la opción está activada. La pestaña **[!UICONTROL Audit]** también incluye consultas SQL.

## Configuración de gestión de errores

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Configuración de gestión de errores"
>abstract="Por determinar"

* Este campo permite definir las acciones que se deben llevar a cabo si una tarea de flujo de trabajo presenta errores. Hay dos opciones posibles:

   Stop the process: el flujo de trabajo se pone en pausa automáticamente. El estado del proceso cambia a Failed. Una vez resuelto el problema, reinicie el flujo de trabajo con los botones Start o Restart.

   Ignore: el estado de la tarea que activó el error cambia a Failed, pero el flujo de trabajo mantiene el estado Started. Esta configuración es importante para tareas recurrentes: si la rama incluye un planificador, la próxima vez que se ejecute el flujo de trabajo se inicia de forma normal.

* Errores consecutivos: Este campo está disponible cuando el valor Ignore está seleccionado en el campo In case of errors . Puede especificar el número de errores que se pueden omitir antes de que se detenga el proceso. Una vez alcanzado este número, el estado del flujo de trabajo cambia a Failed. Si el valor de este campo es 0, el flujo de trabajo nunca se detiene, independientemente del número de errores.
