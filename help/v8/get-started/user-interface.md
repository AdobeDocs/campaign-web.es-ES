---
audience: end-user
title: Descubra la interfaz
description: Interfaz de usuario web de Campaign v8
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 050d97695dd2012644af4a35eca3e6cd9f5f02af
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 2%

---

# Descubra la interfaz {#user-interface}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Descubra la interfaz"
>abstract="La nueva interfaz web de Campaign v8 ofrece una experiencia de usuario integrada, intuitiva y coherente."

La nueva interfaz web de Campaign v8 ofrece una experiencia de usuario moderna e intuitiva para simplificar el diseño y la entrega de las campañas de marketing. Esta nueva interfaz está integrada con Adobe Experience Platform.

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

## Menú de navegación izquierdo

Examine los vínculos de la izquierda para acceder a las funciones web de Campaign v8. Varios vínculos muestran listas de objetos que se pueden ordenar y filtrar. También puede configurar columnas para mostrar toda la información que necesite. Consulte esta [sección](#list-screens). Todas las pantallas de lista son de solo lectura, excepto la lista de envío de correo electrónico. Hacer clic en cualquier elemento de la lista para editarlo o visualizarlo no está disponible en Alpha. Todas las listas se podrán editar en versiones futuras. Los elementos que se muestran en el menú de navegación de la izquierda dependen de los permisos de usuario.

![](assets/home.png)

### Inicio

Esta pantalla incluye vínculos clave y recursos para acceder rápidamente a las principales funciones web de Campaign v8. El **Recientes** proporciona accesos directos a los envíos creados y modificados recientemente. Esta lista muestra sus fechas de creación y modificación, así como el estado.

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

Acceda a las páginas de ayuda de claves web de Campaign v8 desde la sección inferior de la página principal.

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### Explorer

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="El **Explorer** El menú muestra la misma jerarquía de carpetas que la de la consola del cliente. Examine todos los componentes, carpetas y esquemas de Campaign v8. Todas las pantallas de lista son de solo lectura, excepto la lista de envío de correo electrónico."

El **Explorer** El menú muestra la misma jerarquía de carpetas que la de la consola del cliente. Examine todos los componentes, carpetas y esquemas de Campaign v8. Todas las pantallas de lista son de solo lectura, excepto la lista de envío de correo electrónico.

Los elementos que se muestran en el Explorador dependen de los permisos de usuario.

Al igual que en cualquier pantalla de lista, puede configurar columnas para personalizar la visualización y ver toda la información que necesite. Consulte esta [sección](#list-screens).

Para obtener más información sobre el explorador de Campaign, consulte [documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/ac-ui/campaign-ui.html#ac-explorer-ui){target="_blank"}.
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### Campaign Management

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="Campañas"
>abstract="Esta es la lista de sus campañas. Puede ver información útil como las fechas de inicio, finalización o última modificación, así como su estado. Puede filtrar la lista por estado o por fechas de inicio y finalización. Las plantillas de campaña también están disponibles. Estas listas son de solo lectura."

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Entregas"
>abstract="Examine la lista de envíos. Puede ver su estado, la fecha de la última modificación y los indicadores clave de rendimiento (KPI). Puede filtrar la lista por estado, fecha de contacto o canal. Haga clic en una entrega de correo electrónico para abrir su panel. Otros elementos son de solo lectura. También hay disponibles plantillas de envío."

* **Campañas** : Esta es la lista de sus campañas. De forma predeterminada, puede ver sus fechas de inicio, finalización y última modificación, así como su estado. Puede filtrar la lista por estado o por fechas de inicio y finalización. Las plantillas de campaña también están disponibles. Estas listas son de solo lectura.

* **Envíos** - Examine la lista de envíos. De forma predeterminada, puede ver su estado, la fecha de la última modificación y los KPI clave. Puede filtrar la lista por estado, fecha de contacto o canal. Haga clic en una entrega de correo electrónico para abrir su panel y obtener una descripción general de los detalles de la entrega. Las entregas de otros canales son de solo lectura. Las plantillas de envío también están disponibles en modo de solo lectura. Puede utilizar la consola del cliente para editarlos. Ver esto [documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   Utilice el **Más acciones** para eliminar o duplicar una entrega.

   ![](assets/more-actions.png){width="70%" align="left"}

### Administración de clientes

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Recipients"
>abstract="Acceso a la base de datos de destinatarios. Puede ver información útil, como su dirección de correo electrónico, nombre y apellidos. Esta lista es de solo lectura."

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Audiencias"
>abstract="Esta es su lista de audiencias. Puede ver su tipo, origen, fechas de creación/última modificación y etiqueta. Puede filtrar la lista por origen. Esta lista es de solo lectura."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Listas de suscripciones"
>abstract="Examine las listas de suscripciones. Puede ver su tipo, modo y etiqueta. Esta lista es de solo lectura."

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Flujos de trabajo de segmentación"
>abstract="Acceda a la lista de flujos de trabajo de Campaign. Puede ver su estado, las fechas de procesamiento última/siguiente y el entorno. Puede filtrar la lista por estado, última fecha de procesamiento y tipo de flujo de trabajo. Las plantillas de flujo de trabajo también están disponibles. Estas listas son de solo lectura."

* **Destinatarios** : Acceda a la base de datos de destinatarios. De forma predeterminada, puede ver su dirección de correo electrónico, nombre y apellidos. Esta lista es de solo lectura.
* **Audiencias** - Esta es su lista de audiencias. De forma predeterminada, puede ver su tipo, origen, fechas de creación/última modificación y etiqueta. Puede filtrar la lista por origen. Esta lista es de solo lectura.
* **Listas de suscripciones** - Navega por tus listas de suscripciones. De forma predeterminada, puede ver su tipo, modo y etiqueta. Esta lista es de solo lectura.
* **Flujos de trabajo de objetivos** : Acceda a la lista de flujos de trabajo de Campaign. De forma predeterminada, puede ver su estado, las fechas de procesamiento pasadas/siguientes y el entorno. Puede filtrar la lista por estado, última fecha de procesamiento y tipo de flujo de trabajo. Las plantillas de flujo de trabajo también están disponibles. Estas listas son de solo lectura.

### Gestión de decisiones

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Examine la lista de ofertas de interacción. De forma predeterminada, puede ver su estado, las fechas de inicio y finalización y el entorno. Puede filtrar la lista por estado y fechas de inicio y finalización. Las plantillas de oferta también están disponibles. Estas listas son de solo lectura."

* **Ofertas** : Examine la lista de ofertas de interacción. De forma predeterminada, puede ver su estado, las fechas de inicio y finalización y el entorno. Puede filtrar la lista por estado y fechas de inicio y finalización. Las plantillas de oferta también están disponibles. Estas listas son de solo lectura.

## Barra superior

La barra superior de la interfaz de le permite:

* compartir sus comentarios como probador alfa
* cambiar entre organizaciones e instancias
* cambiar entre las aplicaciones de Adobe Experience Cloud
* acceda a las páginas de ayuda, póngase en contacto con el servicio de asistencia y comparta comentarios. Puede buscar artículos de ayuda y vídeos en el campo de búsqueda.

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## Configuración de pantallas de lista {#list-screens}

Varios vínculos del menú de navegación izquierdo, por ejemplo **Envíos** o **Campañas**, muestra listas de objetos. Estas pantallas de lista son de solo lectura, excepto la lista de envío de correo electrónico.

Para buscar elementos más rápido, puede utilizar la barra de búsqueda o filtrar la lista en función de criterios contextuales.

![](assets/filter.png){width="70%" align="left"}

Las listas se muestran en columnas. Puede mostrar información adicional cambiando la configuración de la columna. Para ello, haga clic en el icono en la esquina superior derecha de la lista. Puede agregar o quitar columnas y cambiar el orden en que se muestran.

![](assets/columns.png){width="70%" align="left"}

Puede ordenar los elementos de la lista haciendo clic en cualquier encabezado de columna. Se muestra una flecha (Arriba o Abajo) que indica que la lista está ordenada en esa columna. En el caso de las columnas numéricas o de fecha, la flecha Arriba indica que la lista se ordena en orden ascendente, mientras que la flecha Abajo indica un orden descendente. En el caso de las columnas de cadena o alfanuméricas, los valores se enumeran en orden alfabético.

## Ayuda contextual y guía de incorporación

Hay disponible una ayuda contextual en la interfaz. Cuando esté disponible, haga clic en **?** para mostrar la información de ayuda y los vínculos de documentación relacionados.

![](assets/context-help.png){width="70%" align="left"}

También hay disponible una guía de incorporación para ayudarle a empezar a utilizar la Web de Campaign v8. Haga clic en el icono en la esquina inferior derecha, elija uno de los escenarios paso a paso disponibles y simplemente siga las instrucciones.

![](assets/onboarding.png){width="70%" align="left"}

## Navegadores admitidos {#browsers}

La versión 8 de Campaign Web está diseñada para funcionar de forma óptima en la última versión de Google Chrome, Safari y Microsoft Edge. Es posible que tenga problemas al utilizar determinadas funciones en versiones anteriores u otros exploradores.

## Preferencias de idioma {#language-pref}

La versión 8 de la web de Campaign está disponible actualmente en los siguientes idiomas:

<table>
<tr>
<td>
<p>Inglés (Estados Unidos) - EN-US</p>
<p>Francés (FR)</p>
<p>Alemán (DE)</p>
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

1. Haga clic en el icono de su perfil, en la parte superior derecha, y luego seleccione **Preferencias**.

   ![](assets/preferences.png){width="70%" align="left"}

1. A continuación, haga clic en el idioma mostrado en su dirección de correo electrónico.

   ![](assets/preferences2.png)

1. Seleccione su idioma preferido y haga clic en **Guardar**. Puede seleccionar un segundo idioma en caso de que el componente que utilice no esté localizado en su primer idioma.

   ![](assets/select-language.png)

<!--
## Supported browsers {#browsers}

Adobe Campaign interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
-->

>[!CONTEXTUALHELP]
>id="acw_sms_report_overview"
>title="Resumen del informe SMS"
>abstract="Por definir"

>[!CONTEXTUALHELP]
>id="acw_push_report_overview"
>title="Resumen del informe push"
>abstract="Por definir"

>[!CONTEXTUALHELP]
>id="acw_import_from_a_file"
>title="Importación de una audiencia desde un archivo"
>abstract="Por definir"

>[!CONTEXTUALHELP]
>id="acw_import_from_a_file_formatting"
>title="Configuración de formato"
>abstract="Por definir"

>[!CONTEXTUALHELP]
>id="acw_import_from_a_file_columns"
>title="Configuración de columnas"
>abstract="Por definir"

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Plantilla de notificaciones push"
>abstract="Por definir"
