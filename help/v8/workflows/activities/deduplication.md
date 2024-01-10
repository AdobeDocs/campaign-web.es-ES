---
audience: end-user
title: Uso de la actividad de flujo de trabajo Deduplication
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Deduplicación
badge: label="Disponibilidad limitada"
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: fb72b943b324990f6dd82a4a05bfd28e5452480a
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 60%

---

# Anulación de duplicación {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campos para identificar los duplicados"
>abstract="En la sección **Campos para identificar los duplicados**, haga clic en el botón **Añadir atributo** para especificar los campos para los que los valores idénticos permiten identificar los duplicados, tales como: dirección de correo electrónico, nombre, apellidos, etc. El orden de los campos permite especificar los que se procesarán en primer lugar."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Actividad de anulación de duplicación"
>abstract="La actividad de **anulación de duplicación** permite eliminar duplicados en los resultados de las actividades entrantes. Se utiliza principalmente después de actividades de segmentación y antes de actividades que permiten el uso de datos direccionados."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generación de un complemento"
>abstract="Puede generar una transición saliente adicional con la población restante, que se excluyó como duplicado. Para ello, active la opción **Generar complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configuración de la anulación de duplicación"
>abstract="Para eliminar duplicados en los datos entrantes, defina el método de anulación de duplicación en los campos siguientes. De forma predeterminada, solo se guarda un registro. También debe seleccionar el modo de anulación de duplicación en función de una expresión o un atributo. De forma predeterminada, el registro que se va a excluir de los duplicados se selecciona de forma aleatoria."

El **Deduplicación** la actividad es una **Segmentación** actividad. Esta actividad le permite eliminar duplicados en los resultados de las actividades entrantes, por ejemplo perfiles duplicados en la lista de destinatarios. El **Deduplicación** la actividad se utiliza generalmente después de actividades de segmentación y antes de actividades que permiten el uso de datos de objetivo.

## Configuración de la actividad de anulación de duplicación{#deduplication-configuration}

Siga estos pasos para configurar el **Deduplicación** actividad:

![](../assets/workflow-deduplication.png)

1. Añadir un **Deduplicación** a su flujo de trabajo.

1. En la sección **Campos para identificar los duplicados**, haga clic en el botón **Añadir atributo** para especificar los campos para los que los valores idénticos permiten identificar los duplicados, tales como: dirección de correo electrónico, nombre, apellidos, etc. El orden de los campos permite especificar los que se procesarán en primer lugar.

1. En el **Configuración de deduplicación** , seleccione el número de **Duplicados que mantener**. El valor predeterminado de este campo es 1. El valor 0 le permite mantener todos los duplicados.

   Por ejemplo, si los registros A y B se consideran duplicados del registro Y, y un registro C se considera un duplicado del registro Z:

   * Si el valor del campo es 1: solo se guardan los registros Y y Z.
   * Si el valor del campo es 0: se guardan todos los registros.
   * Si el valor del campo es 2: se conservan los registros C y Z y se conservan dos registros de A, B e Y, al azar o en función del método de deduplicación seleccionado posteriormente.

1. Seleccione el **Método de deduplicación** para usar:

   * **Selección aleatoria**: selecciona de forma aleatoria el registro que se va a excluir de los duplicados.
   * **Uso de una expresión**: esto permite mantener los registros en los que el valor de la expresión introducida es el más pequeño o el más grande.
   * **Following a list of values**: permite definir una prioridad de valor para uno o varios campos. Para definir los valores, haga clic en **Atributo** para seleccionar un campo o crear una expresión, añada los valores a la tabla adecuada. Para definir un nuevo campo, haga clic en el botón Add situado encima de la lista de valores.

1. Seleccione la opción **Generate complement** si desea utilizar la población restante. El complemento está formado por todos los duplicados. A continuación, se agregará una transición adicional a la actividad.

## Ejemplo{#deduplication-example}

En el siguiente ejemplo, utilice una actividad de anulación de duplicación para excluir duplicados del destinatario antes de realizar una entrega. Los destinatarios duplicados identificados se añaden a una audiencia dedicada que se puede reutilizar si es necesario. Elija la **Correo electrónico** para identificar los duplicados. Mantenga 1 entrada y seleccione la **Aleatorio** método de deduplicación.

![](../assets/workflow-deduplication-example.png)
