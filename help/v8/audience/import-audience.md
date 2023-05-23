---
audience: end-user
title: Destinatarios de destino de un archivo
description: Aprenda a utilizar destinatarios de un archivo externo para crear su audiencia de correo electrónico
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a6c85aeed30726532ab6060fec5cb4b5e398d9ec
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 34%

---

# Destinatarios de destino de un archivo {#audience-from-file}

Puede cargar contactos desde un archivo externo. Esta funcionalidad solo está disponible para envíos de correo electrónico. Los formatos admitidos son: archivo de texto (TXT) o archivo de valores separados por comas (CSV). A continuación, se añadirán a la base de datos.

>[!NOTE]
>
>Puede crear un flujo de trabajo de importación para añadir o actualizar varios perfiles.  Más información


Para segmentar perfiles desde un archivo local directamente desde la interfaz, siga estos pasos:

1. En la ventana de creación de envíos de correo electrónico, haga clic en **Seleccionar audiencia** y seleccione el botón **Seleccionar del archivo** opción.

   ![](assets/select-from-file.png)

1. Seleccione el archivo local que desea subir.
1. Obtenga una vista previa de cómo se asignan los datos en la sección central de la pantalla.
1. Elija la columna que contiene la dirección de correo electrónico de la **Campo de dirección** menú desplegable.
1. Ajuste la configuración de columna y cómo dar formato a los datos desde las opciones disponibles.
1. Haga clic en **Confirmar** una vez que la configuración sea correcta.

Al crear y personalizar el contenido del mensaje, puede seleccionar campos del archivo de entrada en el editor de personalización.

![](assets/select-external-perso.png)

## Archivo de muestra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Archivo de muestra"
>abstract="Formatos de archivo compatibles: txt, csv. Usar la primera línea como encabezado de columna."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
