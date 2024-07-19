---
audience: end-user
title: Variables de eventos de flujo de trabajo
description: Descubra cómo aprovechar las variables de eventos en los flujos de trabajo.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 16%

---

# Variables de eventos de flujo de trabajo {#event-variables}

Algunas actividades de flujo de trabajo permiten editar scripts en el editor de expresiones para realizar acciones específicas, como recuperar datos procedentes de actividades anteriores, crear condiciones o calcular nombres de archivo basados en variables de evento.

## ¿Qué son las variables de evento? {#scripting}

Los scripts ejecutados en el contexto de un flujo de trabajo tienen acceso a una serie de **objetos** globales adicionales, como el propio flujo de trabajo que se está ejecutando (`ìnstance`), sus diversas tareas (`task`) o los eventos que activaron una tarea determinada (`event`).

A cada tipo de **objeto** se asocia una categoría de **variables** que se pueden aprovechar en el editor de expresiones al editar scripts en actividades como **[!UICONTROL JavaScript code]** o **[!UICONTROL Test]**.

* **Las variables de instancia** (`instance.vars.xxx`) son comparables a las variables globales. Las comparten todas las actividades.
* **Las variables de tarea** (`task.vars.xxx`) son comparables a las variables locales. Solo se utilizan en la tarea actual. Las actividades persistentes utilizan estas variables para conservar datos y, a veces, se utilizan para intercambiar datos entre las diferentes secuencias de comandos de una misma actividad.
* **Las variables de eventos** (`vars.xxx`) permiten el intercambio de datos entre las tareas básicas de un proceso de flujo de trabajo. La tarea que activó la tarea en curso transfiere estas variables. A continuación, se pasan a las siguientes actividades. **Las variables de eventos** son las variables más utilizadas y deben utilizarse con preferencia sobre las variables de instancia.

>[!NOTE]
>
>Encontrará información adicional sobre scripts y los objetos y variables expuestos en Adobe Campaign en la documentación de Campaign v8 (consola de cliente) en [esta sección](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Tenga en cuenta que, aunque este recurso ofrece perspectivas valiosas, pueden existir discrepancias ya que se aplica específicamente a la consola del cliente en lugar de a la interfaz de usuario web de Campaign.

## Aproveche las variables de evento en el editor de expresiones {#expression-editor}

Las variables de evento predefinidas están disponibles para su uso en el panel lateral izquierdo del editor de expresiones. También puede crear otras nuevas inicializando una nueva variable en el código.

![](assets/event-variables.png)

Además de estas variables de evento, también puede aprovechar el menú **[!UICONTROL Condiciones]** del panel izquierdo para generar condiciones y el menú **[!UICONTROL Agregar fecha actual]** para usar funciones relacionadas con el formato de fecha.
