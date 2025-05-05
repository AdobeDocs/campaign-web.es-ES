---
audience: end-user
title: Utilizar el actividad de señal externa
description: Aprenda a utilizar la señal externa flujo de trabajo actividad
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 10%

---

# Señal externa {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Señal externa"
>abstract="La actividad de **Señal externa** permite activar la ejecución de un flujo de trabajo desde otro flujo de trabajo o una llamada de API."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Parámetros de señal externa"
>abstract="Parámetros de señal externa"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Activadores finales"
>abstract="Activadores finales"

El **actividad de señal** externa es un **actividad de control** Flujo. Permite activar la ejecución de un flujo de trabajo desde otro flujo de trabajo o una llamada de API.

>[!NOTE]
>
>Este Página explica los pasos principales para configurar un **[!UICONTROL actividad de señal]** externa en Campaign interfaz web del usuario y activarlo desde otro flujo de trabajo o una llamada API. En la documentación[&#128279;](https://experienceleague.adobe.com/es/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example) de Campaign v8 (consola de cliente) encontrará información detallada sobre cómo activar una flujo de trabajo, prácticas recomendadas y cómo trabajar con Campaign API.

Siga estos pasos para configurar el actividad de **señal** externa y activar su ejecución:

1. añadir un actividad de señal **&#x200B;**&#x200B;externa en su flujo de trabajo.

1. Todas las aplicaciones la configuración del flujo de trabajo y inicio su ejecución. La **[!UICONTROL actividad de señal]** externa se muestra como &quot;Pendiente&quot;, a la espera de activarse.

   ![El captura de pantalla muestra el actividad de señal externa en estado pendiente.](../assets/external-signal-pending.png)

1. Recupere la siguiente información:

   * El **nombre** interno del flujo de trabajo, que aparece junto a su etiqueta.

     +++Ejemplo de Ver 

     ![El captura de pantalla muestra el nombre interno del flujo de trabajo junto a su etiqueta.](../assets/external-signal-workflow-name.png)

     +++

   * La **señal externa actividad nombre del anuncio**, que se muestra en las opciones **de ejecución del** flujo de trabajo.

     +++Ejemplo de Ver 

     ![El captura de pantalla muestra el nombre del actividad de señal externa en las opciones de ejecución.](../assets/external-signal-name.png)

     +++

1. Para activar el flujo de trabajo, ejecute la función JavaScript `PostEvent` . Esta función permite pasar variables con los valores de su elección y utilizarlos en el flujo de trabajo activado.

   La `PostEvent` función se puede ejecutar desde otro flujo de trabajo o desde una llamada a API.

   * Para activar un **[!UICONTROL actividad de señal]** externa desde una flujo de trabajo, ejecute la función PostEvent desde el **[!UICONTROL panel Script]** de inicialización, accesible desde las opciones **de ejecución del** actividad. Para el **[!UICONTROL código]** de JavaScript actividad, ejecute la función desde la secuencia de comandos del actividad.

     La sintaxis es la siguiente:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Ejemplo de Ver 

   En este ejemplo, se activa el actividad de señal externa &quot;signal1&quot;. Se ha agregado a la flujo de trabajo cuyo nombre interno es &quot;WKF12345&quot;. Se pasa un variable denominado &quot;customID&quot; con el valor &quot;123456&quot;.

   ![El captura de pantalla muestra un ejemplo de cómo activar el actividad de señal externa mediante la función PostEvent.](../assets/external-signal-sample.png)

   +++

   * Para activar un **[!UICONTROL actividad de señal]** externa desde una llamada API, seguir los pasos detallados en la documentación de la API Campaign. [Aprenda a utilizar el método](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html?lang=es) estático`PostEvent`.