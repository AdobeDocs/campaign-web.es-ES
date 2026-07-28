---
audience: end-user
title: Añadir una lista editable al esquema de oferta
description: Obtenga información sobre cómo exponer un vínculo de colección personalizado como una lista editable directamente en la pantalla de detalles de la oferta.
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 043cc60da1938800404964aa7e698f959ef908fd
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 1%

---

# Añadir una lista editable al esquema de oferta {#offer-editable-list}

Al [ampliar el  [!DNL nms:offer] esquema](../administration/schemas.md) con un vínculo de colección personalizado, como un conjunto de segmentos vinculados a una oferta, puede exponerlo como una lista editable directamente en la sección **[!UICONTROL Opciones personalizadas]** de la oferta. En lugar de administrar los registros relacionados a través de una pantalla independiente, la colección se procesa como una lista en el detalle de la oferta y puede crear nuevos registros relacionados en línea a través de un cuadro de diálogo dedicado.

>[!NOTE]
>
>Actualmente, esta capacidad solo está disponible para el esquema de oferta.

## Agregar un campo de vínculo de colección {#add-field}

1. Amplíe el esquema [!DNL nms:offer] con su colección personalizada, luego vaya al menú **[!UICONTROL Esquemas]**, abra el esquema **[!UICONTROL Ofertas de marketing]** y haga clic en **[!UICONTROL Edición de pantalla]**. [Más información](../administration/schemas-browse-access.md#screen-def).

   ![Captura de pantalla que muestra el botón de definición de pantalla.](assets/offers-editable-list.png){zoomable="yes"}

1. En la sección **[!UICONTROL Configuración de pantalla detallada]**, haga clic en el icono de puntos suspensivos sobre la tabla **[!UICONTROL Lista de campos personalizados]** y elija **[!UICONTROL Seleccionar atributos]**. [Más información](../administration/schemas-custom-fields.md).

   ![Captura de pantalla que muestra el botón de definición de pantalla.](assets/offers-editable-list-0.png){zoomable="yes"}

1. Examine los atributos y seleccione el vínculo de colección personalizado, identificado por su icono de colección.

   ![Captura de pantalla que muestra el selector de atributos con un atributo de vínculo de colección.](assets/offers-editable-list-1.png){zoomable="yes"}

   >[!NOTE]
   >
   >Los campos de vínculo de recopilación no pueden ser obligatorios y no admiten subatributos. De forma predeterminada, abarcan dos columnas en el formulario.

1. Confirme la selección. El vínculo de colección se agrega a la tabla **[!UICONTROL Lista de campos personalizados]**, con **[!UICONTROL colección]** como tipo.

   ![Captura de pantalla que muestra los atributos agregados.](assets/offers-editable-list-2.png){zoomable="yes"}

## Configurar la lista editable de la colección {#configure-list}

1. Haga clic en el icono de puntos suspensivos en la fila del campo de colección y elija **[!UICONTROL Editar]** para abrir el cuadro de diálogo **[!UICONTROL Configuración del vínculo de colección]**.

   ![Captura de pantalla que muestra el botón de edición.](assets/offers-editable-list-3.png){zoomable="yes"}

1. En la ficha **[!UICONTROL General]**, establezca de forma opcional una condición **[!UICONTROL Visible si]** o habilite **[!UICONTROL Solo lectura]**.

   ![Captura de pantalla que muestra la pantalla de edición.](assets/offers-editable-list-4.png){zoomable="yes"}

1. En la ficha **[!UICONTROL Configuración de pantalla]**, haga clic en **[!UICONTROL Seleccionar atributos]** y seleccione los atributos que desea utilizar al agregar un nuevo elemento a la lista; por ejemplo, un nombre de segmento y un campo personalizado.

   ![Captura de pantalla que muestra la pestaña de configuración de pantalla del cuadro de diálogo de configuración de vínculos de colección.](assets/offers-editable-list-5.png){zoomable="yes"}

1. En la ficha **[!UICONTROL Diseño]**, mantenga o desactive **[!UICONTROL Abarcar dos columnas]**.

1. Haga clic en **[!UICONTROL Confirmar]** y, a continuación, **[!UICONTROL Guardar]** la definición de pantalla.

## Uso de la lista editable en una oferta {#use-list}

1. En el menú de la izquierda, haga clic en **Ofertas** y abra una oferta. [Más información](create-offer.md#create)

   ![Captura de pantalla que muestra la pantalla de la oferta.](assets/offers-editable-list-7.png){zoomable="yes"}

1. Acceda a las propiedades de la oferta. La colección se representa como una lista en la sección **Opciones personalizadas**.

   ![Captura de pantalla que muestra la representación de la lista editable en la pantalla de detalles de la oferta.](assets/offers-editable-list-6.png){zoomable="yes"}

1. Haz clic en **[!UICONTROL Agregar]** para mostrar los atributos que configuraste, rellénalos y haz clic en **[!UICONTROL Confirmar]**. El nuevo elemento se agrega a la lista.

   Se pueden añadir varios elementos a la misma lista y los detalles de la oferta pueden contener más de una lista editable.

1. Haga clic en **[!UICONTROL Save]**.

<!--
Each element added through the editable list creates a new related record. For instance, adding a segment to an offer generates the following payload:

```xml
<offer ...>
  <offerSegment segmentName="..." _operation="insert"/>
</offer>
```
-->