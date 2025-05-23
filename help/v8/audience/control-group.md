---
audience: end-user
title: Establecer un grupo de control
description: Obtenga información sobre cómo establecer un grupo de control para los mensajes en la interfaz de usuario web de Campaign
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 22%

---

# Establecer un grupo de control {#control-group}

Un grupo de control es una subpoblación excluida del envío. Puede definir un grupo de control para evitar enviar mensajes a una parte de la audiencia y comparar el comportamiento tras la entrega con el destinatario principal. Esta opción ayuda a medir el impacto de la campaña.

➡️ [Descubra esta funcionalidad en vídeo](create-audience.md#video)

## Habilitar grupo de control {#add-a-control-group}

Para añadir un grupo de control, active la opción al definir la audiencia del envío. El grupo de control se puede extraer aleatoriamente del objetivo principal o seleccionarse de una población específica. Por lo tanto, hay dos formas principales de definir un grupo de control:

* Extraer varios perfiles de los destinatarios principales.
* Excluir algunos perfiles de una lista o en función de criterios definidos en una consulta.

Puede combinar ambos métodos al definir un grupo de control.

Todos los perfiles incluidos en el grupo de control en la fase de preparación del envío se eliminan del destinatario principal. No recibirán el mensaje.

>[!CAUTION]
>
>No se pueden utilizar grupos de control al cargar la población de público destinatario [desde un archivo externo](file-audience.md).

Para agregar un grupo de control a un envío, active la opción **[!UICONTROL Habilitar grupo de control]** de la sección **Audiencia** de la pantalla de creación de envíos.

![Activar opción de grupo de control en la pantalla de creación de envíos](assets/control-group1.png)

## Extracción de destinatario {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Modo de extracción"
>abstract="Un grupo de control es un conjunto de perfiles excluidos del envío. Para definir un grupo de control, puede elegir extraer, aleatoriamente o en función de un orden, un porcentaje o un número fijo de perfiles de la población de destinatarios."

### Creación de un grupo de control {#build-extract-target}

Para definir un grupo de control, elija extraer, aleatoriamente o en función de un orden, un porcentaje o un número fijo de perfiles de la población de destinatarios. Si agrega una población adicional, elija la opción **Sin extracción** y seleccione la población adicional [tal como se detalla aquí](#extra-population).

En primer lugar, defina cómo se extraen los perfiles del destinatario: aleatoriamente o en función de un orden.

En la sección **Grupo de control**, elija un **modo de extracción**:

* **Aleatorio**: Al preparar el envío, Adobe Campaign extrae aleatoriamente un número de perfiles correspondiente al porcentaje o al número máximo establecido como límite de tamaño.
* **Clasificado por atributo(s)**: Esta opción excluye un conjunto de perfiles basados en atributos específicos en un orden de clasificación específico.

A continuación, utilice la sección **Límite de tamaño** para establecer el número de perfiles que se extraerán del destinatario principal. Puede ser un número sin procesar (por ejemplo, 50 perfiles que excluir) o un porcentaje de la audiencia inicial (por ejemplo, el 5 % del destinatario principal).

### Muestra del grupo de control {#control-group-sample}

Por ejemplo, para crear un grupo de control con los 100 perfiles más nuevos, siga estos pasos:

1. Seleccione el campo **Age** como criterio de ordenación. Deje la opción de ordenación **Ascendente**.
1. Agregue el campo **Fecha de creación**. Cambie a la opción de orden **Descending**.
1. Defina 100 como el umbral en la sección **Límite de tamaño**.

   ![Configuración del grupo de control para perfiles más jóvenes](assets/control-group2.png){zoomable="yes"}

Estos 100 perfiles más jóvenes se excluyen del destinatario principal.

### Comprobación del grupo de control {#check-control-group}

Vea los registros para comprobar e identificar los perfiles excluidos. Por ejemplo, considere una exclusión aleatoria de cinco perfiles.

![Ejemplo de perfiles excluidos en registros](assets/control-group4.png){zoomable="yes"}

Después de la preparación del envío, revise cómo se aplicaron las exclusiones:

* En el panel de envío, antes de realizar el envío, compruebe el KPI **Para excluir**.

  ![Panel de envío que muestra el KPI &quot;Para excluir&quot;](assets/control-group5.png){zoomable="yes"}

* En los registros de envío, la pestaña Logs muestra el paso de exclusión.

  ![Registros de envío que muestran el paso de exclusión](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* La pestaña **Causas de exclusión** muestra el número de perfiles excluidos para cada regla de tipología.

  ![La exclusión provoca que la pestaña muestre las exclusiones de reglas de tipología](assets/control-group7.png){zoomable="yes"}

Para obtener más información sobre los registros de envío, consulte esta [sección](../monitor/delivery-logs.md).

## Añadir una población adicional {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Población adicional"
>abstract="Un grupo de control es un conjunto de perfiles excluidos del envío. Puede excluir una población específica del público de envío seleccionando un público existente o definiendo una consulta."

Otra forma de definir un grupo de control es seleccionar una población específica en una audiencia existente o definir una consulta.

En la sección **Población adicional** de la pantalla de definición **Grupo de control**, haga clic en el botón **[!UICONTROL Seleccionar público]**.

![Pantalla de selección de población adicional](assets/control-group3.png){zoomable="yes"}

* Para usar un público existente, haga clic en **Seleccionar público**. Obtenga más información en [esta sección](add-audience.md).
* Para definir una nueva consulta, seleccione **Crear la suya** y defina los criterios de exclusión con el modelador de consultas. Obtenga más información en [esta sección](../query/query-modeler-overview.md).

Los perfiles incluidos en la audiencia o que coinciden con el resultado de la consulta se **excluyen** del destino de entrega. No reciben ningún mensaje.

## Comparar los resultados {#control-group-results}

Una vez entregado el envío, extraiga los registros de envío para comparar el comportamiento entre los perfiles que no recibieron la comunicación y el destinatario efectivo. Utilice los registros de envío para crear un nuevo objetivo.

Para ver qué perfiles se eliminaron del destino, consulte **Registros de envío**. Obtenga más información [en esta sección](#check-control-group).