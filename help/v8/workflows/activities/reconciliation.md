---
audience: end-user
title: Uso de la actividad de flujo de trabajo Reconciliación
description: Aprenda a utilizar la actividad del flujo de trabajo Reconciliación
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 22%

---

# Reconciliación {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Actividad de reconciliación"
>abstract="La actividad **Reconciliation** es una actividad **Targeting** que define el vínculo entre los datos de la base de datos de Adobe Campaign y los de una tabla de trabajo. Por ejemplo, la actividad **Reconciliación** se puede colocar después de la actividad **Cargar archivo** para importar datos no estándar a la base de datos. En este caso, la actividad **Reconciliation** define el vínculo entre los datos de la base de datos de Adobe Campaign y los de la tabla externa."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Campo de selección de reconciliación"
>abstract="Campo de selección de reconciliación"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Condición de creación de reconciliación"
>abstract="Condición de creación de reconciliación"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Complemento de generación de reconciliación"
>abstract="Complemento de generación de reconciliación"

La actividad **Reconciliation** es una actividad **Targeting** que define el vínculo entre los datos de la base de datos de Adobe Campaign y los de una tabla de trabajo, como los cargados desde un archivo externo.

Por ejemplo, la actividad **Reconciliación** se puede colocar después de la actividad **Cargar archivo** para importar datos no estándar a la base de datos. En este caso, la actividad **Reconciliation** define el vínculo entre los datos de la base de datos de Adobe Campaign y los de la tabla de resultados.

## Prácticas recomendadas {#reconciliation-best-practices}

Aunque la actividad **Enrichment** define datos adicionales para procesar en el flujo de trabajo (por ejemplo, combinar datos de varios conjuntos o crear vínculos a un recurso temporal), la actividad **Reconciliation** vincula datos no identificados a recursos existentes.

>[!NOTE]
>Las operaciones de reconciliación requieren que los datos de las dimensiones vinculadas ya existan en la base de datos. Por ejemplo, si importa un archivo de compras que muestre qué producto se compró, a qué hora y por qué cliente, el producto y el cliente ya deben existir en la base de datos.

## Configuración de la actividad Reconciliación {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Dimensión de segmentación"
>abstract="Seleccionar la nueva dimensión de segmentación. Una dimensión define la población objetivo: destinatarios, suscriptores de la aplicación, operadores, suscriptores, etc. De forma predeterminada, está seleccionada la dimensión de segmentación actual."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Reglas de reconciliación"
>abstract="Seleccione las reglas de reconciliación para la deduplicación. Para utilizar atributos, seleccione **Atributos simples** y seleccione los campos de origen y destino. Para crear su propia condición de reconciliación utilizando el modelador de consultas, seleccione la opción **Condiciones de reconciliación avanzadas**."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/query-database/query-modeler-overview" text="Trabajar con el modelador de consultas"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Seleccionar la dimensión de segmentación"
>abstract="Seleccione la dimensión de segmentación con la que se reconciliarán los datos de entrada."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=es#targeting-dimensions" text="Dimensiones de segmentación"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Mantener datos no reconciliados"
>abstract="De forma predeterminada, los datos no reconciliados se mantienen en la transición saliente y están disponibles en la tabla de trabajo para su uso futuro. Para quitar los datos no reconciliados, desactive la opción **Conservar datos no reconciliados**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Atributo de reconciliación"
>abstract="Seleccione el atributo que desea utilizar para reconciliar los datos y haga clic en Confirmar."

Siga estos pasos para configurar la actividad **Reconciliation**:

1. Agregue una actividad **Reconciliation** al flujo de trabajo. Esta actividad debe seguir una transición que contenga una población cuya dimensión de segmentación no provenga directamente de Adobe Campaign.

1. Seleccionar la nueva dimensión de segmentación. Una dimensión define la población objetivo: destinatarios, suscriptores de la aplicación, operadores, suscriptores, etc. [Más información sobre las dimensiones de segmentación](../../audience/about-recipients.md#targeting-dimensions).

1. Seleccione los campos que se utilizarán para la reconciliación. Se pueden utilizar uno o más criterios de reconciliación.

   1. Para usar atributos para reconciliar datos, seleccione la opción **Atributos simples**. El campo **Source** enumera los campos disponibles en la transición de entrada que deben conciliarse. El campo **Destino** corresponde a los campos de la dimensión de segmentación seleccionada. Los datos se concilian cuando el origen y el destino son iguales. Por ejemplo, seleccione los campos **Correo electrónico** para anular la duplicación de perfiles según su dirección de correo electrónico.

      Para agregar otro criterio de reconciliación, haga clic en el botón **Agregar regla**. Si se especifican varias condiciones de vínculo, todas deben verificarse para que los datos se vinculen entre sí.

      ![Ejemplo de criterios de reconciliación](../assets/workflow-reconciliation-criteria.png)

   1. Para usar otros atributos para reconciliar datos, seleccione la opción **Condiciones de reconciliación avanzadas**. A continuación, puede crear su propia condición de reconciliación utilizando el modelador de consultas. [Aprenda a trabajar con el modelador de consultas](../../query/query-modeler-overview.md).

1. Filtre los datos para conciliarlos con el botón **Crear filtro**. Esto permite crear una condición personalizada mediante el modelador de consultas. [Aprenda a trabajar con el modelador de consultas](../../query/query-modeler-overview.md).

De forma predeterminada, los datos no reconciliados se mantienen en la transición saliente y están disponibles en la tabla de trabajo para su uso futuro. Para quitar los datos no reconciliados, desactive la opción **Conservar datos no reconciliados**.

## Ejemplo {#reconciliation-example}

En el siguiente ejemplo se muestra un flujo de trabajo que crea una audiencia de perfiles directamente desde un archivo importado que contiene nuevos clientes. Incluye las siguientes actividades:

El flujo de trabajo está diseñado de la siguiente manera:

![Ejemplo de flujo de trabajo](../assets/workflow-reconciliation-sample-1.0.png)

Se crea con las siguientes actividades:

* Una actividad de [Cargar archivo](load-file.md) carga un archivo que contiene datos de perfil extraídos de una herramienta externa.

  Por ejemplo:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* Una actividad **Reconciliation** identifica los datos entrantes como perfiles mediante el uso de los campos **Email** y **Date of birth** como criterios de reconciliación.

  ![Ejemplo de actividad de reconciliación](../assets/workflow-reconciliation-sample-1.1.png)

* Una actividad [Guardar audiencia](save-audience.md) crea una audiencia nueva basada en estas actualizaciones. También puede reemplazar la actividad **Guardar audiencia** con una actividad **Finalizar** si no es necesario crear o actualizar una audiencia específica. Los perfiles de destinatario se actualizan en cualquier caso al ejecutar el flujo de trabajo.

## Compatibilidad {#reconciliation-compat}

La actividad **Reconciliation** no existe en la consola del cliente. Todas las actividades **Enrichment** creadas en la consola del cliente con las opciones de reconciliación habilitadas se muestran como actividades **Reconciliation** en la interfaz de usuario web de Campaign.