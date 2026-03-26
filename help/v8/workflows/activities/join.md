---
audience: end-user
title: Uso de la actividad de flujo de trabajo Unirse
description: Aprenda a utilizar la actividad del flujo de trabajo Unirse
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 20%

---

# Unirse {#join}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Varias ramas de flujo de trabajo y una actividad"
>abstract="Ahora se admiten varias ramas. En lugar de utilizar una bifurcación, puede hacer clic en Agregar rama en la barra de herramientas. También se ha mejorado la actividad AND-join. Ahora es una actividad de unión genérica que le permite elegir entre las opciones de unión AND y OR."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="Actividad AND-join"
>abstract="La actividad **AND-join** le permite sincronizar varias ramas de ejecución de un flujo de trabajo. Se activa una vez que hayan finalizado todas las actividades anteriores. Esto garantiza que determinadas actividades se completen antes de continuar ejecutando el flujo de trabajo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_join"
>title="Unirse a actividad"
>abstract="La actividad **Join** le permite combinar varias transiciones de entrada. Elija si desea continuar cuando se completen todas las transiciones entrantes (Y) o cuando se complete cualquier transición entrante (O)."

La actividad **Join** es una actividad **Flow control**. Sincroniza varias ramas de ejecución de un flujo de trabajo.
Puede elegir cómo se evalúan las transiciones entrantes:

* **AND**: continúa solamente después de que se activen todas las transiciones de entrada seleccionadas.
* **OR**: continúa en cuanto se activa una transición entrante seleccionada.

Cuando se selecciona **AND**, esta actividad almacena en déclencheur su transición saliente solamente después de que se hayan activado todas las transiciones entrantes. En otras palabras, se activa una vez completadas todas las actividades anteriores. Esto garantiza que determinadas actividades hayan finalizado antes de continuar ejecutando el flujo de trabajo.

Cuando se selecciona **OR**, la ejecución continúa en cuanto se activa una de las transiciones de entrada seleccionadas. No espera a cada rama.

## Configuración de la actividad de unión {#join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Combinación de opciones"
>abstract="Seleccione las actividades que desea unir. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante desea conservar."

Siga estos pasos para configurar la actividad **Join**:

1. Añada varias actividades, como actividades de canal, para formar, al menos, dos ramas de ejecución diferentes. Puede usar una **Bifurcación** o agregar una rama separada usando el botón de barra de herramientas **Agregar rama** (+). Consulte [Organizar actividades](../orchestrate-activities.md#toolbar).

   ![Captura de pantalla que muestra dos ramas.](../assets/workflow-join.png)

1. Agregue una actividad **Unirse** a cualquiera de las ramas.

   ![Captura de pantalla que muestra la actividad de unión agregada.](../assets/workflow-join2.png)

1. En las opciones de unión, elige **AND** o **OR** y haz clic en **Continuar**.
1. En la sección **Combinar opciones**, compruebe todas las actividades anteriores a las que desee unirse.
1. En el menú desplegable **Conjunto principal**, elija qué población de transición entrante se debe conservar. La transición saliente solo puede contener una de las poblaciones de transición entrantes.

   >[!NOTE]
   >
   >El campo **Conjunto principal** solo está disponible para la opción de unión **AND**.

   ![Captura de pantalla que muestra la unión configurada.](../assets/workflow-join3.png)

## Ejemplo {#join-example}

El siguiente ejemplo muestra dos ramas de flujo de trabajo con un envío de correo electrónico y SMS. La actividad **Join**, establecida en **AND**, déclencheur cuando ambas transiciones de entrada están habilitadas. Las notificaciones push solo se envían una vez completados ambos envíos. Si establece la opción de unión en **OR**, los mensajes push se enviarán en cuanto se complete la primera actividad de entrega entrante.

![Ejemplo de un flujo de trabajo con dos ramas, que muestra el envío de correo electrónico y SMS seguido de notificaciones push.](../assets/workflow-join4.png){zoomable="yes"}