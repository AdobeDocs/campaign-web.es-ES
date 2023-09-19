---
audience: end-user
title: Introducción a las campañas
description: Obtenga información sobre cómo empezar con campañas en canales múltiples
badge: label="Beta"
source-git-commit: a7a7a345e7e01f30516d2925afc46cfe32738aa4
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 72%

---


# Acceso y administración de campañas{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Programación de campañas"
>abstract="Establezca o modifique la programación de campañas."

Para crear una nueva campaña o administrar las campañas existentes, haga clic en el menú **[!UICONTROL Campañas]** en la navegación de la izquierda.

## Lista de campañas {#access-campaigns}

En la lista de campañas, hay dos pestañas disponibles:

* La pestaña **Examinar** enumera todas las campañas existentes. Puede hacer clic en una campaña para abrir su panel o crear una nueva campaña haciendo clic en el botón **Crear campaña**. Consulte esta [sección](create-campaigns.md#create-campaigns).

* La pestaña **Plantillas** contiene todas las plantillas de campaña disponibles. Puede ver una plantilla existente o crear una nueva. [Más información](manage-campaign-templates.md).

![Lista de campañas](assets/campaign-list.png)

De forma predeterminada, cada campaña de la lista muestra información sobre su estado actual, fecha de creación, la última vez que se modificó, etc.

Puede personalizar las columnas mostradas haciendo clic en el icono **Configurar la columna para un diseño personalizado** situado en la esquina superior derecha de la lista. Esto le permite agregar información adicional a la lista. Además, hay una barra de búsqueda y filtros disponibles para facilitar la búsqueda dentro de la lista. [Más información](../get-started/user-interface.md#list-screens).

Por ejemplo, puede filtrar la programación de su campaña. Abra el panel de filtro y utilice la sección **Fecha de inicio y de finalización**:

![Filtro de campaña](assets/campaign-filter-on-dates.png)

## Panel de campañas{#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Lista de envíos en la campaña"
>abstract="La pestaña **Envíos** lista todos los envíos vinculados a la campaña actual. Haga clic en el nombre de una entrega para editarlo. Utilice el botón Create delivery para añadir una nueva entrega para esta campaña."

En la pestaña **Examinar** de la lista de campañas, haga clic en una campaña para mostrar los detalles.

![Panel de campañas](assets/campaign-dashboard.png)

El estado y la programación de la campaña se muestran en la parte superior de la pantalla. Puede usar el icono **Configuración de la campaña** para modificar las propiedades de la campaña definidas al crear la campaña. Hay tres botones disponibles que permiten ver los registros, crear informes, duplicar o eliminar la campaña. Consulte esta [sección](create-campaigns.md#create-campaigns)

Hay dos pestañas disponibles:

* La pestaña **Flujos de trabajo** contiene todos los flujos de trabajo vinculados a la campaña. Esta pestaña también le permite crear un nuevo flujo de trabajo dentro de la campaña. Consulte esta [sección](create-campaigns.md#create-campaigns).

* La pestaña **Envíos** lista todos los envíos vinculados a la campaña actual. También puede crear un nuevo envío dentro de la campaña. Consulte esta [sección](create-campaigns.md#create-campaigns).

## Duplicación y eliminación de una campaña

Puede duplicar o eliminar una campaña:

* en la lista de campañas, haga clic en el botón de puntos suspensivos y seleccione **Duplicar** o **Eliminar**.
* en la propia campaña, haga clic en el botón **Más** y luego seleccione **Duplicar** o **Eliminar**.

>[!NOTE]
>
>La pestaña **Envíos** muestra todas las envíos vinculadas a la campaña. Sin embargo, los envíos creados en un flujo de trabajo no se pueden eliminar de allí. Para eliminar un envío creado en el contexto de un flujo de trabajo, se debe eliminar la actividad de entrega del flujo de trabajo. [Más información](../msg/gs-messages.md#delivery-delete).

## Trabajo con plantillas de campaña{#manage-campaign-templates}

Las plantillas de campaña contienen ajustes preconfigurados que se pueden reutilizar para crear nuevos flujos de trabajo. Hay disponible un conjunto de plantillas integradas para ayudarle a empezar. Puede crear y configurar las plantillas de campañas y luego crear campañas a partir de estas plantillas.

Una plantilla de campaña puede almacenar la siguiente información:

* la de la campaña **Propiedades** y **Programación** configuración
* plantillas de flujo de trabajo
* plantillas de envío

Para crear una plantilla de campaña, siga estos pasos:

1. Haga clic en **[!UICONTROL Campañas]** , vaya a la **Plantillas** y, a continuación, haga clic en **[!UICONTROL Crear plantilla]** botón.
1. Seleccione el **Plantilla** para utilizar y proporcionar una etiqueta para la campaña. Esto le permite basar la nueva plantilla en una plantilla ya creada.
1. Si es necesario, puede cambiar lo siguiente **Opciones adicionales**: nombre interno, carpeta, usuario asignado, descripción y naturaleza.
1. Defina el **Programación** de la campaña. Obtenga información sobre cómo establecer la programación de campañas en [esta sección](create-campaigns.md#campaign-schedule)
1. Haga clic en **Create**.
1. Añada flujos de trabajo y plantillas de envío a la campaña.
