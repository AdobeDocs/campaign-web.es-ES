---
audience: end-user
title: Utilice el actividad Transferir archivo
description: Aprenda a usar el archivo de transferencia flujo de trabajo actividad
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 27%

---

# Transferir archivo {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="Transferir archivo"
>abstract="La actividad **Transferir archivo** permite recibir o enviar archivos, probar la presencia de archivos o mostrar archivos en un servidor. El protocolo que se utiliza puede ser un protocolo de servidor a servidor o el protocolo HTTP."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="Opciones de transferencia de archivo"
>abstract="Opciones de transferencia de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="Actividad de transferencia de archivo"
>abstract="Actividad de transferencia de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="Transferir archivo al servidor remoto"
>abstract="Especifique el servidor al que desea conectarse."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Transferir origen de archivo"
>abstract="Introduzca el nombre de archivo deseado."

La **actividad Transferir archivo** es un **actividad de administración de** datos. Le permite recibir o enviar archivos, prueba para presencia de archivos o lista archivos en un servidor. El protocolo que se utiliza puede ser un protocolo de servidor a servidor o el protocolo HTTP.

>[!NOTE]
>
>Con la interfaz de usuario web de Campaign, se han consolidado dos actividades en una al combinar las capacidades **Transferencia de archivos** y **Descarga web**. Esta consolidación no afecta a la funcionalidad de la actividad de ninguna manera.

Siga los pasos detallados a continuación para configurar la actividad **Transferir archivo**.

## Seleccione el protocolo y la operación de transferencia {#protocol}

1. añadir un actividad de transferencia **de archivos** en su flujo de trabajo y, a continuación, especifique el tipo de transferencia que desea realizar en función del protocolo que desee utilizar:

   * Para el protocolo HTTP, seleccione **[!UICONTROL Descarga]** web. Esto le permite realizar una operación GET o POST para descargar un archivo en un URL explícito, un cuenta externa o un instancia Adobe Campaign.
   * Para otros protocolos de servidor a servidor y acciones relacionadas, seleccione **[!UICONTROL Archivo transferencia]**.

1. Seleccione la acción que se va a realizar con el actividad. Las acciones disponibles dependen del tipo de transferencia que haya seleccionado. Expanda las secciones siguientes para obtener más información.

   +++Acciones disponibles con las actividades de tipo **Transferencia de archivos**

   * **[!UICONTROL Archivo descargar]**: descargue un archivo del servidor.
   * **[!UICONTROL Archivo cargar]**: subir un archivo al servidor.
   * **[!UICONTROL Test to see if file exists]**: Compruebe si un determinado archivo está presente en el servidor. Genera dos transiciones de salida después del actividad: &quot;Archivo existe&quot; y &quot;Archivo no existe&quot;.
   * **[!UICONTROL Archivo listado]**: Enumere todos los archivos disponibles en el servidor.

+++

   +++Acciones disponibles con **actividades de tipo descargar** web

   * **[!UICONTROL Transferencia simple (GET)]**: recupere un archivo.
   * **[!UICONTROL Transferir mediante un formulario (POST):]** cargue un archivo y parámetros adicionales.

+++

   ![Captura de pantalla que muestra flujo de trabajo las opciones de acción de transferir archivo](../assets/workflow-transfer-file-action.png)

1. De forma predeterminada, para las acciones de cargar archivos, el actividad utiliza el archivo especificado en el actividad anterior. Para usar un archivo diferente, desactive la **[!UICONTROL opción Usar archivo del actividad]** anterior y haga clic en el **[!UICONTROL botón archivo]** añadir.

   En el **[!UICONTROL campo Origen]** , introduzca el nombre de archivo deseado o utilice la editor expresión para calcular el nombre de archivo mediante evento variables. [Aprenda a trabajar con variables evento y con el editor expresión](../event-variables.md). Repita la operación para agregar tantos archivos como sea necesario.

## Definir el destino de la transferencia {#destination}

1. En la sección **[!UICONTROL Servidor remoto]**, especifique el servidor al que desea conectarse mediante uno de estos métodos:

   * **[!UICONTROL Usar parámetros de conexión definidos en una cuenta externa]**: conéctese a un servidor mediante los parámetros de conexión de una cuenta externa. En el campo **[!UICONTROL Carpeta de servidor]**, especifique la ruta al archivo (o a la carpeta para las acciones de lista de archivos).
   * **[!UICONTROL Configuración]** rápida: Introduzca el URL del archivo (o carpeta para las acciones de listado de archivos).
   * **[!UICONTROL Adobe Campaign instancia]** (actividades de tipo descargar web): Descargue un archivo de un servidor instancia de Adobe Campaign.

   ![Captura de pantalla que muestra flujo de trabajo las opciones de configuración del servidor de transferencia de archivos](../assets/workflow-transfer-file-server.png)

1. Para las acciones de POST descargar web, puede pasar parámetros adicionales con la operación. Para ello, haga clic en el botón **[!UICONTROL Agregar parámetro]** y, a continuación, especifique el nombre y el valor de los parámetros. Puede agregar tantos parámetros como sea necesario.

1. De forma predeterminada, para la carga de archivos, los archivos cargados en un servidor se guardan automáticamente. Si no desea conservar este historial, desactive la opción **[!UICONTROL Mantener el historial de archivos enviados]**.

## Configuración de la historización {#historization}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="Historización de archivos"
>abstract="Cada vez que se ejecuta una actividad de **[!UICONTROL Transferencia de archivos]**, almacena los archivos cargados o descargados en una carpeta específica. Se crea una carpeta para cada actividad de Transferencia de archivos de un flujo de trabajo. De manera predeterminada, los archivos se guardan en el directorio de almacenamiento predeterminado de la carpeta de instalación de Adobe Campaign (`/vars`) antes de procesarse. Para usar una carpeta específica, desactive la opción **[!UICONTROL Usar un directorio de almacenamiento predeterminado]** e introduzca la ruta del directorio."

Cada vez que se ejecuta una actividad de **[!UICONTROL Transferencia de archivos]**, almacena los archivos cargados o descargados en una carpeta específica. Se crea una carpeta para cada actividad de Transferencia de archivos de un flujo de trabajo. De manera predeterminada, los archivos se guardan en el directorio de almacenamiento predeterminado de la carpeta de instalación de Adobe Campaign (`/vars`) antes de procesarse. Para usar una carpeta específica, desactive la opción **[!UICONTROL Usar un directorio de almacenamiento predeterminado]** e introduzca la ruta del directorio.

![Captura de pantalla que muestra la configuración de historial de archivos de transferencia de flujo de trabajo](../assets/workflow-transfer-file-historization.png)

Es importante limitar el tamaño de esta carpeta para conservar el espacio físico en el servidor. Para ello, defina un número máximo de archivos o un tamaño total para la carpeta de la actividad. De forma predeterminada, se autorizan 100 archivos y 50 MB.

Cada vez que se ejecuta la actividad, la carpeta se marca de la siguiente manera:

* Solo se tienen en cuenta los archivos creados más de 24 horas antes de la ejecución de la actividad.
* Si el número de archivos incluidos en cuenta supera el valor del campo Número de **[!UICONTROL archivos]** , los archivos más antiguos se eliminan hasta que se alcanza el número máximo permitido de archivos.
* Si el tamaño total de los archivos tomados en cuenta supera el valor del **[!UICONTROL parámetro Tamaño máximo (en MB),]** los archivos más antiguos se eliminan hasta que se alcanza el tamaño máximo permitido.

>[!CAUTION]
>
>Si la actividad no se ejecuta de nuevo, su carpeta no se comprueba ni se purga. Tenga cuidado al transferir archivos grandes.

## Opciones avanzadas y de administración de errores {#advanced}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Eliminar los archivos de origen tras la transferencia"
>abstract="Borre los archivos de origen después de una transferencia correcta."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Mostrar los registros de sesión"
>abstract="La información relacionada con la operación de transferencia se muestra en los registros de flujo de trabajo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Listar todos los archivos"
>abstract="Esta opción indexa todos los archivos presentes en el servidor en la variable de evento **vars.filenames**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Procesar archivos que faltan"
>abstract="Esta opción le permite activar una transición de salida **No hay archivo** después de la actividad."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Errores de proceso"
>abstract="Esta opción le permite activar una transición de salida de **Error** después de la actividad."

1. En las **[!UICONTROL opciones]** de Avanzadas hay disponibles opciones adicionales según el tipo de actividad que esté configurando. Amplíe las secciones siguientes para obtener más información.

   +++Opciones adicionales para las actividades de tipo **[!UICONTROL Transferencia de archivos]**

   * **[!UICONTROL Eliminar los archivos de origen después de la transferencia]**: borre los archivos de origen después de una transferencia correcta.
   * **[!UICONTROL Mostrar los registros de sesión]**: cuando se activa esta opción, la información relacionada con la operación de transferencia se muestra en los registros de flujo de trabajo una vez que se ha ejecutado el flujo de trabajo.
   * **[!UICONTROL Enumerar todos los archivos]** (Acciones de lista de archivos): esta opción indiza todos los archivos presentes en el servidor en la variable de evento `vars.filenames`, en la que los nombres de archivo están separados por los caracteres `n`. [Aprenda a trabajar con variables de eventos](../event-variables.md)

+++

   +++Opciones adicionales para **[!UICONTROL actividades de tipo descargar]** web

   * **[!UICONTROL Siga las redirecciones]**: Archivo redirección le permite utilizar anulaciones para dirigir la entrada o salida de datos a un dispositivos de un tipo diferente.
   * **[!UICONTROL añadir los encabezados HTTP al archivo]**: En algunos casos, es posible que desee agregar encabezados HTTP adicionales a un archivo. Lo más habitual es que estos encabezados se utilicen para proporcionar información adicional para la resolución de problemas, para [Cross-origin Resource Sharing (CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS) o para establecer directivas específicas de almacenamiento en caché.
   * **[!UICONTROL Ignore el código de retorno HTTP]**: los códigos de retorno HTTP, también conocidos como códigos de estado HTTP, indican el resultado de una solicitud HTTP.

1. La opción **[!UICONTROL Process errors]** le permite activar una transición saliente de &quot;Error&quot; después de la actividad si se produce algún error durante la transferencia.

   Además, para las actividades de tipo **Transferencia de archivos**, la opción **[!UICONTROL Procesar archivo que falta]** le permite activar una transición saliente &quot;Sin archivo&quot; después de la actividad si el archivo no está disponible en la ruta especificada.