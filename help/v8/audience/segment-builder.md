---
audience: end-user
title: Creación de una audiencia con el generador de reglas de Campaign
description: Aprenda a trabajar con el generador de reglas
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: 9992ae7007b5af80e927dd96b6fff25840d8c3e1
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 60%

---

# Trabajar con el generador de reglas {#segment-builder}


El generador de reglas permite definir la población objetivo de la entrega filtrando los datos contenidos en la base de datos. Puede utilizarlo para crear una audiencia a partir de un flujo de trabajo mediante una **[!UICONTROL Crear audiencia]** actividad de o directamente al crear una entrega para crear una audiencia única.

* [Obtenga información sobre cómo crear una audiencia](create-audience.md)
* [Obtenga información sobre cómo crear una audiencia única para una entrega](one-time-audience.md)

## La paleta

La paleta, situada en la parte izquierda, contiene todos los elementos que se pueden filtrar para crear un público. Puede utilizar la barra de búsqueda para buscar elementos rápidamente. Los mosaicos contenidos en la paleta deben moverse al lienzo central para que se puedan configurar y tener en cuenta.

![](assets/segment-builder2.png){width="70%" align="left"}

La paleta se divide en dos pestañas:

* **Atributos**: esta pestaña permite acceder a todos los campos disponibles del esquema. La lista de campos depende del esquema de segmentación definido en la plantilla de correo electrónico.

* **Audiencias**: esta pestaña le permite filtrar con una de las audiencias existentes definidas en la consola de Campaign Classic o desde Adobe Experience Platform. [Obtenga información sobre cómo monitorizar y administrar audiencias](manage-audience.md)

  >[!NOTE]
  >
  >Para aprovechar los públicos de Adobe Experience Platform, debe configurar la integración con Destinos. Consulte la [Documentación de destinos de Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=es){target="_blank"}.

## El lienzo

El lienzo es la zona central en la que se pueden configurar y combinar las reglas basadas en los elementos agregados desde la paleta. Para agregar una regla nueva, arrastre un mosaico desde la paleta y suéltelo en el lienzo. A continuación, se le pueden presentar opciones específicas del contexto según el tipo de datos que se agreguen.

![](assets/segment-builder4.png){width="70%" align="left"}

## El panel Propiedades de regla

En el lado derecho, la **Propiedades de regla** le permite realizar las acciones que se indican a continuación.

![](assets/segment-builder5.png){width="70%" align="left"}

* **Ver resultados:** muestra la lista de los destinatarios a quienes se dirige el público.
* **Vista de código**: muestra una versión del público basada en código en SQL.
* **Mostrar atributos avanzados**: marque esta opción si desea ver la lista completa de atributos de la paleta izquierda: nodos, agrupaciones, vínculos 1-1, vínculos 1-N.
* **Calcular**: actualiza y muestra el número de perfiles objetivo por la consulta.
* **Seleccionar o guardar filtro**: utilice un filtro predefinido para filtrar la consulta o guárdela como un nuevo filtro para su reutilización futura. [Aprenda a trabajar con filtros predefinidos](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >En esa versión del producto, algunos filtros predefinidos no están disponibles en la interfaz de usuario. Puede usarlos de todos modos. [Más información](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Atributos**: muestra una descripción del público creado.

## Ejemplo

En este ejemplo, creamos un público para dirigirlo a todos los clientes que viven en Atlanta o Seattle y que nacieron después de 1980.

1. En la pestaña **Atributos** de la paleta, busque el campo **Fecha de nacimiento**. Arrastre el mosaico y suéltelo en el lienzo.

   ![](assets/segment-builder6.png)

1. En el lienzo, elija el operador **Después** e introduzca la fecha deseada.

   ![](assets/segment-builder7.png)

1. En la paleta, busque el campo **Ciudad** y añádalo al lienzo debajo de la primera regla.

   ![](assets/segment-builder8.png)

1. En el campo de texto, introduzca el nombre de la primera ciudad y, a continuación, pulse Intro.

   ![](assets/segment-builder9.png)

1. Repita esta acción para el segundo nombre de ciudad.

   ![](assets/segment-builder10.png)

1. Haga clic en **Ver resultados** para mostrar la lista y el número de destinatarios que coinciden con la consulta. También puede añadir columnas para visualizar y comprobar los datos. En nuestro ejemplo, agregue la columna **Ciudad** y debería ver Atlanta y Seattle.

   ![](assets/segment-builder11.png)

1. Haga clic en **Confirmar**.