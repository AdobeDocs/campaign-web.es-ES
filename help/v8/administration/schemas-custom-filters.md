---
title: Añadir filtros personalizados
description: Obtenga información sobre cómo agregar filtros personalizados como campos de acceso rápido en el panel de filtros de una vista de lista.
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: c2e627d322937b80cb0bc09e86680757d4867dcd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Añadir filtros personalizados {#custom-filters}

La sección **[!UICONTROL Configuración de lista de inventario]** > **[!UICONTROL Filtros personalizados]** le permite elegir qué atributos se muestran como campos de acceso rápido en el [panel de filtros](../query/filter.md) de la vista de lista de un esquema, encima del generador de reglas **[!UICONTROL Filtros avanzados]**.

Para obtener más información sobre la pantalla de definición de pantalla y cómo acceder a ella, consulte la sección [Acceder a la definición de pantalla](schemas-browse-access.md#screen-def).

## Añadir filtros personalizados {#add}

1. Vaya al menú **[!UICONTROL Esquemas]** y busque esquemas editables mediante los filtros.

1. Seleccione el nombre del esquema en la lista para abrirlo y haga clic en el botón **[!UICONTROL Screen edition]** de la vista de detalles del esquema para acceder a la definición de pantalla.

1. Vaya a la sección **[!UICONTROL Configuración de la lista de inventario]** y haga clic en el icono de puntos suspensivos sobre la tabla **[!UICONTROL Filtros personalizados]**. A continuación, elija **[!UICONTROL Seleccionar atributos]**.

   ![Selección de filtros personalizados](assets/schemas-custom-filters1.png)

1. Seleccione uno o varios atributos y confirme.

   Puede seleccionar:

   * Un atributo directo del esquema; por ejemplo, un código o una categoría.
   * Un atributo de vínculo, por ejemplo una marca vinculada a un producto. En este caso, el filtro utiliza un selector de búsqueda restringido al esquema vinculado.
   * Un subatributo de un vínculo, por ejemplo, el nombre completo de una carpeta vinculada o el correo electrónico de un destinatario vinculado.

   ![Selector de atributos que muestra atributos directos y subatributos de vínculos](assets/schemas-custom-filters2.png)

1. Haga clic en **[!UICONTROL Save]**. Puede reordenar los filtros personalizados con las flechas arriba y abajo o arrastrándolos, y eliminar un filtro con el icono de papelera en su fila.

1. Busque la lista de registros de este esquema y abra el panel Filtros. Los atributos que seleccionó se muestran como **[!UICONTROL Filtros personalizados]**, encima del generador de reglas **[!UICONTROL Filtros avanzados]**.

   ![Filtros personalizados mostrados en el panel de filtros](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >Un filtro personalizado basado en un atributo de fecha y hora se muestra como selector de intervalo de fechas.

1. Introduzca o seleccione un valor en uno de los filtros personalizados para restringir la lista.

<!--
## Configure a custom filter's settings {#settings}

To configure specific settings for a custom filter, click the ellipsis icon on its row and select **[!UICONTROL Edit]**.

![Custom filter settings dialog](assets/schemas-custom-filters5.png)

Available settings are:

* **[!UICONTROL Label (custom)]**: The label to display for this filter. If no label is provided, the attribute's label defined in the schema is used.
* **[!UICONTROL Filter settings]** (for link-type custom filters only): Use the query modeler to specify a condition that restricts the values available in the picker. For example, restrict a delivery filter to deliveries using the email channel.
-->