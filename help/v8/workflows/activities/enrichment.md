---
audience: end-user
title: Uso de la actividad de flujo de trabajo Enrichment
description: Aprenda a utilizar la actividad del flujo de trabajo Enriquecimiento
badge: label="Alpha" type="Positive"
source-git-commit: 773d2476232f4e0609346f4f4518c3250c26985a
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 28%

---


# Enriquecimiento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enriquecimiento Actividad"
>abstract="La actividad de enriquecimiento permite mejorar los datos de destino con información adicional de la base de datos. Normalmente se utiliza en un flujo de trabajo después de dirigir las actividades.<br/>Una vez añadidos los datos de enriquecimiento al flujo de trabajo, estos se pueden utilizar en las actividades añadidas después de la actividad de enriquecimiento para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades. También para crear campañas y mensajes de marketing personalizados que tengan más probabilidades de resonar con la audiencia de destinatarios."

El **Enriquecimiento** la actividad es una **Segmentación** actividad. Permite mejorar los datos de destino con información adicional de la base de datos. Normalmente se utiliza en un flujo de trabajo después de actividades de segmentación.

Los datos de enriquecimiento pueden provenir de los siguientes lugares:

* **La misma tabla de trabajo** como el objetivo del flujo de trabajo:

   *Destine la actividad a un grupo de clientes y añada el campo “Fecha de nacimiento” a la tabla de trabajo actual*

* **De otra tabla de trabajo**:

   *Diríjase a un grupo de clientes y añada los campos “Importe” y “Tipo de producto” procedentes de la tabla “Compra”*.

Una vez añadidos los datos de enriquecimiento al flujo de trabajo, se pueden utilizar en las actividades añadidas después de la **Enriquecimiento** actividad para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades, o para crear mensajes de marketing personalizados y campañas que tengan más probabilidades de interesar a la audiencia de destino.

Por ejemplo, puede añadir a la tabla de trabajo del flujo de trabajo información relacionada con las compras de los clientes y utilizar estos datos para personalizar los correos electrónicos con su última compra o la cantidad gastada en estas compras.

## Configuración general

Siga estos pasos para configurar el **Enriquecimiento** actividad:

1. Añada actividades como **Crear audiencia** y **Combinar** actividades.
1. Añadir un **Enriquecimiento** actividad.
1. Clic **Añadir datos de enriquecimiento**.

![](../assets/workflow-enrichment1.png)

Puede seleccionar dos tipos de datos: un solo atributo de la dimensión de destino o un vínculo de recopilación.

## Atributo único

Aquí, simplemente estamos agregando un único atributo de enriquecimiento, por ejemplo, la fecha de nacimiento. Siga estos pasos:

1. Haga clic dentro de **Atributo** field.
1. Seleccione un campo simple de la dimensión de segmentación, la fecha de nacimiento en nuestro ejemplo.
1. Haga clic en **Confirmar**.

![](../assets/workflow-enrichment2.png)

## Vínculo de colección

En este caso de uso más complejo, seleccionaremos un vínculo de colección que es un vínculo con una cardinalidad 1-N entre tablas. Vamos a recuperar las tres últimas compras que son menos de 100 $. Para ello, debe definir lo siguiente:

* un atributo: **Cantidad total** campo
* número de líneas que se van a recuperar: 3
* un filtro: filtre los elementos que sean buenos a más de 100 $
* un orden: orden descendente en el **Fecha de pedido** field.

Siga estos pasos:

### Añadir el atributo

Aquí es donde se selecciona el vínculo de recopilación que se utilizará como datos de enriquecimiento.

1. Haga clic dentro de **Atributo** field.
1. Clic **Mostrar atributos avanzados**.
1. Seleccione el **Cantidad total** del campo **Compras** tabla.

![](../assets/workflow-enrichment3.png)

### Definir la configuración de colección

A continuación, defina cómo se recopilan los datos y el número de registros que desea recuperar.

1. Seleccionar **Recopilación de datos** en el **Seleccione cómo se recopilan los datos** menú desplegable.
1. Escriba &quot;3&quot; en la **Líneas a recuperar (Columnas a crear)** field.

![](../assets/workflow-enrichment4.png)

Si desea, por ejemplo, obtener la cantidad promedio de compras para un cliente, seleccione **Datos agregados** en su lugar, seleccione **Media** en el **Función de agregado** menú desplegable.

![](../assets/workflow-enrichment5.png)

### Definición de los filtros

Aquí, definimos el valor máximo del atributo. Filtramos los elementos que sean buenos a 100 $.

1. Clic **Editar filtros**.
1. Añada los dos filtros siguientes: **Cantidad total** existe Y **Cantidad total** es menor que 100. El primero filtra los valores NULL tal como aparecerían como el valor más bueno.
1. Haga clic en **Confirmar**.

![](../assets/workflow-enrichment6.png)

### Definición de la ordenación

Ahora necesitamos aplicar la ordenación para recuperar los tres **última versión** compras.

1. Activar el **Habilitar ordenación** opción.
1. Haga clic dentro de **Atributo** field.
1. Seleccione el **Fecha de pedido** field.
1. Haga clic en **Confirmar**.
1. Seleccionar **Descendente** desde el **Ordenar** menú desplegable.

![](../assets/workflow-enrichment7.png)

<!--
cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->