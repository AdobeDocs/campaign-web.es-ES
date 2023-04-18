---
audience: end-user
title: Trabajo con actividades de gestión de datos de flujos de trabajo
description: Aprenda a utilizar las actividades de gestión de datos en los flujos de trabajo web de Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 0b5bfea60b65fd52f397f276e0c31e854adddb7b
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 1%

---

# Actividades de administración de datos {#data-management}

información general: para qué uso puede realizar con ellos

enumerar actividades disponibles + descripción breve + referencia a sección

## Enriquecimiento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enriquecimiento Actividad"
>abstract="La actividad Enrichment permite mejorar los datos de destino con información adicional de la base de datos. Normalmente se utiliza en un flujo de trabajo después de actividades de segmentación.<br/>Una vez añadidos los datos de enriquecimiento al flujo de trabajo, estos se pueden utilizar en las actividades añadidas después de la actividad de enriquecimiento para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades, o para crear campañas y mensajes de marketing personalizados que tengan más probabilidades de resonar con la audiencia de destino."

La actividad Enrichment permite mejorar los datos de destino con información adicional de la base de datos. Normalmente se utiliza en un flujo de trabajo después de actividades de segmentación.

Los datos de enriquecimiento pueden venir de:

* **Desde la misma tabla de trabajo** como el objetivo del flujo de trabajo:

   *Dirija la actividad a un grupo de clientes y añada el campo &quot;Fecha de nacimiento&quot; a la tabla de trabajo actual*

* **De otra tabla de trabajo**:

   *Dirija la actividad a un grupo de clientes y añada los campos &quot;Importe&quot; y &quot;Tipo de producto&quot; procedentes de la tabla &quot;Compra&quot;*.

Una vez añadidos los datos de enriquecimiento al flujo de trabajo, estos se pueden utilizar en las actividades añadidas después de la actividad de enriquecimiento para segmentar a los clientes en grupos distintos según sus comportamientos, preferencias y necesidades, o para crear mensajes de marketing personalizados y campañas que tengan más probabilidades de resonar con la audiencia de destino.

Por ejemplo, puede añadir a la tabla de trabajo del flujo de trabajo información relacionada con las compras de los clientes y utilizar estos datos para personalizar los correos electrónicos con su última compra o la cantidad gastada en estas compras.

Para añadir una actividad Enrichement al flujo de trabajo, siga estos pasos:

1. añadir actividad
1. seleccionar atributo para utilizarlo como datos de enriquecimiento

   botón mostrar campos avanzados, opción i

   nota: atributos de la dimensión de destino

1. Seleccionar cómo se recopilan los datos
1. número de registros que desea recuperar si desea recuperar una colección de varios registros
1. Aplicar filtros y generar regla

   seleccionar un filtro existente guardar el filtro para reutilizar los resultados de vista del filtro visualmente o en la vista de código

1. ordenar registros mediante un atributo

aprovechar los datos de enriquecimiento en campaign

donde podemos usar los datos de enriquecimiento: personalice el correo electrónico, ¿otros casos de uso?
