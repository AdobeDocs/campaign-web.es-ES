---
audience: end-user
title: Uso de la actividad Transferir archivo
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Transferir archivo
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 15%

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
>abstract="Transferir archivo al servidor remoto"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Transferir origen de archivo"
>abstract="Transferir origen de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Eliminar los archivos de origen tras la transferencia"
>abstract="Eliminar los archivos de origen tras la transferencia"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Mostrar los registros de sesión"
>abstract="Mostrar los registros de sesión"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Listar todos los archivos"
>abstract="Listar todos los archivos"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="Historización de archivos"
>abstract="Historización de archivos"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Procesar archivos que faltan"
>abstract="Procesar archivos que faltan"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Errores de proceso"
>abstract="Errores de proceso"

El **Transferir archivo** la actividad es una **Administración de datos** actividad. Permite recibir o enviar archivos, probar la presencia de archivos o mostrar archivos en un servidor. El protocolo que se utiliza puede ser un protocolo de servidor a servidor o el protocolo HTTP.

>[!NOTE]
>
>Con la interfaz de usuario web de Campaign, hemos consolidado dos actividades en una al combinar ambas **Transferencia de archivos** y **Descarga web** funciones. Esta consolidación no afecta a la funcionalidad de la actividad de ninguna manera.

Siga los pasos detallados a continuación para configurar el **Transferir archivo** actividad.

## Seleccione el protocolo y la operación de transferencia {#protocol}

1. Añadir un **Transferir archivo** actividad en el flujo de trabajo y, a continuación, especifique el tipo de transferencia que se va a realizar según el protocolo que desee utilizar:

   * Para el protocolo HTTP, seleccione **[!UICONTROL Descarga web]**. Esto le permite hacer que un GET o POST descargue un archivo en una dirección URL explícita, una cuenta externa o una instancia de Adobe Campaign.
   * Para otros protocolos de servidor a servidor y acciones relacionadas, seleccione **[!UICONTROL Transferencia de archivos]**.

1. Seleccione la acción que se realizará con la actividad. Las acciones disponibles dependen del tipo de transferencia que haya seleccionado. Expanda las secciones siguientes para obtener más información.

   +++Acciones disponibles con **Transferencia de archivos** actividades de tipo

   * **[!UICONTROL Descarga de archivos]**: descargue un archivo del servidor.
   * **[!UICONTROL Carga de archivo]**: Cargue un archivo en el servidor.
   * **[!UICONTROL Comprobar si el archivo existe]**: compruebe si un archivo determinado está presente en el servidor. Genera dos transiciones salientes después de la actividad: &quot;El archivo existe&quot; y &quot;El archivo no existe&quot;.
   * **[!UICONTROL Lista de archivos]**: enumera todos los archivos disponibles en el servidor.

+++

   +++Acciones disponibles con **Descarga web** actividades de tipo

   * **[!UICONTROL Transferencia simple (GET)]**: Recupere un archivo.
   * **[!UICONTROL Transferencia mediante un formulario (POST)]**: Cargue un archivo y parámetros adicionales.

+++

   ![](../assets/workflow-transfer-file-action.png)

1. De forma predeterminada, para las acciones de carga de archivos, la actividad utiliza el archivo especificado en la actividad anterior. Para utilizar un archivo diferente, cambie el **[!UICONTROL Usar archivo de actividad anterior]** y haga clic en la opción **[!UICONTROL Añadir archivo]** botón.

   En el **[!UICONTROL Origen]** , introduzca el nombre de archivo deseado o utilice el editor de expresiones para calcular el nombre de archivo mediante variables de evento. [Aprenda a trabajar con variables de eventos y el editor de expresiones](../event-variables.md). Repita la operación para agregar tantos archivos como sea necesario.

## Definir el destino de la transferencia {#destination}

1. En el **[!UICONTROL Servidor remoto]** , especifique el servidor al que conectarse mediante uno de estos métodos:

   * **[!UICONTROL Usar parámetros de conexión definidos en una cuenta externa]**: Conéctese a un servidor mediante los parámetros de conexión de una cuenta externa. En el **[!UICONTROL Carpeta del servidor]** , especifique la ruta al archivo (o a la carpeta para las acciones de lista de archivos).
   * **[!UICONTROL Configuración rápida]**: introduzca la dirección URL del archivo (o carpeta para acciones de lista de archivos).
   * **[!UICONTROL Instancia de Adobe Campaign]** (Actividades de tipo Web download): Descargue un archivo desde un servidor de instancias de Adobe Campaign.

   ![](../assets/workflow-transfer-file-server.png)

1. Para las acciones del POST de descarga web, puede pasar parámetros adicionales con la operación. Para ello, haga clic en el **[!UICONTROL Añadir parámetro]** a continuación, especifique el nombre y el valor de los parámetros. Puede añadir tantos parámetros como sea necesario.

1. De forma predeterminada, para la carga de archivos, los archivos cargados en un servidor se guardan automáticamente. Si no desea conservar este historial, alterne el **[!UICONTROL Mantener el historial de archivos enviados]** opción desactivada.

## Configuración de historización {#historization}

Cada vez que **[!UICONTROL Transferir archivo]** Cuando se ejecuta la actividad, almacena los archivos cargados o descargados en una carpeta dedicada. Se crea una carpeta para cada actividad Transferir archivo de un flujo de trabajo. De forma predeterminada, los archivos se guardan en el directorio de almacenamiento predeterminado de la carpeta de instalación de Adobe Campaign (`/vars`) antes de procesarse. Para utilizar una carpeta específica, cambie el **[!UICONTROL Usar un directorio de almacenamiento predeterminado]** e introduzca la ruta del directorio.

![](../assets/workflow-transfer-file-historization.png)

Es importante poder limitar el tamaño de esta carpeta para conservar el espacio físico en el servidor. Para ello, puede definir un número máximo de archivos o un tamaño total para la carpeta de la actividad. De forma predeterminada, se autorizan 100 archivos y 50 MB.

Cada vez que se ejecuta la actividad, la carpeta se marca de la siguiente manera:

* Solo se tienen en cuenta los archivos creados más de 24 horas antes de la ejecución de la actividad.
* Si el número de archivos que se tiene en cuenta es mayor que el valor del **[!UICONTROL Número de archivos]** , se eliminarán los archivos más antiguos hasta que se alcance el número máximo de archivos permitidos.
* Si el tamaño total de los archivos que se tienen en cuenta es mayor que el valor del **[!UICONTROL Tamaño máximo (en MB)]** , se eliminarán los archivos más antiguos hasta que se alcance el tamaño máximo permitido (en MB).

>[!CAUTION]
>
>Si la actividad no se vuelve a ejecutar, no se comprueba ni depura la carpeta. Tenga esto en cuenta a la hora de transferir archivos de gran tamaño.

## Opciones avanzadas y de administración de errores {#advanced}

1. En el **[!UICONTROL Opciones avanzadas]**, hay opciones adicionales disponibles en función del tipo de actividad que esté configurando. Expanda las secciones siguientes para obtener más información.

   +++Opciones adicionales para **[!UICONTROL Transferencia de archivos]** actividades de tipo

   * **[!UICONTROL Eliminar los archivos de origen después de la transferencia]**: borre los archivos de origen después de una transferencia correcta.
   * **[!UICONTROL Mostrar los registros de sesión]**: Cuando se activa esta opción, la información relacionada con la operación de transferencia se muestra en los registros de flujo de trabajo una vez ejecutado el flujo de trabajo.
   * **[!UICONTROL Mostrar todos los archivos]** (Acciones de lista de archivos): esta opción indexa todos los archivos presentes en el servidor en el `vars.filenames` , en la que los nombres de archivo están separados por el evento `n` caracteres. [Aprenda a trabajar con variables de eventos](../event-variables.md)

+++

   +++Opciones adicionales para **[!UICONTROL Descarga web]** actividades de tipo

   * **[!UICONTROL Seguir redirecciones]**: la redirección de archivos permite utilizar invalidaciones para dirigir la entrada o salida de datos a un dispositivo de un tipo diferente.
   * **[!UICONTROL Añadir los encabezados HTTP al archivo]**: En algunos casos, es posible que desee agregar encabezados HTTP adicionales a un archivo. Normalmente, estos encabezados se utilizan para proporcionar información adicional con fines de resolución de problemas, por ejemplo [Intercambio de recursos de origen cruzado (CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS)o para establecer directivas de almacenamiento en caché específicas.
   * **[!UICONTROL Omitir el código de retorno HTTP]**: los códigos de retorno HTTP, también conocidos como códigos de estado HTTP, indican el resultado de una solicitud HTTP.

1. El **[!UICONTROL Errores de proceso]** La opción le permite activar una transición saliente de &quot;error&quot; después de la actividad si se produce algún error durante la transferencia.

   Además, para **Transferencia de archivos** actividades de tipo, la variable **[!UICONTROL Procesar el archivo que falta]** La opción le permite activar una transición saliente &quot;Sin archivo&quot; después de la actividad si el archivo no está disponible en la ruta especificada.
