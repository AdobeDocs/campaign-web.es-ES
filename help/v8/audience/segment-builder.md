---
audience: end-user
title: Creación de una audiencia con el generador de reglas de Campaign
description: Aprenda a trabajar con el generador de reglas
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 57%

---

# Trabajar con el generador de reglas {#segment-builder}

El generador de reglas permite definir la población objetivo de la entrega filtrando los datos contenidos en la base de datos. Puede utilizarlo para crear una audiencia a partir de un flujo de trabajo con una actividad **[!UICONTROL Generar audiencia]** o directamente al crear una entrega para crear una audiencia única.

* [Obtenga información sobre cómo crear y guardar una audiencia](create-audience.md)
* [Obtenga información sobre cómo crear una audiencia única para una entrega](one-time-audience.md)

## La paleta

La paleta, situada en la parte izquierda, contiene todos los elementos que se pueden filtrar para crear un público. Puede utilizar la barra de búsqueda para buscar elementos rápidamente. Los mosaicos contenidos en la paleta deben moverse al lienzo central para que se puedan configurar y tener en cuenta.

![](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

La paleta se divide en dos pestañas:

* **Atributos**: esta pestaña permite acceder a todos los campos disponibles del esquema. La lista de campos depende del esquema de segmentación definido en la plantilla de correo electrónico.

* **Audiencias**: esta pestaña le permite filtrar con una de las audiencias existentes definidas en la consola de Campaign Classic o desde Adobe Experience Platform. Aprenda a monitorizar y administrar las audiencias en [esta sección](manage-audience.md)

  >[!NOTE]
  >
  >Para aprovechar los públicos de Adobe Experience Platform, debe configurar la integración con Destinos. Consulte la [documentación de destinos de Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=es){target="_blank"}.

## El lienzo

El lienzo es la zona central en la que se pueden configurar y combinar las reglas basadas en los elementos agregados desde la paleta. Para agregar una regla nueva, arrastre un mosaico desde la paleta y suéltelo en el lienzo. A continuación, se le pueden presentar opciones específicas del contexto según el tipo de datos que se agreguen.

![](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## El panel Propiedades de regla

A la derecha, el panel **Propiedades de regla** le permite realizar las acciones que se indican a continuación.

![](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **Ver resultados:** muestra la lista de perfiles dirigidos por la audiencia.
* **Vista de código**: muestra una versión del público basada en código en SQL.
* **Mostrar atributos avanzados**: marque esta opción si desea ver la lista completa de atributos de la paleta izquierda: nodos, agrupaciones, vínculos 1-1, vínculos 1-N.
* **Calcular**: actualiza y muestra el número de perfiles dirigidos por la consulta.
* **Seleccione o guarde el filtro**: use un filtro predefinido para filtrar la consulta o guárdela como un nuevo filtro para su reutilización futura. [Aprenda a trabajar con filtros predefinidos](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >En esa versión del producto, algunos filtros predefinidos no están disponibles en la interfaz de usuario. Puede usarlos de todos modos. [Más información](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Atributos**: muestra una descripción del público creado.

## Ejemplo

En este ejemplo, creamos un público para dirigirlo a todos los clientes que viven en Atlanta o Seattle y que nacieron después de 1980.

1. En la pestaña **Atributos** de la paleta, busque el campo **Fecha de nacimiento**. Arrastre el mosaico y suéltelo en el lienzo.

   ![](assets/segment-builder6.png){zoomable="yes"}

1. En el lienzo, elija el operador **Después** e introduzca la fecha deseada.

   ![](assets/segment-builder7.png){zoomable="yes"}

1. En la paleta, busque el campo **Ciudad** y añádalo al lienzo debajo de la primera regla.

   ![](assets/segment-builder8.png){zoomable="yes"}

1. En el campo de texto, introduzca el nombre de la primera ciudad y, a continuación, pulse Intro.

   ![](assets/segment-builder9.png){zoomable="yes"}

1. Repita esta acción para el segundo nombre de ciudad.

   ![](assets/segment-builder10.png){zoomable="yes"}

1. Haga clic en **Ver resultados** para mostrar la lista y el número de destinatarios que coinciden con la consulta. También puede añadir columnas para visualizar y comprobar los datos. En nuestro ejemplo, agregue la columna **Ciudad** y debería ver Atlanta y Seattle.

   ![](assets/segment-builder11.png){zoomable="yes"}

1. Haga clic en **Confirmar**.