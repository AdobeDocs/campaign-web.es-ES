---
audience: end-user
title: Descubra la interfaz
description: Interfaz de usuario web de Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha" type="Positive"
source-git-commit: 5a99d2145bcc4ac1c3cdc00ef745049c728c2a28
workflow-type: tm+mt
source-wordcount: '1372'
ht-degree: 34%

---

# Descubra la interfaz {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Descubra la interfaz"
>abstract="La nueva interfaz web de Campaign v8 ofrece una experiencia de usuario integrada, intuitiva y coherente."

La nueva interfaz web de Campaign v8 ofrece una experiencia de usuario moderna e intuitiva para simplificar el diseño y el envío de las campañas de marketing. Esta nueva interfaz está integrada con Adobe Experience Platform.

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>Esta documentación se actualiza con frecuencia para reflejar los cambios más recientes en la interfaz de usuario del producto. Sin embargo, algunas capturas de pantalla pueden diferir ligeramente de la interfaz de usuario.


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## Menú de navegación izquierda

Examine los vínculos de la izquierda para acceder a las funciones web de Campaign v8. Varios vínculos muestran listas de objetos que se pueden ordenar y filtrar. También puede configurar columnas para que muestren toda la información que necesite. Consulte esta [sección](#list-screens). Todas las pantallas de lista son de solo lectura, excepto la lista de envío de correo electrónico. Hacer clic en cualquier elemento de la lista para su edición o visualización no está disponible en Alpha. Todas las listas se podrán editar en versiones futuras. Los elementos mostrados en el menú de navegación de la izquierda dependen de los permisos de usuario.

![](assets/home.png)

### Inicio

Esta pantalla incluye vínculos y recursos clave para acceder rápidamente a las funciones web principales de Campaign v8. La variable **Recientes** proporciona accesos directos a los envíos creados y modificados recientemente. Esta lista muestra sus fechas de creación y modificación y su estado.

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Acceda a las páginas de ayuda de la clave web de Campaign v8 desde la sección inferior de la página principal.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorer

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="El menú **Explorer** muestra la misma jerarquía de carpetas que la de la consola del cliente. Examine todos los componentes, las carpetas y los esquemas de Campaign v8. Todas las pantallas de lista son de solo lectura, excepto la lista de envío de correo electrónico."

El menú **Explorer** muestra la misma jerarquía de carpetas que la de la consola del cliente. Examine todos los componentes, las carpetas y los esquemas de Campaign v8. Todas las pantallas de lista son de solo lectura, excepto la lista de envío de correo electrónico.

Los elementos mostrados en el Explorador dependen de los permisos de usuario.

Como en cualquier pantalla de lista, puede configurar columnas para personalizar la visualización y ver toda la información que necesite. Consulte esta [sección](#list-screens).

Para obtener más información sobre el explorador de Campaign, consulte esta [documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Campaign Management

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Campañas"
>abstract="Esta es la lista de sus campañas. Puede ver información útil, como las fechas de inicio/finalización/última modificación, así como su estado. Puede filtrar la lista por estado o fechas de inicio/finalización. Las plantillas de campaña también están disponibles. Estas listas son de solo lectura."

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Entregas"
>abstract="Examine la lista de envíos. Puede ver su estado, la fecha de la última modificación y los KPI clave. Puede filtrar la lista por estado, fecha de contacto o canal. Haga clic en un envío de correo electrónico para abrir su tablero. Otros elementos son de solo lectura. Las plantillas de envío también están disponibles."

* **Campañas** - Esta es la lista de sus campañas. De forma predeterminada, puede ver las fechas de inicio/fin/última modificación, así como su estado. Puede filtrar la lista por estado o fechas de inicio/finalización. Las plantillas de campaña también están disponibles. Estas listas son de solo lectura.

* **Entregas** - Examine la lista de envíos. De forma predeterminada, puede ver su estado, la fecha de la última modificación y los KPI clave. Puede filtrar la lista por estado, fecha de contacto o canal. Haga clic en una entrega por correo electrónico para abrir su panel y obtener una descripción general de los detalles de la entrega. Los envíos de otros canales son de solo lectura. Las plantillas de envío también están disponibles en modo de solo lectura. Puede utilizar la consola de cliente para editarlas. Consulte esta [documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   Utilice la variable **Más acciones** para eliminar o duplicar una entrega.

   ![](assets/more-actions.png){width="70%" align="left"}

### Administración de clientes

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Recipients"
>abstract="Acceda a la base de datos de destinatarios. Puede ver información útil, como su dirección de correo electrónico, nombre y apellidos. Esta lista es de solo lectura."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiencias"
>abstract="Esta es su lista de audiencias. Puede ver su tipo, origen, fechas de creación/última modificación y etiqueta. Puede filtrar la lista por origen. Esta lista es de solo lectura."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Listas de suscripciones"
>abstract="Examine las listas de suscripciones. Puede ver su tipo, modo y etiqueta. Esta lista es de solo lectura."

* **Destinatarios** - Acceda a la base de datos de destinatarios. De forma predeterminada, puede ver su dirección de correo electrónico, nombre y apellidos. Esta lista es de solo lectura.
* **Audiencias** - Esta es su lista de audiencias. De forma predeterminada, puede ver su tipo, origen, fechas de creación/última modificación y etiqueta. Puede filtrar la lista por origen. Esta lista es de solo lectura.
* **Listas de suscripciones** - Examine las listas de suscripciones. De forma predeterminada, puede ver su tipo, modo y etiqueta. Esta lista es de solo lectura.
* **Flujos de trabajo de objetivos** : Acceda a su lista de flujos de trabajo de Campaign. De forma predeterminada, puede ver su estado, las fechas de procesamiento últimas/siguientes y el entorno. Puede filtrar la lista por estado, fecha de último procesamiento y tipo de flujo de trabajo. Las plantillas de flujo de trabajo también están disponibles. Estas listas son de solo lectura.

### Gestión de decisiones

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Examine la lista de ofertas de interacción. De forma predeterminada, puede ver su estado, fechas de inicio/finalización y entorno. Puede filtrar la lista por estado y fechas de inicio/finalización. También están disponibles las plantillas de oferta. Estas listas son de solo lectura."

* **Ofertas** - Examine la lista de ofertas de interacción. De forma predeterminada, puede ver su estado, fechas de inicio/finalización y entorno. Puede filtrar la lista por estado y fechas de inicio/finalización. También están disponibles las plantillas de oferta. Estas listas son de solo lectura.

## Barra superior

La barra superior de la interfaz le permite:

* comparta sus comentarios como evaluador alfa
* cambiar entre organizaciones e instancias
* cambiar entre las aplicaciones de Adobe Experience Cloud
* acceda a páginas de ayuda, póngase en contacto con el servicio de asistencia técnica y comparta sus comentarios. Puede buscar artículos de ayuda y vídeos desde el campo de búsqueda .

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Configurar pantallas de lista {#list-screens}

Varios vínculos del menú de navegación de la izquierda, por ejemplo **Entregas** o **Campañas**, mostrar listas de objetos. Estas pantallas de lista son de solo lectura, excepto la lista de envío de correo electrónico.

Para buscar elementos más rápidamente, puede utilizar la barra de búsqueda o filtrar la lista según criterios contextuales.

![](assets/filter.png){width="70%" align="left"}

Las listas se muestran en columnas. Puede mostrar información adicional cambiando la configuración de la columna. Para ello, haga clic en el icono situado en la esquina superior derecha de la lista. Puede añadir o eliminar columnas y cambiar el orden en que se muestran.

![](assets/columns.png){width="70%" align="left"}

Para ordenar los elementos de la lista, haga clic en cualquier encabezado de columna. Se muestra una flecha (arriba o abajo) que indica que la lista está ordenada en esa columna. Para las columnas numéricas o de fecha, la flecha arriba indica que la lista se ordena en orden ascendente, mientras que la flecha abajo indica un orden descendente. Para las columnas de cadena o alfanuméricas, los valores se enumeran en orden alfabético.

## Ayuda contextual y guía de incorporación

Hay disponible una ayuda contextual en la interfaz de . Cuando esté disponible, haga clic en la **?** para mostrar información de ayuda y vínculos de documentación relacionados.

![](assets/context-help.png){width="70%" align="left"}

También hay disponible una guía de integración para ayudarle a empezar a utilizar Campaign v8 Web. Haga clic en el icono en la esquina inferior derecha, elija uno de los escenarios paso a paso disponibles y simplemente siga las instrucciones.

![](assets/onboarding.png){width="70%" align="left"}

## Navegadores admitidos {#browsers}

La web de Campaign v8 está diseñada para funcionar de forma óptima en la última versión de Google Chrome, Safari y Microsoft Edge. Es posible que tenga problemas al utilizar determinadas funciones en versiones anteriores u otros navegadores.

## Preferencias de idioma {#language-pref}

La web de Campaign v8 está disponible actualmente en los siguientes idiomas:

<table>
<tr>
<td>
<p>Inglés (EE. UU.) - EN-US</p>
<p>Francés - FR</p>
<p>Alemán - DE</p>
<p>Italiano - IT</p>
</td>
<td>
<p>Español - ES</p>
<p>Portugués (Brasil) - PTBR</p>
<p>Japonés: JP</p>
</td>
<td>
<p>Coreano - KR</p>
<p>Chino simplificado - CHS</p>
<p>Chino tradicional - CHT</p>
</td>
</tr>
</table>

El idioma predeterminado de la interfaz está determinado por el idioma preferido especificado en el perfil de usuario.

Para cambiar el idioma:

1. Haga clic en el icono de perfil, en la parte superior derecha, y luego seleccione **Preferencias**.

   ![](assets/preferences.png){width="70%" align="left"}

1. A continuación, haga clic en el idioma mostrado debajo de su dirección de correo electrónico.

   ![](assets/preferences2.png)

1. Seleccione el idioma preferido y haga clic en **Guardar**. Puede seleccionar un segundo idioma en caso de que el componente que esté utilizando no esté localizado en su primer idioma.

   ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->

>[!CONTEXTUALHELP]
>id="acw_sms_report_overview"
>title="Resumen del informe SMS"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_push_report_overview"
>title="Resumen del informe push"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Plantilla de notificaciones push"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Propiedades de creación de campañas"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="Programación de creación de campañas"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Atributos avanzados del Generador de reglas"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Métricas enviadas"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Métricas de errores"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Insertar contenido de Android"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="Insertar contenido de iOS"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_content"
>title="Contenido de SMS"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Suscriptores de la aplicación"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Población de ensayo"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Modo de vista previa"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Datos de enriquecimiento"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalización"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Selección de archivos"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definición de columnas"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parámetros de formato"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="Envío de informes"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="Seguimiento de informes"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Información general sobre la creación de informes"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Estadísticas de objetivo de informes"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="Creación de informes acumulados seleccionar una entrega"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Propiedades de campaña"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Lista de flujos de trabajo"
>abstract="Por determinar"

<!--BETA-->
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campos de deduplicación"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configuración de deduplicación"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Complemento de deduplicación"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Complemento de Dimension"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Permiso obligatorio"
>abstract="Por determinar"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Permiso obligatorio"
>abstract="Por determinar"
