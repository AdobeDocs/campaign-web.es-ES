---
audience: end-user
title: Importación de destinatarios desde un archivo
description: Obtenga información sobre cómo importar destinatarios desde un archivo externo
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ef8418294540ee0462725cdaf6824ba7ee4d9b59
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 97%

---

# Importación de destinatarios desde un archivo {#audience-from-file}

Puede agregar o actualizar contactos desde la interfaz de envío cargando un archivo de texto (.txt) o un archivo de valores separado por comas (.csv). A continuación, se añadirán a la base de datos.

>[!NOTE]
>
>También puede generar un flujo de trabajo de importación para añadir o actualizar varios perfiles.


Para añadir perfiles desde un archivo local directamente desde la interfaz, siga estos pasos:

1. En la ventana de creación de envíos, haga clic en el botón **Seleccionar la audiencia** y seleccione la opción **Seleccionar desde un archivo**.
1. Seleccione el archivo local que desea subir.
1. Defina la configuración de la columna y cómo dar formato a los datos. Puede omitir una columna utilizando la opción **Ignorar columna**.
1. Obtenga una vista previa de cómo se asignan los datos en la sección central de la pantalla.
1. Haga clic en **Confirmar** una vez que la configuración sea correcta.

Al crear y personalizar el contenido del mensaje, puede seleccionar campos del archivo de entrada en el editor de personalización.

## Archivo de muestra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Archivo de muestra"
>abstract="Formatos de archivo compatibles: txt, csv. Usar la primera línea como encabezado de columna."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
