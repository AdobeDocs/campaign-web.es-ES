---
audience: end-user
title: Uso de la actividad de flujo de trabajo Deduplication
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Deduplicación
badge: label="Beta"
source-git-commit: bf98ca98510f51fb7496a380f6547b0d3e954006
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 23%

---


# Anulación de duplicación {#deduplication}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fork activity"
>abstract="The Deduplication activity allows you to..."
-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generar un complemento"
>abstract="Puede generar una transición saliente adicional con la población restante, que se excluyó como duplicado. Para ello, active la opción **Generar complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configuración de la anulación de duplicación"
>abstract="Para eliminar duplicados en los datos entrantes, defina el método de anulación de duplicación en los campos siguientes. De forma predeterminada, solo se guarda un registro. También debe seleccionar el modo de deduplicación en función de una expresión o un atributo. De forma predeterminada, el registro que se va a excluir de los duplicados se selecciona de forma aleatoria."

El **Deduplicación** la actividad es una **Segmentación** actividad. Esta actividad le permite eliminar duplicados en los resultados de las actividades entrantes. El **Deduplicación** la actividad se utiliza generalmente después de actividades de segmentación y antes de actividades que permiten el uso de datos de objetivo.

## Configuración

Siga estos pasos para configurar el **Deduplicación** actividad:

1. Añadir un **Deduplicación** a su flujo de trabajo.

   ![](../assets/workflow-deduplication.png)

1. En el **Campos para identificar duplicados** , haga clic en **Añadir atributo** para especificar los campos para los que los valores idénticos permiten identificar los duplicados: dirección de correo electrónico, nombre, apellidos, etc. El orden de los campos permite especificar los que se procesarán primero.

1. Seleccione el número de **Duplicados que mantener**. El valor predeterminado de este campo es 1. El valor 0 le permite mantener todos los duplicados.

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. Seleccione el **Método de deduplicación** para usar:

   * **Selección aleatoria**: selecciona de forma aleatoria el registro que se va a excluir de los duplicados.
   * **Uso de una expresión**: esto permite mantener los registros en los que el valor de la expresión introducida es el más pequeño o el más grande. Expresión ++ ++ orden
   * **Following a list of values**: permite definir una prioridad de valor para uno o varios campos. Para definir los valores, haga clic en **Atributo** para seleccionar un campo o crear una expresión, añada los valores a la tabla adecuada. Para definir un nuevo campo, haga clic en el botón Add situado sobre la lista de valores. ++ Ordenar

1. Seleccione la opción **Generate complement** si desea utilizar la población restante. El complemento está formado por todos los duplicados. A continuación, se agregará una transición adicional a la actividad.

## Ejemplo

