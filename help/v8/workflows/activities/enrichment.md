---
audience: end-user
title: Uso de la actividad de flujo de trabajo Enriquecimiento
description: Aprenda a utilizar la actividad de flujo de trabajo Enriquecimiento
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
source-git-commit: 490c2723f8e06f7360b21c8101c65961b0cfdfc3
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 44%

---

# Enriquecimiento  {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="Actividad de enriquecimiento"
>abstract="La actividad de **enriquecimiento** permite mejorar los datos de destino con información adicional de la base de datos. Normalmente se utiliza en un flujo de trabajo después de actividades de segmentación."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Actividad de enriquecimiento"
>abstract="Una vez añadidos los datos de enriquecimiento al flujo de trabajo, estos se pueden utilizar en las actividades añadidas después de la actividad Enriquecimiento para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades. También para crear campañas y mensajes de marketing personalizados que tengan más probabilidades de resonar con el público destinatario."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_simplejoin"
>title="Cree un vínculo entre los datos de la tabla de trabajo y la base de datos de Adobe Campaign. Por ejemplo, si se cargan datos de un archivo que contiene el número de cuenta, el país y el correo electrónico de los destinatarios, se debe crear un vínculo hacia la lista del país para actualizar esta información en sus perfiles."
>abstract="Definición de vínculo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_reconciliation"
>title="Reconciliación de enriquecimiento"
>abstract="reconciliación de enriquecimiento"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Datos de enriquecimiento"
>abstract="Seleccione los datos que desee utilizar para enriquecer el flujo de trabajo. Se pueden seleccionar dos tipos de datos de enriquecimiento: un único atributo de enriquecimiento de la dimensión de público destinatario o un vínculo de recopilación, que es un vínculo con una cardinalidad 1-N entre las tablas."

La actividad **Enriquecimiento** es una actividad de **Segmentación**. La actividad de enriquecimiento permite mejorar los datos segmentados con información adicional de la base de datos. Normalmente se utiliza en un flujo de trabajo después de actividades de segmentación.

Los datos de enriquecimiento pueden provenir de los siguientes lugares:

* **La misma tabla de trabajo** que la que tiene como destinatario en el flujo de trabajo:

  *Oriente un grupo de clientes y agregue el campo &quot;Fecha de nacimiento&quot; a la tabla de trabajo actual*.

* **De otra tabla de trabajo**:

  *Seleccione como público destinatario a un grupo de clientes y añada los campos “Cantidad” y “Tipo de producto” procedentes de la tabla “Comprar”*.

Una vez añadidos los datos de enriquecimiento al flujo de trabajo, se pueden utilizar en las actividades añadidas después de **Enriquecimiento** actividad para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades, o para crear mensajes de marketing personalizados y campañas que tengan más probabilidades de interesar a la audiencia de destino.

Por ejemplo, puede añadir a la tabla de trabajo del flujo de trabajo información relacionada con las compras de los clientes y utilizar estos datos para personalizar los correos electrónicos con su última compra o la cantidad gastada en estas compras.

## Añadir una actividad de enriquecimiento {#enrichment-configuration}

Siga estos pasos para configurar la actividad **Enriquecimiento**:

1. Añada actividades como **Generar público destinatario** y **Combinar**.
1. Añada una actividad **Enriquecimiento**
1. Si se han configurado varias transiciones en el flujo de trabajo, puede utilizar el **[!UICONTROL Conjunto principal]** para definir qué transición debe utilizarse como conjunto principal para enriquecerse con datos.

## Añadir datos de enriquecimiento {#enrichment-add}

1. Clic **Añadir datos de enriquecimiento** y seleccione el atributo que se utilizará para enriquecer los datos.

   Puede seleccionar dos tipos de datos de enriquecimiento: un único atributo de enriquecimiento de la dimensión de destino o un vínculo de recopilación. Cada uno de estos tipos se detalla en los ejemplos siguientes:
   * [Atributo de enriquecimiento único](#single-attribute)
   * [Vínculo de colección](#collection-link)

   >[!NOTE]
   >
   >El **Botón Editar expresión** en la pantalla de selección de atributos permite crear expresiones avanzadas para seleccionar el atributo. [Aprenda a trabajar con el editor de expresiones](../../query/expression-editor.md)

   ![](../assets/workflow-enrichment1.png)

## Creación de vínculos entre tablas {#create-links}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Vínculos entre tablas"
>abstract="Ahora puede crear un vínculo entre los datos de la tabla de trabajo y la base de datos de Adobe Campaign en la actividad de flujo de trabajo Enriquecimiento."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

El **[!UICONTROL Definición de vínculo]** permite crear un vínculo entre los datos de la tabla de trabajo y la base de datos de Adobe Campaign. Por ejemplo, si se cargan datos de un archivo que contiene el número de cuenta, el país y el correo electrónico de los destinatarios, se debe crear un vínculo hacia la lista del país para actualizar esta información en sus perfiles.

Hay varios tipos de vínculos disponibles:

* **[!UICONTROL 1 enlace simple de cardinalidad]**: Cada registro del conjunto principal se puede asociar con un registro de los datos vinculados y solo con uno.
* **[!UICONTROL 0 o 1 enlace simple de cardinalidad]**: Cada registro del conjunto principal puede asociarse con 0 o 1 registro de los datos vinculados, pero no más de uno.
* **[!UICONTROL Enlace de colección de cardinalidad N]**: Cada registro del conjunto principal se puede asociar con 0, 1 o más registros (N) de los datos vinculados.

Para crear un vínculo, siga estos pasos:

1. En el **[!UICONTROL Definición de vínculo]** , haga clic en **[!UICONTROL Añadir vínculo]** botón.

   ![](../assets/workflow-enrichment-link.png)

1. En el **Tipo de relación** , elija el tipo de vínculo que desea crear.

1. Identifique el objetivo al que desea vincular el conjunto principal:

   * Para vincular una tabla existente en la base de datos, elija **[!UICONTROL Esquema de base]** y seleccione la tabla que desee en la **[!UICONTROL Esquema de destino]** field.
   * Para vincular con datos de la transición de entrada, elija **Esquema temporal** y seleccione la transición cuyos datos desee utilizar.

1. Defina los criterios de reconciliación para hacer coincidir los datos del conjunto principal con el esquema vinculado. Hay dos tipos de uniones disponibles:

   * **Unión simple**: seleccione un atributo específico para hacer coincidir los datos de los dos esquemas. Clic **Añadir unión** y seleccione la **Origen** y **Destino** atributos que se utilizarán como criterios de reconciliación.
   * **Unión avanzada**: cree un vínculo con condiciones avanzadas. Clic **Añadir unión** y haga clic en **Crear condición** para abrir el modelador de consultas.

Un ejemplo de flujo de trabajo con vínculos está disponible en la [Ejemplos](#link-example) sección.

## Ejemplos {#example}

### Atributo de enriquecimiento único {#single-attribute}

A continuación, simplemente añadimos un único atributo de enriquecimiento, por ejemplo, la fecha de nacimiento. Siga estos pasos:

1. Haga clic dentro del campo **Atributo**.
1. Seleccione un campo simple de la dimensión de segmentación, en nuestro ejemplo, la fecha de nacimiento.
1. Haga clic en **Confirmar**.

![](../assets/workflow-enrichment2.png)

### Vínculo de colección {#collection-link}

En este caso de uso más complejo, seleccionaremos un vínculo de colección, que es un vínculo con una cardinalidad 1-N entre tablas. Vamos a recuperar las tres últimas compras con un importe menor a 100 €. Para ello, debe definir lo siguiente:

* un atributo de enriquecimiento: el campo **Cantidad total**
* número de líneas que se van a recuperar: 3
* un filtro: filtre los artículos que superen los 100 €
* un orden: orden descendente en el campo **Fecha del pedido**.

#### Añadir el atributo {#add-attribute}

Aquí es donde se selecciona el vínculo de colección que se utilizará como datos de enriquecimiento.

1. Haga clic dentro del campo **Atributo**.
1. Haga clic en **Mostrar atributos avanzados**.
1. Seleccione el campo **Cantidad total** de la tabla **Compras**.

![](../assets/workflow-enrichment3.png)

#### Definir la configuración de la colección{#collection-settings}

A continuación, defina cómo se recopilan los datos y el número de registros que desea recuperar.

1. Seleccionar **Recopilar datos** en el menú desplegable **Seleccione cómo se recopilan los datos**.
1. Escriba &quot;3&quot; en el campo **Líneas a recuperar (Columnas a crear)**.

![](../assets/workflow-enrichment4.png)

Si desea, por ejemplo, obtener la cantidad promedio de compras para un cliente, seleccione **Datos acumulados** en su lugar y seleccione **Promedio** en el menú desplegable **Función de acumulado**.

![](../assets/workflow-enrichment5.png)

#### Definición de los filtros{#collection-filters}

Aquí, definimos el valor máximo del atributo de enriquecimiento. Filtramos los elementos superiores a 100 $. [Aprenda a trabajar con el modelador de consultas](../../query/query-modeler-overview.md)

1. Haga clic en **Editar filtros**.
1. Añada los dos filtros siguientes: **Cantidad total** existe Y **Cantidad total** es menor que 100. El primero filtra los valores NULOS, ya que aparecerían como el valor más alto.
1. Haga clic en **Confirmar**.

![](../assets/workflow-enrichment6.png)

#### Definición de la ordenación{#collection-sorting}

Ahora necesitamos aplicar la ordenación para recuperar las tres **últimas** compras.

1. Active la opción **Habilitar ordenación**.
1. Haga clic dentro del campo **Atributo**.
1. Seleccione el campo **Fecha del pedido**.
1. Haga clic en **Confirmar**.
1. Seleccione **Descendente** desde el menú desplegable **Ordenar**.

![](../assets/workflow-enrichment7.png)


### Enriquecimiento con datos vinculados {#link-example}

El ejemplo siguiente muestra un flujo de trabajo configurado para crear un vínculo entre dos transiciones. La primera transición identifica los datos de perfil mediante una actividad de consulta, mientras que la segunda transición incluye datos de compra almacenados en un archivo cargado mediante una actividad de archivo de carga.

* El primero **Enriquecimiento** la actividad vincula nuestro conjunto principal (datos del **Consulta** actividad) con el esquema de **Cargar archivo** actividad. Esto nos permite hacer coincidir cada perfil objetivo por la consulta con los datos de compra correspondientes.
* Un segundo **Enriquecimiento** actividad se añade para enriquecer los datos de la tabla de flujo de trabajo con los datos de compra procedentes de **Cargar archivo** actividad. Esto nos permite utilizar esos datos en actividades adicionales, por ejemplo, para personalizar mensajes enviados a los clientes con información sobre su compra.

  ![](../assets/workflow-enrichment-example.png)





<!--

Add other fields
use it in delivery


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
