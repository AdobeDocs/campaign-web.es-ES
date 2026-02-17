---
title: Creación y publicación de esquemas
description: Obtenga información sobre cómo crear, ampliar y publicar esquemas.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Creación y publicación de esquemas {#create-publish}

## Creación y administración de esquemas {#create-schemas}

Puede crear nuevos esquemas, ampliar los esquemas existentes y acceder a bases de datos externas.

### Creación o ampliación de un esquema {#create-new}

Para crear o ampliar un esquema:

1. Vaya a **[!UICONTROL Administración]** > **[!UICONTROL Esquemas]**.
1. Haga clic en **[!UICONTROL Crear esquema]**.

   ![Cuadro de diálogo de creación de esquemas](assets/schemas-create1.png)

1. Escriba un área de nombres para el esquema (por ejemplo, `cus` para esquemas personalizados).
1. Introduzca un nombre y una etiqueta únicos y elija si desea crear un nuevo esquema o ampliar uno existente.

1. Haga clic en **[!UICONTROL Crear]**.
   ![Cuadro de diálogo de creación de esquemas](assets/schemas-create2.png)

El esquema se crea y se muestra la estructura de esquema generada.

De forma predeterminada, el esquema está vacío. Ahora debe agregar los campos que desea incluir en el esquema mediante el editor de esquemas:

1. Haga clic en el icono de lápiz en la sección **[!UICONTROL Contenido]** de la pantalla de detalles del esquema.
2. Añada los elementos necesarios y guarde. Este es un ejemplo de estructura de esquema personalizada:

   ![Cuadro de diálogo de creación de esquemas](assets/schemas-create3.png)

El sistema valida automáticamente la estructura XML y genera el esquema.

### Definición de la edición de pantalla {#define-attributes}

Después de crear el esquema, debe definir la edición de pantalla.

Para obtener más información sobre la pantalla de definición de pantalla y cómo acceder a ella, consulte la sección [Acceder a la definición de pantalla](schemas-browse-access.md#screen-def).

En nuestro ejemplo, simplemente agregamos dos campos personalizados:

1. Haga clic en el botón **[!UICONTROL Edición de pantalla]** de la vista de detalles del esquema para acceder a la definición de pantalla.

1. Haga clic en el icono de puntos suspensivos sobre la tabla **[!UICONTROL Lista de campos personalizados]** y elija **[!UICONTROL Seleccionar atributos]**.
1. Seleccione los campos personalizados que desee añadir y confirmar.

   ![Cuadro de diálogo de creación de esquemas](assets/schemas-create4.png)

## Publicación y sincronización de esquemas {#publish}

Después de crear o modificar un esquema, debe publicarlo para sincronizar el esquema lógico con la estructura física de la base de datos.

### Publicar cambios de esquema {#publish-changes}

>[!CAUTION]
>
>La publicación de cambios de esquema modifica la estructura de la base de datos. Asegúrese de comprender el impacto de estos cambios antes de confirmar la publicación.

Para publicar los cambios de esquema:

1. Vaya a **[!UICONTROL Administración]** > **[!UICONTROL Esquemas]** para acceder a la lista de esquemas.
1. Haga clic en **[!UICONTROL Publicación]** y confirme.

   ![Cuadro de diálogo de publicación de esquema que muestra los cambios que se aplicarán](assets/schemas-publish1.png)

1. Seleccione, en la lista, el esquema que desee sincronizar.

   ![Cuadro de diálogo de publicación de esquema que muestra los cambios que se aplicarán](assets/schemas-publish2.png)

1. Revise el script SQL que se ejecutará para actualizar la estructura de la base de datos.
1. Haga clic en **[!UICONTROL Publicar]** y confirme que desea continuar con la publicación.

>[!NOTE]
>
>El proceso puede tardar algún tiempo en función del tamaño de la base de datos y de la complejidad de los cambios.

### Crear una entrada de navegación {#navigation}

Después de publicar un esquema personalizado, puede crear una entrada de navegación en el Explorador para acceder a los datos personalizados:

1. Vaya al menú **[!UICONTROL Explorador]** y seleccione una carpeta en la que desee colocar el esquema personalizado.
1. Haga clic en el icono de puntos suspensivos y luego en **[!UICONTROL Crear nueva carpeta]**.
   ![Creación de la entrada de navegación para el esquema personalizado](assets/schemas-publish3.png)
1. Agregue una etiqueta y elija su esquema en el campo **[!UICONTROL Tipo de carpeta]**.
   ![Creación de la entrada de navegación para el esquema personalizado](assets/schemas-publish5.png)
1. Ahora se podrá obtener acceso al esquema personalizado desde la vista **[!UICONTROL Explorer]**.

Desde la nueva carpeta, puede:

* Vea la lista de registros en su esquema personalizado.
* Crear registros nuevos.
* Editar y eliminar registros existentes.
* Personalice qué columnas se muestran de forma predeterminada en la vista de lista.
