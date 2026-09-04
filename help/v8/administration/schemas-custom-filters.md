---
title: Añadir filtros personalizados
description: Obtenga información sobre cómo agregar filtros personalizados como campos de acceso rápido en el panel de filtros de una vista de lista.
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 3%

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

1. Haga clic en **[!UICONTROL Save]**. Puede reordenar los filtros personalizados con las flechas arriba y abajo o arrastrándolos. Para quitar un filtro, haga clic en el icono de puntos suspensivos de su fila y seleccione **[!UICONTROL Eliminar]**.

1. Busque la lista de registros de este esquema y abra el panel Filtros. Los atributos que seleccionó se muestran como **[!UICONTROL Filtros personalizados]**, encima del generador de reglas **[!UICONTROL Filtros avanzados]**.

   ![Filtros personalizados mostrados en el panel de filtros](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >Un filtro personalizado basado en un atributo de fecha y hora se muestra como selector de intervalo de fechas.

1. Introduzca o seleccione un valor en uno de los filtros personalizados para restringir la lista.

## Restringir valores para un filtro personalizado de tipo vínculo {#settings}

Para un filtro personalizado basado en un atributo de vínculo, puede restringir qué valores están disponibles en el selector.

>[!NOTE]
>
>La opción **[!UICONTROL Edit]** descrita a continuación solo está disponible para filtros personalizados basados en un atributo de vínculo. Los filtros personalizados basados en otros tipos de atributos solo se pueden reordenar o eliminar.

1. En la fila de un filtro personalizado de tipo vínculo, haga clic en el icono de puntos suspensivos y seleccione **[!UICONTROL Editar]**.

   ![Editar opción en un filtro personalizado de tipo vínculo](assets/schemas-custom-filters4.png)

1. En la ficha **[!UICONTROL Configuración del filtro]**, haga clic en **[!UICONTROL Editar filtro]** y use el modelador de consultas para definir una condición que restrinja los valores disponibles en el selector. Por ejemplo, restrinja un filtro de envío a las entregas que utilizan el canal de correo electrónico.

   ![Ficha Configuración de filtro en el cuadro de diálogo Configuración de vínculo](assets/schemas-custom-filters5.png)

1. Confirme los cambios.
