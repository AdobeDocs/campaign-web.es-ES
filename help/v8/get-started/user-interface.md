---
audience: end-user
title: Descubra la interfaz
description: Interfaz de usuario de Adobe Campaign Web
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 9657343409e2c577aac90320d403006af0250e7a
workflow-type: tm+mt
source-wordcount: '2011'
ht-degree: 82%

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

![](assets/home.png){zoomable="yes"}

Los **indicadores clave de rendimiento** le permiten comprobar la eficacia de la plataforma mediante indicadores clave de rendimiento (KPI) frecuentes. Obtenga más información acerca de los indicadores clave de rendimiento (KPI) en [esta página](../reporting/kpis.md).

La lista **Recientes** proporciona accesos directos a los envíos creados y modificados recientemente. Esta lista muestra su canal, estado, propietario y fechas de creación y modificación. Haga clic en el vínculo **Mostrar más** para cargar más envíos.

Además, puede acceder a las páginas de ayuda principales de Adobe Campaign Web desde la sección **Aprendizaje** de la página.

### Acerca del vínculo {#user-interface-about}


>[!CONTEXTUALHELP]
>id="acw_about"
>title="Página Acerca de"
>abstract="La página Acerca de proporciona detalles sobre la instancia de Adobe Campaign"

>[!CONTEXTUALHELP]
>id="acw_about_instance"
>title="Acerca de la instancia"
>abstract="La sección Instancia proporciona información clave sobre el cliente de la consola, incluida la versión y el número de compilación asociado"

>[!CONTEXTUALHELP]
>id="acw_about_web"
>title="Acerca de la web"
>abstract="La sección Web muestra la versión de la interfaz de usuario web de Campaign, con la última fecha de actualización de la misma, si está disponible."

>[!CONTEXTUALHELP]
>id="acw_about_packages"
>title="Acerca de los paquetes instalados"
>abstract="La sección Paquetes instalados enumera todos los módulos, funciones e integraciones presentes en la instancia."

En la parte inferior de la página, el vínculo **[!UICONTROL Acerca de]** proporciona detalles acerca de su instancia de Adobe Campaign. esa información está en modo de solo lectura.

![](assets/about-link.png){zoomable="yes"}

La sección **Instance** proporciona información clave sobre su cliente de consola, incluidos la **versión** y el número **build** asociado.

* La **versión** hace referencia a la versión oficial que está utilizando,
* La **compilación** hace referencia a una iteración específica de esa versión.

Tanto los números de versión como los de compilación son cruciales para la resolución de problemas, ya que ayudan a determinar exactamente qué funciones y correcciones están presentes en su entorno.

La sección **Web** muestra la versión de la interfaz de usuario web de Campaign, con la última fecha de actualización, si está disponible. Esto ayuda a realizar un seguimiento de los cambios o mejoras realizados en la interfaz de usuario web de Campaign.

La sección **Paquetes instalados** enumera todos los módulos, características e integraciones presentes en su instancia. Estos paquetes amplían la funcionalidad de Adobe Campaign, lo que le permite realizar tareas especializadas como la integración con otras soluciones de Adobe o la activación de flujos de trabajo específicos. Dado el gran número de paquetes, puede realizar un estudio dentro de esta sección para comprobar rápidamente si hay un módulo en particular instalado en la instancia.

![](assets/about.png){zoomable="yes"}

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

  ![](assets/more-actions.png){zoomable="yes"}{width="70%" align="left"}

* **Flujos de trabajo**: en esta pantalla, puede acceder a la lista completa de flujos de trabajo y plantillas de flujo de trabajo. Puede comprobar su estado, las fechas de última/siguiente ejecución y crear un nuevo flujo de trabajo o una nueva plantilla de flujo de trabajo. Puede filtrar la lista con los mismos criterios que para otros objetos. Además, puede filtrar los flujos de trabajo que pertenecen o no a una campaña. Puede obtener más información sobre los flujos de trabajo [en esta sección](../workflows/gs-workflows.md).


### Administración de contenido {#user-interface-content-management}

En la sección ADMINISTRACIÓN DE CONTENIDO, puede ver las plantillas y fragmentos de contenido.

* **Plantillas de contenido**: para un proceso de diseño acelerado y mejorado, puede crear plantillas independientes para reutilizar fácilmente el contenido personalizado en [!DNL Adobe Campaign]. Esta funcionalidad, que solo está disponible para correos electrónicos, permite a los usuarios orientados a contenido trabajar en plantillas independientes para que los usuarios de marketing puedan reutilizarlas y adaptarlas dentro de sus propias campañas de correo electrónico. Obtenga más información en [esta sección](../email/create-email-templates.md).

* **Fragmentos**: un fragmento es un componente reutilizable al que se puede hacer referencia en uno o varios envíos de distintas campañas. Al modificar un fragmento, se actualiza todo el contenido que lo utiliza. [Aprenda a trabajar con fragmentos](../content/fragments.md)

Esta funcionalidad se utiliza para la construcción previa de múltiples bloques de contenido personalizado que pueden ser utilizados por los usuarios de marketing para combinar rápidamente los contenidos de correo electrónico en un proceso de diseño mejorado.

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

### Administración {#left-nav-admin}


* **Pista de auditoría**: la entrada **Pista de auditoría** proporciona a los usuarios una visibilidad completa de todas las modificaciones realizadas en entidades importantes dentro de la instancia, normalmente aquellas que afectan significativamente al funcionamiento sin problemas de la instancia. [Más información](../reporting/audit-trail.md)

* **Cuentas externas**: cree nuevas cuentas externas usando la interfaz de usuario web para satisfacer sus necesidades específicas y garantizar transferencias de datos sin problemas. [Más información](../administration/external-account.md)

* **Esquemas**: los campos personalizados son atributos adicionales agregados a los esquemas predeterminados a través de la consola de Adobe Campaign. [Más información](../administration/custom-fields.md)

* **Alerta de entrega** - Alerta de entrega es un sistema de administración de alertas que permite a grupos de usuarios recibir automáticamente notificaciones por correo electrónico con información sobre sus ejecuciones de entrega. [Más información](../msg/delivery-alerting.md)

<!--
## Contextual Help {#user-interface-help} 

A contextual help is available in the interface. When available, click on the `?` icon to display help information and related documentation links. 

![](assets/do-not-localize/context-help.png){zoomable="yes"}{width="40%" align="left"}

Currently released as a Beta version within the new Campaign Web user interface, the **AI-powered Knowledge Assistant** embedded within contextual help revolutionizes documentation searching and answering how-to questions with effortlessly sifting through vast documentation repositories, instantly pinpointing the precise information you need.

Thanks to Campaign Gen AI's capabilities, this assistant transforms your experience, making information retrieval and problem-solving a breeze. Whether you're seeking guidance in a complex task or navigating extensive documents, our AI-powered Knowledge Assistant is your ultimate companion, providing unmatched efficiency and accuracy in every interaction.

Learn more in [this section](using-ai.md).

-->

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

<!-- IDs -->


>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields"
>title="Editar atributos personalizados"
>abstract="Editar atributos personalizados"



<!--Schema-->

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Esquema"
>abstract="Esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_type"
>title="Tipos de esquema"
>abstract="Tipos de esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_properties"
>title="Propiedades del esquema"
>abstract="Esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_existing"
>title="Seleccionar esquema existente"
>abstract="Esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_external"
>title="Seleccionar base de datos externa"
>abstract="Esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_add_tables"
>title="Añadir tablas"
>abstract="Esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_logs_tasks"
>title="Registros y tareas de flujo de trabajo"
>abstract="Esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_update"
>title="Actualizar base de datos"
>abstract="Esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_update_script"
>title="Actualizar script"
>abstract="Esquema"

>[!CONTEXTUALHELP]
>id="acw_schema_start_update"
>title="Iniciar actualización de base de datos"
>abstract="Esquema"
