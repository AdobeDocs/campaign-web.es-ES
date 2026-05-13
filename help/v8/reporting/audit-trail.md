---
product: campaign
title: Pista de auditoría
description: Obtenga información sobre cómo monitorizar la instancia con la pista de auditoría de Campaign
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
TQID: https://experienceleague.adobe.com/J3c5k0g22amplf8KqJGCByig3OKIqSZ-Hk87ea8C7mM
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
subfeature_v2:
  - id: cebd7cfa-b9fa-4d9f-a2ab-fce31f32c4a3
  - id: cfc95e9b-b035-4403-a6a9-b27a8a053a37
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 649
ht-degree: 1%

---

# Pista de auditoría {#audit-trail}

En la interfaz de usuario web de Adobe Campaign, la función **[!UICONTROL Pista de auditoría]** proporciona a los usuarios una visibilidad completa de todas las modificaciones realizadas en entidades importantes de su instancia, normalmente aquellas que afectan significativamente al funcionamiento sin problemas de la instancia.

>[!IMPORTANT]
>
>* La interfaz de usuario web de Adobe Campaign no audita los cambios realizados en los derechos de usuario, las plantillas, la personalización o las campañas.
>* Solo los administradores de la instancia pueden administrar la pista de auditoría.

La función **[!UICONTROL Pista de auditoría]** registra constantemente un registro detallado de las acciones y eventos que se producen en la instancia de Adobe Campaign en tiempo real. Ofrece un método cómodo para acceder a un registro cronológico de datos, y abordar consultas como el estado de los flujos de trabajo, las personas más recientes para modificarlos o las actividades realizadas por los usuarios dentro de la instancia.

+++ Más información sobre las Entidades disponibles de pista de auditoría

* **Seguimiento de auditoría de esquemas de Source** le permite supervisar las actividades y las modificaciones recientes realizadas en los esquemas dentro de la consola del cliente de Campaign v8.

  Para obtener información detallada sobre los esquemas, consulte [Documentación de Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Registro de auditoría de flujo de trabajo** le permite realizar un seguimiento de las actividades y los cambios recientes realizados en los flujos de trabajo, incluidos sus estados actuales, como:

   * Start
   * Pause
   * Stop
   * Restart
   * Limpieza, que es igual a la acción Purgar historial
   * Simular, que es igual a la acción Iniciar en modo de simulación
   * Activación, que es igual a la acción Ejecutar tareas pendientes ahora
   * Interrupción incondicional

  Para obtener más información sobre los flujos de trabajo, consulte esta [página](../workflows/gs-workflows.md).

* **Seguimiento de auditoría de opciones** le permite supervisar las actividades y las modificaciones recientes realizadas en las opciones de Campaign v8.

  Para obtener más información sobre las opciones, consulte esta [página](https://experienceleague.adobe.com/es/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Registro de auditoría de envíos** le permite comprobar las actividades y las últimas modificaciones realizadas en los envíos.

  Para obtener más información sobre las entregas, consulte esta [página](../msg/gs-deliveries.md).

* **Cuenta externa** le permite comprobar las modificaciones realizadas en cuentas externas en Campaign v8, utilizadas por procesos técnicos como flujos de trabajo técnicos o flujos de trabajo de campaña.

  Para obtener más información sobre cuentas externas, consulte esta [página](../administration/external-account.md).

* **Asignación de entregas** le permite supervisar las actividades y las modificaciones recientes realizadas en la asignación de entregas en Campaign v8.

  Para obtener más información sobre la asignación de envíos, consulte esta [página](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Aplicación web** le permite comprobar las modificaciones realizadas en los formularios web en Campaign v8, utilizados para crear páginas con campos de entrada y selección, y que pueden incluir datos de la base de datos.

  Para obtener más información sobre las aplicaciones web, consulte esta [página](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/content/webapps).

* **Oferta** le permite comprobar las actividades y las últimas modificaciones realizadas en sus ofertas.

  Para obtener más información sobre las ofertas, consulte esta [página](../msg/offers.md).

* **Operador** le permite supervisar las actividades y las modificaciones recientes realizadas en sus Operadores en Campaign v8.

  Para obtener más información sobre los operadores, consulte esta [página](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Acceso a Pista de auditoría {#accessing-audit-trail}

Para acceder a la **[!UICONTROL pista de auditoría]** de su instancia:

1. En el menú **[!UICONTROL Administración]**, seleccione **[!UICONTROL Pista de auditoría]**.

   ![Captura de pantalla que muestra el menú Administración con la opción Pista de auditoría seleccionada](assets/audit-trail-1.png)

1. La ventana **[!UICONTROL Pista de auditoría]** se abre con la lista de sus entidades. La interfaz de usuario web de Adobe Campaign audita las acciones de creación, edición y eliminación de flujos de trabajo, opciones, envíos y esquemas.

   Seleccione una de las entidades para obtener más información sobre las últimas modificaciones.

1. La ventana **[!UICONTROL Entidad de auditoría]** proporciona información detallada sobre la entidad elegida, como:

   * **[!UICONTROL Tipo]**: flujo de trabajo, opciones, envíos o esquemas.
   * **[!UICONTROL Entidad]**: Nombre interno de sus actividades.
   * **[!UICONTROL Modificado por]**: Nombre de usuario de la última persona que modificó esta entidad.
   * **[!UICONTROL Acción]**: última acción realizada en esta entidad, ya sea Creada, Modificada o Eliminada.
   * **[!UICONTROL Fecha de modificación]**: Fecha de la última acción realizada en esta entidad.

   El bloque de código proporciona más información sobre lo que se ha cambiado exactamente en la entidad.

   ![Captura de pantalla que muestra la ventana Entidad de auditoría con información detallada sobre las modificaciones](assets/audit-trail-2.png)