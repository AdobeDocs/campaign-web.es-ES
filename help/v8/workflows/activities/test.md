---
audience: end-user
title: Uso de la actividad Test workflow
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Prueba
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 37%

---


# Prueba {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="Actividad de prueba"
>abstract="La actividad **Prueba** es una actividad de **Control de flujo**. Permite habilitar transiciones en función de condiciones especificadas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="Condiciones"
>abstract="La actividad **Prueba** puede tener varias transiciones de salida. Durante la ejecución del flujo de trabajo, cada condición se prueba secuencialmente hasta que se cumpla una de ellas. Si no se cumple ninguna de las condiciones, el flujo de trabajo continúa en la ruta de la **[!UICONTROL condición predeterminada]**. Si no se activa ninguna condición predeterminada, el flujo de trabajo se detiene en este punto."

La actividad **Prueba** es una actividad de **Control de flujo**. Permite habilitar transiciones en función de condiciones especificadas.

## Configuración de la actividad Test {#test-configuration}

Siga estos pasos para configurar la actividad **Test**:

1. Añada una actividad **Test** al flujo de trabajo.

1. De manera predeterminada, la actividad **[!UICONTROL Test]** presenta una prueba booleana simple. Si se cumple la condición definida en la transición &quot;True&quot;, se activa esta transición. De lo contrario, se activa una transición predeterminada &quot;False&quot;.

1. Para configurar la condición asociada con una transición, haga clic en el icono **[!UICONTROL Abrir cuadro de diálogo de personalización]**. Utilice el editor de expresiones para definir las reglas necesarias para activar esta transición. También puede utilizar variables de evento, condiciones y funciones de fecha y hora. [Aprenda a trabajar con variables de eventos y el editor de expresiones](../event-variables.md).

   Además, modifique el campo **[!UICONTROL Label]** para personalizar el nombre de la transición en el lienzo del flujo de trabajo.

   ![Configuración predeterminada de la actividad de prueba](../assets/workflow-test-default.png)

1. Agregue varias transiciones de salida a una actividad **[!UICONTROL Test]**. Para ello, haga clic en el botón **[!UICONTROL Agregar condición]** y configure la etiqueta y la condición asociada para cada transición.

1. Durante la ejecución del flujo de trabajo, cada condición se prueba secuencialmente hasta que se cumpla una de ellas. Si no se cumple ninguna de las condiciones, el flujo de trabajo continúa en la ruta de la **[!UICONTROL condición predeterminada]**. Si no se activa ninguna condición predeterminada, el flujo de trabajo se detiene en este punto.

## Ejemplo {#example}

En este ejemplo, se activan distintas transiciones en función del número de perfiles objetivo por una actividad **[!UICONTROL Generar audiencia]**:
* Si hay más de 10 000 perfiles de destino, se envía un mensaje de correo electrónico.
* Para entre 1000 y 10 000 perfiles, se envía un SMS.
* Si los perfiles objetivo caen por debajo de 1000, se les dirige a una transición de &quot;no contactar&quot;.

![Ejemplo de transiciones de actividad de prueba](../assets/workflow-test-example.png)

Para conseguirlo, se utiliza la variable de evento `vars.recCount` en las condiciones &quot;email&quot; y &quot;sms&quot; para contar el número de perfiles de destino y activar la transición adecuada.

![Ejemplo de configuración de actividad de prueba](../assets/workflow-test-example-config.png)
