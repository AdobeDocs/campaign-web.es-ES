---
audience: end-user
title: Uso de la actividad de flujo de trabajo Enrichment
description: Aprenda a utilizar la actividad del flujo de trabajo Enriquecimiento
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 96%

---


# Enriquecimiento {#enrichment}

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

