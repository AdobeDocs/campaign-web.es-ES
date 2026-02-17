---
title: Trabajar con formularios personalizados
description: Aprenda a crear, editar y administrar registros en esquemas personalizados mediante formularios de entrada de datos.
source-git-commit: be4876090ecaac853aaa88948505c444bef27ec2
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Trabajar con formularios personalizados {#custom-forms}

Los formularios personalizados son interfaces de entrada de datos que permiten administrar registros en esquemas personalizados directamente desde la interfaz de usuario web. Cada formulario personalizado corresponde a un esquema personalizado específico y proporciona una vista de lista para examinar los registros y una vista de detalles para crear, editar y eliminar registros.

Los formularios personalizados se basan en la definición de formulario (definición de pantalla) del esquema, que configura qué campos se muestran y cómo están organizados.

>[!NOTE]
>
>Los formularios personalizados solo están disponibles para esquemas que tienen una definición de formulario configurada.

## Creación y publicación de esquemas personalizados {#form-schema}

Primero debe crear y publicar los esquemas personalizados. Para obtener instrucciones detalladas, consulte esta [sección](schemas-create-publish.md).

Este es el modelo de datos utilizado para este ejemplo:

* Un destinatario realiza varias compras
* Una compra está vinculada a un producto
* Un producto está vinculado a una marca

Para este caso de uso, se crean tres esquemas: los esquemas Purchases, Products y Brand. Este es un ejemplo.

![Formularios personalizados](assets/schemas-forms.png)

## Configuración de la definición de pantalla {#form-screen-schema}

Defina qué campos se muestran y cómo están organizados. Para obtener instrucciones detalladas, consulte esta [sección](schemas-browse-access.md#screen-def).

Este es un ejemplo para el esquema de marca en el que se agrega la lista personalizada Productos. A continuación, el formulario muestra la lista de productos vinculados a la marca.

![Formularios personalizados](assets/schemas-forms2.png)

Para el esquema Products, agregamos la lista personalizada Purchases. Y para el esquema Purchases, los campos Product y Recipient.

## Crear entradas de navegación {#form-screen-entries}

Cree carpetas en el Explorador para acceder a su formulario personalizado. Para obtener instrucciones detalladas, consulte esta [sección](schemas-create-publish.md#navigation).

![Formularios personalizados](assets/schemas-forms3.png)

La vista de lista muestra todos los registros de ese esquema. Si el esquema tiene configurada una definición de formulario, la lista se puede editar y puede crear, editar y eliminar registros.
![Formularios personalizados](assets/schemas-forms4.png)

A continuación, puede:

* **Ver y editar registros**: haga clic en un registro de la vista de lista para abrirlo en la vista de detalles y editar los campos directamente.
* **Crear registros nuevos**: haga clic en el botón **[!UICONTROL Crear]** y rellene los campos obligatorios. Para los campos vinculados, utilice el icono de búsqueda para seleccionar entre los registros relacionados disponibles.
* **Eliminar registros**: seleccione un registro y utilice la acción de eliminación disponible en los detalles del registro o en la vista de lista.
* **Ver datos relacionados en las fichas**: acceda a los registros relacionados a través de fichas dedicadas en la vista de detalles (por ejemplo, ver todos los productos vinculados a una marca o todas las compras vinculadas a un producto).
* **Aplicar filtros**: utilice el panel de filtro para restringir la vista de lista y buscar registros específicos basados en cualquier campo del esquema.
* **Personalizar columnas de lista**: configure qué columnas se muestran de forma predeterminada en las vistas de lista a través de la definición de pantalla.
