---
audience: end-user
title: Notas de la versión de Campaign Web v8
description: Notas de la versión de Campaign Web v8
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---


# Notas de la versión {#release-notes}

Esta página lista las últimas funciones y mejoras de Campaign Web v8.

## Versión Alpha{#alpha-release}

Esta nueva interfaz web de Campaign actualmente solo está disponible para **Profesionales alfa** con las siguientes capacidades:

**Experiencia moderna, intuitiva y unificada**

La nueva interfaz de usuario web de Campaign ofrece una nueva experiencia de usuario, alineada con todas las soluciones y aplicaciones de Adobe Experience Cloud. Ofrece:

* Acceso a la nueva interfaz y a otras soluciones de Adobe con una sola sesión de usuario compartida
* Nueva experiencia de navegación, con todos los menús y carpetas disponibles en el carril izquierdo
* Conmutadores de soluciones y organizaciones de la barra superior
* Integración con Unified Shell, con acceso directo a la comunidad, el centro de ayuda y el soporte
<!--
No search and pulse notifications in Alpha
-->

Obtenga más información sobre la nueva interfaz de usuario en [esta página](../get-started/user-interface.md).

**Cree, inicie y mida su campaña de correo electrónico**

Utilice la nueva interfaz de usuario web de Campaign para:

* Diseñe contenido de correo electrónico personalizado con el creador de correo electrónico: [Más información](../content/edit-content.md)
* Defina audiencias de destino con el generador de reglas: [Más información](../audience/about-audiences.md)
* Previsualización, prueba y envío de mensajes de correo electrónico: [Más información](../monitor/prepare-send.md)
* Monitorice el envío y mida los resultados con informes integrados: [Más información](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## Actualizaciones terminológicas{#terminology-updates}

Como usuario existente de Campaign, tenga en cuenta que se ha cambiado el nombre de algunos conceptos para que se ajusten a los estándares terminológicos más recientes. Estos cambios solo se aplican a la interfaz de usuario web de Campaign y no se reflejan en la consola de cliente. Se resumen a continuación.

* Las pruebas ahora **Probar correos electrónicos**: para enviar una prueba, utilice la variable **Prueba** en la interfaz de usuario de envío de correo electrónico. El objetivo de las pruebas objetivo ahora se denomina **Perfiles de prueba**
* Las direcciones semilla ahora se utilizan como **Perfiles de prueba**: enviar el correo electrónico de prueba a las direcciones semilla, que son destinatarios adicionales y ficticios de la base de datos
* El análisis de entrega ahora es **preparación de entregas**. Cuando necesite iniciar el análisis, haga clic en el botón **Preparación** botón
* La vista previa del correo electrónico ya está disponible a través del **Simular contenido** botón
* Las listas ahora **Audiencias**

## Limitaciones{#limitations-alpha}

Algunas funciones clave de Campaign, como campañas en canales múltiples y administración de flujos de trabajo, estarán disponibles con la versión Beta.

Las limitaciones siguientes se aplican a esta versión Alpha:

* Los únicos objetos editables son Envíos. Los demás son de solo lectura. Utilice filtros para explorarlos todos.
* Esta versión está diseñada para una de las campañas de correo electrónico. Otros canales aún no son compatibles.
* La interfaz de usuario de Administración no está disponible.
* Las métricas de informes (como aperturas y datos de seguimiento) se actualizan cada hora.
* Los KPI del panel de envío se actualizan cada 5 minutos. - pero la preparación de la entrega es en tiempo real.
* Las notificaciones de Adobe Experience Cloud y la Ayuda unificada disponibles en la barra superior aún no están integradas.

