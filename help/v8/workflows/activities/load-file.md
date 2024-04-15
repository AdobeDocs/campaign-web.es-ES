---
audience: end-user
title: Uso de la actividad de flujo de trabajo Cargar archivo
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Cargar archivo
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 935fba929c26d6d7b3057ee7c24148215a04e45e
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 42%

---

# Carga de archivo {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Actividad de carga de archivo"
>abstract="La actividad **Cargar archivo** es una actividad de **Administración de datos**. Utilice esta actividad para trabajar con datos almacenados en un archivo externo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Archivo de muestra"
>abstract="Archivo de muestra"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Nombre del archivo"
>abstract="Nombre del archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Base de datos de destino"
>abstract="Base de datos de destino"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Rechazar administración para la actividad Cargar archivo"
>abstract="Rechazar administración para la actividad Cargar archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Rechazar transición de salida de administración"
>abstract="Rechazar transición de salida de administración"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Rechazar transición de salida de administración para rechazos"
>abstract="Rechazar transición de salida de administración para rechazos"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formato para la actividad Cargar archivo"
>abstract="Formato para la actividad Cargar archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Archivo de destino para la actividad Carga de archivo"
>abstract="Archivo de destino para la actividad Carga de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Reasignación de valores para la actividad Carga de archivo"
>abstract="Reasignación de valores para la actividad Carga de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Comando Cargar archivo"
>abstract="Permitir el comando arbitrario para el preprocesamiento es un problema de seguridad. Deshabilite la opción de seguridad XtkSecurity_Disable_Preproc para forzar el uso de una lista predefinida de comandos."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Eliminar archivo tras la importación"
>abstract="Alternar el **Eliminar archivo tras importar** para eliminar el archivo original del servidor después de importar el archivo."

La actividad **Cargar archivo** es una actividad de **Administración de datos**. Utilice esta actividad para trabajar con perfiles y datos almacenados en un archivo externo. Los perfiles y los datos no se añaden a la base de datos, pero todos los campos del archivo de entrada están disponibles para [personalización](../../personalization/gs-personalization.md), o para actualizar perfiles o cualquier otra tabla.

>[!NOTE]
>Los formatos de archivo admitidos son: texto (TXT) y valor separado por comas (CSV).

Esta actividad se puede utilizar con un [Reconciliación](reconciliation.md) actividad para vincular datos no identificados a recursos existentes. Por ejemplo, la variable **Cargar archivo** la actividad se puede colocar antes de una **Reconciliación** actividad si importa datos no estándar en la base de datos.

## Configuración de la actividad Cargar archivo {#load-configuration}

Siga estos pasos para configurar el **Cargar archivo** actividad:

1. Añadir un **Cargar archivo** en el flujo de trabajo. Haga clic en **Seleccionar del archivo** botón.

1. Seleccione el archivo local que desea utilizar. El formato debe estar alineado con esto [archivo de muestra](../../audience/file-audience.md#sample-file).

1. Obtenga una vista previa y compruebe cómo se asignan los datos en la sección central de la pantalla.

   ![](../assets/load-file.png)

1. Utilice el **Columnas** del panel izquierdo para ajustar el tipo de datos y el ancho de cada columna.

1. En el **Formato** , ubicada en la configuración de columnas, especifique el formato del archivo externo para garantizar que los datos se importen correctamente.

1. Haga clic en **Confirmar** una vez que la configuración sea correcta.

## Ejemplo{#load-example}

Un ejemplo de carga de archivo externo utilizado con el **Reconciliación** la actividad está disponible en [esta sección](reconciliation.md#reconciliation-example).
