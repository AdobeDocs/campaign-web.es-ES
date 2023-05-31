---
audience: end-user
title: Trabajo con flujos de trabajo y actividades
description: Descubra más información sobre las actividades de flujo de trabajo
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 38db8be3319c348d3afc6af02a65dce582e3cc97
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 52%

---


# Actividades de flujo de trabajo {#workflow-activities}

## Actividades de segmentación {#targeting}

Estas actividades permiten crear uno o más objetivos definiendo conjuntos y dividiendo o combinando estos conjuntos mediante operaciones de intersección, unión o exclusión.

### Generar público destinatario {#build-audience}

Esta actividad le permite definir una audiencia. Puede seleccionar una audiencia de Campaign existente o utilizar el generador de reglas para definir su propia consulta.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

Para crear su propia consulta:

1. Seleccionar **Cree su propio (consulta)**.
1. Elija la **Dimensión de segmentación**. La dimensión de segmentación permite definir la población objetivo de la operación: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. De forma predeterminada, el objetivo se selecciona en los destinatarios. Consulte la [Documentación de v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Haga clic en **Continue**.
1. Utilice el generador de reglas para definir la consulta, del mismo modo que crea una audiencia al diseñar un nuevo correo electrónico. Consulte esta [sección](../audience/segment-builder.md).

Para seleccionar una audiencia existente,

1. Seleccionar **Leer audiencia**.
1. Haga clic en **Continue**.
1. Seleccione la audiencia, del mismo modo que utiliza una audiencia cuando diseña un nuevo correo electrónico. Consulte esta [sección](../audience/add-audience.md).

### Combinar {#combine}

Esta actividad le permite procesar conjuntos de datos entrantes. Por lo tanto, puede combinar varias poblaciones, excluir parte de ellas o solo mantener datos comunes para varios objetivos. Estos son los tipos de segmentación disponibles:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* El **Union** permite agrupar el resultado de varias actividades en un solo destino.
* El **Intersección** permite mantener solo los elementos comunes a las diferentes poblaciones de entrada de la actividad.
* El **Exclusión** permite excluir elementos de una población según determinados criterios.

Siga estos pasos para configurar el **Combinar** actividad:

1. Añada su **Combinar** actividad a cualquiera de las transiciones de segmentación anteriores.
1. Seleccione el tipo de segmentación: unión, intersección o exclusión.
1. Haga clic en **Continue**.
1. En el **Configura para unirse** , compruebe todas las actividades anteriores a las que desee unirse.

Para el **Union**, siga estos pasos:

1. Seleccione el Tipo de reconciliación para definir cómo se gestionan los duplicados:
   * Keys only: este es el modo predeterminado. La actividad solo mantiene un elemento cuando los elementos de las distintas transiciones de entrada tienen la misma clave. Puede usar esta opción solo si las poblaciones entrantes son homogéneas.
   * A selection of columns: seleccione esta opción para definir la lista de columnas a las que desea aplicar la reconciliación de datos. Primero debe seleccionar el conjunto principal (el que contiene los datos de origen) y luego las columnas que se utilizarán para la unión.

Para el **Intersección** siga estos pasos:

1. Seleccione el Tipo de reconciliación para definir cómo se gestionan los duplicados. Consulte la **Union** sección anterior.
1. Marque la opción Generate completement.

Para el **Exclusión**, siga estos pasos:

1. En el **Configura para unirse** , seleccione la **Conjunto principal** de las transiciones de entrada. Es el conjunto desde el que se excluyen los elementos. Los demás conjuntos coinciden con elementos antes de excluirse del conjunto principal.
1. Marque la opción Generate completement.












Intersection: permite mantener solo los elementos comunes a las diferentes poblaciones de entrada de la actividad.

Exclusion: permite excluir elementos de una población según determinados criterios.

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

### AND-join {#join}


### Espera {#wait}

### Fin {#end}

## Actividades de administración de datos {#data-management}

Información general: para qué se utilizan, 
qué caso de uso puede realizar con ellos

lista de actividades disponibles, descripción breve y referencia a la sección

