---
audience: end-user
title: Creación de una audiencia con el generador de reglas de Campaign
description: Aprenda a trabajar con el generador de reglas
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: 95d44fa2c44a346aad3aab1962e84917532cc966
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 95%

---

# Definición de una audiencia con el generador de reglas {#segment-builder}

En esta sección se describe cómo crear una audiencia al diseñar un nuevo correo electrónico. La audiencia creada solo se puede utilizar en este correo electrónico.

El generador de reglas permite definir la población objetivo del mensaje filtrando los datos contenidos en la base de datos. Si desea seleccionar una audiencia existente, consulte esta [sección](add-audience.md).

Para obtener más información sobre el generador de reglas, consulte la [documentación del servicio de segmentación](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html?lang=es).

Para crear una audiencia nueva al diseñar un correo electrónico, siga estos pasos:

1. En la sección **Audiencia** del asistente de creación de envíos, haga clic en el botón **[!UICONTROL Seleccionar la audiencia]**.

   ![](assets/segment-builder0.png)

1. Seleccione **Crear la suya propia**. Se muestra el generador de reglas.

   ![](assets/segment-builder.png)

## La paleta

La paleta, situada en la parte izquierda, contiene todos los elementos que se pueden filtrar para crear una audiencia. Los mosaicos contenidos en la paleta deben moverse al lienzo central para que se puedan configurar y tener en cuenta. La paleta se divide en dos pestañas:

* **Atributos**: esta pestaña permite acceder a todos los campos disponibles del esquema. La lista de campos depende del esquema de segmentación definido en la plantilla de correo electrónico.

  ![](assets/segment-builder2.png){width="70%" align="left"}

* **Audiencias**: esta pestaña le permite filtrar con una de las audiencias existentes definidas en la consola de Campaign Classic o desde Adobe Experience Platform.

  ![](assets/segment-builder3.png){width="70%" align="left"}

  >[!NOTE]
  >
  >Para aprovechar las audiencias de Adobe Experience Platform, debe configurar la integración con Destinos. Consulte la [Documentación de destinos de Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=es){target="_blank"}.

Puede utilizar la barra de búsqueda para encontrar los elementos rápidamente.

## El lienzo

El lienzo es la zona central en la que se pueden configurar y combinar las reglas basadas en los elementos agregados desde la paleta. Para agregar una regla nueva, arrastre un mosaico desde la paleta y suéltelo en el lienzo. A continuación, se le pueden presentar opciones específicas del contexto según el tipo de datos que se agreguen.

![](assets/segment-builder4.png){width="70%" align="left"}

## El panel Propiedades de regla

En el lado derecho, el panel **Propiedades de regla** permite realizar las siguientes acciones:

![](assets/segment-builder5.png){width="70%" align="left"}

* **Ver resultados:** muestra la lista de los destinatarios a quienes se dirige la audiencia.
* **Vista de código**: muestra una versión de la audiencia basada en código en SQL.
* **Mostrar atributos avanzados**: marque esta opción si desea ver la lista completa de atributos de la paleta izquierda: nodos, agrupaciones, vínculos 1-1, vínculos 1-N.
* **Atributos**: muestra una descripción de la audiencia creada.

## Ejemplo

En este ejemplo, creamos una audiencia para dirigirla a todos los clientes que viven en Atlanta o Seattle y que nacieron después de 1980.

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

La audiencia está definida y lista para utilizarse en el correo electrónico.