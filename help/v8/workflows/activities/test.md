---
audience: end-user
title: Utilizar el Test flujo de trabajo actividad
description: Aprenda a utilizar el actividad de flujo de trabajo de prueba
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

## Configurar el actividad de prueba {#test-configuration}

Siga estos pasos para configurar el **actividad de prueba** :

1. Añada una actividad **Test** al flujo de trabajo.

1. De forma predeterminada, el **[!UICONTROL actividad de prueba]** presenta un prueba booleano simple. Si se cumple la condición definida en el transición &quot;True&quot;, este transición se activa. De lo contrario, se activa un transición predeterminado &quot;False&quot;.

1. Para configurar la condición asociada a una transición, haga clic en el icono Abrir **[!UICONTROL personalización cuadro de diálogo]** . Utilice el editor expresión para definir las reglas necesarias para activar este transición. También puede utilizar evento variables, condiciones y funciones de fecha y hora. [Aprenda a trabajar con variables evento y con el editor expresión](../event-variables.md).

   Además, modifique el **[!UICONTROL campo Etiquetar]** para personalizar el nombre del transición en el lienzo del flujo de trabajo.

   ![Configuración predeterminada del actividad de prueba](../assets/workflow-test-default.png)

1. añadir varias transiciones de salida a un **[!UICONTROL actividad de prueba]** . Para ello, haga clic en el botón condición **** de añadir y configure la etiqueta y la condición asociada para cada transición.

1. Durante la ejecución del flujo de trabajo, cada condición se prueba secuencialmente hasta que se cumpla una de ellas. Si no se cumple ninguna de las condiciones, el flujo de trabajo continúa en la ruta de la **[!UICONTROL condición predeterminada]**. Si no se activa ninguna condición predeterminada, el flujo de trabajo se detiene en este punto.

## Ejemplo {#example}

En este ejemplo, se activan diferentes transiciones en función del número de perfiles segmentados por un **[!UICONTROL actividad de audiencia]** de compilación:
* Si se segmentan más de 10000 perfiles, se envía un mensaje correo electrónico.
* Se envía un SMS para 1000 a 10.000 perfiles.
* Si los perfiles objetivo son inferiores a 1.000, se les dirige a un transición de &quot;no contacto&quot;.

![Ejemplo de transiciones de actividad de prueba](../assets/workflow-test-example.png)

Para lograr esto, el `vars.recCount` variable evento se utiliza en las condiciones &quot;correo electrónico&quot; y &quot;sms&quot; para contar el número de perfiles objetivo y activar el transición apropiado.

![Configuración del ejemplo de actividad de prueba](../assets/workflow-test-example-config.png)
