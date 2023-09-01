---
audience: end-user
title: Introducción a las campañas
description: Obtenga información sobre cómo empezar con campañas en canales múltiples
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 100%

---


# Acceso y administración de campañas{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Programación de campañas"
>abstract="Establezca o modifique la programación de campañas."

Para crear una nueva campaña o administrar las campañas existentes, haga clic en el menú **[!UICONTROL Campañas]** en la navegación de la izquierda.

## La lista de campañas{#access-campaigns}

En la lista de campañas, hay dos pestañas disponibles:

* La pestaña **Examinar** enumera todas las campañas existentes. Puede hacer clic en una campaña para abrir su panel o crear una nueva campaña haciendo clic en el botón **Crear campaña**. Consulte esta [sección](create-campaigns.md#create-campaigns).

* La pestaña **Plantillas** contiene todas las plantillas de campaña disponibles. Las plantillas de campaña están preconfiguradas para que se puedan reutilizar al crear nuevas campañas. Se crean desde la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=es)

![Lista de campañas](assets/campaign-list.png)

De forma predeterminada, cada campaña de la lista muestra información sobre su estado actual, fecha de creación, la última vez que se modificó, etc.

Puede personalizar las columnas mostradas haciendo clic en el icono **Configurar la columna para un diseño personalizado** situado en la esquina superior derecha de la lista. Esto le permite agregar información adicional a la lista. Además, hay una barra de búsqueda y filtros disponibles para facilitar la búsqueda dentro de la lista. [Más información](../get-started/user-interface.md#list-screens).

Por ejemplo, puede filtrar la programación de su campaña. Abra el panel de filtro y utilice la sección **Fecha de inicio y de finalización**:

![Filtro de campaña](assets/campaign-filter-on-dates.png)

## El panel de campañas{#campaign-dashboard}

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
