---
audience: end-user
title: Público destinatario desde un archivo
description: Aprenda a utilizar destinatarios de un archivo externo para crear su audiencia de correo electrónico
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: f60f0e34dc5d85808c208223d83d234e22a41c34
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Carga de una audiencia de correo electrónico desde un archivo {#audience-from-file}

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

Puede cargar contactos desde un archivo externo. Los perfiles no se añaden a la base de datos, pero todos los campos del archivo de entrada están disponibles para [personalización](../personalization/gs-personalization.md). Los formatos de archivo admitidos son: texto (TXT) y valor separado por comas (CSV).

>[!CAUTION]
>
>* Esta funcionalidad solo está disponible para **envíos de correo electrónico independientes**. No se puede utilizar en flujos de trabajo ni con envíos SMS o Push.
>
>* No puede utilizar [grupos de control](control-group.md) al cargar la población de público destinatario desde un archivo externo.



Para segmentar perfiles desde un archivo local directamente desde la interfaz de correo electrónico, siga estos pasos:

1. Abra una entrega de correo electrónico existente o [creación de un nuevo envío de correo electrónico](../email/create-email.md).
1. En la ventana de creación de envíos de correo electrónico, en la sección **Audiencia**, haga clic en el botón **Seleccionar audiencia** y seleccione la opción **Seleccionar del archivo**.

   ![](assets/select-from-file.png)

1. Seleccione el archivo local que desea subir. El formato debe alinearse con la variable [archivo de muestra](#sample-file).
1. Obtenga una vista previa y compruebe cómo se asignan los datos en la sección central de la pantalla.
1. Elija la columna que contiene la dirección de correo electrónico del menú desplegable **Campo de dirección**. También puede seleccionar la columna de lista de bloqueados si dispone de dicha información en el archivo de entrada.
1. Ajuste la configuración de columna y cómo dar formato a los datos desde las opciones disponibles.
1. Haga clic en **Confirmar** una vez que la configuración sea correcta.

Al crear y personalizar el contenido del mensaje, puede seleccionar campos del archivo de entrada en la [Editor de personalización](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## Archivo de muestra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Archivo de muestra"
>abstract="Formatos de archivo compatibles: txt, csv. Usar la primera línea como encabezado de columna."

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
