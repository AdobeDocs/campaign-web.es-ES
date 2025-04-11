---
audience: end-user
title: Uso de la actividad Señal externa
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Señal externa
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

La actividad **Señal externa** es una actividad **Control de flujo**. Permite almacenar en déclencheur la ejecución de un flujo de trabajo desde otro flujo de trabajo o una llamada de API.

>[!NOTE]
>
>En esta página se explican los pasos principales para configurar una actividad **[!UICONTROL Señal externa]** en la interfaz de usuario web de Campaign y almacenarla en déclencheur desde otro flujo de trabajo o una llamada de API. Encontrará información detallada sobre cómo almacenar en déclencheur un flujo de trabajo, prácticas recomendadas y cómo trabajar con las API de Campaign en [Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example).

Siga estos pasos para configurar la actividad **Señal externa** y déclencheur su ejecución:

1. Agregue una actividad **Señal externa** a su flujo de trabajo.

1. Complete la configuración del flujo de trabajo e inicie su ejecución. La actividad **[!UICONTROL Señal externa]** se muestra como &quot;Pendiente&quot; esperando a activarse.

   ![La captura de pantalla muestra la actividad Señal externa en un estado pendiente.](../assets/external-signal-pending.png)

1. Recupere la siguiente información:

   * El nombre interno del **flujo de trabajo**, que se muestra junto a su etiqueta.

     +++Ver ejemplo

     ![La captura de pantalla muestra el nombre interno del flujo de trabajo junto a su etiqueta.](../assets/external-signal-workflow-name.png)

+++

   * **Nombre de la actividad de señal externa**, que se muestra en **[!UICONTROL Opciones de ejecución]** del flujo de trabajo.

     +++Ver ejemplo

     ![La captura de pantalla muestra el nombre de la actividad Señal externa en las Opciones de ejecución.](../assets/external-signal-name.png)

+++

1. Para almacenar en déclencheur el flujo de trabajo, ejecute la función de JavaScript `PostEvent`. Esta función permite pasar variables con los valores que elija y utilizarlas en el flujo de trabajo activado.

   La función `PostEvent` se puede ejecutar desde otro flujo de trabajo o desde una llamada de API.

   * Para almacenar en déclencheur una actividad **[!UICONTROL External signal]** de un flujo de trabajo, ejecute la función PostEvent desde el panel **[!UICONTROL Secuencia de comandos de inicialización]**, al que se puede acceder desde las **[!UICONTROL Opciones de ejecución]** de la actividad. Para la actividad **[!UICONTROL JavaScript code]**, ejecute la función desde el script de la actividad.

     La sintaxis es la siguiente:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Ver ejemplo

   En este ejemplo, se activa la actividad de señal externa &quot;signal1&quot;. Se ha agregado al flujo de trabajo cuyo nombre interno es &quot;WKF12345&quot;. Se pasa una variable denominada &quot;customID&quot; con el valor &quot;123456&quot;.

   ![La captura de pantalla muestra un ejemplo de activación de la actividad Señal externa mediante la función PostEvent.](../assets/external-signal-sample.png)

+++

   * Para almacenar en déclencheur una actividad **[!UICONTROL External signal]** desde una llamada API, siga los pasos detallados en la documentación de la API de Campaign. [Aprenda a utilizar el método `PostEvent` estático](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html?lang=es).