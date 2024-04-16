---
audience: end-user
title: Descubra la interfaz
description: Interfaz de usuario de Adobe Campaign Web
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: c2382359ee6777277fa9dd4f8fd4282fb2381b38
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 98%

---

# Descubra la interfaz {#user-interface}

La nueva interfaz de Adobe Campaign Web ofrece una experiencia de usuario moderna e intuitiva para simplificar el diseño y el envío de las campañas de marketing. Esta nueva interfaz está integrada con las aplicaciones y soluciones de Adobe Experience Cloud.

Aprenda a conectarse a Adobe Campaign y descubra conceptos básicos de navegación de Experience Cloud [en este artículo](connect-to-campaign.md).


>[!NOTE]
>
>Esta documentación se actualiza frecuentemente para reflejar los cambios recientes en la interfaz de usuario del producto. Sin embargo, algunas capturas de pantalla pueden diferir ligeramente de la interfaz de usuario.

## Página de inicio de Campaign {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Recientes"
>abstract="La lista **Recientes** proporciona accesos directos a los envíos creados y modificados recientemente. Esta lista muestra su canal, estado, propietario y fechas de creación y modificación."

La página de inicio de Campaign permite examinar rápida y fácilmente recursos, indicadores y componentes clave.

La sección superior de la página de inicio proporciona detalles sobre las últimas actualizaciones y las nuevas funcionalidades disponibles en el producto, con vínculo a las Notas de la versión y documentación detallada. Utilice la flecha izquierda para desplazarse por las tarjetas de características.

![](assets/home.png){zoomable=&quot;yes&quot;}

Los **indicadores clave de rendimiento** le permiten comprobar la eficacia de la plataforma mediante indicadores clave de rendimiento (KPI) frecuentes. Obtenga más información acerca de los indicadores clave de rendimiento (KPI) en [esta página](../reporting/kpis.md).

La lista **Recientes** proporciona accesos directos a los envíos creados y modificados recientemente. Esta lista muestra su canal, estado, propietario y fechas de creación y modificación. Haga clic en el vínculo **Mostrar más** para cargar más envíos.

Además, puede acceder a las páginas de ayuda principales de Adobe Campaign Web desde la sección **Aprendizaje** de la página.

## Menú de navegación izquierdo {#user-interface-left-nav}

Examine los vínculos de la izquierda para acceder a las funcionalidades de Adobe Campaign Web. Varios vínculos muestran listas de objetos que se pueden ordenar y filtrar. También puede configurar columnas para que muestren toda la información que necesite. Consulte esta [sección](#list-screens). Algunas pantallas de lista son de solo lectura. Los elementos mostrados en el menú de navegación de la izquierda dependen de los permisos de usuario. Puede obtener más información sobre permisos en [esta sección](permissions.md).


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

  ![](assets/more-actions.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}

* **Flujos de trabajo**: en esta pantalla, puede acceder a la lista completa de flujos de trabajo y plantillas de flujo de trabajo. Puede comprobar su estado, las fechas de última/siguiente ejecución y crear un nuevo flujo de trabajo o una nueva plantilla de flujo de trabajo. Puede filtrar la lista con los mismos criterios que para otros objetos. Además, puede filtrar los flujos de trabajo que pertenecen o no a una campaña. Puede obtener más información sobre los flujos de trabajo [en esta sección](../workflows/gs-workflows.md).


### Administración de contenido {#user-interface-content-management}

En la sección ADMINISTRACIÓN DE CONTENIDO, puede ver las plantillas y fragmentos de contenido.

* **Plantillas de contenido**: para un proceso de diseño acelerado y mejorado, puede crear plantillas independientes para reutilizar fácilmente el contenido personalizado en [!DNL Adobe Campaign]. Esta funcionalidad, que solo está disponible para correos electrónicos, permite a los usuarios orientados a contenido trabajar en plantillas independientes para que los usuarios de marketing puedan reutilizarlas y adaptarlas dentro de sus propias campañas de correo electrónico. Obtenga más información en [esta sección](../email/create-email-templates.md).

<!--
* **Fragments** -
-->

### Administración de clientes {#user-interface-customer-management}

En la sección ADMINISTRACIÓN DE CLIENTES, puede ver los perfiles, los públicos y las suscripciones. Estas listas son de solo lectura.

* **Perfiles**: cree y administre perfiles, y acceda a la base de datos de destinatarios. De forma predeterminada, puede ver su dirección de correo electrónico, nombre y apellidos. Más información sobre perfiles en [esta sección](../audience/about-recipients.md).
* **Públicos**: esta es su lista de públicos. De forma predeterminada, puede ver su tipo, origen, fechas de creación/última modificación y etiqueta. Puede filtrar la lista por origen. Obtenga más información sobre públicos y listas en [esta sección](../audience/about-recipients.md).
* **Servicios de suscripciones**: examine las listas de suscripciones. De manera predeterminada, puede ver su tipo, modo y etiqueta. Obtenga información sobre cómo administrar suscripciones y bajas en [Documentación de Adobe Campaign v8 (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=es){target="_blank"}.
* **Filtros predefinidos**: los filtros predefinidos son filtros personalizados que se crean y guardan para que estén disponibles para su uso futuro. Se pueden utilizar como accesos directos durante cualquier operación de filtrado con el modelador de consultas, por ejemplo, al filtrar una lista de datos o crear el público de un envío. Obtenga más información en [esta sección](predefined-filters.md).


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

* **Informes**: la entrada **Informe** ofrece un resumen general consolidado de las métricas de tráfico y participación de cada canal dentro del entorno de Campaign. Estos informes constan de varios widgets, cada uno de los cuales ofrece una perspectiva distinta sobre el rendimiento de la campaña o del envío. Obtenga más información en [esta sección](../reporting/global-reports.md).


## Ayuda contextual {#user-interface-help}

Hay disponible una ayuda contextual en la interfaz. Cuando esté disponible, haga clic en el icono `?` para mostrar la información de ayuda y los vínculos de documentación relacionados.

![](assets/do-not-localize/context-help.png){zoomable=&quot;yes&quot;}{width="40%" align="left"}

Actualmente disponible como versión Beta dentro de la nueva interfaz web de Campaign, el **asistente de conocimientos con tecnología de IA** integrado dentro de la ayuda contextual revoluciona la búsqueda de documentación y la respuesta a preguntas sobre procedimientos al examinar sin esfuerzo amplios repositorios de documentación y localizar al instante la información precisa que necesita.

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

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Envío de informes globales"
>abstract="Las métricas de la creación de informes de seguimiento se pueden ver en esta pantalla"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Seguimiento de informes globales"
>abstract="Las métricas de la creación de informes de seguimiento se pueden ver en esta pantalla"


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

<!--ML: not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Simulación de selección de perfiles de prueba"
>abstract="Simulación de selección de perfiles de prueba"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Simulación de envío de perfiles de prueba"
>abstract="Simulación de envío de perfiles de prueba"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="Simulación de registro de correo electrónico"
>abstract="Simulación de registro de correo electrónico"

<!-- ML: beta wiki page - not visible in UI-->

<!-- FOR POST-GA -->



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
>title="Esta plantilla es de solo lectura"
>abstract="No tiene permisos para editar esta plantilla. Si es necesario, póngase en contacto con el administrador para que le conceda acceso."

<!-- Subscription activity-->

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Página de aterrizaje predeterminada"
>abstract="Seleccione la página de aterrizaje predeterminada asociada a este servicio de suscripción."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Actividad del servicio de suscripción"
>abstract="Utilice Adobe Campaign para crear y monitorizar sus servicios, como los boletines informativos, y para comprobar las suscripciones o las bajas a estos servicios. Las suscripciones solo se aplican al envío de correo electrónico y SMS."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Parámetros del servicio de suscripción"
>abstract="Seleccione y confirme la configuración del servicio de suscripción."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Transición saliente de servicios de suscripción"
>abstract="Alterne la opción **Generar una transición saliente** para añadir una transición después de la actividad."


<!--Update file-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata"
>title="Actualización de datos"
>abstract="La actividad **Actualizar datos** realiza una actualización en masa de los campos de la base de datos."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_operationtype"
>title="Seleccione cómo actualizar los datos"
>abstract="El campo **Tipo de operación** permite elegir el proceso que se realizará sobre los datos de la base de datos. Seleccione la primera opción para añadir datos o actualizarlos (si ya se han añadido). También puede solo añadir, actualizar o eliminar datos. Seleccione **Actualizar y combinar colecciones** para seleccionar un registro principal al que vincular duplicados y eliminarlos de forma segura."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_recordid"
>title="Identificación de registro"
>abstract="Especifique cómo identificar los registros de la base de datos: si los datos están relacionados con una dimensión de segmentación existente, seleccione la opción **Uso de la dimensión de segmentación** y seleccione la dimensión de segmentación y los campos que desea actualizar. De lo contrario, especifique uno o más vínculos personalizados para identificar los datos en la base de datos o use directamente las claves de reconciliación."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_fieldsupdate"
>title="Seleccione los campos que desea actualizar"
>abstract="Seleccione los campos que desea actualizar y la configuración de reconciliación. Puede utilizar la opción **Asignación automática** para identificar automáticamente los campos que se van a actualizar."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_advancedoptions"
>title="Opciones avanzadas para actualizar datos"
>abstract="La sección **Opciones avanzadas** le permite especificar configuraciones adicionales para administrar datos y duplicados."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition"
>title="Generar una transición saliente"
>abstract="Alterne la opción **Generar una transición saliente** para añadir una transición saliente que se activará al final de la ejecución de la actividad **Actualizar datos**. Por lo general, la actualización marca el final de un flujo de trabajo de segmentación y, por lo tanto, la opción no está activada de forma predeterminada."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition_rejects"
>title="Genere una transición saliente para rechazos."
>abstract="Alternar la opción **Generar una transición saliente para rechazos** para añadir una transición saliente que contenga registros que no se hayan procesado correctamente después de la actualización (por ejemplo, si hay un duplicado). Por lo general, la actualización marca el final de un flujo de trabajo de segmentación y, por lo tanto, la opción no está activada de forma predeterminada."



<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Señal externa"
>abstract="La actividad **Señal externa** le permite activar la ejecución de un conjunto de tareas en un flujo de trabajo desde una API u otro flujo de trabajo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Parámetros de señal externa"
>abstract="Parámetros de señal externa"


>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Activadores finales"
>abstract="Activadores finales"


<!--JavaScript-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="Código JavaScript"
>abstract="La actividad de **Código JavaScript** ejecuta un código JavaScript en el contexto de un flujo de trabajo. "

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="Fragmento de JavaScript"
>abstract="Configure el código que se va a ejecutar."
>additional-url="https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/developer/api" text="Más información en la documentación de Campaign v8 (consola)"


>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="Ejecución de Javascript"
>abstract="De forma predeterminada, la fase de ejecución no puede exceder de 1 hora. Tras este retraso, el proceso se anula con un mensaje de error y la ejecución de la actividad falla. Alterne la opción **Detener ejecución después** para definir un retraso personalizado. Para omitir este límite, establezca el valor en 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="Errores de proceso"
>abstract="Alternar la opción **Errores de proceso** para añadir una transición saliente que contenga errores."



<!--ExtractFile-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Extracción de archivos"
>abstract="Extraer actividad de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="Archivo que extraer"
>abstract="Seleccione el archivo que va a extraer."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Formato de destino"
>abstract="Seleccione el formato."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Posprocesamiento"
>abstract="Definir un paso de posprocesamiento"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Transición saliente"
>abstract="Alternar la opción **Generar una transición saliente** para añadir una transición saliente después de la actividad actual."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Errores de proceso"
>abstract="Alterne la opción **Errores de proceso** para añadir una transición saliente que contenga errores."

<!-- Workflow settings -->

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initscript"
>title="Script de inicialización"
>abstract="Script de inicialización"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_properties"
>title="Propiedades de ejecución"
>abstract="Propiedades de ejecución"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_error"
>title="Error de ejecución"
>abstract="Error de ejecución"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_initscript"
>title="Script de inicialización de ejecución"
>abstract="Script de inicialización de ejecución"


<!--incremental querry -->

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Consulta incremental"
>abstract="Consulta incremental"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Historial de consultas incrementales"
>abstract="Historial de consultas incrementales"


<!-- Transfer file activity -->

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="Transferencia de archivo"
>abstract="Transferencia de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="Opciones de transferencia de archivos"
>abstract="Opciones de transferencia de archivos"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="Transferir actividad de archivo"
>abstract="Transferir actividad de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="Transferir archivo al servidor remoto"
>abstract="Transferir archivo al servidor remoto"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Transferir origen de archivo"
>abstract="Transferir origen de archivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Eliminar los archivos de origen después de la transferencia"
>abstract="Eliminar los archivos de origen después de la transferencia"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Mostrar los registros de sesión"
>abstract="Mostrar los registros de sesión"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Mostrar todos los archivos"
>abstract="Mostrar todos los archivos"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="File historization"
>abstract="File historization"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Procesar archivos que faltan"
>abstract="Procesar archivos que faltan"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Errores de proceso"
>abstract="Errores de proceso"

>[!CONTEXTUALHELP]
>id="acw_deliveries_alerting"
>title="Alertas de envío"
>abstract="Alertas de envío"
