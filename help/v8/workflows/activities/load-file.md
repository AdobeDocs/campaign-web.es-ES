---
audience: end-user
title: Uso de la actividad de flujo de trabajo Cargar archivo
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Cargar archivo
badge: label="Disponibilidad limitada"
source-git-commit: 47fd0ab358a28ed09d9ab0de3b9dfab5a1592634
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 33%

---

# Carga de archivo {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Actividad de carga de archivo"
>abstract="El **Cargar archivo** la actividad es una **Administración de datos** actividad. Utilice esta actividad para trabajar con datos almacenados en un archivo externo."

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


El **Cargar archivo** la actividad es una **Administración de datos** actividad. Utilice esta actividad para trabajar con perfiles y datos almacenados en un archivo externo. Los perfiles y los datos no se añaden a la base de datos, pero todos los campos del archivo de entrada están disponibles para [personalización](../../personalization/gs-personalization.md), o para actualizar perfiles o cualquier otra tabla.

>[!NOTE]
>Los formatos de archivo admitidos son: texto (TXT) y valor separado por comas (CSV).

Esta actividad se puede utilizar con un [Reconciliación](reconciliation.md) actividad para vincular datos no identificados a recursos existentes. Por ejemplo, la variable **Cargar archivo** la actividad se puede colocar antes de una **Reconciliación** actividad si importa datos no estándar en la base de datos.

## Configuración de la actividad Cargar archivo {#load-configuration}

Siga estos pasos para configurar el **Cargar archivo** actividad:

1. Arrastrar y soltar una **Cargar archivo** en el flujo de trabajo. Haga clic en **Seleccionar del archivo** botón.

1. Seleccione el archivo local que desea utilizar. El formato debe estar alineado con esto [archivo de muestra](../../audience/file-audience.md#sample-file).

1. Obtenga una vista previa y compruebe cómo se asignan los datos en la sección central de la pantalla.

   ![](../assets/load-file.png)

1. Ajuste la configuración de columna y cómo dar formato a los datos desde las opciones disponibles.

1. Haga clic en **Confirmar** una vez que la configuración sea correcta.

## Ejemplo{#load-example}

Hay disponible una muestra de un archivo externo de carga con el **Reconciliación** actividad en [esta sección](reconciliation.md#example).