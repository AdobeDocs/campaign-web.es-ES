---
audience: end-user
title: Notas de la versión 8 de la web de Campaign
description: Notas de la versión 8 de la web de Campaign
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 100%

---


# Notas de la versión {#release-notes}

Esta página incluye las últimas funciones y mejoras de la versión 8 de la web de Campaign.

## Versión alfa{#alpha-release}

Esta nueva interfaz web de Campaign actualmente solo está disponible para **profesionales de alfa** con las siguientes capacidades:

**Experiencia moderna, intuitiva y unificada**

La nueva IU de la web de Campaign ofrece una nueva experiencia del usuario, alineada con todas las soluciones y aplicaciones de Adobe Experience Cloud. Ofrece lo siguiente:

* Acceso a la nueva interfaz y a otras soluciones de Adobe con una sola sesión de usuario compartida
* Una nueva experiencia de navegación. Todos los menús y carpetas están disponibles en el carril izquierdo
* Conmutadores de soluciones y organizaciones de la barra superior
* Integración con Unified Shell, con acceso directo a la comunidad, al centro de ayuda y soporte
<!--
No search and pulse notifications in Alpha
-->

Obtenga más información sobre la nueva IU en [esta página](../get-started/user-interface.md).

**Cree, inicie y mida su campaña de correo electrónico**

Utilice la nueva IU de la web de Campaign para lo siguiente:

* Crear contenido de correo electrónico personalizado con el diseñador de correo electrónico: [más información](../content/edit-content.md)
* Definir audiencias de destinatarios con el generador de reglas: [más información](../audience/about-audiences.md)
* Previsualización, prueba y envío de mensajes de correo electrónico: [Más información](../monitor/prepare-send.md)
* Monitorizar el envío y medir los resultados con informes integrados: [Más información](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## Actualizaciones terminológicas{#terminology-updates}

Como usuario existente de Campaign, tenga en cuenta que se ha cambiado el nombre de algunos conceptos para que se ajusten a los estándares terminológicos más recientes. Estos cambios solo se aplican a la IU de la web de Campaign y no se reflejan en la Consola del cliente. Se encuentran detalladas a continuación.

* Ahora, las pruebas son **correos electrónicos de prueba**: para enviar una prueba, utilice el botón **Prueba** en la IU para envío de correo electrónico. El destinatario de las pruebas ahora se denomina **Perfiles de prueba**
* Las direcciones semilla ahora se utilizan como **Perfiles de prueba**: envíe el correo electrónico de prueba a las direcciones semilla, que son destinatarios adicionales y ficticios en la base de datos
* El análisis del envío ahora es la **preparación del envío**. Cuando necesite iniciar el análisis, haga clic en el botón **Preparar**
* La vista previa del correo electrónico ya está disponible a través del botón **Simular contenido**
* Las listas son ahora **Audiencias**

## Limitaciones{#limitations-alpha}

Algunas funciones clave de Campaign, como las campañas en canales múltiples y administración de flujos de trabajo, estarán disponibles con la versión Beta.

Las limitaciones siguientes se aplican a esta versión alfa:

* Los únicos objetos editables son los envíos. Los demás son de solo lectura. Utilice los filtros para explorarlos todos.
* Esta versión está diseñada para una de las campañas de correo electrónico. Otros canales aún no son compatibles.
* La interfaz de usuario de Administración no está disponible.
* Las métricas de creación de informes (como aperturas y datos de seguimiento) se actualizan cada hora.
* Los KPI del panel de envío se actualizan cada cinco minutos. Sin embargo, la preparación del envío es en tiempo real.
* Las notificaciones de Adobe Experience Cloud y la Ayuda unificada disponibles en la barra superior aún no están integradas.

