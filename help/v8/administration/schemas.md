---
title: Trabajo con esquemas
description: Aprenda a trabajar con esquemas.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 24%

---

# Trabajo con esquemas {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Usar esquemas"
>abstract="Ahora puede acceder a los detalles de un esquema seleccionando su nombre en la lista. También puede acceder a la edición de campos personalizados en el botón **Editar detalle personalizado**."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Esquemas"
>abstract="**[!DNL Adobe Campaign]** utiliza esquemas basados en XML para definir la estructura física y lógica de los datos dentro de la aplicación. Desde esta pantalla, puede ver todos los esquemas existentes y acceder a los detalles de un esquema seleccionando su nombre en la lista. Hay filtros disponibles para ayudarle a restringir la lista, como mostrar solo los esquemas editables."

## Acerca de los esquemas {#about}

**[!DNL Adobe Campaign]** utiliza esquemas basados en XML para definir la estructura física y lógica de los datos dentro de la aplicación. Un esquema es un documento XML vinculado a una tabla de base de datos que define:

* La estructura de tabla SQL, incluidos el nombre de tabla, los campos y las relaciones.
* La estructura de datos XML, que incluye elementos, atributos, jerarquía, tipos, valores predeterminados y etiquetas.

Los esquemas juegan un función clave en:

* Asignar datos de aplicación a tablas de bases de datos.
* Definición de relaciones entre objetos de datos.
* Especificar la estructura y las propiedades de cada campo.

Cada entidad en Adobe Campaign tiene un esquema dedicado, lo que garantiza la coherencia y la organización de los datos.

Puede encontrar información detallada sobre los esquemas en la documentación](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"} de la [consola Campaign.

## Esquemas de acceso en la interfaz de usuario web {#access}

Los esquemas son accesibles desde el **[!UICONTROL menú Administración]** > **[!UICONTROL Esquemas]** .

![Pantalla de lista de esquemas que muestre los esquemas y filtros disponibles](assets/schemas-list.png)

Desde esta pantalla puede vista todos los esquemas existentes. Hay filtros disponibles para ayudarle a restringir la lista, como mostrar solo los esquemas editables.

Para abrir una esquema, seleccione su nombre. Se muestra un vista detallado de esquema.

![Pantalla Detalles del esquema que muestra esquema propiedades y contenido](assets/schema-details.png)

### Información general del esquema {#overview}

El **[!UICONTROL pestaña Información general]** proporciona una vista general del esquema:

* La **[!UICONTROL sección Propiedades]** muestra información clave, como el nombre del esquema, el espacio de nombres y el nombre de tabla asociado.

* La **[!UICONTROL sección Definición]** de esquema muestra detalles sobre la definición de esquema, incluida la clave principal utilizada para la reconciliación de datos y sus vínculos con otras tablas.

  Haga clic en la **[!UICONTROL botón Esquema previsualización]** para vista los distintos campos y vínculos que componen el esquema. Esto permite comprobar la estructura completa de una esquema. Si la esquema se ha ampliado con campos personalizados, puede visualizar todas sus extensiones.

* La **[!UICONTROL sección Contenido]** muestra el contenido XML del esquema, lo que permite cambiar entre la sintaxis de origen y la generada.

### Datos de esquema {#data}

El **[!UICONTROL pestaña Datos]** proporciona información sobre los datos esquema.

![Datos de esquema pestaña que muestran la estructura y los atributos de los datos](assets/schemas-data.png)

## Editar campos personalizados {#fields}

Los campos personalizados son atributos adicionales que se añaden a los esquemas preestablecidos a través de la consola Adobe Campaign. Permiten personalizar los esquemas incluyendo nuevos atributos para adaptarlos a las necesidades de la organización.

Los campos personalizados se pueden mostrar en varias pantallas, como perfil detalles en la interfaz web de Campaign. Puede controlar qué campos son visibles y cómo aparecen en la interfaz. Para ello, haga clic en la **[!UICONTROL botón de detalles]** personalizados Editar del **[!UICONTROL menú Esquemas]** .

![Pantalla de campos personalizados que muestra atributos editables](assets/schemas-custom.png)

Para obtener información detallada sobre cómo editar campos personalizados en una esquema, consulte esta sección: [Configuración de campos personalizados](../administration/custom-fields.md).