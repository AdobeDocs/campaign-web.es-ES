---
audience: end-user
title: Establecer un grupo de control
description: Documentación web de Campaign v8
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 41%

---

# Establecer un grupo de control {#control-group}

Puede utilizar grupos de control para evitar el envío de mensajes a una parte de la audiencia a fin de medir el impacto de sus campañas.

Para ello, cree un grupo de control al definir la audiencia de la entrega. Los perfiles se agregan al grupo de control aleatoriamente, se filtran o no, o se basan en criterios. A continuación, podrá comparar el comportamiento de la población de destinatarios que recibió el mensaje con el comportamiento de los contactos a los que no estaban destinados.

El grupo de control se puede extraer aleatoriamente del objetivo principal o seleccionarse de una población específica. Por lo tanto, hay dos formas principales de definir un grupo de control:

* Extraer varios perfiles del destinatario principal.
* Excluir algunos perfiles según los criterios definidos en una consulta.

Puede utilizar ambos métodos al definir un grupo de control.

Todos los perfiles que formen parte del grupo de control en la fase de preparación del envío se eliminarán del destinatario principal. No recibirán el mensaje una vez que se envíe.

Para crear un grupo de control, haga clic en el botón **[!UICONTROL Establecer grupo de control]** , en el **Audiencia** del asistente de creación de envíos.

![](assets/control-group1.png)

## Extraer a partir del público objetivo {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extraer a partir del público objetivo"
>abstract="TBC"

Para definir un grupo de control, puede elegir extraer, aleatoriamente o en función de un orden, un porcentaje o un número fijo de perfiles de la población de destinatarios.

En primer lugar, defina la forma en que se extraerán los perfiles del destinatario: aleatoriamente o en función de un orden.

En el **Extraer de target** , elija un **Tipo de exclusión**:

* **Aleatorio**: al preparar la entrega, Adobe Campaign extraerá aleatoriamente un número de perfiles correspondiente al porcentaje o al número máximo que se establecerá como límite de tamaño.

   ![](assets/control-group.png)

* **Clasificación por atributos**: esta opción permite excluir un conjunto de perfiles en función de atributos específicos de un orden de clasificación específico.

   ![](assets/control-group2.png)

A continuación, defina la variable **Límite de tamaño**: debe definir cómo va a limitar el número de perfiles que extraiga del destinatario principal.

**Ejemplo**

Puede ver los registros para comprobar e identificar los perfiles excluidos. Veamos el ejemplo de una exclusión aleatoria en cinco perfiles.

![](assets/control-group4.png)

Después de la preparación de la entrega, puede ver las exclusiones en las pantallas siguientes:

* La variable **Para excluir** KPI en el panel de envío, antes del envío.

   ![](assets/control-group5.png)

* La variable **Registros de exclusión** mostrar cada perfil y la ejecución relacionada **Razón**.

   ![](assets/control-group6.png)

* La variable **Causas de exclusión** muestra el número de perfiles ejecutados para cada regla de tipología.

   ![](assets/control-group7.png)

Para obtener más información sobre los registros de envío, consulte esta [sección](../monitor/delivery-logs.md).

## Población adicional {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Población adicional"
>abstract="TBC"

Otra forma de definir un grupo de control es excluir una población específica del objetivo utilizando una audiencia existente o definiendo una consulta.

En el **Población adicional** de la sección **Grupo de control** pantalla de definición, haga clic en el botón **[!UICONTROL Seleccionar audiencia]** botón.

![](assets/control-group3.png)

* Para usar una audiencia existente, haga clic en **Seleccionar la audiencia**. Consulte esta [sección](add-audience.md).

* Para definir una nueva consulta, seleccione **Cree sus propios** y defina los criterios de exclusión mediante el generador de reglas. Consulte esta [sección](segment-builder.md).

Los perfiles incluidos en la audiencia o que coinciden con el resultado de la consulta se excluirán del destinatario.