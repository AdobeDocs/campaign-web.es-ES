---
audience: end-user
title: Utilizar el archivo de carga flujo de trabajo actividad
description: Aprenda a usar el actividad de flujo de trabajo Cargar archivo
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 30%

---

# Carga de archivo {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Actividad Cargar archivo"
>abstract="La actividad **Cargar archivo** es una actividad de **Administración de datos**. Utilice esta actividad para trabajar con los datos almacenados en un archivo externo. Los perfiles y los datos no se añaden a la base de datos, pero todos los campos del archivo de entrada están disponibles para la personalización, o para actualizar perfiles o cualquier otra tabla."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Rechazar transición de salida de administración"
>abstract="Rechazar transición de salida de administración"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Rechazar transición de salida de administración para rechazos"
>abstract="Rechazar transición de salida de administración para rechazos"

La actividad **Cargar archivo** es una actividad de **Administración de datos**. Utilice esta actividad para trabajar con perfiles y datos almacenados en un archivo externo. Los perfiles y los datos no se agregan a la base de datos, pero todos los campos del archivo de entrada están disponibles para [personalización](../../personalization/gs-personalization.md), para actualizar perfiles o cualquier otra tabla.

>[!NOTE]
>Los formatos de archivo admitidos son: texto (TXT) y valor separado por comas (CSV). Puede cargar archivos con un tamaño máximo de 50 MB.

Este actividad puede utilizarse con un [actividad de reconciliación](reconciliation.md) para vincular datos no identificados a los recursos existentes. Por ejemplo, la **actividad Cargar archivo** puede colocarse ante una **actividad de reconciliación** si importa datos no estándar en la base de datos.

## Configure el actividad de carga de archivos {#load-configuration}

La **configuración del actividad del archivo** de carga consta de dos pasos. En primer lugar, defina la estructura de archivos esperada cargando un archivo de muestra. Una vez hecho esto, especifique el origen del archivo cuyos datos se importarán. Siga los pasos a continuación para configurar la actividad.

![Captura de pantalla de configuración de actividad de archivo de carga de flujo de trabajo](../assets/workflow-load-file.png)

### Configurar el archivo de muestra {#sample}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Archivo de muestra"
>abstract="Para seleccionar la estructura de archivo prevista cargue un archivo de muestra. "

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formato para la actividad Cargar archivo"
>abstract="En la sección **Formato**, especifique cómo se formatea el archivo para garantizar que los datos se importen correctamente."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Reasignación de valores para la actividad Carga de archivo"
>abstract="Utilice esta opción para asignar valores específicos de los archivos cargados con valores nuevos. Por ejemplo, si la columna contiene valores &#39;True&#39;/&#39;False&#39;, puede agregar una asignación para reemplazar automáticamente esos valores por caracteres &#39;0&#39;/&#39;1&#39;."

Siga estos pasos para configurar el archivo de ejemplo utilizado para definir la estructura de archivos esperada:

1. añadir un actividad **de** archivo de carga en su flujo de trabajo.

1. Seleccione el archivo de muestra que se utilizará para definir la estructura de archivos que se desee. Para ello, haga clic en el botón Seleccionar **archivo en la**[!UICONTROL  sección Archivo de muestra ]**y seleccione el archivo local** que desea utilizar.

   >[!NOTE]
   >
   >Los datos del archivo de muestra se utilizan para configurar la actividad, pero no se importan. Utilice un archivo de muestra que contenga pocos datos. El formato del archivo debe estar alineado con este [archivo](../../audience/file-audience.md#sample-file) de muestra.

1. Se muestra una vista previa del archivo de muestra, que muestra un máximo de 30 líneas.

1. En la lista desplegable **[!UICONTROL Tipo de archivo]**, especifique si el archivo utiliza columnas delimitadas o de ancho fijo.

   ![Ejemplo de captura de pantalla de la configuración de Archivo](../assets/workflow-load-file-sample.png)

1. Para los tipos de archivo de columnas delimitadas, utilice la **sección Columnas** para configurar las propiedades de cada columna.

   +++Opciones disponibles para las columnas de archivos

   * **[!UICONTROL Etiquetar]**: Etiquetar mostrar para la columna.
   * **[!UICONTROL Tipo de datos]**: Tipo de datos contenidos en la columna.
   * **[!UICONTROL Width]** (tipo de datos de cadena): número máximo de caracteres que se mostrarán en la columna.
   * **[!UICONTROL Transformación de datos]** (tipo de datos de cadena): aplique la transformación a los valores contenidos en la columna.
   * **[!UICONTROL Administración de espacios en blanco]** (tipo de datos de cadena): especifique cómo administrar los espacios contenidos en la columna.
   * **[!UICONTROL Separadores]** (tipos de datos de fecha, hora, entero y número): especifique los caracteres que se usarán como separadores.
   * **[!UICONTROL Permitir valores NULL: especifique cómo administrar valores vacíos]** en la columna. La opción &quot;Adobe Campaign valor predeterminado&quot; arrojará un error si hay un valor vacío.
   * **[!UICONTROL Error procesamiento]** (tipo de datos de cadena): Especifique el comportamiento en caso de errores en una de las líneas.
   * **[!UICONTROL Valor reasignación]**: Esta opción le permite asignar valores específicos por otros nuevos. Por ejemplo, si la columna contiene valores &quot;True&quot;/&quot;False&quot;, puede añadir una asignación para reemplazar automáticamente esos valores por los caracteres &quot;0&quot;/&quot;1&quot;.

+++

1. En la sección **Formato**, especifique cómo se formatea el archivo para garantizar que los datos se importen correctamente.

### Definición del archivo de destino para cargar {#target}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Archivo de destino para la actividad Cargar archivo"
>abstract="En la sección **[!UICONTROL Archivo de destino]**, especifique cómo recuperar el archivo para cargarlo en el servidor."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Nombre del archivo"
>abstract="Especifique el nombre del campo que se va a cargar en el servidor. Haga clic en el icono de **[!UICONTROL Abrir cuadro de diálogo de personalización]** para utilizar el editor de expresiones, incluidas las variables de evento, para calcular el nombre del archivo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Base de datos de destino"
>abstract="Si accede a una actividad **[!UICONTROL Cargar archivo]** que ya se ha configurado en la consola del cliente, hay disponible una sección **[!UICONTROL Base de datos de Target]** adicional si ha configurado la actividad para cargar el archivo en una base de datos externa."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Comando Cargar archivo"
>abstract="Permitir el comando arbitrario para el preprocesamiento es un problema de seguridad. Deshabilite la opción de seguridad XtkSecurity_Disable_Preproc para forzar el uso de una lista predefinida de comandos."

>[!CAUTION]
>
>Antes de cargar el archivo de destino, asegúrese de que se adhiera al formato del archivo de muestra. Cualquier discrepancia en el formato de archivo, la estructura de columnas o el número de columnas puede provocar errores durante la ejecución del flujo de trabajo.

Para definir el archivo destino que desea cargar, seguir estos pasos:

1. En la **[!UICONTROL sección Target archivo]** , especifique la acción que debe realizar al recuperar el archivo para cargar en el servidor.

   * **[!UICONTROL Cargar archivo desde el equipo]** local: Seleccione el archivo que desea cargar desde su equipo.

   * **[!UICONTROL Especificado en el transición]**: Cargue el archivo especificado en el transición entrante próximo de un actividad anterior, como **[!UICONTROL Transferir archivo]**.

   * **[!UICONTROL Preprocesar el archivo]**: Cargue el archivo especificado en la transición anterior y aplíquele un comando de preprocesamiento, como **[!UICONTROL Descompresión]** o **[!UICONTROL Descifrar]**.

   * **[!UICONTROL Calculado]**: cargue el archivo cuyo nombre se especifique en el **[!UICONTROL campo Nombre Archivo]** . Haga clic en el icono de **[!UICONTROL Abrir cuadro de diálogo de personalización]** para utilizar el editor de expresiones, incluidas las variables de evento, para calcular el nombre del archivo.

   ![Captura de pantalla de configuración Archivo de Target](../assets/workflow-load-file-config.png)

   >[!NOTE]
   >
   >Si está accediendo a un **[!UICONTROL actividad de carga de archivo]** que ya se ha configurado en la consola del cliente, se mostrará una sección adicional **[!UICONTROL de base de datos]** Target si ha configurado el actividad para cargar el archivo a una base de datos externa. Permite especificar si desea cargar el archivo en el servidor Campaign o en la base de datos externa.

### Opciones adicionales {#options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Gestión de rechazo para la actividad Cargar archivo"
>abstract="En la sección **Rechazar administración**, especifique cómo debe comportarse la actividad en caso de errores. Puede definir el número máximo de errores que desea permitir y activar la opción **[!UICONTROL Mantener rechazos en un archivo]** para descargar en el servidor un archivo que contenga los errores producidos durante la importación."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Eliminar archivo tras la importación"
>abstract="Active **Eliminar el archivo tras la importación** para eliminar el archivo original del servidor después de importar el archivo."

1. En la **sección Administración** de rechazos, especifique cómo debe comportarse el actividad en caso de errores:

   * En el **[!UICONTROL campo Número de errores permitidos]** , especifique el número máximo de errores que se autorizan al procesar el archivo que se va a cargar. Por ejemplo, si el valor se establece en &quot;20&quot;, la ejecución del flujo de trabajo fallará si hay más de 20 errores al cargar el archivo.

   * Para evitar errores al cargar el archivo, active la opción **[!UICONTROL Conservar rechazos en un archivo]** y especifique el nombre que desee para el archivo en el campo **[!UICONTROL Archivo rechazado]**.

     Después de activar esta opción, se agrega una transición de salida adicional denominada &quot;Complemento&quot; después de la actividad. Cualquier error que se produzca durante la importación se almacenará en el archivo especificado del servidor.

1. Para eliminar el archivo cargado del servidor después de ejecutar el flujo de trabajo, active la opción **[!UICONTROL Eliminar archivo después de importar]**.

   ![Captura de pantalla de configuración de opciones adicionales](../assets/workflow-load-file-options.png)

1. Haga clic en **Confirmar** una vez que la configuración sea correcta.

## Ejemplo {#load-example}

En esta sección](reconciliation.md#reconciliation-example) encontrará un ejemplo de carga de archivos externos que se utilizará con el **actividad [de reconciliación**.