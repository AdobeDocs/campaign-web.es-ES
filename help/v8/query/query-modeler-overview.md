---
audience: end-user
title: Trabajar con el modelador de consultas
description: Aprenda a trabajar con el modelador de consultas web de Adobe Campaign.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 21%

---

# Trabajar con el modelador de consultas {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="Nuevo modelador de consultas"
>abstract="Adobe Campaign Web incluye un modelador de consultas que simplifica el proceso de filtrado de bases de datos para seleccionar destinos específicos según diversos criterios. Incluye el uso de expresiones avanzadas y operadores. El modelador de consultas está disponible en todos los contextos en los que necesite definir reglas para filtrar los datos."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Modelador de consultas"
>abstract="Defina criterios de filtrado para destinatarios o cualquier otra dimensión de segmentación de la base de datos. Aproveche el público de Adobe Experience Platform para detallar aún más el público destinatario y maximizar el impacto de su campaña."

La interfaz de usuario web de Adobe Campaign incluye un modelador de consultas que simplifica el proceso de filtrado de la base de datos en función de diversos criterios. Garantiza la compatibilidad total con las consultas creadas en la consola del cliente, lo que facilita una transición sin problemas a la interfaz de usuario web.

Además, el modelador de consultas puede administrar consultas muy complejas y largas de forma eficaz, lo que ofrece una mayor flexibilidad y precisión. Además, admite filtros predefinidos dentro de las condiciones, lo que le permite refinar las consultas con facilidad mientras utiliza expresiones avanzadas y operadores para estrategias completas de segmentación y segmentación de audiencia.

## Acceso al modelador de consultas

El modelador de consultas está disponible en todos los contextos en los que necesite definir reglas para filtrar los datos.

| Uso | Ejemplo |
|  ---  |  ---  |
| **Definir audiencias**: especifique la población a la que desea dirigirse en los mensajes o flujos de trabajo y cree nuevas audiencias adaptadas a sus necesidades sin esfuerzo. [Aprenda a crear audiencias](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Personalizar actividades de flujo de trabajo**: aplique reglas dentro de las actividades de flujo de trabajo, como **Split** y **Reconciliación**, para cumplir con sus requisitos específicos. [Descubra más información sobre las actividades de flujo de trabajo](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Filtros predefinidos**: Cree filtros predefinidos que sirvan de accesos directos durante varias operaciones de filtrado, tanto si trabaja con listas de datos como si forma la audiencia para una entrega. [Aprenda a trabajar con filtros predefinidos](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Filtrado de datos de informes**: Añada una regla para filtrar los datos mostrados en los informes. [Aprenda a trabajar con informes](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Personalización de listas**: Cree reglas personalizadas para filtrar los datos mostrados en listas como destinatarios, envíos, listas, etc. [Obtenga información sobre cómo filtrar listas](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |
| **Creación de contenido condicional**: haga que el contenido del correo electrónico sea dinámico mediante la creación de condiciones que definan qué contenido debe mostrarse a distintos destinatarios, lo que garantiza mensajes personalizados y relevantes. [Aprenda a crear contenido condicional](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} |

## Interfaz del modelador de consultas {#interface}

El modelador de consultas proporciona un lienzo central en el que generar la consulta y un panel derecho que proporciona información sobre la misma.

![](assets/query-interface.png){zoomable="yes"}

### El lienzo central {#canvas}

El lienzo central del modelador de consultas es donde se agregan y combinan los diferentes componentes de la creación de la consulta. [Obtenga información sobre cómo crear una consulta](build-query.md)

La barra de herramientas situada en la esquina superior derecha del lienzo proporciona opciones para manipular fácilmente los componentes de la consulta y desplazarse por el lienzo:

* **Modo de selección múltiple**: seleccione varios componentes de filtrado para copiarlos y pegarlos en la ubicación que desee.
* **Rotar**: cambie el lienzo verticalmente.
* **Ajustar a pantalla**: adapte el nivel de zoom del lienzo a la pantalla.
* **Alejar** / **Ampliar**: Aleje o en el lienzo.
* **Mostrar mapa**: abre una instantánea del lienzo en el que se muestra que se encuentra.

### El panel Propiedades de la regla {#rule-properties}

En el lado derecho, la **[!UICONTROL Propiedades de regla]** Este panel proporciona información sobre la consulta. Permite realizar varias operaciones para comprobar la consulta y asegurarse de que se adapta a sus necesidades. [Obtenga información sobre cómo comprobar y validar la consulta](build-query.md#check-and-validate-your-query)
