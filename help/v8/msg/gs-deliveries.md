---
product: campaign
title: Acceso a los envíos
description: Obtenga información sobre cómo acceder y administrar los envíos en Campaign Web
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 3afff35c-c15f-46f8-b791-9bad5e38ea44
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 34%

---

# Acceso a los envíos {#work-with-deliveries}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Envíos"
>abstract="Una entrega de de es una comunicación enviada a una audiencia a través de un canal específico: correo electrónico, SMS o push. En esta pantalla, puede editar, duplicar y eliminar los envíos existentes. También puede ver los informes de los envíos completados. Haga clic en el botón **Crear envío** para añadir un nuevo envío."

## Acceso a los envíos {#access}

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_target"
>title="Destino adicional"
>abstract="Estas reglas solo pueden modificarse en la consola del cliente. "

Se puede acceder a los envíos desde el menú **[!UICONTROL Envíos]** del panel de navegación izquierdo. Todos los envíos creados desde la consola de cliente o la interfaz de usuario web aparecen en esta lista. Desde esta pantalla, puede monitorizar todas las entregas existentes, duplicarlas o eliminarlas, o crear otras nuevas.

![Lista de envíos mostrados en la interfaz](assets/deliveries-list.png)

Para abrir una entrega, haga clic en su nombre en la lista. La entrega se abre, lo que le permite realizar varias acciones, como editar sus parámetros, comprobar su ejecución o monitorizar su rendimiento mediante informes dedicados.

![Pantalla de detalles de envío que muestra parámetros e informes](assets/delivery-details.png)

>[!NOTE]
>
>Si abre una entrega creada en la consola del cliente, puede que se muestre la sección **[!UICONTROL Destino adicional]** para la audiencia. Esto indica que se han configurado varios objetivos para este envío. Estos parámetros solo se pueden modificar en la consola.
>
>![Mensaje de advertencia sobre la configuración de destino adicional](assets/target-warning-audience.png){zoomable="yes"}

## Duplicación de un envío {#delivery-duplicate}

Puede crear una copia de un envío existente, ya sea desde la lista de envíos o desde el panel de envíos.

Para duplicar un envío de la lista de envíos, siga estos pasos:

1. Haga clic en el botón de tres puntos de la derecha, junto al nombre del envío que desea duplicar.
1. Seleccione **[!UICONTROL Duplicar]**.
1. Confirme la duplicación. El nuevo panel de envío se abre en la pantalla central.

Para duplicar un envío desde su panel, siga estos pasos:

1. Abra la entrega y haga clic en el botón **[!UICONTROL ...Más]** en la sección superior de la pantalla.
1. Seleccione **[!UICONTROL Duplicar]**.
1. Confirme la duplicación. La nueva entrega reemplaza la entrega actual en la pantalla central.

## Eliminación de un envío {#delivery-delete}

Las entregas se eliminan de la lista de entregas, ya sea de la entrada de entrega principal en el carril izquierdo o de la lista de entregas de una campaña.

Para eliminar un envío de la lista de envíos, siga estos pasos:

1. Haga clic en el botón de tres puntos de la derecha, junto al nombre de la entrega que desea eliminar.
1. Seleccione **[!UICONTROL Delete]**.
1. Confirme la eliminación.

![Eliminando un envío de la interfaz de la lista de envíos](assets/delete-delivery-from-list.png)

Todas los envíos están disponibles en estas listas, pero los envíos creados en un flujo de trabajo no se pueden eliminar de allí. Para eliminar una entrega creada en el contexto de un flujo de trabajo, elimine la actividad de entrega del flujo de trabajo.

Para eliminar un envío de un flujo de trabajo, siga estos pasos:

1. Seleccione la actividad envío.
1. Haga clic en el icono **[!UICONTROL Eliminar]** en el panel derecho.
1. Confirme la eliminación. Si la entrega tiene nodos secundarios, elija eliminarlos también o mantenerlos.

![Eliminando una actividad de envío dentro de un flujo de trabajo](assets/delete-delivery-from-wf.png)