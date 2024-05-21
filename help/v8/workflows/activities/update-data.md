---
audience: end-user
title: Uso de la actividad de flujo de trabajo Actualizar datos
description: Aprenda a utilizar la actividad del flujo de trabajo Actualización de datos
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 32%

---

# Actualización de datos {#update-data}

El **Actualización de datos** la actividad es una **Administración de datos** actividad. Permite realizar una actualización masiva de los campos de la base de datos. Varias opciones permiten personalizar la actualización de datos.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## Configure la actividad Update data{#update-data-configuration}

Para configurar la variable **Actualización de datos** actividad, comience añadiendo la actividad al flujo de trabajo y defina una etiqueta.

![](../assets/workflow-update-data.png)

### Tipo de operación

El campo **Operation type** permite elegir el proceso que se lleva a cabo en la información de la base de datos:

* **Insertar o actualizar**: insertar datos o actualizarlos si los registros ya existen en la base de datos.
* **Insertar**: insertar solo datos. Los registros que ya existen no se actualizan. Si se definen los criterios de reconciliación, solo se añaden los registros que no se han cuadrado.
* **Actualizar**: actualizar los datos de los registros que ya existen solo en la base de datos.
* **Delete**: eliminar datos.

El campo **Batch size** permite seleccionar el número de elementos de transición entrantes que se deben actualizar. Por ejemplo, si establece 500, se actualizarán los 500 primeros registros analizados.

### Identificación de registro

Esta sección le permite especificar cómo identificar los registros de la base de datos:

* Si las entradas de datos están relacionadas con una dimensión de segmentación existente, seleccione la **Uso de la dimensión objetivo** y selecciónela en la pestaña **Dimensión de segmentación a actualizar** field.
* También puede seleccionar la variable **Uso de vínculos personalizados** y especifique uno o más vínculos que permitan la identificación de los datos en la base de datos
* Si el tipo de operación seleccionado requiere una actualización, debe utilizar el **Uso de reglas de reconciliación** opción.

### Campos que actualizar

En el **Campos para actualizar** , añada los campos en los que se aplicará la actualización y, si es necesario, añada condiciones para que se realice la actualización. Para ello, utilice el **Se tendrá en cuenta si** field. Las condiciones se aplican una tras otra en orden de lista. Utilice las flechas de la derecha para cambiar el orden de las actualizaciones. Puede utilizar el mismo campo de destino varias veces.

Los campos se pueden vincular automáticamente mediante la variable **Asignación automática** botón. La vinculación automática detecta los campos con el mismo nombre.

Durante un **Insertar o actualizar** tipo de operación, puede seleccionar individualmente la operación que desea aplicar a cada campo. Para ello, seleccione el valor que desee en la **Tipo de operación** field.

### Opciones avanzadas

El **Opciones avanzadas** permite especificar opciones adicionales para trabajar con la actualización de datos y para administrar duplicados.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

Las dos últimas opciones permiten realizar acciones específicas:

* **Generación de una transición saliente**: crea una transición saliente que se activa al final de la ejecución. La actualización normalmente indica el final de un flujo de trabajo de objetivos, por lo que la opción no se activa de forma predeterminada.

* **Generar una transición saliente para los rechazos**: crea una transición saliente que contiene registros que no se han procesado correctamente después de la actualización (por ejemplo, si hay un duplicado). Por lo general, la actualización marca el final de un flujo de trabajo de segmentación y, por lo tanto, la opción no está activada de forma predeterminada.
