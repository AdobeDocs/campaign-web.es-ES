---
audience: end-user
title: Utilice el archivo Extract flujo de trabajo actividad
description: Aprenda a usar el archivo de Extract flujo de trabajo actividad
exl-id: fa50ab5b-2539-4517-9d7b-93315f1e505c
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 10%

---

# Extracción de archivos {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Extracción de archivos"
>abstract="La actividad **Extraer archivo** permite exportar datos desde Adobe Campaign en forma de archivo externo. A continuación, los datos se pueden exportar a una ubicación de servidor, como SFTP, almacenamiento en la nube o el servidor campaña mediante un actividad de transferencia de archivos."

El **actividad del archivo** Extract es un **actividad de administración de** datos. Utilice este actividad para exportar datos de Adobe Campaign en forma de archivo externo. A continuación, los datos se pueden exportar a una ubicación de servidor, como SFTP, almacenamiento en la nube o el servidor campaña mediante un actividad de transferencia de archivos.

Para configurar el **archivo de Extract** actividad, agregue un actividad de **archivo** Extract a su flujo de trabajo y luego seguir los pasos que se indican a continuación.

## Configurar el archivo que va a extraer {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="Archivo que extraer"
>abstract="Seleccione el archivo que va a extraer."

La **[!UICONTROL sección Archivo a extracción]** permite configurar las propiedades del archivo y los datos que se van a incluir.

![Captura de pantalla que muestra las opciones de configuración del archivo a extracción.](../assets/extract-file-file.png)

1. En el **[!UICONTROL campo Nombre Archivo]** , escriba el nombre deseado para el archivo que desea extracción.

   Puede personalizar el nombre del archivo mediante evento variables, condiciones y funciones de fecha y hora. Para ello, haga clic en el icono Abrir **[!UICONTROL personalización cuadro de diálogo]** para abrir el editor expresión. [Aprenda a trabajar con variables evento y con el editor expresión](../event-variables.md).

1. Especifique las columnas que desea presentar en el archivo extraído. Para ello, siga estos pasos:

   1. Haga clic en la añadir columna **&#x200B;**&#x200B;de salida.
   1. Seleccione el atributo que desea mostrar en la columna y, a continuación, confirme la selección. Los atributos disponibles dependen del dimensión de segmentación del flujo de trabajo. [Aprenda a seleccionar atributos y agregarlos a favoritos](../../get-started/attributes.md).
   1. Una vez añadida la columna, puede cambiar su **[!UICONTROL Etiquetar y modificar el atributo asociado**&#x200B;**.]**
   1. Si desea aplicar un transformación a los valores de la columna, selecciónelo en la lista desplegable. Por ejemplo, puede cambiar todos los valores de la columna seleccionada a mayúsculas.

1. Repita estos pasos para agregar tantas columnas como sea necesario en el archivo extracción. Para cambiar la posición de una columna, utilice las flechas arriba y abajo.

1. Para eliminar todas las filas duplicado del archivo extraído, active la **[!UICONTROL opción Quitar duplicado filas (Listado).]**

1. Para ordenar el archivo extraído en función de un atributo, active la **[!UICONTROL opción Habilitar ordenación]** y, a continuación, elija el atributo por el que desea ordenar el archivo, junto con el método de ordenación deseado (ascendente o de bajada). Puede ordenar cualquier atributo del dimensión de segmentación actual, independientemente de si se ha agregado o no a las columnas del archivo.

## Configurar el formato del archivo extraído {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Formato de destino"
>abstract="Seleccione las distintas opciones para configurar el formato del archivo extraído."

La **[!UICONTROL sección formato de destino]** le permite configurar el formato del archivo extraído.

1. Elija el formato Output **[!UICONTROL para el archivo extraído:** Texto **,** Texto con columnas **de ancho fijo,** CSV (Excel)**o** XML **.]**

1. Haga clic en el **[!UICONTROL botón formato]** extracción para acceder a opciones específicas relacionadas con el formato seleccionado. Amplíe la sección siguiente para obtener más información.

+++ Opciones de formato de extracción disponibles

   * **[!UICONTROL Use la primera línea como encabezado]** de columna (texto / CSV (Excel) formato): active esta opción para usar la primera columna como encabezado.
   * **[!UICONTROL Separador]** de columnas (formato de texto): especifique el carácter que se utilizará como separador de columnas en el archivo de salida.
   * **[!UICONTROL Delimitador]** de cadenas (formato de texto): especifique cómo delimitar las cadenas en el archivo de salida.
   * **[!UICONTROL Final de línea]** (texto formato): especifique cómo delimitar el final de líneas en el archivo de salida.
   * **[!UICONTROL Codificación]**: elija la codificación del archivo de salida.
   * **[!UICONTROL formato y separadores de fecha:]** especifique cómo se debe dar formato a las fechas en el archivo de salida.
   * **[!UICONTROL Número formato]**: especifique cómo se debe dar formato a los números en el archivo de salida.
   * **[!UICONTROL Exportar etiquetas en lugar de valores internos de enumeraciones]**: active esta opción si exporta valores de lista desglosada y desea recuperar etiquetas de columna, que son más fáciles de entender, en lugar de ID internos.

+++

   ![Captura de pantalla que muestra las opciones de configuración del archivo a extracción.](../assets/extract-file-format.png)

## Añadir una fase posprocessamiento {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Posprocesamiento"
>abstract="Defina un paso de procesamiento electrónico de entrada para aplicar, gustar compresión o cifrado."

La **[!UICONTROL secuencia de comandos]** de modificación Exportar permite aplicar un fase de procesamiento para ejecutar durante el extracción de datos, como compresión o cifrado. Para ello, haga clic en la secuencia de comandos **de** Editar botón.

Se abrirá la editor expresión, permitiéndole introducir el comando que desea aplicar al archivo. El panel izquierdo proporciona sintaxis predefinida que puede impulsar para versión la secuencia de comandos. [Aprenda a trabajar con variables evento y con el editor expresión](../event-variables.md).

![Captura de pantalla que muestra el editor de secuencia de comandos para el procesamiento entrada.](../assets/extract-file-script.png)

## Opciones adicionales {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Transición saliente"
>abstract="Alternar la opción **Generar una transición saliente** para añadir una transición saliente después de la actividad actual."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Errores de proceso"
>abstract="Alternar la opción **Errores de proceso** para añadir una transición saliente que contenga errores."

Una vez configurada la extracción del archivo de salida, hay disponibles opciones adicionales relacionadas con las transiciones y la gestión de errores:

* **[!UICONTROL Generar transición]** saliente: active esta opción para añadir un transición saliente y configurar su etiqueta.
* **[!UICONTROL No generar un archivo si el transición entrante está vacío]**: active esta opción para omitir el extracción de archivo si el transición entrante no contiene datos.
* **[!UICONTROL Error]** de proceso: active esta opción para agregar un transición saliente si se encuentra algún error durante el extracción del archivo.

## Ejemplo {#example}

En el ejemplo siguiente, una **actividad de audiencia** de compilación va seguida de un **archivo** Extract actividad para extracción todos los perfiles de destino en un archivo CSV.

![Captura de pantalla que muestra un ejemplo flujo de trabajo con un actividad de audiencia de compilación seguido de un actividad de archivo Extract.](../assets/extract-file-example.png)

* El **[!UICONTROL campo Nombre Archivo]** está configurado para incluir la fecha del extracción.

  ![Captura de pantalla que muestra la configuración del nombre de archivo con la fecha incluida.](../assets/extract-file-example-name.png)

* Se agregan columnas para mostrar los nombres y apellidos de los perfiles, sus ID de cliente y las fechas de creación en la base de datos.

  ![Captura de pantalla que muestra la configuración de columnas en el archivo extraído.](../assets/extract-file-example-columns.png)