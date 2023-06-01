---
audience: end-user
title: Trabajo con flujos de trabajo y actividades
description: Descubra más información sobre las actividades de flujo de trabajo
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 3bbdd45571d09258bba34e22de39f5281c02d248
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 8%

---


# Acerca de las actividades de flujo de trabajo {#workflow-activities}

Las actividades de flujo de trabajo se agrupan en tres categorías. Según el contexto, las actividades disponibles pueden diferir.

Todas las actividades se detallan en las secciones siguientes:

* [Actividades de segmentación](#targeting)
* [Actividades de canal](#channel)
* [Actividades de control de flujo](#flow-control)

![](../assets/workflow-activities.png)

## Actividades de segmentación {#targeting}

Estas actividades son específicas para dirigir, manipular y enriquecer los datos de población. Permiten crear uno o más objetivos definiendo una audiencia y dividiendo o combinando estas audiencias mediante operaciones de intersección, unión o exclusión.

* El [Crear audiencia](build-audience.md) La actividad de le permite definir la población objetivo. Puede seleccionar una audiencia existente o utilizar el generador de reglas para definir su propia consulta.
* El [Combinar](combine.md) La actividad de permite realizar la segmentación en la población entrante. Puede utilizar una unión, una intersección o una exclusión.
* El [Enriquecimiento](enrichment.md) La actividad de le permite definir datos adicionales para procesarlos en el flujo de trabajo. Con esta actividad, puede aprovechar la transición entrante y configurar la actividad para completar la transición de salida con datos adicionales.

## Actividades de canal {#channel}

Adobe Campaign Web le permite automatizar y ejecutar campañas de marketing en varios canales, como correo electrónico, SMS o push. Con los flujos de trabajo de Adobe Campaign, puede combinar actividades de canal en el lienzo para crear flujos de trabajo entre canales que puedan almacenar en déclencheur acciones basadas en el comportamiento del cliente.

Por ejemplo, puede crear una campaña de correo electrónico de bienvenida que incluya una serie de mensajes en diferentes canales, como correo electrónico, SMS y push. También puede enviar un correo electrónico de seguimiento después de que un cliente haya completado una compra o enviar un mensaje de cumpleaños personalizado a un cliente a través de SMS.

Mediante las actividades de canal, puede crear campañas completas y personalizadas que atraigan a los clientes en varios puntos de contacto e impulsen las conversiones.

* [Correo electrónico](email.md)
* [Push](push.md)
* [SMS](sms.md)

## Actividades de control de flujo {#flow-control}

Las siguientes actividades son específicas para organizar y ejecutar flujos de trabajo. Su tarea principal es coordinar las demás actividades:

* El [And-join](and-join.md) Esta actividad permite sincronizar varias ramas de ejecución de un flujo de trabajo.
* El [Fin](end.md) Esta actividad le permite marcar de forma gráfica el final de un flujo de trabajo. Estas actividades no tienen impacto funcional y, por lo tanto, son opcionales.
* El [Tenedor](fork.md) La actividad de le permite crear transiciones salientes para el inicio de varias actividades al mismo tiempo.
* El [Esperar](wait.md) la actividad suspende momentáneamente la ejecución de una parte de un flujo de trabajo.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

