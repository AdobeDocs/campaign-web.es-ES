---
audience: end-user
title: Uso de la actividad de flujo de trabajo JavaScript code
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo JavaScript code
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 29%

---

# Código JavaScript {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="Código JavaScript"
>abstract="La actividad de **Código JavaScript** le permite ejecutar una secuencia de comandos JavaScript en el contexto de un flujo de trabajo. Esto le permite realizar acciones o recopilar información de la base de datos. Utilice actividades de código JavaScript **sencillo** para ejecutar un fragmento de código en la ejecución del flujo de trabajo. **Avanzadas** Las actividades de código JavaScript permiten realizar operaciones más complejas ejecutando dos fragmentos de código diferentes en orden secuencial. La primera vez que se inicia el flujo de trabajo, se ejecuta la primera llamada. Cada vez que se vuelve a ejecutar el flujo de trabajo, se ejecuta el código definido en la segunda llamada."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="Fragmento de JavaScript"
>abstract="Defina la secuencia de comandos que se ejecutará al ejecutar la actividad. Si está configurando una actividad de JavaScript **avanzada**, es necesario editar dos fragmentos de código: el primer código de llamada que se ejecuta en la primera ejecución del flujo de trabajo y el siguiente código de llamada que se ejecuta en las siguientes llamadas del flujo de trabajo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="Ejecución de Javascript"
>abstract="Configure el retraso de ejecución para detener la actividad después de un periodo de ejecución. De forma predeterminada, la fase de ejecución no puede exceder de 1 hora. Tras este retraso, el proceso se anula con un mensaje de error y la ejecución de la actividad falla. Para omitir este límite, establezca el valor en 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="Transición de JavaScript"
>abstract="Si desea añadir varias transiciones de salida, haga clic en el botón **[!UICONTROL Añadir transiciones]**. Esto le permite, por ejemplo, activar una transición específica basada en una condición específica definida en la actividad del código JavaScript. Esta opción solo está disponible en las actividades de código JavaScript **avanzadas**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="Transición de JavaScript"
>abstract="Active la opción **[!UICONTROL Procesar errores]** para mantener los errores que se producen durante la ejecución del script en una transición de salida adicional."

La actividad **JavaScript code** es una actividad de **administración de datos**. Utilice esta actividad para ejecutar un script de JavaScript en el contexto de un flujo de trabajo. Esto le permite recopilar información de la base de datos o realizar otras operaciones complejas.

## Configuración de la actividad JavaScript code {#javascript-code-configuration}

Siga estos pasos para configurar la actividad **JavaScript code**:

1. Agregue una actividad **JavaScript code** a su flujo de trabajo.

1. Elija el tipo de actividad que desea crear:

   * **Simple**: ejecute un fragmento de código.
   * **Avanzado**: esta opción le permite realizar operaciones más avanzadas mediante la ejecución de dos fragmentos de código diferentes. [Aprenda a configurar una actividad avanzada de JavaScript](#advanced)

   >[!NOTE]
   >
   >Con la interfaz de usuario web de Campaign, hemos consolidado dos actividades en una al combinar las funcionalidades de código JavaScript **Simple** y **Advanced**. Esta consolidación no afecta a la funcionalidad de la actividad de ninguna manera.

1. Confirme y haga clic en el botón **[!UICONTROL Editar código]** para abrir el editor de expresiones. El panel izquierdo proporciona sintaxis predefinida que puede aprovechar para crear su código, incluidas variables de evento. [Aprenda a trabajar con variables de eventos y el editor de expresiones](../event-variables.md)

   ![](../assets/javascript-editor.png)

1. En la sección **[!UICONTROL Execution]**, configure el retraso para detener la actividad después de un período de ejecución. De forma predeterminada, la fase de ejecución no puede exceder de 1 hora. Tras este retraso, el proceso se anula con un mensaje de error y la ejecución de la actividad falla. Para omitir este límite, establezca el valor en 0.

   ![](../assets/javascript-config.png)

1. Active la opción **[!UICONTROL Procesar errores]** para mantener los errores que se producen durante la ejecución del script en una transición de salida adicional.

## Actividades de código JavaScript avanzadas {#advanced}

Las actividades avanzadas de JavaScript le permiten realizar operaciones complejas. Le permite hacer lo siguiente:

* Ejecute dos fragmentos de código diferentes. El primer fragmento de código se ejecuta la primera vez que se inicia el flujo de trabajo. Cada vez que se vuelve a ejecutar el flujo de trabajo, se ejecuta el fragmento de código definido en la segunda llamada.
* Añada varias transiciones de salida con las que pueda interactuar dinámicamente mediante una secuencia de comandos.

Para configurar una actividad de Advanced JavaScript code, siga estos pasos:

1. Seleccione el tipo **Advanced** y, a continuación, configure los fragmentos de código para ejecutar:

   * Haga clic en **[!UICONTROL Editar el código de la primera llamada]** para definir el script que se ejecutará durante la primera llamada.
   * Haga clic en **[!UICONTROL Editar código de llamada siguiente]** para definir el script que se ejecutará durante las siguientes llamadas del flujo de trabajo. (opcional)

1. Para agregar una o varias transiciones de salida, haga clic en el botón **[!UICONTROL Agregar transiciones]** y especifique una etiqueta y un nombre interno para cada transición.

   En este ejemplo hemos configurado dos transiciones activadas por la secuencia de comandos en el fragmento de código en función de condiciones específicas.

   ![](../assets/javascript-transitions.png)

1. Complete la configuración de la actividad e inicie el flujo de trabajo.

## Ejemplo {#javascript-code-example}

### Inicializar variables según la población entrante {#example1}

Este ejemplo muestra cómo inicializar una variable en función del número de perfiles objetivo por un flujo de trabajo.

![](../assets/javascript-example1.png)

VIP A continuación, se muestran perfiles de segmentación de perfiles de la base de datos de. Queremos crear una variable denominada &quot;canal&quot; con un valor que dependa del número de perfiles objetivo por la actividad Generar audiencia:

* Si hay más de 1000 perfiles objetivo, inicialice la variable con el valor &quot;email&quot;.
* De lo contrario, inícielo con el valor &quot;sms&quot;.

Para ello, siga estos pasos:

1. Agregue una actividad **JavaScript code** con el tipo **Simple** después de la actividad **Generar audiencia**.

1. Haga clic en **Editar código** y configure el fragmento de código como se muestra a continuación:

   ```
   if (vars.recCount > 1000)
       vars.channel ="email"
   else
       vars.channel = "sms"
   ```

1. Inicie el flujo de trabajo. La variable &quot;channel&quot; se crea con el valor &quot;email&quot; o &quot;sms&quot;, según el número de perfiles objetivo por la actividad **Generar audiencia**.

### Déclencheur transiciones basadas en el valor de una variable {#example2}

Este ejemplo muestra cómo almacenar en déclencheur una transición en función del valor de una variable.

![](../assets/javascript-example2-transitions.png)

En este caso, el flujo de trabajo comienza con una actividad **Señal externa**, a la cual se pasa una variable (`interest`) desde otro flujo de trabajo. El valor de la variable es &quot;running&quot; o &quot;yoga&quot;, según las operaciones de filtrado realizadas en el flujo de trabajo inicial.

Queremos almacenar en déclencheur diferentes transiciones en el flujo de trabajo, en función del valor de la variable.

Para ello, siga estos pasos:

1. Agregue una actividad **JavaScript code** después de la actividad External signal con el tipo **Advanced**.

1. Añada dos transiciones: una para cada valor de variable posible (&quot;running&quot;, &quot;yoga&quot;).

1. Haga clic en **Editar el código de la primera llamada** y configure el fragmento de código como se muestra a continuación:

   ```
   if (vars.interest=="running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. Complete la configuración de cada transición para adaptarla a sus necesidades e inicie el flujo de trabajo. Una de las dos transiciones de salida está activada, según el valor de la variable `interest` que se ha pasado a través de la actividad **Señal externa**.
