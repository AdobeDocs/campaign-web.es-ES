---
title: Creación y uso de filtros predefinidos
description: Obtenga información sobre cómo crear y administrar filtros predefinidos en la IU web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
source-git-commit: 78b779051a71a89d45c73502a5e9220cedfa7498
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 1%

---

# Trabajo con filtros predefinidos {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Administración de filtros predefinidos"
>abstract="La web de Campaign ahora le ofrece una interfaz fácil de usar para administrar y personalizar sin esfuerzo los filtros predefinidos para satisfacer sus necesidades específicas. Cree una vez y guárdela para usarla en el futuro."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Filtros predefinidos"
>abstract="La web de Campaign ahora le ofrece una interfaz fácil de usar para administrar y personalizar sin esfuerzo los filtros predefinidos para satisfacer sus necesidades específicas. Cree una vez y guárdela para usarla en el futuro."

Los filtros predefinidos son filtros personalizados que se crean y guardan para que estén disponibles para su uso futuro. Se pueden utilizar como accesos directos durante cualquier operación de filtrado con el generador de reglas, por ejemplo al filtrar una lista de datos o crear la audiencia de una entrega.

Puede utilizar filtros integrados existentes para acceder a un subconjunto específico de sus datos o crear sus propios filtros predefinidos y guardarlos.

![](assets/predefined-filters-menu.png)


## Creación de un filtro predefinido {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="Creación de un filtro predefinido"
>abstract="Introduzca una etiqueta para el filtro predefinido y seleccione la tabla a la que se aplica. Abra las opciones adicionales para agregar una descripción y establecer este filtro como favorito. A continuación, utilice el botón &quot;Crear regla&quot; para definir las condiciones de filtrado."


>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="Creación de reglas de filtro predefinidas"
>abstract="Para definir las condiciones de filtrado del filtro personalizado, haga clic en el botón Crear regla."


Para guardar un filtro personalizado en el generador de reglas, siga los pasos a continuación:

1. Abra el generador de reglas y defina las condiciones de filtrado. En el ejemplo siguiente, se filtran los destinatarios que viven en Madrid.
1. Haga clic en **Seleccionar o guardar filtro** y seleccione. **Guardar como filtro**.

   ![](assets/predefined-filters-save.png)

1. Seleccionar **Creación de un nuevo filtro** y escriba un nombre y una descripción para ese filtro.

   ![](assets/predefined-filters-save-filter.png)

1. (opcional) Habilite la opción **Guardar como favorito** si desea ver este filtro predefinido en sus favoritos.


   Cuando un filtro se guarda como favorito, está disponible para todos los usuarios en la **Filtros favoritos** de la lista de creación de filtros, como se muestra a continuación:

   ![](assets/predefined-filters-favorite.png)


1. Clic **Confirmar** para guardar los cambios.

El filtro personalizado ahora está disponible en la **Filtros predefinidos** y accesibles para todos los usuarios de Campaign.

También puede crear un filtro desde el **Filtros predefinidos** en el menú de la izquierda. Para ello, siga los pasos a continuación:

1. Examine la **Filtros predefinidos** en el menú de la izquierda.
1. Haga clic en **Crear filtro** botón.
1. Introduzca el nombre del filtro y, en **Tipo de documento** , seleccione el esquema al que se aplica. El esquema predeterminado es `Recipients(nms)`.
1. Defina la regla para el filtro. Por ejemplo, perfiles mayores de 30.

   ![](assets/filter-30+.png)

1. Guarde los cambios. El filtro se agrega a la lista de filtros predefinidos.

## Uso de un filtro predefinido {#use-predefined-filter}

Los filtros predefinidos están disponibles al definir las propiedades de la regla. Para acceder a los filtros predefinidos, seleccione **Seleccionar filtro personalizado** en la lista desplegable del generador de reglas.

A continuación, puede acceder a la lista completa de filtros predefinidos disponibles para el contexto actual.

También puede utilizar los métodos abreviados de filtro disponibles en la variable **Filtros favoritos** de la lista desplegable.

Por ejemplo, para crear una audiencia a partir de un filtro predefinido, siga estos pasos:

1. Examine la **Audiencias** en el menú de la izquierda.
1. Haga clic en **Crear audiencia** botón.
1. Introduzca el nombre de la audiencia y haga clic en **Crear audiencia** botón.
1. Seleccione el **Consulta** actividad y, en el panel derecho, haga clic en **Crear audiencia** botón.

   ![](assets//build-audience-from-filter.png)

1. Desde el **Botón Seleccionar o guardar filtro**, elija la **Seleccionar filtro personalizado** opción.

   ![](assets/build-audience-select-custom-filter.png)

1. Vaya al filtro predefinido que se utilizará para crear la audiencia, selecciónelo y confirme la acción.

   ![](assets/build-audience-filter-list.png)

1. Compruebe las propiedades de la regla para este filtro y confirme.

   ![](assets/build-audience-check.png)

   El filtro ahora se utiliza como consulta en la **Consulta** actividad.

   ![](assets/build-audience-confirm.png)

1. Guarde los cambios y haga clic en **Inicio** para crear la audiencia y que esté disponible en la lista de audiencias.

## Administrar los filtros predefinidos {#manage-predefined-filter}

Los filtros predefinidos se agrupan en la entrada dedicada del menú de navegación de la izquierda.

A partir de esta lista, puede crear un nuevo filtro como se detalla más arriba, y:

* editar un filtro existente y cambiarlo por reglas y propiedades
* duplicar un filtro predefinido
* eliminación de un filtro predefinido

## Filtros predefinidos integrados {#ootb-predefined-filter}

Campaign viene con un conjunto de filtros predefinidos creados a partir de la consola del cliente. Estos filtros se pueden utilizar para definir audiencias y reglas. No deben modificarse.
