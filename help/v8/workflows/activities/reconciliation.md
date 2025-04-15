---
audience: end-user
title: Utilizar el flujo de trabajo de reconciliación actividad
description: Aprenda a utilizar la actividad del flujo de trabajo de reconciliación
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
>abstract="La **actividad de reconciliación** es una **actividad de segmentación** que define la vincular entre los datos de la base de datos Adobe Campaign y los datos de una tabla de trabajo. Por ejemplo, la actividad **Reconciliación** se puede colocar después de la actividad **Cargar archivo** para importar datos no estándar a la base de datos. En este caso, la **actividad Reconciliación** define el vincular entre los datos de la base de datos Adobe Campaign y los datos de la tabla externa."

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

La **actividad de reconciliación** es un **actividad de destino** que define el vincular entre los datos de la base de datos Adobe Campaign y los datos de una tabla de trabajo, como los datos cargados desde un archivo externo.

Por ejemplo, la actividad **Reconciliación** se puede colocar después de la actividad **Cargar archivo** para importar datos no estándar a la base de datos. En este caso, la **actividad Reconciliación** define el vincular entre los datos de la base de datos Adobe Campaign y los datos de la tabla de trabajo.

## Prácticas recomendadas {#reconciliation-best-practices}

Mientras que la **actividad de enriquecimiento** define datos adicionales para procesar en su flujo de trabajo (por ejemplo, combinar datos de varios conjuntos o crear vínculos a un recurso temporal), la **actividad de reconciliación** vincula datos no identificados a recursos existentes.

>[!NOTE]
>Las operaciones de reconciliación requieren que los datos de las dimensiones vinculadas ya existan en la base de datos. Por ejemplo, si importa un archivo de compras que muestra qué producto se compró, en qué momento y por qué cliente, el producto y el cliente ya deben existir en la base de datos.

## Configuración de la actividad Reconciliación {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Dimensión de segmentación"
>abstract="Seleccionar la nueva dimensión de segmentación. Un dimensión define la población objetivo: destinatarios, suscriptores de la aplicación, operadores, suscriptores y más. De forma predeterminada, está seleccionada la dimensión de segmentación actual."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Reglas de reconciliación"
>abstract="Seleccione las reglas de reconciliación para deduplicación. Para utilizar atributos, seleccione **Atributos simples** y seleccione los campos de origen y destino. Para crear su propia condición de reconciliación utilizando el modelador de consultas, seleccione la opción **Condiciones de reconciliación avanzadas**."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/query-database/query-modeler-overview" text="Trabajar con el modelador de consultas"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Seleccionar la dimensión de segmentación"
>abstract="Seleccione la dimensión de segmentación con la que se reconciliarán los datos de entrada."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=es#targeting-dimensions" text="Dimensiones de segmentación"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Mantener datos no reconciliados"
>abstract="De forma predeterminada, los datos no conciliados se guardan en el transición saliente y están disponibles en la tabla de trabajo para su uso futuro. Para eliminar los datos no reconciliados, desactive la opción Mantener los **datos** no reconciliados."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Atributo de reconciliación"
>abstract="Seleccione el atributo que desea utilizar para conciliar los datos y haga clic en Confirmar."

Siga estos pasos para configurar el **actividad de reconciliación** :

1. añadir una **Reconciliación** actividad a su flujo de trabajo. Este actividad debe seguir una transición que contenga una población cuyo dimensión de segmentación no provenga directamente de Adobe Campaign.

1. Seleccionar la nueva dimensión de segmentación. Un dimensión define la población objetivo: destinatarios, suscriptores de la aplicación, operadores, suscriptores y más. [Obtenga más información sobre direccionamiento dimensiones](../../audience/about-recipients.md#targeting-dimensions).

1. Seleccione los campos que se utilizarán en la reconciliación. Se pueden utilizar uno o más criterios de reconciliación.

   1. Para utilizar atributos para conciliar datos, seleccione la **opción Atributos** simples. El **campo Origen** enumera los campos disponibles en la transición de entrada y que se van a conciliar. El **campo Destino** corresponde a los campos del dimensión de segmentación seleccionado. Los datos se concilian cuando el origen y el destino son iguales. Por ejemplo, seleccione los campos Correo electrónico **para anular la duplicación de perfiles en función de** su dirección correo electrónico.

      Para añadir otro criterio de reconciliación, haga clic en la **añadir regla** botón. Si se especifican varias condiciones de unión, deben verificarse todas para que los datos se vinculen entre sí.

      ![Ejemplo de criterios de conciliación](../assets/workflow-reconciliation-criteria.png)

   1. Para utilizar otros atributos para conciliar datos, seleccione la **opción Avanzadas condiciones** de reconciliación. A continuación, puede crear su propia condición de reconciliación utilizando el consulta modelador. [Aprenda a trabajar con el consulta modelador](../../query/query-modeler-overview.md).

1. Filtrar datos para conciliar mediante el filtro **de** Crear botón. Esto permite crear una condición personalizada utilizando el modelador consulta. [Aprenda a trabajar con el consulta modelador](../../query/query-modeler-overview.md).

De forma predeterminada, los datos no conciliados se guardan en el transición saliente y están disponibles en la tabla de trabajo para su uso futuro. Para eliminar los datos no reconciliados, desactive la opción Mantener los **datos** no reconciliados.

## Ejemplo {#reconciliation-example}

En el siguiente ejemplo se muestra un flujo de trabajo que crea una audiencia de perfiles directamente desde un archivo importado que contiene nuevos clientes. Incluye las siguientes actividades:

El flujo de trabajo está diseñado de la siguiente manera:

![Ejemplo de flujo de trabajo](../assets/workflow-reconciliation-sample-1.0.png)

Se crea con las siguientes actividades:

* Un [archivo](load-file.md) de carga actividad carga un archivo que contiene datos perfil extraídos de un herramienta externo.

  Por ejemplo:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* Un **actividad de reconciliación** identifica los datos entrantes como perfiles utilizando los **campos Correo electrónico** y **Fecha de nacimiento** como criterios de conciliación.

  ![Ejemplo de reconciliación actividad](../assets/workflow-reconciliation-sample-1.1.png)

* Un [actividad audiencia](save-audience.md) Guardar crea un nuevo audiencia basado en estas actualizaciones. También puede reemplazar el **actividad audiencia** Guardar por un **actividad** final si no es necesario crear o actualizar un audiencia específico. En cualquier caso, los perfiles de destinatario se actualizan al ejecutar el flujo de trabajo.

## Compatibilidad {#reconciliation-compat}

La **actividad Reconciliación** no existe en la consola del cliente. Todas las **actividades de enriquecimiento** creadas en la consola del cliente con las opciones de reconciliación activadas se muestran como **actividades de reconciliación** en la interfaz de Campaign Web usuario.