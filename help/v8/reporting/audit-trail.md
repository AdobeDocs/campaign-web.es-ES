---
product: campaign
title: Pista de auditoría
description: Obtenga información sobre cómo monitorizar la instancia con la pista de auditoría de Campaign
feature: Audit Trail, Monitoring, Workflows
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 6%

---

# Pista de auditoría{#audit-trail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Pista de auditoría"
>abstract="La nueva pista de auditoría proporciona un registro detallado y cronológico de todas las acciones y eventos que se han realizado en la instancia de Adobe Campaign en tiempo real."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"


En la interfaz de usuario web de Adobe Campaign, la variable **[!UICONTROL Pista de auditoría]** Esta función proporciona a los usuarios una visibilidad completa de todas las modificaciones realizadas en entidades importantes de la instancia, normalmente las que afectan significativamente al funcionamiento sin problemas de la instancia.

>[!IMPORTANT]
>
>* La interfaz de usuario web de Adobe Campaign no audita los cambios realizados en los derechos de usuario, plantillas, personalización o campañas.
>* Solo los administradores de la instancia pueden administrar la pista de auditoría.

**[!UICONTROL Pista de auditoría]** registra constantemente un registro detallado de las acciones y eventos que se producen dentro de la instancia de Adobe Campaign en tiempo real. Ofrece un método cómodo para acceder a un registro cronológico de datos, y abordar consultas como: el estado de los flujos de trabajo, las personas más recientes para modificarlos o las actividades realizadas por los usuarios dentro de la instancia.

+++ Más información sobre las Entidades disponibles de pista de auditoría

* **Pista de auditoría del esquema de origen** permite monitorizar las actividades y modificaciones recientes realizadas en los esquemas dentro de la consola del cliente de Campaign V8.

  Para obtener información detallada sobre los esquemas, consulte [Documentación de Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Pista de auditoría de flujo de trabajo** le permite realizar un seguimiento de las actividades y los cambios recientes realizados en los flujos de trabajo, incluidos sus estados actuales como:

   * Start
   * Pause
   * Stop
   * Restart
   * Limpieza igual al historial de purga de acciones
   * Simular, que es igual a la acción Iniciar en modo de simulación
   * Activación igual a la acción Ejecutar tareas pendientes ahora
   * Interrupción incondicional

  Para obtener más información sobre los flujos de trabajo, consulte [página](../workflows/gs-workflows.md).

* **Pista de auditoría de opción** permite supervisar las actividades y las modificaciones recientes realizadas en las opciones de Campaign V8.

  Para obtener más información, consulte [página](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Pista de auditoría de envíos** permite comprobar las actividades y las últimas modificaciones realizadas en los envíos.

  Para obtener más información sobre las entregas, consulte [página](../msg/gs-deliveries.md).

* **Cuenta externa** permite comprobar las modificaciones realizadas en cuentas externas en Campaign V8, utilizadas por procesos técnicos como flujos de trabajo técnicos o flujos de trabajo de campaña.

  Para obtener más información sobre la cuenta externa, consulte [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts).

* **Asignación de envíos** permite supervisar las actividades y las modificaciones recientes realizadas en la asignación de entregas en Campaign V8.

  Para obtener más información sobre la asignación de envíos, consulte esta sección [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Aplicación web** permite comprobar las modificaciones realizadas en los formularios web en Campaign V8 utilizados para crear páginas con campos de entrada y selección, y que pueden incluir datos de la base de datos.

  Para obtener más información sobre la aplicación web, consulte [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Oferta** permite comprobar las actividades y las últimas modificaciones realizadas en las ofertas.

  Para obtener más información sobre las ofertas, consulte [página](../msg/offers.md).

* **Operador** permite supervisar las actividades y las modificaciones recientes realizadas en los operadores en Campaign V8.

  Para obtener más información sobre los operadores, consulte [página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Acceso a Pista de auditoría {#accessing-audit-trail}

Para acceder a la de **[!UICONTROL Pista de auditoría]**:

1. En el **[!UICONTROL Administration]** menú, seleccione **[!UICONTROL Pista de auditoría]** .

   ![](assets/audit-trail-1.png)

1. El **[!UICONTROL Pista de auditoría]** se abre con la lista de las entidades. La interfaz de usuario web de Adobe Campaign audita las acciones de creación, edición y eliminación de flujos de trabajo, opciones, envíos y esquemas.

   Seleccione una de las entidades para obtener más información sobre las últimas modificaciones.

1. El **[!UICONTROL Entidad de auditoría]** Esta ventana proporciona información más detallada sobre la entidad elegida, como:

   * **[!UICONTROL Tipo]** : Flujo de trabajo, opciones, envíos o esquemas.
   * **[!UICONTROL Entidad]** : Nombre interno de las actividades.
   * **[!UICONTROL Modificado por]** : Nombre de usuario de la última persona que modificó esta entidad por última vez.
   * **[!UICONTROL Acción]** : última acción realizada en esta entidad, ya sea Creada, Modificada o Eliminada.
   * **[!UICONTROL Fecha de modificación]** : Fecha de la última acción realizada en esta entidad.

   El bloque de código proporciona más información sobre lo que se ha cambiado exactamente en la entidad.

   ![](assets/audit-trail-2.png)

