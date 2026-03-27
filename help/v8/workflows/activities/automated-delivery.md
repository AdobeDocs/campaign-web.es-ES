---
audience: end-user
title: Actividad del flujo de trabajo Entrega automatizada
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Envío automatizado
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---

# Envío automatizado {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Actividad de envío automatizado"
>abstract="La actividad Flujo de trabajo de envío automatizado ya está disponible en la paleta Flujo de trabajo. Puede utilizarlo para crear o ejecutar acciones de envío (preparar, enviar una prueba, preparar e iniciar, etc.) directamente dentro del flujo de trabajo."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="Actividad de envío automatizado"
>abstract="La actividad **Envío automatizado** se usa para la automatización: cree o reutilice un envío en el flujo de trabajo y, a continuación, elija la acción que desea realizar (preparar, preparar e iniciar, enviar prueba, etc.). Puede seleccionar una entrega explícita existente creada fuera del flujo de trabajo o crear una nueva entrega a partir de una plantilla cada vez que se ejecute la actividad."

La actividad **Envío automatizado** le permite crear, configurar y ejecutar acciones de envío directamente en el flujo de trabajo. Utilícelo cuando desee ejecutar una entrega predefinido en una programación o como parte de un flujo automatizado, o cuando desee generar una nueva entrega a partir de una plantilla cada vez que se ejecute la actividad.

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. -->

Para configurar esta actividad, siga estos pasos:

1. Defina la configuración de envío, [leer más](#delivery-settings)
1. Seleccione la acción que desea realizar, [leer más](#action-to-execute)
1. Configura la transición, [leer más](#transition-to-execute)
1. Defina un script de modificación, [leer más](#script)

## Definición de la configuración de envío {#delivery-settings}

Al configurar la actividad, puede elegir de dónde proviene la entrega. Hay dos opciones disponibles en esta sección:

![Captura de pantalla que muestra el envío automatizado](../assets/automated-delivery.png){zoomable="yes"}

* Seleccione **Envío explícito** cuando desee actuar sobre un envío existente, por ejemplo un envío independiente o un envío creado a partir de una campaña. Elija la entrega con el botón **Seleccionar entrega**. Cada vez que el flujo de trabajo se ejecuta y alcanza esta actividad, actúa en **la misma entrega de**. No se crea ningún nuevo envío por ejecución. La actividad reutiliza el mismo envío. Esto resulta útil cuando tiene una sola entrega que desea preparar o enviar repetidamente, por ejemplo en una programación o después de un paso de aprobación.

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* Seleccione **Nuevo, creado a partir de una plantilla** cuando quiera que se cree un envío **nuevo** cada vez que se ejecute la actividad. Elija la plantilla de envío con el botón **Seleccionar plantilla**. Cada ejecución genera un nuevo envío basado en esa plantilla. Utilícelo cuando cada ejecución del flujo de trabajo deba dar como resultado su propia entrega distinta (por ejemplo, un correo electrónico por ejecución).

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>Las opciones **Especificadas en la transición** y **Calculadas por script**, utilizadas para casos de uso avanzados, solo se pueden configurar en la consola del cliente. Consulte la [documentación de Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}.

## Seleccione la acción que desea realizar {#action-to-execute}

En esta sección, elija qué hace la actividad con el envío. Estas son las opciones disponibles:

![Captura de pantalla que muestra las acciones que se ejecutarán en el envío automatizado](../assets/automated-delivery2.png){zoomable="yes"}

* **Guardar**: crea y guarda el envío sin analizarlo ni enviarlo.
* **Estimar el objetivo**: calcula el objetivo del envío para evaluar su potencial (primera fase del análisis).
* **Prepare**: ejecuta el análisis completo (cálculo del objetivo y preparación de contenido). No se realiza la entrega.
* **Enviar una prueba**: envía una prueba del envío.
* **Preparar e iniciar**: ejecuta el análisis completo (cálculo del objetivo y preparación de contenido) y realiza la entrega.

## Configuración de la transición {#transition-to-execute}

Esta sección le permite elegir si desea generar transiciones después de la actividad. Estas son las opciones disponibles:

![Captura de pantalla que muestra las transiciones en el envío automatizado](../assets/automated-delivery3.png){zoomable="yes"}

* **Generar una transición saliente**: genera una transición saliente cuando finaliza la actividad.
* **Etiqueta de transición**: permite personalizar la etiqueta mostrada en la transición en el lienzo.
* **Errores de proceso**: Agrega una transición adicional para administrar errores.

## Definición de un script de modificación {#script}

Puede utilizar una secuencia de comandos para cambiar el comportamiento de la actividad como, por ejemplo, los parámetros de envío como la etiqueta de actividad. Utilícelo cuando necesite lógica personalizada para esta actividad.

Haga clic en **Crear script** y escriba la lógica de modificación en el editor.

## Temas relacionados {#related}

* [Acerca de las actividades de flujo de trabajo](about-activities.md)
* [Envío continuo](continuous-delivery.md)
* [Actividades de correo electrónico, SMS, push, correo directo](channels.md)
* [Plantillas de envíos](../../msg/delivery-template.md)
