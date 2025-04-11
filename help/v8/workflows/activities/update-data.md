---
audience: end-user
title: Uso de la actividad de flujo de trabajo Actualizar datos
description: Aprenda a utilizar la actividad del flujo de trabajo Actualización de datos
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 22%

---

# Actualización de datos {#update-data}

La actividad **Actualizar datos** es una actividad **Administración de datos**. Permite realizar una actualización masiva de los campos de la base de datos. Varias opciones permiten personalizar la actualización de datos.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update it if it has already been added. You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely.

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or directly use reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section lets you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example, if there is a duplicate). The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.
-->

## Configure la actividad Update data {#update-data-configuration}

Para configurar la actividad **Actualizar datos**, agregue la actividad al flujo de trabajo y defina una etiqueta.

![Actividad de actualización de datos del flujo de trabajo](../assets/workflow-update-data.png)

### Tipo de operación

El campo **Operation type** permite elegir el proceso que se lleva a cabo en la información de la base de datos:

* **Insertar o actualizar**: inserte datos o actualícelos si los registros ya existen en la base de datos.
* **Insertar**: Insertar solo datos. Los registros que ya existen no se actualizan. Si se definen los criterios de reconciliación, solo se añaden los registros que no se han cuadrado.
* **Actualizar**: actualice los datos de los registros que ya existen solamente en la base de datos.
* **Eliminar**: Elimine datos.

El campo **Batch size** permite seleccionar el número de elementos de transición entrantes que se deben actualizar. Por ejemplo, si especifica 500, se actualizarán los 500 primeros registros procesados.

### Identificación de registro

Esta sección le permite especificar cómo identificar los registros de la base de datos:

* Si las entradas de datos están relacionadas con una dimensión de segmentación existente, seleccione la opción **Usando la dimensión de segmentación** y elíjala en el campo **Dimensión de segmentación que se actualizará**.
* También puede seleccionar **Utilizando vínculos personalizados** y especificar uno o más vínculos que permitan la identificación de los datos en la base de datos.
* Si el tipo de operación seleccionado requiere una actualización, use la opción **Usar reglas de reconciliación**.

### Campos que actualizar

En la sección **Campos para actualizar**, agregue los campos en los que se aplicará la actualización. Si es necesario, agregue condiciones para que se realice esta actualización. Utilice el campo **Tenido en cuenta si** para definir condiciones. Las condiciones se aplican secuencialmente en orden de lista. Utilice las flechas de la derecha para cambiar el orden de las actualizaciones. Puede utilizar el mismo campo de destino varias veces.

Vincular campos automáticamente con el botón **Asignación automática**. La vinculación automática detecta los campos con el mismo nombre.

Durante un tipo de operación **Insert or update**, seleccione individualmente la operación que desea aplicar a cada campo. Utilice el campo **Tipo de operación** para especificar el valor deseado.

### Opciones avanzadas

La sección **Opciones avanzadas** le permite especificar opciones adicionales para administrar la actualización de datos y los duplicados.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

Las dos últimas opciones permiten realizar acciones específicas:

* **Generar una transición saliente**: crea una transición saliente que se activará al final de la ejecución. La actualización normalmente indica el final de un flujo de trabajo de objetivos, por lo que la opción no se activa de forma predeterminada.

* **Generar una transición saliente para los rechazos**: crea una transición saliente que contiene registros que no se han procesado correctamente después de la actualización (por ejemplo, si hay un duplicado). Por lo general, la actualización marca el final de un flujo de trabajo de objetivos, y la opción no está activada de forma predeterminada.