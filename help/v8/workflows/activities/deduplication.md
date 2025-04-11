---
audience: end-user
title: Uso de la actividad de flujo de trabajo Deduplication
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Deduplicación
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 19%

---

# Deduplicación {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campos para identificar los duplicados"
>abstract="En la sección **Campos para identificar duplicados**, haga clic en el botón **Agregar atributo** para especificar los campos para los que valores idénticos permiten identificar duplicados, como la dirección de correo electrónico, el nombre y los apellidos. El orden de los campos especifica los que se procesarán primero."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Actividad de deduplicación"
>abstract="La actividad **Deduplication** elimina los duplicados en los resultados de las actividades entrantes. Se utiliza principalmente después de las actividades de segmentación y antes de las actividades que utilizan datos de objetivo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generación de un complemento"
>abstract="Puede generar una transición saliente adicional con la población restante excluida como duplicadas. Para ello, active la opción **Generar complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configuración de la deduplicación"
>abstract="Para eliminar duplicados en los datos entrantes, defina el método de deduplicación en los campos siguientes. De forma predeterminada, solo se guarda un registro. Seleccione el modo de deduplicación en función de una expresión o un atributo. De forma predeterminada, el registro que se va a excluir de los duplicados se selecciona de forma aleatoria."

La actividad **Deduplication** es una actividad de **segmentación**. Esta actividad elimina los duplicados en los resultados de las actividades entrantes, como los perfiles duplicados en la lista de destinatarios. La actividad **Deduplication** se utiliza generalmente después de las actividades de segmentación y antes de las actividades que utilizan datos de objetivo.

## Configuración de la actividad de anulación de duplicación {#deduplication-configuration}

Siga estos pasos para configurar la actividad **Deduplication**:

![Proceso de configuración de anulación de duplicación del flujo de trabajo](../assets/workflow-deduplication.png)

1. Agregue una actividad **Deduplication** a su flujo de trabajo.

1. En la sección **Campos para identificar duplicados**, haga clic en el botón **Agregar atributo** para especificar los campos para los que valores idénticos permiten identificar duplicados, como la dirección de correo electrónico, el nombre y los apellidos. El orden de los campos especifica los que se procesarán primero. [Aprenda a seleccionar atributos y agregarlos a favoritos](../../get-started/attributes.md).

1. En la sección **Configuración de anulación de duplicación**, seleccione el número de **duplicados únicos que desea conservar**. El valor predeterminado de este campo es 1. El valor 0 mantiene todos los duplicados.

   Por ejemplo, si los registros A y B se consideran duplicados del registro Y, y el registro C se considera un duplicado del registro Z:

   * Si el valor del campo es 1: solo se guardan los registros Y y Z.
   * Si el valor del campo es 0: se guardan todos los registros.
   * Si el valor del campo es 2: se conservan los registros C y Z, y se conservan dos registros de A, B e Y, al azar o en función del método de deduplicación seleccionado.

1. Seleccione el **método de deduplicación** que se va a utilizar:

   * **Selección aleatoria**: Selecciona aleatoriamente el registro que se va a excluir de los duplicados.
   * **Uso de una expresión**: conserva los registros en los que el valor de la expresión introducida es el más pequeño o el más grande.
   * **Valores no vacíos**: Mantiene los registros para los que la expresión no está vacía.
   * **Siguiendo una lista de valores**: Define una prioridad de valor para uno o varios campos. Para definir los valores, haga clic en **Atributo** para seleccionar un campo o crear una expresión y, a continuación, agregue los valores a la tabla adecuada. Para definir un nuevo campo, haga clic en el botón **Add** situado sobre la lista de valores.

1. Marque la opción **Generate complement** para aprovechar la población restante. El complemento está formado por todos los duplicados. A continuación, se añade una transición adicional a la actividad.

## Ejemplo {#deduplication-example}

En el siguiente ejemplo, utilice una actividad de anulación de duplicación para excluir duplicados del destinatario antes de realizar una entrega. Los perfiles duplicados identificados se añaden a una audiencia dedicada que se puede reutilizar si es necesario. Elija la dirección de **correo electrónico** para identificar los duplicados. Mantenga 1 entrada y seleccione el método de deduplicación **Random**.

![Ejemplo de actividad de anulación de duplicación en un flujo de trabajo](../assets/workflow-deduplication-example.png)