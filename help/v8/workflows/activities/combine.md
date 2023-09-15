---
audience: end-user
title: Uso de la actividad de flujo de trabajo Combinar
description: Aprenda a utilizar la actividad de flujo de trabajo Combinar
badge: label="Beta"
source-git-commit: d5b0777ba51f595733c6b7e366d0a9a21a13d84a
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 85%

---


# Combinar {#combine}

El **Combinar** la actividad es una **Segmentación** actividad. Esta actividad le permite realizar la segmentación de la población entrante. Por lo tanto, puede combinar varias poblaciones, excluir parte de ellas o solo mantener datos comunes para varios públicos destinatarios. Estos son los tipos de segmentación disponibles:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* La **Unión** le permite agrupar el resultado de varias actividades en un solo público destinatario.
* La **Intersección** permite mantener solo los elementos comunes a las diferentes poblaciones entrantes de la actividad.
* La **Exclusión** permite excluir elementos de una población según determinados criterios.

## Configuración general {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Opciones de combinación de intersección"
>abstract="La intersección permite mantener solo los elementos comunes a las diferentes poblaciones entrantes en la actividad. En la sección Conjuntos que unir, compruebe todas las actividades anteriores que desee unir."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Opciones de combinación de exclusión"
>abstract="La exclusión permite excluir elementos de una población según determinados criterios. En la sección Conjuntos que unir, compruebe todas las actividades anteriores que desee unir."

Siga estos pasos comunes para comenzar a configurar la actividad **Combinar**:

1. Añada varias actividades, como actividades **Generar público destinatario** para formar al menos dos ramas de ejecución diferentes.
1. Añada una actividad **Combinar** a cualquiera de las ramas anteriores.
1. Seleccione el tipo de segmentación: [unión](#union), [intersección](#intersection) o [exclusión](#exclusion).
1. Haga clic en **Continuar**.
1. En la sección **Conjuntos que unir**, compruebe todas las actividades anteriores que desee unir.

## Unión {#union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Opciones de reconciliación de intersección"
>abstract="Seleccione el tipo de reconciliación para definir cómo se gestionan los duplicados."

En el **Combinar** actividad, puede configurar un **Union**. Para ello, debe seleccionar la **Tipo de reconciliación** para definir cómo se gestionan los duplicados:

* **Solo claves**: este es el modo predeterminado. La actividad solo mantiene un elemento cuando los elementos de las distintas transiciones entrantes tienen la misma clave. Puede usar esta opción solo si las poblaciones entrantes son homogéneas.
* **Una selección de columnas**: seleccione esta opción para definir la lista de columnas a las que desea aplicar la reconciliación de datos. Primero debe seleccionar el conjunto principal (el que contiene los datos de origen) y luego las columnas que se utilizarán para la unión.

## Intersección {#intersection}

En el **Combinar** actividad, puede configurar un **Intersección**. Para ello, debe seguir los pasos adicionales a continuación:

1. Seleccione el **Tipo de reconciliación** para definir cómo se gestionan los duplicados. Consulte la sección [Unión](#union).
1. Seleccione la opción **Generar complemento** si desea procesar la población restante. El complemento contendrá la unión de los resultados de todas las actividades entrantes menos la intersección. A continuación, se añadirá una transición saliente adicional a la actividad.

## Exclusión {#exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Exclusión  reglas"
>abstract="Si es necesario, puede manipular las tablas entrantes. De hecho, para excluir un público destinatario de otra dimensión, se debe devolver este público destinatario a la misma dimensión de segmentación que el público destinatario principal. Para ello, haga clic en Añadir una regla en la sección Reglas de exclusión y especifique las condiciones del cambio de dimensión. La reconciliación de datos se lleva a cabo mediante un atributo o una unión."

En el **Combinar** actividad, puede configurar un **Exclusión**. Para ello, debe seguir los pasos adicionales a continuación:

1. En la sección **Conjuntos que unir**, seleccione el **Conjunto principal** de las transiciones entrantes. Es el conjunto desde el que se excluyen los elementos. Los demás conjuntos coinciden con elementos antes de excluirse del conjunto principal.
1. Si es necesario, puede manipular las tablas entrantes. De hecho, para excluir un público destinatario de otra dimensión, se debe devolver este público destinatario a la misma dimensión de segmentación que el público destinatario principal. Para ello, haga clic en **Añadir una regla** en la sección **Reglas de exclusión** y especifique las condiciones del cambio de dimensión. La reconciliación de datos se lleva a cabo mediante un atributo o una unión.
1. Seleccione la opción **Generar complemento** si desea procesar la población restante. Consulte la sección [Intersección](#intersection).

## Ejemplos

En el siguiente ejemplo, se utiliza un **Combinar** y agregamos una actividad de **unión** recuperar todos los perfiles de las dos consultas: personas entre 18 y 27 años y personas entre 34 y 40 años.

![](../assets/workflow-union-example.png)

El siguiente ejemplo muestra la **intersección** entre dos actividades de consulta. Se está utilizando aquí para recuperar perfiles de entre 18 y 27 años y cuya dirección de correo electrónico se ha proporcionado.

![](../assets/workflow-intersection-example.png)

El siguiente ejemplo de **exclusión** muestra dos consultas configuradas para filtrar perfiles que tienen entre 18 y 27 años y que tienen un dominio de correo electrónico de Adobe. A continuación, los perfiles con un dominio de correo electrónico de Adobe se excluyen del primer conjunto.

![](../assets/workflow-exclusion-example.png)


