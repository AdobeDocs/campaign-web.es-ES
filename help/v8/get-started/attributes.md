---
audience: end-user
title: Seleccionar atributos y añadirlos a favoritos
description: Aprenda a trabajar con atributos y acceda fácilmente a los atributos favoritos y utilizados recientemente.
exl-id: 27663e57-fdab-4371-b7c6-12064ed6526f
source-git-commit: 6ed904273453ad355c615d330c234462cf3985e8
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 100%

---

# Seleccionar atributos y añadirlos a favoritos {#folders}

La interfaz de usuario web de Campaign permite a los usuarios seleccionar atributos de la base de datos en varias ubicaciones, según la acción que se lleve a cabo. Por ejemplo, se pueden seleccionar atributos al definir columnas de salida para un envío de correo directo o un archivo que se desee extraer. Del mismo modo, puede seleccionar atributos al utilizar el modelador de consultas para crear reglas o filtros, o para generar públicos.

![Seleccione atributos en la interfaz de base de datos, mostrando las opciones de atributos.](assets/attributes-list.png)

Para reutilizar rápidamente atributos que se utilicen con frecuencia, añádalos a favoritos. Esto garantiza que sean fácilmente accesibles para tareas futuras. Además de los favoritos, los usuarios pueden ver y utilizar los atributos seleccionados más recientemente.

La interfaz también proporciona una herramienta de distribución de valores, que le permite visualizar la distribución de los valores de un atributo dentro de una tabla. Esta herramienta ayuda a identificar el rango y la frecuencia de los valores, lo que garantiza la coherencia de los datos al crear consultas o expresiones.

## Atributos favoritos y recientes {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Favoritos y recientes"
>abstract="El menú **[!UICONTROL Favoritos y recientes]** del selector de atributos proporciona una vista organizada de los atributos que ha añadido a favoritos, junto con una lista de los atributos utilizados recientemente. Los atributos favoritos aparecen primero, seguidos de los utilizados recientemente, lo que facilita la localización de los atributos que necesita."

El menú **[!UICONTROL Favoritos y recientes]** del selector de atributos proporciona una vista organizada de los atributos añadidos a favoritos, junto con una lista de los atributos utilizados recientemente. Los atributos favoritos aparecen primero, seguidos de los utilizados recientemente, lo que facilita la localización de los atributos requeridos.

![Menú Favoritos y atributos recientes, que muestra los atributos favoritos y los utilizados recientemente.](assets/attributes-favorite.png)

Para añadir un atributo a favoritos, haga clic en el botón Expandir y seleccione **[!UICONTROL Añadir a favoritos]**. A continuación, el atributo se añade automáticamente a la lista de favoritos. Para eliminar un atributo de favoritos, vuelva a seleccionar el icono de estrella.

Los usuarios pueden añadir hasta 20 atributos favoritos. Los atributos favoritos y recientes están asociados con cada usuario dentro de una organización, lo que garantiza la accesibilidad entre diferentes máquinas y proporciona una experiencia perfecta en toda dispositivos.

## Identificar la distribución de valores dentro de una tabla {#distribution}

El botón **Distribución de valores**, aparece al hacer clic en el botón de expansión situado junto al atributo, y permite a los usuarios analizar la distribución de valores de ese atributo dentro de la tabla. Esta función es útil para comprender los valores disponibles, sus recuentos y sus porcentajes. También ayuda a evitar problemas como la incoherencia en las mayúsculas o en la ortografía al crear consultas o expresiones.

![Interfaz de herramienta de distribución de valores, que muestra recuentos y porcentajes de valores de atributo.](assets/attributes-distribution-values.png)

En el caso de los atributos con un gran número de valores, la herramienta solo muestra los veinte primeros. En estos casos, aparece una notificación **[!UICONTROL Carga parcial]** para indicar esta limitación. Aplique filtros avanzados para restringir los resultados mostrados y centrarse en valores específicos o subconjuntos de datos. Encontrará instrucciones detalladas sobre el uso de filtros [aquí](../get-started/work-with-folders.md#filter-the-values).

Para obtener información adicional sobre el uso de la herramienta de distribución de valores en diferentes contextos, consulte las siguientes secciones:

* [Distribución de valores en una carpeta](../get-started/work-with-folders.md##distribution-values-folder)
* [Distribución de valores en una consulta](../query/build-query.md#distribution-values-query)