---
audience: end-user
title: Trabajo con actividades de gestión de datos de flujos de trabajo
description: Aprenda a utilizar las actividades de gestión de datos en los flujos de trabajo web de Adobe Campaign
badge: label="Alpha" type="Positive"
source-git-commit: ee418ea42bc4568f2ff1f0fe9080825764fee65d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Actividades de administración de datos {#data-management}

información general: para qué uso puede realizar con ellos

enumerar actividades disponibles + descripción breve + referencia a sección

## Enriquecimiento {#enrichment}

descripción: añada uno o varios datos de enriquecimiento; puede aprovechar para personalizar el caso de uso de las entregas: recupere la última compra o la última suscripción digital y la cantidad total de una compra y personalice un correo electrónico con él

ejemplo de uso del proceso: recupere 4 compras más recientes que sean inferiores a 100$ y personalice un correo electrónico con él
1. añadir actividad
1. seleccionar atributo para utilizarlo como datos de enriquecimiento

   + opción mostrar campos avanzados
   + botón i

   nota: atributos de la dimensión de destino

1. Seleccionar cómo se recopilan los datos
1. número de registros que desea recuperar si desea recuperar una colección de varios registros
1. Aplicar filtros y generar regla

   + seleccionar un filtro existente
   + guardar el filtro para reutilizarlo
   + ver los resultados del filtro visualmente o en la vista de código

1. ordenar registros mediante un atributo

aprovechar los datos de enriquecimiento en campaign

donde podemos usar los datos de enriquecimiento: personalice el correo electrónico, ¿otros casos de uso?
