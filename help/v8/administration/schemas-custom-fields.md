---
title: Editar campos personalizados
description: Obtenga información sobre cómo configurar campos personalizados y su visibilidad en la interfaz.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 5%

---

# Editar campos personalizados {#fields}

Los campos personalizados son atributos adicionales añadidos a los esquemas predeterminados a través de la consola de Adobe Campaign. Permiten personalizar esquemas incluyendo nuevos atributos para adaptarlos a las necesidades de la organización.

Los campos personalizados se pueden mostrar en varias pantallas, como los detalles de perfil en la interfaz. Puede controlar qué campos son visibles y cómo aparecen en la interfaz.

Para obtener más información sobre la pantalla de definición de pantalla y cómo acceder a ella, consulte la sección [Acceder a la definición de pantalla](schemas-browse-access.md#screen-def).

Para agregar campos personalizados a la lista:

1. Vaya al menú **[!UICONTROL Esquemas]** y busque esquemas editables mediante los filtros.

1. Seleccione el nombre del esquema en la lista para abrirlo y haga clic en el botón **[!UICONTROL Screen edition]** de la vista de detalles del esquema para acceder a la definición de pantalla.

1. Haga clic en el icono de puntos suspensivos sobre la tabla **[!UICONTROL Lista de campos personalizados]** y elija **[!UICONTROL Seleccionar atributos]** para seleccionar uno o varios campos personalizados que se mostrarán en la interfaz.
   ![Pantalla de campos personalizados que muestra atributos editables](assets/schemas-custom5.png)
1. Seleccione los campos personalizados que desee añadir y confirmar.

   ![Pantalla de campos personalizados que muestra atributos editables](assets/schemas-custom2.png)

   >[!NOTE]
   >
   > También puede seleccionar **[!UICONTROL Rellenar automáticamente la lista de campos personalizados]** para agregar todos los campos personalizados definidos para el esquema a la interfaz.

Una vez añadidos los campos personalizados, se puede obtener una vista previa de ellos, reordenarlos, hacerlos obligatorios, editar su configuración u organizarlos en subsecciones.

## Configurar ajustes de campo {#field-settings}

Para establecer una configuración específica para cada campo personalizado, haga clic en el icono de puntos suspensivos de una fila de campo en la lista y seleccione **[!UICONTROL Editar]**.

![Cuadro de diálogo Configuración de atributos](assets/schemas-attribute-settings.png)

Los ajustes disponibles son:

* **[!UICONTROL Atributo]**: Nombre del campo personalizado (solo lectura).
* **[!UICONTROL Etiqueta (personalizada)]**: La etiqueta que se mostrará en la interfaz. Si no se proporciona ninguna etiqueta, se mostrará la etiqueta definida en el esquema.
* **[!UICONTROL Visible si]**: defina una condición con una expresión xtk que controle cuándo se muestra el campo. Por ejemplo, oculte este campo si hay otro campo vacío.
* **[!UICONTROL Obligatorio]**: haga que el campo sea obligatorio en la interfaz.
* **[!UICONTROL Solo lectura]**: convierta el campo en de solo lectura en la interfaz. Los usuarios no podrán editar el valor del campo.
* **[!UICONTROL Configuración del filtro]** (para campos de tipo de vínculo): use el modelador de consultas para especificar reglas para mostrar un campo personalizado de tipo de vínculo. Por ejemplo, restrinja los valores de lista en función de la entrada de otro campo.

  +++Ver ejemplo

  También puede hacer referencia al valor introducido en otros campos de las condiciones mediante la sintaxis `$(<field-name>)`. Esto le permite hacer referencia al valor actual de un campo tal como se introduce en el formulario, aunque aún no se haya guardado en la base de datos.

  En el ejemplo siguiente, la condición comprueba si el valor del campo @ref coincide con el valor introducido en el campo @refCom. Por el contrario, si se usa `@refCom` en lugar de `$(@refCom)`, se hará referencia al valor del campo @ref tal como existe en la base de datos.

  ![Captura de pantalla que muestra un ejemplo de configuración de filtro para campos personalizados](assets/custom-fields-ref.png)

  +++

* **[!UICONTROL Abarcar dos columnas]**: de forma predeterminada, los campos personalizados se muestran en la interfaz en dos columnas. Active esta opción para mostrar el campo personalizado en todo el ancho de la pantalla en lugar de en dos columnas.

## Previsualizar campos personalizados {#preview}

Haga clic en **[!UICONTROL Vista previa]** para mostrar los campos personalizados en una pantalla de muestra. Esto le permite ver cómo aparecen los campos en la interfaz, incluidos los campos marcados como obligatorios.

![Vista previa de campos personalizados](assets/schemas-custom4.png)

## Organización de campos en subsecciones {#separator}

Puede añadir separadores para agrupar campos personalizados en la interfaz para mejorar la legibilidad. Para ello, siga estos pasos:

1. Haga clic en el icono de puntos suspensivos sobre la tabla **[!UICONTROL Lista de campos personalizados]** y elija **[!UICONTROL Agregar separador]**.

1. Se agrega a la lista una nueva línea que representa el separador. Haga clic en el icono de puntos suspensivos en la fila de separación y elija **[!UICONTROL Editar]**.

1. Escriba una **[!UICONTROL Etiqueta]** para el separador y (opcional) establezca una condición **[!UICONTROL Visible si]** para controlar cuándo se muestra el separador.

   ![Cuadro de diálogo de propiedades del separador](assets/schemas-custom3.png)

1. Utilice las flechas arriba y abajo para mover el separador a la ubicación deseada. Los campos enumerados debajo del separador se agrupan debajo de él.

   En este ejemplo, los campos &quot;Colecciones interesadas&quot; y &quot;Marca&quot; se agrupan en una subsección &quot;Colección&quot;.

   | Configuración de campos personalizados | Procesamiento en la interfaz |
   |  ---  |  ---  |
   | ![Captura de pantalla que muestra la configuración de un separador](assets/custom-fields-separator.png){zoomable="yes"} | ![Captura de pantalla que muestra el procesamiento de una subsección en la interfaz](assets/custom-fields-section.png){zoomable="yes"} |
