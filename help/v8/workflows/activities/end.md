---
audience: end-user
title: Uso de la actividad End workflow
description: Descubra más información sobre cómo utilizar la actividad End workflow
source-git-commit: a9c701b9c3ac2d16d8a2dda8e851f09ac801a13e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 54%

---

# Finalizar {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Actividad final"
>abstract="La actividad **Finalizar** le permite marcar de forma gráfica el final de un flujo de trabajo. Cuando haya más de una transición entrante disponible, utilice la sección **Conjuntos que unir** para seleccionar qué transiciones conectar a la actividad."

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="Conjuntos que unir"
>abstract="Compruebe las actividades anteriores que desea conectar como transiciones entrantes de la actividad de **Finalización**. Las actividades seleccionadas se conectan entonces a **Finalización**. Esta sección solo se muestra cuando hay más de una transición entrante disponible para conectar a la actividad."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="Señal externa"
>abstract="marcador para la sección de señal externa en los parámetros de la actividad de finalización. Disponible solo para campañas orquestadas. NO ELIMINAR"

La actividad **End** es una actividad **Flow control**. Permite marcar de forma gráfica el final de un flujo de trabajo. Esta actividad es opcional.

La actividad admite varias transiciones de entrada cuando hay más de una transición de entrada disponible.

En la sección **Conjuntos para unirse**, compruebe las actividades anteriores que desea conectar como transiciones entrantes de la actividad **End**. Las actividades seleccionadas se enlazan a continuación con **End** en el lienzo del flujo de trabajo.

![Proceso de configuración de anulación de duplicación del flujo de trabajo](../assets/workflow-end.png)
