---
audience: end-user
title: Uso de la actividad de flujo de trabajo Deduplication
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Deduplicación
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
TQID: https://experienceleague.adobe.com/gpvGRMzvpKR3yi3yUiUe9NJPt-FR2FO-qzbhFsBd6ms
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
source-git-commit: 1c4cdd5164d0cf572e9b88881bbe240b06308866
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 36%
---
# Deduplicación {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campos para identificar duplicados"
>abstract="En la sección **Campos para identificar duplicados**, haga clic en el botón **Añadir atributo** para especificar los campos para los que los valores idénticos permiten identificar los duplicados, tales como: dirección de correo electrónico, nombre y apellidos, etc. El orden de los campos especifica los que se procesarán en primer lugar."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Actividad de deduplicación"
>abstract="La actividad **Deduplicación** elimina los duplicados de los resultados de las actividades entrantes. Se utiliza principalmente después de las actividades de segmentación y antes de las actividades que permiten el uso de datos segmentados. Cuando haya más de una transición entrante disponible, utilice la sección **Conjuntos que unir** para seleccionar qué transiciones conectar a la actividad."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_sets"
>title="Conjuntos que unir"
>abstract="Compruebe las actividades anteriores que desea conectar como transiciones entrantes de la actividad **Deduplicación**. Las actividades seleccionadas se conectarán entonces a la **deduplicación**. Esta sección solo se muestra cuando hay más de una transición entrante disponible para conectar a la actividad."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generación de un complemento"
>abstract="Puede generar una transición de salida adicional con la población restante excluida como duplicados. Para ello, active la opción **Generar complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configuración de la deduplicación"
>abstract="Para eliminar duplicados en los datos entrantes, defina el método de deduplicación en los campos siguientes. De forma predeterminada, solo se guarda un registro. Seleccione el modo de deduplicación en función de una expresión o un atributo. De forma predeterminada, el registro que se va a excluir de los duplicados se selecciona de forma aleatoria."

La actividad **Deduplication** es una actividad de **segmentación**. Esta actividad elimina los duplicados en los resultados de las actividades entrantes, como los perfiles duplicados en la lista de destinatarios. La actividad **Deduplication** se utiliza generalmente después de las actividades de segmentación y antes de las actividades que utilizan datos de objetivo.

La actividad admite varias transiciones de entrada. Cuando haya más de una transición entrante disponible, utilice la sección **Sets to join** en las propiedades de la actividad para seleccionar qué transiciones conectar con la actividad. Las transiciones seleccionadas se vincularán a continuación a la **anulación de duplicación** en el lienzo del flujo de trabajo.

## Configuración de la actividad de anulación de duplicación {#deduplication-configuration}

Siga estos pasos para configurar la actividad **Deduplication**:

![Proceso de configuración de anulación de duplicación del flujo de trabajo](../assets/workflow-deduplication.png)

1. Agregue una actividad **Deduplication** a su flujo de trabajo.

1. En la sección **Conjuntos para unirse**, compruebe las actividades anteriores que desea conectar como transiciones entrantes de la actividad **Deduplication**. Las actividades seleccionadas se enlazan a continuación con la **anulación de duplicación** en el lienzo del flujo de trabajo. Utilice el campo **Conjunto principal** para definir la transición entrante de referencia. Los registros de los demás conjuntos se comparan con el conjunto principal para identificar duplicados.

   >[!NOTE]
   >
   >Esta sección solo se muestra cuando hay más de una transición entrante disponible.

1. En la sección **Campos para identificar duplicados**, haga clic en el botón **Añadir atributo** para especificar los campos para los que los valores idénticos permiten identificar los duplicados, tales como: dirección de correo electrónico, nombre y apellidos, etc. El orden de los campos especifica los que se procesarán en primer lugar. [Aprenda a seleccionar atributos y agregarlos a favoritos](../../get-started/attributes.md).

1. En la sección **Configuración de anulación de duplicación**, seleccione el número de **duplicados únicos que desea conservar**. El valor predeterminado de este campo es 1. El valor 0 mantiene todos los duplicados.

   Por ejemplo, si los registros A y B se consideran duplicados del registro Y, y el registro C se considera un duplicado del registro Z:

   * Si el valor del campo es 1: solo se guardan los registros Y y Z.
   * Si el valor del campo es 0: se guardan todos los registros.
   * Si el valor del campo es 2: se conservan los registros C y Z, y se conservan dos registros de A, B e Y, al azar o en función del método de deduplicación seleccionado.

1. Seleccione el **método de deduplicación** que se va a utilizar:

   * **[!UICONTROL Selección aleatoria]**: Selecciona aleatoriamente el registro que se va a excluir de los duplicados.
   * **[!UICONTROL Usar una expresión]**: conserva los registros para los que la expresión especificada tiene el valor más pequeño o más grande. Escriba la **[!UICONTROL Expresión]** y, a continuación, elija el orden **[!UICONTROL Ordenar]**: **[!UICONTROL Ascendente (primero los valores más pequeños)]** o **[!UICONTROL Descendente (primero los valores más altos)]**.
   * **[!UICONTROL Valor no vacío]**: conserva los registros para los que la expresión no está vacía.
   * **[!UICONTROL Siguiendo una lista de valores]**: Define la prioridad de registro al hacer coincidir uno o más valores para un atributo o expresión. Haga clic en **[!UICONTROL Agregar atributo]** para agregar un atributo. Para cada atributo:

     * En el campo **[!UICONTROL Atributo]**, seleccione el atributo o cree una expresión.
     * Haga clic en **[!UICONTROL Agregar valor]** para generar la lista ordenada de valores a priorizar.
     * Utilice la lista desplegable **[!UICONTROL Ordenar por otros valores]** para elegir cómo ordenar los valores que no están en la lista, por ejemplo **[!UICONTROL Indiferente (aleatorio)]**.

     Cuando se definen varios atributos, el primero se utiliza como criterio principal de ordenación y los atributos siguientes actúan como desempate, en orden.

1. Marque la opción **Generate complement** para aprovechar la población restante. El complemento está formado por todos los duplicados. A continuación, se añade una transición adicional a la actividad.

## Ejemplo {#deduplication-example}

En el siguiente ejemplo, utilice una actividad de anulación de duplicación para excluir duplicados del destinatario antes de realizar una entrega. Los perfiles duplicados identificados se añaden a una audiencia dedicada que se puede reutilizar si es necesario. Elija la dirección de **correo electrónico** para identificar los duplicados. Mantenga 1 entrada y seleccione el método de deduplicación **Random**.

![Ejemplo de actividad de anulación de duplicación en un flujo de trabajo](../assets/workflow-deduplication-example.png)