---
audience: end-user
title: Importación de un público de correo electrónico desde un archivo
description: Obtenga información sobre cómo cargar perfiles de un archivo externo para crear su audiencia de correo electrónico
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 29%

---

# Importación de un público de correo electrónico desde un archivo {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Selección de archivos"
>abstract="Seleccione el archivo local que desea subir. Los formatos compatibles son TXT y CSV. Alinee el formato del archivo con el archivo de muestra vinculado a continuación."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definición de columnas"
>abstract="Compruebe el formato de las columnas en el archivo externo."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parámetros de formato"
>abstract="Especifique el formato del archivo externo para asegurarse de que los datos se importan correctamente."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="Vista previa del archivo"
>abstract="Compruebe la previsualización de las columnas del archivo externo. Esta pantalla solo muestra hasta 30 registros."

La interfaz de usuario web de Adobe Campaign permite segmentar perfiles almacenados en un archivo externo. Una vez cargados los perfiles, todos los campos del archivo de entrada están disponibles para su uso para personalizar el envío [Aprenda a personalizar el contenido](../personalization/personalize.md).

Los perfiles del archivo de entrada no se agregan a la base de datos. Se cargan y están disponibles únicamente para este envío de correo electrónico independiente específico.

>[!NOTE]
>
>Esta página describe cómo cargar perfiles externos desde un archivo al crear un envío de correo electrónico independiente. Para cargar datos de un archivo en el contexto de un flujo de trabajo, consulte [esta página](../workflows/activities/load-file.md).

## Lectura obligatoria {#must-read}

* Esta capacidad está disponible para **envíos de correo electrónico** solo.
* Los formatos de archivo admitidos son: texto (TXT) y valor separado por comas (CSV).
* No puede utilizar [grupos de control](control-group.md) al cargar la población de público destinatario desde un archivo externo.

## Selección y configuración del archivo de entrada {#upload}

Para segmentar perfiles a partir de un archivo en los correos electrónicos, siga estos pasos:

1. Abra una entrega de correo electrónico existente o [creación de un nuevo envío de correo electrónico](../email/create-email.md).
1. En el **Audiencia** , haga clic en **Seleccionar audiencia** y luego elija **Seleccionar del archivo**.

   ![](assets/select-from-file.png){zoomable=&quot;yes&quot;}

1. Seleccione el archivo local que desea cargar. El formato de archivo debe alinearse con la variable [archivo de muestra](#sample-file).
1. Obtenga una vista previa y compruebe cómo se asignan los datos en la sección central de la pantalla.

   ![](assets/select-from-file-map.png)

1. Especifique la columna que contiene la dirección de correo electrónico de la **Campo de dirección** lista desplegable. También puede seleccionar la columna de lista de bloqueados si dispone de dicha información en el archivo de entrada.
1. Ajuste la configuración de columna y cómo dar formato a los datos desde las opciones disponibles.
1. Haga clic en **Confirmar** una vez que la configuración sea correcta.

Al crear el contenido del mensaje, puede añadir personalización aprovechando los campos del archivo de entrada. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable=&quot;yes&quot;}

## Archivo de muestra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Importación de un público desde un archivo"
>abstract="Los formatos compatibles son TXT y CSV. Usar la primera línea como encabezado de columna. Alinee el formato del archivo con el archivo de muestra proporcionado en el vínculo siguiente."

Al cargar un archivo externo para segmentar perfiles en los envíos, asegúrese de que el archivo de entrada coincida con las recomendaciones siguientes:

* Los formatos compatibles son TXT y CSV.
* La primera línea del archivo es el encabezado de columna.
* Alinee el formato del archivo con el archivo de ejemplo siguiente:

  ```javascript
  {
  lastname,firstname,city,birthdate,email,denylist
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
  }
  ```

## Previsualización y prueba del correo electrónico {#test}

La web de Campaign le permite obtener una vista previa y enviar pruebas cuando se utiliza una audiencia cargada desde un archivo. Para ello, siga estos pasos:

1. Haga clic en **[!UICONTROL Botón Simular contenido]** en la pantalla de edición de contenido de la entrega y haga clic en **[!UICONTROL Añadir perfil(es) de prueba]** botón.

1. Se muestran los perfiles contenidos en el archivo cargado. Seleccione los perfiles que desee utilizar para obtener una vista previa del contenido y haga clic en **[!UICONTROL Seleccionar]**.

1. En el panel derecho de la pantalla aparece una vista previa del contenido de la entrega. Los elementos personalizados se sustituyen por los datos del perfil seleccionado en el panel izquierdo. [Más información sobre la previsualización del contenido de envío](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png){zoomable=&quot;yes&quot;}

1. Para enviar pruebas, haga clic en **[!UICONTROL Enviar prueba]** botón.

1. Haga clic en **[!UICONTROL Cargar perfiles de prueba]** y seleccione el archivo .txt o .csv que contiene los destinatarios de prueba.

   >[!CAUTION]
   >
   >Asegúrese de que el formato de archivo coincida con el utilizado para cargar la audiencia. Cualquier error de formato mostrará una alerta.

1. Cuando haya añadido los perfiles de prueba y esté listo para enviar las pruebas, haga clic en el **[!UICONTROL Enviar prueba]** y confirme el envío.

   ![](assets/file-upload-test.png){zoomable=&quot;yes&quot;}

1. Puede monitorizar el envío de la prueba mediante el **[!UICONTROL Ver pruebas]** botón en cualquier momento. [Más información sobre la monitorización de pruebas](../preview-test/test-deliveries.md#access-test-deliveries)
