---
audience: end-user
title: Trabajo con actividades de gestión de datos de flujos de trabajo
description: Aprenda a utilizar las actividades de gestión de datos en los flujos de trabajo web de Adobe Campaign
badge: label="Alpha" type="Positive"
source-git-commit: 5efcdf2da104b86bf3ee37ee7162495c2d99fb48
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Actividades de administración de datos {#data-management}

información general: para qué uso puede realizar con ellos

enumerar actividades disponibles + descripción breve + referencia a sección

## Enriquecimiento {#enrichment}

La actividad Enrichment se utiliza comúnmente en un flujo de trabajo después de segmentar las actividades. Permite mejorar los datos de destino con información adicional de la base de datos.

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
