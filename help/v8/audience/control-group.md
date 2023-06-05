---
audience: end-user
title: Establecer un grupo de control
description: Obtenga información sobre cómo establecer un grupo de control para los mensajes en la IU de la web de Campaign
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
badge: label="Alpha" type="Positive"
source-git-commit: 3ebe92659916cf2fa4cacb8d28b79d7b6d5359f3
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 56%

---

# Establecer un grupo de control {#control-group}

Un grupo de control es una subpoblación excluida del envío. Puede definir un grupo de control para evitar enviar mensajes a una parte de la audiencia y comparar el comportamiento tras la entrega con el destinatario principal. Esta opción le ayuda a medir el impacto de su campaña.

Para añadir un grupo de control, active la opción al definir la audiencia del envío. El grupo de control se puede extraer aleatoriamente del objetivo principal o seleccionarse de una población específica. Por lo tanto, hay dos formas principales de definir un grupo de control:

* Extraer varios perfiles de los destinatarios principales.
* Excluir algunos perfiles de una lista o en función de criterios definidos en una consulta.

Puede combinar ambos métodos al definir un grupo de control.

Todos los perfiles del grupo de control en la fase de preparación del envío se eliminan del destinatario principal. No recibirán el mensaje.

>[!CAUTION]
>
>No se pueden utilizar grupos de control al cargar la población objetivo [desde un archivo externo](file-audience.md).

Para añadir un grupo de control a una entrega, active la variable **[!UICONTROL Habilitar grupo de control]** alternar, desde el **Audiencia** de la pantalla de creación de envíos.

![Habilitar opción de grupo de control](assets/control-group1.png)


## Extracción de destinatario {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Modo de extracción"
>abstract="Para definir un grupo de control, puede elegir extraer, aleatoriamente o en función de un orden, un porcentaje o un número fijo de perfiles de la población de destinatarios."


### Creación de un grupo de control {#build-extract-target}

Para definir un grupo de control, puede elegir extraer, aleatoriamente o en función de un orden, un porcentaje o un número fijo de perfiles de la población de destinatarios. Si prefiere agregar una población adicional, elija la opción **Sin extracción** y seleccione la población adicional [como se detalla aquí](#extra-population).

En primer lugar, defina la forma en que se extraen los perfiles del destinatario: aleatoriamente o en función de un orden.

En el **Grupo de control** , elija un **Modo de extracción**:

* **Aleatorio**: al preparar el envío, Adobe Campaign extraerá aleatoriamente un número de perfiles correspondiente al porcentaje o al número máximo que se establecerá como límite de tamaño.

* **Clasificación por atributos**: esta opción permite excluir un conjunto de perfiles en función de los atributos específicos de un orden de clasificación específico.

   ![](assets/control-group2.png)

A continuación, utilice el **Límite de tamaño** para establecer el número de perfiles que debe extraer del destinatario principal. Puede ser un número sin procesar o un porcentaje de la audiencia inicial.

### Comprobación del grupo de control {#check-extract-target}

Puede ver los registros para comprobar e identificar los perfiles excluidos. Veamos el ejemplo de una exclusión aleatoria en cinco perfiles.

![](assets/control-group4.png)

Después de la preparación de la entrega, puede revisar cómo se aplicaron las exclusiones:

* En el panel de envío, antes de realizar el envío, compruebe lo siguiente **Para excluir** KPI.

   ![](assets/control-group5.png)

* En los registros de envío, la pestaña Logs muestra el paso de exclusión.

   ![](assets/control-group-sample-logs.png)


* El **Registros de exclusión** muestra cada perfil y la exclusión relacionada **Motivo**.

   ![](assets/control-group6.png)

* El **Causas de exclusión** pestaña muestra el número de perfiles excluidos para cada regla de tipología.

   ![](assets/control-group7.png)

Para obtener más información sobre los registros de envío, consulte esta [sección](../monitor/delivery-logs.md).

## Adición de una población adicional {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Población adicional"
>abstract="Otra forma de definir un grupo de control es excluir una población específica del destinatario mediante una audiencia existente o definiendo una consulta."

Otra forma de definir un grupo de control es excluir una población específica del destinatario mediante una audiencia existente o definiendo una consulta.

En la sección **Población adicional** de la pantalla de definición **Grupo de control**, haga clic en el botón **[!UICONTROL Seleccionar audiencia]**.

![](assets/control-group3.png)

* Para usar una audiencia existente, haga clic en **Seleccionar audiencia**. Consulte esta [sección](add-audience.md).

* Para definir una nueva consulta, seleccione **Crear su propia consulta** y defina los criterios de exclusión mediante el generador de reglas. Consulte esta [sección](segment-builder.md).

Los perfiles incluidos en la audiencia o que coinciden con el resultado de la consulta se excluyen del destinatario.