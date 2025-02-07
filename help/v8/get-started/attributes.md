---
audience: end-user
title: Seleccione atributos y agréguelos a favoritos
description: Aprenda a trabajar con atributos y acceder fácilmente a los atributos favoritos y utilizados recientemente.
exl-id: 27663e57-fdab-4371-b7c6-12064ed6526f
source-git-commit: 3bedb4562c5858cd6057fd8a17064ccac8303c39
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 6%

---

# Seleccione atributos y agréguelos a favoritos {#folders}

La interfaz de usuario web de Campaign permite seleccionar atributos de la base de datos en varias ubicaciones, según la acción que desee realizar. Por ejemplo, puede seleccionar atributos al definir columnas de salida para una entrega de correo directo o un archivo que desee extraer. Del mismo modo, se pueden seleccionar atributos al utilizar el modelador de consultas para crear reglas, filtros o audiencias.

![](assets/attributes-list.png)

Para reutilizar rápidamente atributos que se utilizan con frecuencia, puede agregarlos a Favoritos. Esto garantiza que sean fácilmente accesibles para tareas futuras. Además de los favoritos, también puede ver y utilizar los atributos seleccionados más recientemente.

La interfaz también proporciona una herramienta de distribución de valores, que le permite visualizar la distribución de los valores de un atributo dentro de una tabla. Esta herramienta puede ayudarle a identificar el rango y la frecuencia de los valores, lo que garantiza la coherencia de los datos al crear consultas o expresiones.

## Favoritos y atributos recientes {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Favoritos y Recientes"
>abstract="El menú **[!UICONTROL Favoritos y recientes]** del selector de atributos proporciona una vista organizada de los atributos que ha agregado a favoritos, junto con una lista de los atributos utilizados recientemente. Los atributos favoritos aparecen primero, seguidos de los utilizados recientemente, lo que facilita la localización de los atributos que necesita."

El menú **[!UICONTROL Favoritos y recientes]** del selector de atributos proporciona una vista organizada de los atributos que ha agregado a favoritos, junto con una lista de los atributos utilizados recientemente. Los atributos favoritos aparecen primero, seguidos de los utilizados recientemente, lo que facilita la localización de los atributos que necesita.

![](assets/attributes-favorites.png)

Para añadir un atributo a favoritos, pase el ratón sobre el botón de información y seleccione el icono de estrella. A continuación, el atributo se agregará automáticamente a la lista de favoritos. Si ya no desea mantener un atributo como favorito, puede eliminarlo seleccionando de nuevo el icono de estrella.

Puede añadir hasta 20 atributos como favoritos. Los atributos favoritos y recientes se asocian con cada usuario dentro de una organización. Esto significa que son accesibles desde diferentes máquinas, lo que garantiza una experiencia perfecta entre dispositivos.

## Identificar la distribución de valores dentro de una tabla {#distribution}

El botón **Distribución de valores**, disponible en el panel de información de un atributo, le permite analizar la distribución de valores para ese atributo dentro de la tabla. Esta función es especialmente útil para comprender los valores disponibles, sus recuentos y porcentajes. También ayuda a evitar problemas como mayúsculas y minúsculas incoherentes o ortografía al crear consultas o expresiones.

![](assets/attributes-distribution-values.png)

Para atributos con un gran número de valores, la herramienta muestra solo los veinte primeros. En estos casos, aparecerá una notificación **[!UICONTROL Carga parcial]** para indicar esta limitación. Puede aplicar filtros avanzados para restringir los resultados mostrados y centrarse en valores específicos o subconjuntos de datos. Encontrará instrucciones detalladas sobre el uso de filtros [aquí](../get-started/work-with-folders.md#filter-the-values).

Para obtener información adicional sobre el uso de la herramienta de distribución de valores en diferentes contextos, consulte las siguientes secciones:

- [Distribución de valores en una carpeta](../get-started/work-with-folders.md##distribution-values-folder)
- [Distribución de valores en una consulta](../query/build-query.md#distribution-values-query)
