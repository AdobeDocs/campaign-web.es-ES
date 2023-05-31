---
audience: end-user
title: Trabajo con flujos de trabajo y actividades
description: Descubra más información sobre las actividades de flujo de trabajo
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: acc3f2cdc50fc8727a472d427c2f8077775a8744
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 74%

---


# Actividades de flujo de trabajo {#workflow-activities}

## Actividades de segmentación {#targeting}

contenido por determinar

<!--à reformuler-->Estas actividades permiten crear uno o más objetivos definiendo conjuntos y dividiendo o combinando estos conjuntos mediante operaciones de intersección, unión o exclusión.

### Generar público destinatario {#build-audience}

### Combinar {#combine}

## Actividades de canal {#channel}

Adobe Campaign Web le permite automatizar y ejecutar campañas de marketing en varios canales, como correo electrónico, SMS o push. Con los flujos de trabajo de Adobe Campaign, puede combinar actividades de canal en el lienzo para crear flujos de trabajo entre canales que puedan almacenar en déclencheur acciones basadas en el comportamiento del cliente.

Por ejemplo, puede crear una campaña de correo electrónico de bienvenida que incluya una serie de mensajes en diferentes canales, como correo electrónico, SMS y push. También puede enviar un correo electrónico de seguimiento después de que un cliente haya completado una compra o enviar un mensaje de cumpleaños personalizado a un cliente a través de SMS.

Mediante las actividades de canal, puede crear campañas completas y personalizadas que atraigan a los clientes en varios puntos de contacto e impulsen las conversiones.

Las actividades de canal están disponibles en la paleta, en el lado izquierdo de la pantalla, en la sección Canales.

### Correo electrónico {#email}

Descripción, qué caso de uso puede realizar (otras actividades comunes que puede vincular antes o después de la actividad)

Cómo añadir y configurar la actividad

Ejemplo de una actividad configurada dentro de un flujo de trabajo


La actividad Entrega de correo electrónico permite configurar la entrega de un correo electrónico en un flujo de trabajo.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Los destinatarios del correo electrónico se definen antes de la actividad en el mismo flujo de trabajo, a través de una actividad de segmentación de audiencia.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### Notificación push (Android) {#push-android}

### Notificación push (iOS) {#push-ios}

## Actividades de control de flujo {#flow-control}

contenido por determinar

<!--à reformuler-->Estas actividades permiten crear uno o más objetivos definiendo conjuntos y dividiendo o combinando estos conjuntos mediante operaciones de intersección, unión o exclusión.

Las actividades de control de flujo se utilizan para coordinar las actividades de flujo de trabajo.

### Bifurcación {#fork}

### AND-join {#end}


### Espera {#end}

### Fin {#end}

## Actividades de administración de datos {#data-management}

Información general: para qué se utilizan, 
qué caso de uso puede realizar con ellos

lista de actividades disponibles, descripción breve y referencia a la sección

### Enriquecimiento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enriquecimiento Actividad"
>abstract="La actividad de enriquecimiento permite mejorar los datos de destino con información adicional de la base de datos. Normalmente, se utiliza en un flujo de trabajo después de actividades de segmentación.<br/>Una vez añadidos los datos de enriquecimiento al flujo de trabajo, estos se pueden utilizar en las actividades añadidas después de la actividad de enriquecimiento para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades. También para crear campañas y mensajes de marketing personalizados que tengan más probabilidades de resonar con la audiencia de destinatarios."

La actividad de enriquecimiento permite mejorar los datos de destino con información adicional de la base de datos. Normalmente, se utiliza en un flujo de trabajo después de actividades de segmentación.

Los datos de enriquecimiento pueden provenir de los siguientes lugares:

* **La misma tabla de trabajo** como el objetivo del flujo de trabajo:

   *Destine la actividad a un grupo de clientes y añada el campo “Fecha de nacimiento” a la tabla de trabajo actual*

* **De otra tabla de trabajo**:

   *Diríjase a un grupo de clientes y añada los campos “Importe” y “Tipo de producto” procedentes de la tabla “Compra”*.

Una vez añadidos los datos de enriquecimiento al flujo de trabajo, estos se pueden utilizar en las actividades añadidas después de la actividad de enriquecimiento para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades, o para crear mensajes de marketing personalizados y campañas que tengan más probabilidades de resonar con la audiencia de destinatarios.

Por ejemplo, puede añadir a la tabla de trabajo del flujo de trabajo información relacionada con las compras de los clientes y utilizar estos datos para personalizar los correos electrónicos con su última compra o la cantidad gastada en estas compras.

Para añadir una actividad de Enriquecimiento al flujo de trabajo, siga estos pasos:

1. añadir actividad
1. seleccionar atributo para utilizarlo como datos de enriquecimiento

   opción mostrar campos avanzados,
botón i

   Nota: atributos de la dimensión de destinatario

1. Seleccionar cómo se recopilan los datos
1. número de registros si desea recuperar una colección de varios registros
1. Aplicar filtros y generar regla

   seleccionar un filtro existente
guardar el filtro para reutilizarlo
ver resultados del filtro visualmente o en la vista de código

1. ordenar registros mediante un atributo

aprovechar los datos de enriquecimiento en Campaign

Donde podemos usar los datos de enriquecimiento: personalice el correo electrónico, ¿otros casos de uso?
