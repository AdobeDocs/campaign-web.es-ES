---
audience: end-user
title: Uso de la actividad de flujo de trabajo Enriquecimiento
description: Aprenda a utilizar la actividad de flujo de trabajo Enriquecimiento
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 49%

---

# Enriquecimiento  {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="Actividad de enriquecimiento"
>abstract="La actividad de **enriquecimiento** permite mejorar los datos de destino con información adicional de la base de datos. Normalmente se utiliza en un flujo de trabajo después de actividades de segmentación."

La actividad **Enriquecimiento** es una actividad de **Segmentación**. La actividad de enriquecimiento permite mejorar los datos segmentados con información adicional de la base de datos. Normalmente se utiliza en un flujo de trabajo después de actividades de segmentación.

Los datos de enriquecimiento pueden provenir de los siguientes lugares:

* **La misma tabla de trabajo** que la que tiene como destinatario en el flujo de trabajo:

  *Asigne un grupo de clientes y agregue el campo &quot;Fecha de nacimiento&quot; a la tabla de trabajo actual*.

* **De otra tabla de trabajo**:

  *Seleccione como público destinatario a un grupo de clientes y añada los campos “Cantidad” y “Tipo de producto” procedentes de la tabla “Comprar”*.

Una vez que los datos de enriquecimiento se hayan agregado al flujo de trabajo, se pueden usar en las actividades agregadas después de la actividad **Enrichment** para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades, o para crear mensajes de marketing personalizados y campañas que probablemente interesen más a la audiencia de destino.

Por ejemplo, puede añadir a la tabla de trabajo del flujo de trabajo información relacionada con las compras de los clientes y utilizar estos datos para personalizar los correos electrónicos con su última compra o la cantidad gastada en estas compras.

## Añadir una actividad de enriquecimiento {#enrichment-configuration}

Siga estos pasos para configurar la actividad **Enriquecimiento**:

1. Añada actividades como **Generar público destinatario** y **Combinar**.
1. Añada una actividad **Enriquecimiento**
1. Si se han configurado varias transiciones en el flujo de trabajo, puede utilizar el campo **[!UICONTROL Conjunto principal]** para definir qué transición debe utilizarse como conjunto principal para enriquecerse con datos.

## Adición de datos de enriquecimiento {#enrichment-add}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Datos de enriquecimiento"
>abstract="Seleccione los datos que desee utilizar para enriquecer el flujo de trabajo. Se pueden seleccionar dos tipos de datos de enriquecimiento: un único atributo de enriquecimiento de la dimensión de público destinatario o un vínculo de recopilación, que es un vínculo con una cardinalidad 1-N entre las tablas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Actividad de enriquecimiento"
>abstract="Una vez añadidos los datos de enriquecimiento al flujo de trabajo, estos se pueden utilizar en las actividades añadidas después de la actividad Enriquecimiento para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades. También para crear campañas y mensajes de marketing personalizados que tengan más probabilidades de resonar con el público destinatario."

1. Haga clic en **Agregar datos de enriquecimiento** y seleccione el atributo que se utilizará para enriquecer los datos.

   Puede seleccionar dos tipos de datos de enriquecimiento: un único atributo de enriquecimiento de la dimensión de destino o un vínculo de recopilación. Cada uno de estos tipos se detalla en los ejemplos siguientes:
   * [Atributo de enriquecimiento único](#single-attribute)
   * [Vínculo de colección](#collection-link)

   >[!NOTE]
   >
   >El **botón Editar expresión** de la pantalla de selección de atributos le permite generar expresiones avanzadas para seleccionar el atributo. [Aprenda a trabajar con el editor de expresiones](../../query/expression-editor.md)

   ![](../assets/workflow-enrichment1.png)

## Creación de vínculos entre tablas {#create-links}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_simplejoin"
>title="Definición de vínculo"
>abstract="Cree un vínculo entre los datos de la tabla de trabajo y la base de datos de Adobe Campaign. Por ejemplo, si carga datos de un archivo que contiene el número de cuenta, el país y el correo electrónico de los destinatarios, debe crear un vínculo hacia la tabla del país para actualizar esta información en sus perfiles."

La sección **[!UICONTROL Link definition]** le permite crear un vínculo entre los datos de la tabla de trabajo y la base de datos de Adobe Campaign. Por ejemplo, si carga datos de un archivo que contiene el número de cuenta, el país y el correo electrónico de los destinatarios, debe crear un vínculo hacia la tabla del país para actualizar esta información en sus perfiles.

Hay varios tipos de vínculos disponibles:

* **[!UICONTROL 1 vínculo simple de cardinalidad]**: cada registro del conjunto principal se puede asociar con un registro de los datos vinculados y solo con uno.
* **[!UICONTROL 0 o 1 vínculo simple de cardinalidad]**: cada registro del conjunto principal puede asociarse con 0 o 1 registro de los datos vinculados, pero no más de uno.
* **[!UICONTROL Vínculo de recopilación de cardinalidad N]**: Cada registro del conjunto principal puede asociarse con 0, 1 o más registros (N) de los datos vinculados.

Para crear un vínculo, siga estos pasos:

1. En la sección **[!UICONTROL Definición de vínculo]**, haga clic en el botón **[!UICONTROL Agregar vínculo]**.

   ![](../assets/workflow-enrichment-link.png)

1. En la lista desplegable **Tipo de relación**, elija el tipo de vínculo que desea crear.

1. Identifique el objetivo al que desea vincular el conjunto principal:

   * Para vincular una tabla existente en la base de datos, elija **[!UICONTROL Esquema de base de datos]** y seleccione la tabla deseada del campo **[!UICONTROL Esquema de destino]**.
   * Para vincularse con datos de la transición de entrada, elija **Esquema temporal** y seleccione la transición cuyos datos desee utilizar.

1. Defina los criterios de reconciliación para hacer coincidir los datos del conjunto principal con el esquema vinculado. Hay dos tipos de uniones disponibles:

   * **Combinación simple**: seleccione un atributo específico para hacer coincidir los datos de los dos esquemas. Haga clic en **Agregar unión** y seleccione los atributos **Source** y **Destination** que se utilizarán como criterios de reconciliación.
   * **Unión avanzada**: cree una unión con condiciones avanzadas. Haga clic en **Agregar unión** y haga clic en el botón **Crear condición** para abrir el modelador de consultas.

Hay disponible un ejemplo de flujo de trabajo con vínculos en la sección [Ejemplos](#link-example).

## Reconciliación de datos {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_reconciliation"
>title="Reconciliación"
>abstract="La actividad **Enriquecimiento** ahora se puede utilizar para reconciliar los datos del esquema de la base de datos de Campaign con los datos de otro esquema o con los datos procedentes de un esquema temporal como, por ejemplo, los datos cargados mediante una actividad Carga de archivo. Este tipo de vínculo define una reconciliación hacia un registro único. Adobe Campaign crea un vínculo a una tabla de destino añadiendo una clave externa en la tabla objetivo para almacenar una referencia al registro único."

La actividad **Enriquecimiento** ahora se puede utilizar para reconciliar los datos del esquema de la base de datos de Campaign con los datos de otro esquema o con los datos procedentes de un esquema temporal como, por ejemplo, los datos cargados mediante una actividad Carga de archivo. Este tipo de vínculo define una reconciliación hacia un registro único. Adobe Campaign crea un vínculo a una tabla de destino añadiendo una clave externa en la tabla objetivo para almacenar una referencia al registro único.

Por ejemplo, puede utilizar esta opción para reconciliar el país de un perfil, especificado en un archivo cargado, con uno de los países disponibles en la tabla dedicada de la base de datos de Campaign.

Siga los pasos para configurar una actividad **Enrichment** con un vínculo de reconciliación:

1. Haga clic en el botón **Agregar vínculo** en la sección **Reconciliación**.
1. Identifique los datos con los que desea crear un vínculo de reconciliación.

   * Para crear un vínculo de reconciliación con los datos de la base de datos de Campaign, seleccione **Database schema** y elija el esquema donde se almacena el destino.
   * Para crear un vínculo de reconciliación con datos procedentes de la transición de entrada, seleccione **Temporary schema** y elija la transición de flujo de trabajo en la que se almacenan los datos de destino.

1. Los campos **Etiqueta** y **Nombre** se rellenan automáticamente en función del esquema de destino seleccionado. Si es necesario, puede cambiar sus valores.

1. En la sección **Criterios de reconciliación**, especifique cómo desea reconciliar los datos de las tablas de origen y destino:

   * **Combinación simple**: concilie un campo específico de la tabla de origen con otro campo de la tabla de destino. Para ello, haga clic en el botón **Agregar unión** y especifique los campos **Source** y **Destino** que se utilizarán para la reconciliación.

     >[!NOTE]
     >
     >Puede usar uno o más criterios **Simple join**, en cuyo caso todos deben verificarse para que los datos puedan vincularse.

   * **Unión avanzada**: use el modelador de consultas para configurar los criterios de reconciliación. Para ello, haga clic en el botón **Crear condición** y defina los criterios de reconciliación creando su propia regla con las operaciones AND y OR.

El ejemplo siguiente muestra un flujo de trabajo configurado para crear un vínculo entre la tabla de destinatarios de la base de datos de Adobe Campaign y una tabla temporal que ha generado una actividad **Cargar archivo**. En este ejemplo, la actividad Enrichment concilia ambas tablas utilizando la dirección de correo electrónico como criterios de reconciliación.

![](../assets/enrichment-reconciliation.png)

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

El ejemplo siguiente muestra un flujo de trabajo configurado para crear un vínculo entre dos transiciones. La primera transición identifica los datos de perfil mediante una actividad **Query**, mientras que la segunda transición incluye datos de compra almacenados en un archivo cargado mediante una actividad de archivo Load.

![](../assets/enrichment-uc-link.png)

* La primera actividad **Enrichment** vincula el conjunto principal (datos de la actividad **Query**) con el esquema de la actividad **Cargar archivo**. Esto nos permite hacer coincidir cada perfil objetivo por la consulta con los datos de compra correspondientes.

  ![](../assets/enrichment-uc-link-purchases.png)

* Se agrega una segunda actividad **Enrichment** para enriquecer los datos de la tabla de flujo de trabajo con los datos de compra procedentes de la actividad **Cargar archivo**. Esto nos permite utilizar esos datos en actividades adicionales, por ejemplo, para personalizar mensajes enviados a los clientes con información sobre su compra.

  ![](../assets/enrichment-uc-link-data.png)

