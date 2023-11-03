---
audience: end-user
title: Público destinatario desde un archivo
description: Aprenda a utilizar destinatarios de un archivo externo para crear su audiencia de correo electrónico
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: 5dada8e96ff5b1db7ecc18b5a442fae56a4a31f2
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 40%

---

# Importación de un público destinatario de correo electrónico desde un archivo {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Selección de archivos"
>abstract="Seleccione el archivo local que desea subir. Los formatos compatibles son TXT y CSV. Alinee el formato del archivo con el archivo de muestra vinculado a continuación."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definición de columnas"
>abstract="Compruebe el formato de las columnas que desea insertar desde el archivo local."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parámetros de formato"
>abstract="Compruebe los parámetros de formato del archivo."


>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="Vista previa del archivo"
>abstract="Compruebe la vista previa de su archivo. Esta pantalla solo muestra hasta 30 registros."



No puede cargar perfiles directamente en Campaign desde la interfaz, pero puede segmentar perfiles almacenados en un archivo externo. Los perfiles no se añaden a la base de datos, pero todos los campos del archivo de entrada están disponibles para [personalización](../personalization/gs-personalization.md). Los formatos de archivo admitidos son: texto (TXT) y valor separado por comas (CSV).

>[!CAUTION]
>
>* Esta funcionalidad solo está disponible para **envíos de correo electrónico independientes**. No se puede utilizar en flujos de trabajo ni con envíos SMS o Push.
>
>* No puede utilizar [grupos de control](control-group.md) al cargar la población de público destinatario desde un archivo externo.
>
>* Los perfiles no se añaden a la base de datos y solo se cargan y están disponibles para este envío de correo electrónico independiente específico.

## Seleccionar y configurar el archivo {#upload}

Para segmentar perfiles desde un archivo local directamente desde la interfaz de correo electrónico, siga estos pasos:

1. Abra una entrega de correo electrónico existente o [creación de un nuevo envío de correo electrónico](../email/create-email.md).
1. En la ventana de creación de envíos de correo electrónico, en la sección **Audiencia**, haga clic en el botón **Seleccionar audiencia** y seleccione la opción **Seleccionar del archivo**.

   ![](assets/select-from-file.png)

1. Seleccione el archivo local que desea utilizar. El formato debe alinearse con la variable [archivo de muestra](#sample-file).
1. Obtenga una vista previa y compruebe cómo se asignan los datos en la sección central de la pantalla.
1. Elija la columna que contiene la dirección de correo electrónico del menú desplegable **Campo de dirección**. También puede seleccionar la columna de lista de bloqueados si dispone de dicha información en el archivo de entrada.
1. Ajuste la configuración de columna y cómo dar formato a los datos desde las opciones disponibles.
1. Haga clic en **Confirmar** una vez que la configuración sea correcta.

Al crear y personalizar el contenido del mensaje, puede seleccionar campos del archivo de entrada en la [Editor de personalización](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)

## Archivo de muestra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Importación de un público desde un archivo"
>abstract="Los formatos compatibles son TXT y CSV. Usar la primera línea como encabezado de columna. Alinee el formato del archivo con el archivo de muestra proporcionado en el vínculo siguiente."

Los formatos compatibles son TXT y CSV. La primera línea es el encabezado de columna.

Alinee el formato del archivo con el archivo de ejemplo siguiente:

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

La web de Campaign le permite realizar previsualizaciones y enviar correos electrónicos de prueba al utilizar una audiencia cargada desde un archivo. Para ello, siga estos pasos:

1. Haga clic en **[!UICONTROL Botón Simular contenido]** en la pantalla de edición de contenido de la entrega y haga clic en **[!UICONTROL Añadir perfil(es) de prueba]** botón.

1. Se muestran los perfiles contenidos en el archivo cargado. Seleccione los perfiles que desee utilizar para obtener una vista previa del contenido y haga clic en **[!UICONTROL Seleccionar]**.

1. En el panel derecho de la pantalla aparece una vista previa del contenido de la entrega. Los elementos personalizados se sustituyen por los datos del perfil seleccionado en el panel izquierdo. [Más información sobre la previsualización del contenido de envío](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png)

1. Para enviar correos electrónicos de prueba, haga clic en **[!UICONTROL Prueba]** botón.

1. Haga clic en **[!UICONTROL Cargar perfiles de prueba]** y seleccione el archivo .txt o .csv que contiene los destinatarios de prueba.

   >[!CAUTION]
   >
   >Asegúrese de que el formato de archivo coincida con el utilizado para cargar la audiencia. Cualquier error de formato mostrará una alerta.

1. Cuando haya añadido los destinatarios de prueba y esté listo para enviar las pruebas, haga clic en el **[!UICONTROL Enviar correo electrónico de prueba]** y confirme el envío.

   ![](assets/file-upload-test.png)

1. Puede monitorizar el envío del correo electrónico de prueba en cualquier momento mediante el botón Ver registro de correo electrónico de prueba. [Más información sobre la monitorización de correos electrónicos de prueba](../preview-test/test-deliveries.md#access-sent-test-deliveries-access-proofs)
