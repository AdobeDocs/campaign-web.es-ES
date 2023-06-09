---
audience: end-user
title: Uso de la actividad Combinar flujo de trabajo
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Combinar
badge: label="Alpha" type="Positive"
source-git-commit: 1ac80ffaabea210bbc02588475ad6e81af4820b1
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 21%

---


# Combinar {#combine}

Esta actividad le permite realizar la segmentación en la población entrante. Por lo tanto, puede combinar varias poblaciones, excluir parte de ellas o solo mantener datos comunes para varios objetivos. Estos son los tipos de segmentación disponibles:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* El **Union** permite agrupar el resultado de varias actividades en un solo destino.
* El **Intersección** permite mantener solo los elementos comunes a las diferentes poblaciones de entrada de la actividad.
* El **Exclusión** permite excluir elementos de una población según determinados criterios.

## Configuración general {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Opciones de combinación de intersecciones"
>abstract="La intersección permite mantener solo los elementos comunes a las diferentes poblaciones de entrada de la actividad. En la sección Conjuntos para unirse, compruebe todas las actividades anteriores a las que desee unirse."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Opciones de combinación de exclusión"
>abstract="La exclusión permite excluir elementos de una población según determinados criterios. En la sección Conjuntos para unirse, compruebe todas las actividades anteriores a las que desee unirse."

Siga estos pasos comunes para comenzar a configurar el **Combinar** actividad:

1. Añada varias actividades, como **Crear audiencia** actividades para formar al menos dos ramas de ejecución diferentes.
1. Añadir un **Combinar** actividad a cualquiera de las ramas anteriores.
1. Seleccione el tipo de segmentación: [unión](#union), [intersección](#intersection) o [exclusión](#exclusion).
1. Haga clic en **Continue**.
1. En el **Configura para unirse** , compruebe todas las actividades anteriores a las que desee unirse.

## Unión {#union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Opciones de reconciliación de intersección"
>abstract="Seleccione el tipo de reconciliación para definir cómo se gestionan los duplicados."

Para el **Union**, debe seleccionar la **Tipo de reconciliación** para definir cómo se gestionan los duplicados:

* **Keys only**: este es el modo predeterminado. La actividad solo mantiene un elemento cuando los elementos de las distintas transiciones de entrada tienen la misma clave. Puede usar esta opción solo si las poblaciones entrantes son homogéneas.
* **Una selección de columnas**: seleccione esta opción para definir la lista de columnas a las que desea aplicar la reconciliación de datos. Primero debe seleccionar el conjunto principal (el que contiene los datos de origen) y luego las columnas que se utilizarán para la unión.

## Intersección {#intersection}

Para el **Intersección** Sin embargo, debe seguir estos pasos adicionales:

1. Seleccione el **Tipo de reconciliación** para definir cómo se gestionan los duplicados. Consulte la [Union](#union) sección.
1. Puede consultar la **Generar finalización** si desea procesar la población restante. El complemento contendrá la unión de los resultados de todas las actividades entrantes menos la intersección. A continuación, se agregará una transición saliente adicional a la actividad.

## Exclusión {#exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Exclusión reglas"
>abstract="Si es necesario, puede manipular las tablas entrantes. De hecho, para excluir un objetivo de otra dimensión, se debe devolver este objetivo a la misma dimensión objetivo que el objetivo principal. Para ello, haga clic en Add a rule en la sección Exclusion rules y especifique las condiciones del cambio de dimensión. La reconciliación de datos se realiza mediante un atributo o una unión."

Para el **Exclusión** Sin embargo, debe seguir estos pasos adicionales:

1. En el **Configura para unirse** , seleccione la **Conjunto principal** de las transiciones de entrada. Es el conjunto desde el que se excluyen los elementos. Los demás conjuntos coinciden con elementos antes de excluirse del conjunto principal.
1. Si es necesario, puede manipular las tablas entrantes. De hecho, para excluir un objetivo de otra dimensión, se debe devolver este objetivo a la misma dimensión objetivo que el objetivo principal. Para ello, haga clic en **Añadir una regla** en el **Reglas de exclusión** y especifique las condiciones del cambio de dimensión. La reconciliación de datos se realiza mediante un atributo o una unión.
1. Puede consultar la **Generar finalización** si desea procesar la población restante. Consulte la [Intersección](#intersection) sección.

## Ejemplos

En el siguiente ejemplo, agregamos un **unión** que recupera todos los perfiles de las dos consultas: personas entre 18 y 27 años y personas entre 34 y 40 años.

![](../assets/workflow-union-example.png)

El siguiente ejemplo muestra el **intersección** entre dos actividades de consulta. Se está utilizando aquí para recuperar perfiles de entre 18 y 27 años y cuya dirección de correo electrónico se ha proporcionado.

![](../assets/workflow-intersection-example.png)

Lo siguiente **exclusión** Este ejemplo muestra dos consultas configuradas para filtrar perfiles que tienen entre 18 y 27 años y tienen un dominio de correo electrónico de Adobe. Los perfiles con un dominio de correo electrónico de Adobe se excluyen del primer conjunto.

![](../assets/workflow-exclusion-example.png)


