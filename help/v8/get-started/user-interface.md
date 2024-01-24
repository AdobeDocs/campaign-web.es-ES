---
audience: end-user
title: Descubra la interfaz
description: Interfaz de usuario de la web de la versión 8 de Campaign
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Disponibilidad limitada"
source-git-commit: 59929983859687081859e007b4e3b48a6279edee
workflow-type: tm+mt
source-wordcount: '1646'
ht-degree: 80%

---

# Descubra la interfaz {#user-interface}

La nueva interfaz de la web de la versión 8 de Campaign ofrece una experiencia de usuario moderna e intuitiva para simplificar el diseño y el envío de las campañas de marketing. Esta nueva interfaz está integrada con las aplicaciones y soluciones de Adobe Experience Cloud.

Obtenga información sobre cómo conectarse a Adobe Campaign y descubrir conceptos básicos de navegación para Experience Cloud [en este artículo](connect-to-campaign.md).


>[!NOTE]
>
>Esta documentación se actualiza frecuentemente para reflejar los cambios recientes en la interfaz de usuario del producto. Sin embargo, algunas capturas de pantalla pueden diferir ligeramente de la interfaz de usuario.

## Página de inicio de Campaign {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Recientes"
>abstract="La lista **Recientes** proporciona accesos directos a los envíos creados y modificados recientemente. Esta lista muestra sus fechas de canal, estado, propietario, creación y modificación."

La página de inicio de Campaign permite examinar rápida y fácilmente recursos, indicadores y componentes clave.

La sección superior de la página de inicio proporciona detalles sobre las últimas actualizaciones y las nuevas funciones disponibles en el producto, con vínculo a las Notas de la versión y documentación detallada. Utilice la flecha izquierda para desplazarse por las tarjetas de características.

![](assets/home.png)

Los **indicadores clave de rendimiento** le permiten comprobar la eficacia de la plataforma mediante indicadores clave de rendimiento (KPI) frecuentes. Obtenga más información acerca de los indicadores clave de rendimiento (KPI) en [esta página](../reporting/kpis.md).

La lista **Recientes** proporciona accesos directos a los envíos creados y modificados recientemente. Esta lista muestra sus fechas de canal, estado, propietario, creación y modificación. Haga clic en el vínculo **Mostrar más** para cargar más envíos.

Además, puede acceder a las páginas de ayuda con claves web de Campaign v8 desde el **Aprendizaje** de la página.

## Menú de navegación izquierdo {#user-interface-left-nav}

Examine los vínculos de la izquierda para acceder a las funciones de la web de la versión 8 de Campaign. Varios vínculos muestran listas de objetos que se pueden ordenar y filtrar. También puede configurar columnas para que muestren toda la información que necesite. Consulte esta [sección](#list-screens). Algunas pantallas de lista son de solo lectura. Los elementos mostrados en el menú de navegación de la izquierda dependen de los permisos de usuario. Puede obtener más información sobre permisos en [esta sección](permissions.md).


### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="El menú **Explorer** muestra todos los componentes y objetos de Campaign con la misma jerarquía de carpetas que la de la consola del cliente. Examine todos los componentes, carpetas y esquemas de Campaign v8, compruebe los permisos asociados y cree carpetas y subcarpetas desde este menú."

El menú **Explorer** muestra todos los recursos y objetos de Campaign con la misma jerarquía de carpetas que la consola del cliente. Examine todos los componentes, carpetas y esquemas de Campaign v8 y cree envíos, flujos de trabajo y campañas.

Los elementos mostrados en **Explorer** dependen de los permisos de usuario. También puede agregar carpetas y subcarpetas, si tiene los derechos adecuados. Puede obtener más información sobre permisos en [esta sección](permissions.md).

Puede configurar columnas para personalizar la visualización y ver toda la información que necesite. Consulte esta [sección](#list-screens). También puede agregar carpetas y subcarpetas, tal como se detalla en [esta sección](permissions.md#folders).

Para obtener más información sobre Campaign Explorer, la jerarquía de carpetas y los recursos, consulte esta sección [Documentación de Campaign v8 (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=es#ac-explorer-ui){target="_blank"}.

### Administración de campañas {#user-interface-campaign-management}

En la sección ADMINISTRACIÓN DE CAMPAÑAS, puede acceder a campañas de marketing, envíos y flujos de trabajo.

* **Campañas**: esta es la lista de sus campañas y plantillas de campaña. De forma predeterminada, para cada campaña se pueden ver las fechas de inicio, finalización, creación y última modificación, el estado actual y el nombre del operador de Campaign que la creó. Puede filtrar la lista por estado, fechas de inicio/finalización, carpeta o crear un filtro avanzado para definir sus propios criterios de filtrado. Obtenga más información acerca de las campañas de [en esta sección](../campaigns/gs-campaigns.md).

* **Envíos**: examine la lista de envíos. De forma predeterminada, puede ver su estado, la fecha de la última modificación y los KPI principales. Puede filtrar la lista por estado, fecha de contacto o canal. Haga clic en un envío de correo electrónico para abrir el panel y obtener una descripción general de los detalles del envío. Los envíos en otros canales son de solo lectura. Puede obtener más información sobre los envíos [en esta sección](../msg/gs-messages.md).

  Utilice el botón **Más acciones** para eliminar o duplicar un envío.

  ![](assets/more-actions.png){width="70%" align="left"}

* **Flujos de trabajo**: en esta pantalla, puede acceder a la lista completa de flujos de trabajo y plantillas de flujo de trabajo. Puede comprobar su estado, las fechas de última/siguiente ejecución y crear un nuevo flujo de trabajo o una nueva plantilla de flujo de trabajo. Puede filtrar la lista con los mismos criterios que para otros objetos. Además, puede filtrar los flujos de trabajo que pertenecen o no a una campaña. Puede obtener más información sobre los flujos de trabajo [en esta sección](../workflows/gs-workflows.md).


### Administración de contenido {#user-interface-content-management}

En la sección GESTIÓN DE CONTENIDO, puede ver sus plantillas de contenido y fragmentos.

* **Plantillas de contenido** : Para un proceso de diseño acelerado y mejorado, puede crear plantillas independientes para reutilizar fácilmente el contenido personalizado en [!DNL Adobe Campaign]. Esta funcionalidad, que solo está disponible para correos electrónicos, permite a los usuarios orientados a contenido trabajar en plantillas independientes para que los usuarios de marketing puedan reutilizarlas y adaptarlas dentro de sus propias campañas de correo electrónico. Obtenga más información en [esta sección](../email/create-email-templates.md).

<!--
* **Fragments** -
-->

### Administración de clientes {#user-interface-customer-management}

En la sección CUSTOMER MANAGEMENT, puede ver sus perfiles, audiencias y suscripciones. Estas listas son de solo lectura.

* **Perfiles** : Cree y administre perfiles, y acceda a la base de datos de destinatarios. De forma predeterminada, puede ver su dirección de correo electrónico, nombre y apellidos. Obtenga más información sobre los perfiles en [esta sección](../audience/about-recipients.md).
* **Públicos**: esta es su lista de públicos. De forma predeterminada, puede ver su tipo, origen, fechas de creación/última modificación y etiqueta. Puede filtrar la lista por origen. Obtenga más información sobre públicos y listas en [esta sección](../audience/about-recipients.md).
* **Servicios de suscripción** - Navega por tus listas de suscripciones. De manera predeterminada, puede ver su tipo, modo y etiqueta. Obtenga información sobre cómo administrar suscripciones y bajas en [Documentación de Adobe Campaign v8 (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=es){target="_blank"}.
* **Filtros predefinidos** - Los filtros predefinidos son filtros personalizados que se crean y guardan para que estén disponibles para su uso futuro. Se pueden utilizar como accesos directos durante cualquier operación de filtrado con el modelador de consultas, por ejemplo al filtrar una lista de datos o crear la audiencia de una entrega. Obtenga más información en [esta sección](predefined-filters.md).


### Gestión de decisiones {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Examine las listas de ofertas y las plantillas de ofertas que se han creado en la consola utilizando el módulo **Interacción**. Estas listas son de solo lectura."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=es" text="Adición de ofertas a un envío"

En la sección GESTIÓN DE DECISIONES, puede ver las ofertas y las plantillas de ofertas. Estas listas son de solo lectura.

* **Ofertas** : examine la lista de ofertas y las plantillas de ofertas que se han creado en la consola con el módulo **Interacción**. De forma predeterminada, puede ver su estado, fechas de inicio/finalización y entorno. Puede filtrar la lista por estado y fechas de inicio/finalización. También están disponibles las plantillas de oferta.

Obtenga información sobre cómo crear y enviar ofertas en correos electrónicos y SMS en [esta sección](../msg/offers.md).

### Creación de informes {#left-nav-reporting}

* **Informes** - El **Informe** Esta entrada ofrece un resumen general consolidado de las métricas de tráfico y participación de cada canal dentro del entorno de Campaign. Estos informes constan de varios widgets, cada uno de los cuales ofrece una perspectiva distinta sobre el rendimiento de la campaña o la entrega. Obtenga más información en [esta sección](../reporting/global-reports.md).


## Ayuda contextual {#user-interface-help}

Hay disponible una ayuda contextual en la interfaz. Cuando esté disponible, haga clic en el icono `?` para mostrar la información de ayuda y los vínculos de documentación relacionados.

![](assets/do-not-localize/context-help.png){width="40%" align="left"}

Lanzado como versión beta dentro de la nueva interfaz de usuario web de Campaign, el **Asistente de conocimientos con tecnología de IA** la ayuda contextual integrada revoluciona la búsqueda de documentación y la respuesta a preguntas sobre procedimientos al examinar sin esfuerzo vastos repositorios de documentación y localizar al instante la información precisa que necesita.

Gracias a las funciones Gen IA de Campaign, este asistente transforma su experiencia, lo que facilita la recuperación de información y la resolución de problemas. Tanto si busca orientación en una tarea compleja como si navega por documentos extensos, nuestro Asistente de conocimientos con tecnología de IA es su mejor compañero, ya que proporciona una eficacia y precisión inigualables en cada interacción.

Obtenga más información en [esta sección](using-ai.md).



## Más información {#learn-more}

Obtenga información sobre cómo examinar, buscar y filtrar listas disponibles en su entorno de Campaign [en esta página](list-filters.md).



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Permiso obligatorio"
>abstract="El administrador debe concederle permiso para poder crear un segmento."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Permiso obligatorio"
>abstract="El administrador debe concederle permiso para poder crear un segmento."

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Envío de informes globales"
>abstract="Las métricas de la creación de informes de seguimiento se pueden ver en esta pantalla"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Seguimiento de informes globales"
>abstract="Las métricas de la creación de informes de seguimiento se pueden ver en esta pantalla"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Lista de flujos de trabajo de una campaña"
>abstract="Lista de flujos de trabajo de una campaña"

<!-- delivery settings-->






<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->




<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="Creación de destinatarios"
>abstract="Creación de destinatarios"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Información general de tarjeta de destinatarios"
>abstract="Información general de tarjeta de destinatarios"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Puntos de contacto de destinatarios"
>abstract="Puntos de contacto de destinatarios"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Selección de suscripciones de destinatarios"
>abstract="Selección de suscripciones de destinatarios"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Lista apta de ofertas de destinatarios"
>abstract="Lista apta de ofertas de destinatarios"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Previsualización de ofertas de destinatarios"
>abstract="Previsualización de ofertas de destinatarios"

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="Perfil de sólo lectura de los destinatarios"
>abstract="Perfil de sólo lectura de los destinatarios"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Plantilla de envíos de suscripciones"
>abstract="Plantilla de envíos de suscripciones"

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Páginas de aterrizaje"
>abstract="Páginas de aterrizaje"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Propiedades de páginas de aterrizaje"
>abstract="Propiedades de páginas de aterrizaje"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Páginas de páginas de aterrizaje"
>abstract="Páginas de páginas de aterrizaje"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Programación de páginas de aterrizaje"
>abstract="Programación de páginas de aterrizaje"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Página principal de páginas de aterrizaje"
>abstract="Página principal de páginas de aterrizaje"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Suscripción a páginas de aterrizaje"
>abstract="Suscripción a páginas de aterrizaje"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Llamada a la acción de las páginas de aterrizaje"
>abstract="Llamada a la acción de las páginas de aterrizaje"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulación de las páginas de aterrizaje"
>abstract="Simulación de las páginas de aterrizaje"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Actividad no editable"
>abstract="Actividad no editable"




>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Fragmentos"
>abstract="Fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Guardar fragmentos"
>abstract="Guardar fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Creación de fragmentos"
>abstract="Creación de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Propiedades de fragmentos"
>abstract="Propiedades de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Tipo de fragmentos"
>abstract="Tipo de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Lista de fragmentos"
>abstract="Lista de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Detalles de fragmentos"
>abstract="Detalles de fragmentos"






>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Filtro de guardado de contenido condicional"
>abstract="Filtro de guardado de contenido condicional"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Filtro de selección de contenido condicional"
>abstract="Filtro de selección de contenido condicional"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Contenido condicional en la línea de asunto"
>abstract="Contenido condicional en la línea de asunto"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Condición de línea de asunto de contenido condicional"
>abstract="Condición de línea de asunto de contenido condicional"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="Simulación de perfiles de prueba"
>abstract="Simulación de perfiles de prueba"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Simulación de selección de perfiles de prueba"
>abstract="Simulación de selección de perfiles de prueba"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Simulación de envío de perfiles de prueba"
>abstract="Simulación de envío de perfiles de prueba"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="Simulación de registro de correo electrónico"
>abstract="Simulación de registro de correo electrónico"


>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Contenido para correo directo"
>abstract="Contenido para correo directo"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Propiedades de archivo para correo directo"
>abstract="Propiedades de archivo para correo directo"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Propiedades de contenido para correo directo"
>abstract="Propiedades de contenido para correo directo"


<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Mostrar atributos avanzados"
>abstract="Solo los atributos más comunes se muestran de forma predeterminada en la lista de atributos. Active el selector **Mostrar atributos avanzados** para ver todos los atributos disponibles para la lista actual en la paleta izquierda del generador de reglas, como nodos, agrupaciones, vínculos 1-1 y vínculos 1-N."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Campos avanzados del generador de reglas"
>abstract="Solo los atributos más comunes se muestran de forma predeterminada en la lista de atributos. Active el selector **Mostrar atributos avanzados** para ver todos los atributos disponibles para la lista actual en la paleta izquierda del generador de reglas, como nodos, agrupaciones, vínculos 1-1 y vínculos 1-N."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Atributos avanzados del generador de reglas"
>abstract="Solo los atributos más comunes se muestran de forma predeterminada en la lista de atributos. Active el selector **Mostrar atributos avanzados** para ver todos los atributos disponibles para la lista actual en la paleta izquierda del generador de reglas, como nodos, agrupaciones, vínculos 1-1 y vínculos 1-N."



>[!CONTEXTUALHELP]
>id="acw_contenttemplate_readonlymode"
>title="Esta plantilla solo está lista"
>abstract="Continuará"


