---
audience: end-user
title: Uso de la actividad del flujo de trabajo División
description: Aprenda a utilizar la actividad del flujo de trabajo División
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
source-git-commit: 6d43966bd8283b62bf457b1a63ce968950b54c26
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 85%

---

# División {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Actividad de división"
>abstract="La actividad **División** permite segmentar las poblaciones entrantes en varios subconjuntos en función de diferentes criterios de selección, como las reglas de filtrado o el tamaño de la población."

La actividad **División** es una actividad **Segmentación** que permite segmentar las poblaciones entrantes en varios subconjuntos en función de diferentes criterios de selección, como reglas de filtrado o tamaño de población.

## Configuración de la actividad División {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segmentos de actividad dividida"
>abstract="Añada todos los subconjuntos que quiera para segmentar la población entrante.<br/></br>Cuando se ejecuta la actividad **División**, la población se segmenta en los diferentes subconjuntos en el orden en el que se añaden a la actividad. Antes de iniciar el flujo de trabajo, asegúrese de haber ordenado los subconjuntos en el orden que mejor se adapte a sus necesidades mediante los botones de flecha."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Filtro de la actividad de división"
>abstract="Para aplicar una condición de filtrado al subconjunto, haga clic en **[!UICONTROL Crear filtro]** y configure la regla de filtrado que desee mediante el modelador de consultas. Por ejemplo, incluya perfiles de la población entrante cuya dirección de correo electrónico existe en la base de datos."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign-web/v8/query-database/query-modeler-overview" text="Trabajar con el modelador de consultas"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Límite de la actividad de división"
>abstract="Para limitar el número de perfiles seleccionados por el subconjunto, active la opción **[!UICONTROL Habilitar límite]** y especifique el número o los porcentajes de la población que desea incluir."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="Ordenación de la actividad de división"
>abstract="Al establecer un límite de población para un subconjunto, puede clasificar los perfiles seleccionados en función de un atributo de perfil específico, en orden ascendente o descendente. Para ello, active la opción **Habilitar ordenación**. Por ejemplo, puede restringir un subconjunto para incluir solo los 50 perfiles con la cantidad de compra más alta."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="Dividir generar complemento"
>abstract="Una vez configurados todos los subconjuntos, puede seleccionar la población restante que no coincide con ninguno de los subconjuntos e incluirlos en una transición saliente adicional. Para ello, active la opción **Generar complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Generar todos los subconjuntos de la misma tabla"
>abstract="Active esta opción para agrupar todos los subconjuntos en una sola transición de salida."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_emptytransition"
>title="Omitir transición vacía"
>abstract="Omitir transición vacía."

Siga estos pasos para configurar la actividad **División**:

1. Añada una actividad **División** al flujo de trabajo.

1. El panel de configuración de actividad se abre con un subconjunto predeterminado. Haga clic en el botón **Añadir segmento** para añadir tantos subconjuntos como desee para segmentar la población entrante.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Si la variable **Split** Cuando se ejecuta la actividad, la población se segmenta en los diferentes subconjuntos en el orden en que se añaden a la actividad. Por ejemplo, si el primer subconjunto recupera el 70 % de la población inicial, el siguiente subconjunto añadido aplicará sus criterios de selección solo al 30 % restante, y así sucesivamente.
   >
   >Antes de iniciar el flujo de trabajo, asegúrese de haber ordenado los subconjuntos en el orden que se adapte a sus necesidades. Para ello, utilice los botones de flecha para cambiar la posición de un subconjunto.

1. Una vez creados los subconjuntos, la actividad muestra de forma predeterminada tantas transiciones de salida como subconjuntos. Se recomienda encarecidamente cambiar la etiqueta de cada subconjunto para identificarlo fácilmente en el lienzo del flujo de trabajo.

1. Configure cómo debe filtrar cada subconjunto la población entrante. Para ello, siga estos pasos:

   1. Abra el subconjunto para mostrar sus propiedades.

   1. Para aplicar una condición de filtrado al subconjunto, haga clic en **[!UICONTROL Crear filtro]** y configure la regla de filtrado que desee mediante el modelador de consultas. Por ejemplo, incluya perfiles de la población entrante cuya dirección de correo electrónico existe en la base de datos. [Aprenda a trabajar con el modelador de consultas](../../query/query-modeler-overview.md)

   1. Para limitar el número de perfiles seleccionados por el subconjunto, active la opción **[!UICONTROL Habilitar límite]** y especifique el número o los porcentajes de la población que desea incluir.

      ![](../assets/workflow-split-subset.png)


      >[!NOTE]
      >
      >Al establecer un límite de población para un subconjunto, puede clasificar los perfiles seleccionados en función de un atributo de perfil específico, en orden ascendente o descendente. Para ello, active la opción **[!UICONTROL Habilitar ordenación]**. Por ejemplo, puede restringir un subconjunto para incluir solo los 50 perfiles con la cantidad de compra más alta.

1. Una vez configurados todos los subconjuntos, puede seleccionar la población restante que no coincide con ninguno de los subconjuntos e incluirlos en una transición saliente adicional. Para ello, active la opción **[!UICONTROL Generar complemento]**.

   ![](../assets/workflow-split-complement.png)

   >[!NOTE]
   >
   >El **[!UICONTROL Generar todos los subconjuntos de la misma tabla]** permite agrupar todos los subconjuntos en una sola transición de salida.

La actividad está configurada. En la ejecución del flujo de trabajo, la población se segmenta en los diferentes subconjuntos, en el orden en que se hayan añadido a la actividad.

## Ejemplo{#split-example}

En el ejemplo siguiente, la actividad **[!UICONTROL División]** se utiliza para segmentar un público en distintos subconjuntos basados en el canal de comunicación que queremos utilizar:

* **Subconjunto 1 &quot;push&quot;**: este subconjunto incluye todos los perfiles que han instalado nuestra aplicación móvil.
* **Subconjunto 2 &quot;sms&quot;**: usuarios de teléfonos móviles: para la población restante que no pertenecía al subconjunto 1, el subconjunto 2 aplica una regla de filtrado para seleccionar perfiles con teléfonos móviles en la base de datos.
* **Transición de complemento**: esta transición captura todos los perfiles restantes que no coinciden con el subconjunto 1 o el subconjunto 2. Específicamente, incluye perfiles que no han instalado la aplicación móvil ni tienen teléfono móvil, como usuarios que no han instalado la aplicación móvil o que carecen de un número de móvil registrado.

![](../assets/workflow-split-example.png)
