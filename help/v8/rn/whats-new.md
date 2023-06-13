---
audience: end-user
title: Novedades de la versión 8 de Campaign Web
description: Descubra la nueva funcionalidad que se incluye con Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 61%

---


# Novedades {#new}

## Versión Alpha 2.0{#alpha-release}

Esta nueva interfaz web de Campaign actualmente solo está disponible para **profesionales de alfa** con las siguientes capacidades:

**Experiencia moderna, intuitiva y unificada**

La nueva IU de la web de Campaign ofrece una nueva experiencia del usuario, alineada con todas las soluciones y aplicaciones de Adobe Experience Cloud. Ofrece lo siguiente:

* Acceso a la nueva interfaz y a las demás soluciones de Adobe con una sola sesión de usuario compartida
* Una nueva experiencia de navegación. Todos los menús y carpetas están disponibles en el carril izquierdo
* Conmutadores de soluciones y organizaciones de la barra superior
* Integración con Unified Shell, con acceso directo a la comunidad, al centro de ayuda y soporte

**Nuevas y potentes funciones y procesos sin problemas**

* Interfaz de lienzo de flujo de trabajo reinventada para diseñar y administrar sus procesos
* Contenido dinámico para ofrecer experiencias con un alto nivel de segmentación y personalización a su audiencia
* Integración nativa con audiencias de Adobe Experience Platform
* Administración de plantillas para flujos de trabajo, envíos, campañas y contenido

Obtenga más información sobre la nueva IU en [esta página](../get-started/user-interface.md).

**Cree, inicie y mida su campaña**

Utilice la nueva IU de la web de Campaign para lo siguiente:

* Crear contenido de correo electrónico personalizado con el diseñador de correo electrónico: [más información](../content/edit-content.md)
* Envíe campañas en canales múltiples, incluidos SMS y notificaciones push.
* Definir audiencias de destinatarios con el generador de reglas: [más información](../audience/about-audiences.md)
* Previsualización, prueba y envío de mensajes de correo electrónico: [Más información](../monitor/prepare-send.md)
* Monitorizar el envío y medir los resultados con informes integrados: [Más información](../reporting/delivery-reports.md)


## Transición a la IU web de Campaign

Como usuario de Campaign, puede seguir accediendo a la consola del cliente para crear y administrar recursos y componentes de Campaign. Los datos y la configuración se sincronizan de un entorno a otro. Obtenga más información en [esta sección](../get-started/get-started.md#about-campaign-client-consoleac-client).

Además, todos los datos y la configuración ya disponibles en la consola del cliente se pueden ver en la interfaz de usuario de Campaign Web desde la navegación izquierda del explorador. Obtenga más información sobre la vista del explorador en [esta sección](../get-started/user-interface.md#explorer-user-interface-explorer).


## Actualizaciones terminológicas {#terminology-updates}

Como usuario existente de Campaign, tenga en cuenta que se ha cambiado el nombre de algunos conceptos para que se ajusten a los estándares terminológicos más recientes. Estos cambios solo se aplican a la interfaz de usuario web de Campaign y no se reflejan en la consola del cliente. Se encuentran detalladas a continuación.

* Ahora, las pruebas son **correos electrónicos de prueba**: para enviar una prueba, utilice el botón **Prueba** en la IU para envío de correo electrónico. El destinatario de las pruebas ahora se denomina **Perfiles de prueba**.
* Las direcciones semilla ahora se utilizan como **Perfiles de prueba**: envíe el correo electrónico de prueba a las direcciones semilla, que son destinatarios adicionales y ficticios en la base de datos.
* El análisis del envío ahora es la **preparación del envío**. Cuando necesite iniciar el análisis, haga clic en el botón **Preparar**.
* La vista previa del correo electrónico ya está disponible a través del botón **Simular contenido.**
* Las listas son ahora **Audiencias**.

## Limitaciones{#limitations-alpha}

Las limitaciones siguientes se aplican a esta versión alfa:

* Los únicos objetos editables son Deliveries, Campaigns, Workflows, Audiences y Templates. Los demás son de solo lectura. Utilice los filtros para explorarlos todos.
* Las audiencias no se pueden guardar para un uso futuro.
* La interfaz de usuario de Administración no está disponible.
* Las métricas de creación de informes (como aperturas y datos de seguimiento) se actualizan cada hora.
* Los KPI del panel de envío se actualizan cada cinco minutos. Sin embargo, la preparación del envío es en tiempo real.
* Las notificaciones de Adobe Experience Cloud y la Ayuda unificada disponibles en la barra superior aún no están integradas.

