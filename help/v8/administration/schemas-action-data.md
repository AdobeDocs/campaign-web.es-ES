---
title: Controlar las acciones sobre los datos
description: Obtenga información sobre cómo restringir las acciones de creación, edición y eliminación en registros de esquema personalizados.
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 13%
---
# Controlar las acciones sobre los datos {#action-data}

>[!CONTEXTUALHELP]
>id="acw_schema_action_data"
>title="Datos de acciones"
>abstract="Configure las acciones disponibles para las pantallas de detalles y listas del esquema. Habilite **[!UICONTROL Solo lectura]** para establecer la pantalla de detalles como de solo lectura y quitar acciones de la lista. Habilite **[!UICONTROL No permitir eliminación]** para quitar la acción de eliminación de las pantallas de detalles y lista."

La sección **[!UICONTROL Datos de acción]** le permite restringir las acciones disponibles en los registros de un esquema personalizado, independientemente de las [reglas de seguridad](../get-started/work-with-folders.md) configuradas en carpetas individuales. Esta restricción se aplica al nivel de esquema, en todas las carpetas, para cada usuario, incluidos los administradores.

>[!NOTE]
>
>Esta sección solo está disponible para esquemas personalizados.

Para obtener más información sobre la pantalla de definición de pantalla y cómo acceder a ella, consulte la sección [Acceder a la definición de pantalla](schemas-browse-access.md#screen-def).

Para configurar los datos de acción, siga los pasos a continuación:

1. Vaya al menú **[!UICONTROL Esquemas]** y busque esquemas editables mediante los filtros.

1. Seleccione el nombre del esquema en la lista para abrirlo y haga clic en el botón **[!UICONTROL Screen edition]** de la vista de detalles del esquema para acceder a la definición de pantalla.

1. Desplácese hacia abajo hasta la sección **[!UICONTROL Datos de acción]**, en la parte inferior de la definición de pantalla.

   ![Sección de datos de acción en la definición de pantalla](assets/schemas-action-data1.png)

1. Seleccione una o varias de las opciones disponibles:

   * **[!UICONTROL Solo lectura]**: La pantalla de detalles se convierte en de solo lectura para todos los usuarios. No hay ninguna acción de creación, duplicado, actualización o eliminación disponible en la lista, y las acciones de eliminación y duplicado están ocultas en la pantalla de detalles. Seleccionar esta opción es similar a configurar una vista: los usuarios aún pueden abrir registros y reutilizarlos, por ejemplo al segmentar una entrega, pero no pueden modificarlos.

   * **[!UICONTROL No permitir eliminación]**: la acción de eliminación se quita de la pantalla de detalles y de la lista, en todas las carpetas. Otras acciones, como crear, duplicar y actualizar, siguen estando disponibles.

   * **[!UICONTROL No permitir duplicados]**: la acción duplicar se quita de la pantalla de detalles y de la lista, en cada carpeta. Otras acciones, como crear, eliminar y actualizar, siguen estando disponibles.

     >[!NOTE]
     >
     >Habilitar **[!UICONTROL Solo lectura]** también cubre automáticamente la eliminación y la duplicación, por lo que las opciones **[!UICONTROL No permitir eliminación]** y **[!UICONTROL No permitir duplicados]** están deshabilitadas mientras que **[!UICONTROL Solo lectura]** está seleccionado.

1. Haga clic en **[!UICONTROL Save]**.

1. Examine la lista de registros de este esquema para comprobar el resultado.

   En este ejemplo, **[!UICONTROL Solo lectura]** está habilitado: la lista ya no muestra las acciones de duplicar y eliminar.

   ![Representación de solo lectura en la pantalla de la lista](assets/schemas-action-data2.png)

1. Abra un registro para comprobar la pantalla de detalles. Sus campos se muestran sin permitir ninguna edición.

   ![Procesamiento de solo lectura en la pantalla de detalles](assets/schemas-action-data3.png)
