---
product: campaign
title: Pista de auditoría
description: Obtenga información sobre cómo monitorizar la instancia con la pista de auditoría de Campaign
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: 0fe12b469810c946ab0b9472e9a877aaaa41581d
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 6%

---

# Pista de auditoría{#audit-trail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Pista de auditoría"
>abstract="La nueva pista de auditoría proporciona un registro detallado y cronológico de todas las acciones y eventos que se han realizado en la instancia de Adobe Campaign en tiempo real."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"


En la interfaz de usuario web de Adobe Campaign, la función **[!UICONTROL Pista de auditoría]** proporciona a los usuarios una visibilidad completa de todas las modificaciones realizadas en entidades importantes de su instancia, normalmente aquellas que afectan de manera significativa al funcionamiento sin problemas de la instancia.

>[!IMPORTANT]
>
>* La interfaz de usuario web de Adobe Campaign no audita los cambios realizados en los derechos de usuario, plantillas, personalización o campañas.
>* Solo los administradores de la instancia pueden administrar la pista de auditoría.

La función **[!UICONTROL Pista de auditoría]** registra constantemente en tiempo real un registro detallado de las acciones y eventos que tienen lugar en la instancia de Adobe Campaign. Ofrece un método cómodo para acceder a un registro cronológico de datos, y abordar consultas como: el estado de los flujos de trabajo, las personas más recientes para modificarlos o las actividades realizadas por los usuarios dentro de la instancia.

+++ Más información sobre las Entidades disponibles de pista de auditoría

* **Seguimiento de auditoría de esquemas de Source** le permite supervisar las actividades y las modificaciones recientes realizadas en los esquemas en la consola del cliente de Campaign V8.

  Para obtener información detallada sobre los esquemas, consulte [Documentación de Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Registro de auditoría de flujo de trabajo** le permite realizar un seguimiento de las actividades y los cambios recientes realizados en los flujos de trabajo, incluidos sus estados actuales, como:

   * Start
   * Pause
   * Stop
   * Restart
   * Limpieza igual al historial de purga de acciones
   * Simular, que es igual a la acción Iniciar en modo de simulación
   * Activación igual a la acción Ejecutar tareas pendientes ahora
   * Interrupción incondicional

  Para obtener más información sobre los flujos de trabajo, consulte esta [página](../workflows/gs-workflows.md).

* **Seguimiento de auditoría de opciones** le permite supervisar las actividades y las modificaciones recientes realizadas en las opciones de Campaign V8.

  Para obtener más información sobre las opciones, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Registro de auditoría de envíos** le permite comprobar las actividades y las últimas modificaciones realizadas en los envíos.

  Para obtener más información sobre las entregas, consulte esta [página](../msg/gs-deliveries.md).

* **Cuenta externa** le permite comprobar las modificaciones realizadas en cuentas externas en la versión 8 de Campaign, utilizadas por procesos técnicos como flujos de trabajo técnicos o flujos de trabajo de campaña.

  Para obtener más información sobre la cuenta externa, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts).

* **Asignación de entregas** le permite supervisar las actividades y las modificaciones recientes realizadas en la asignación de entregas en Campaign V8.

  Para obtener más información sobre la asignación de envíos, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Aplicación web** le permite comprobar las modificaciones realizadas en los formularios web de Campaign V8 que se usan para crear páginas con campos de entrada y selección, y que pueden incluir datos de la base de datos.

  Para obtener más información sobre la aplicación web, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Oferta** le permite comprobar las actividades y las últimas modificaciones realizadas en sus ofertas.

  Para obtener más información sobre las ofertas, consulte esta [página](../msg/offers.md).

* **Operador** le permite supervisar las actividades y las modificaciones recientes realizadas en sus Operadores en Campaign V8.

  Para obtener más información sobre los operadores, consulte esta [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Acceso a Pista de auditoría {#accessing-audit-trail}

Para acceder a la **[!UICONTROL pista de auditoría]** de su instancia:

1. En el menú **[!UICONTROL Administración]**, seleccione **[!UICONTROL Pista de auditoría]** .

   ![](assets/audit-trail-1.png)

1. La ventana **[!UICONTROL Pista de auditoría]** se abre con la lista de sus entidades. La interfaz de usuario web de Adobe Campaign audita las acciones de creación, edición y eliminación de flujos de trabajo, opciones, envíos y esquemas.

   Seleccione una de las entidades para obtener más información sobre las últimas modificaciones.

1. La ventana **[!UICONTROL Entidad de auditoría]** le proporciona información más detallada sobre la entidad elegida, como:

   * **[!UICONTROL Tipo]** : flujo de trabajo, opciones, envíos o esquemas.
   * **[!UICONTROL Entidad]** : Nombre interno de sus actividades.
   * **[!UICONTROL Modificado por]** : Nombre de usuario de la última persona que modificó esta entidad por última vez.
   * **[!UICONTROL Acción]** : última acción realizada en esta entidad, ya sea Creada, Modificada o Eliminada.
   * **[!UICONTROL Fecha de modificación]** : Fecha de la última acción realizada en esta entidad.

   El bloque de código proporciona más información sobre lo que se ha cambiado exactamente en la entidad.

   ![](assets/audit-trail-2.png)
