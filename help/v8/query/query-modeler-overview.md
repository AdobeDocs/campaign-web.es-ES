---
audience: end-user
title: Trabajar con el modelador de consultas
description: Aprenda a trabajar con el modelador de consultas web de Adobe Campaign.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 8006eeb6088d7d6ef99f374b2b846978cd679c01
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 18%

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

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="Refinamiento de destinatarios"
>abstract="Estas reglas solo pueden modificarse en la consola del cliente. "

La interfaz de usuario web de Adobe Campaign incluye un modelador de consultas que simplifica el proceso de filtrado de la base de datos en función de diversos criterios. Garantiza la compatibilidad total con las consultas creadas en la consola del cliente, lo que facilita una transición sin problemas a la interfaz de usuario web.

Además, el modelador de consultas administra consultas muy complejas y largas de forma eficaz, lo que ofrece una mayor flexibilidad y precisión. También admite filtros predefinidos dentro de las condiciones, lo que permite a los usuarios refinar las consultas con facilidad mientras utiliza expresiones avanzadas y operadores para estrategias completas de segmentación y segmentación de audiencia.

## Acceso al modelador de consultas

El modelador de consultas está disponible en todos los contextos en los que necesite definir reglas para filtrar los datos.

| Uso | Ejemplo |
|  ---  |  ---  |
| **Definir audiencias**: especifique la población a la que desee dirigirse en sus mensajes o flujos de trabajo y cree nuevas audiencias adaptadas a sus necesidades sin esfuerzo. [Aprenda a crear audiencias](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Imagen que muestra cómo acceder a la interfaz de creación de audiencias] |
| **Personalizar actividades de flujo de trabajo**: aplique reglas dentro de las actividades de flujo de trabajo, como **División** y **Reconciliación**, para alinearlas con sus requisitos específicos. [Más información sobre las actividades del flujo de trabajo](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [imagen que muestra cómo acceder a las opciones de personalización del flujo de trabajo] |
| **Filtros predefinidos**: Cree filtros predefinidos que sirvan de accesos directos durante diversas operaciones de filtrado, tanto si está trabajando con listas de datos como formando la audiencia para una entrega. [Aprenda a trabajar con filtros predefinidos](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [imagen que muestra cómo acceder a los filtros predefinidos] |
| **Filtrar datos de informes**: agregue reglas para filtrar los datos mostrados en los informes. [Aprenda a trabajar con informes](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Imagen que muestra cómo filtrar datos en los informes] |
| **Personalizar listas**: cree reglas personalizadas para filtrar los datos mostrados en listas como las de destinatarios o entregas. [Aprenda a filtrar listas](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [imagen que muestra cómo personalizar filtros de lista] |
| **Generar contenido condicional**: haga que el contenido del correo electrónico sea dinámico al crear condiciones que definan qué contenido debe mostrarse a distintos destinatarios, lo que garantiza mensajes personalizados y relevantes. [Aprenda a crear contenido condicional](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} [imagen que muestra cómo crear contenido condicional] |

>[!NOTE]
>
>Al acceder a un objeto creado en la consola del cliente donde se han aplicado reglas, como una audiencia o un filtro predefinido, puede mostrarse la sección **[!UICONTROL Refinar destino]**. Esto significa que se han configurado parámetros adicionales para refinar el objetivo de la regla. Estos parámetros solo se pueden modificar en la consola.
>
>![Imagen que muestra una advertencia sobre el refinamiento de destinos](assets/target-warning.png){zoomable="yes"}

## Interfaz del modelador de consultas {#interface}

El modelador de consultas proporciona un lienzo central en el que generar la consulta y un panel derecho que proporciona información sobre la misma.

>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="Nueva experiencia de usuario"
>abstract="Utilice este conmutador para cambiar entre el modelador de consultas clásico y la nueva experiencia del generador de reglas."

![Imagen que muestra la interfaz del modelador de consultas](assets/query-interface.png){zoomable="yes"}

### El lienzo central {#canvas}

El lienzo central del modelador de consultas es donde se agregan y combinan los diferentes componentes para generar la consulta. [Aprenda a crear una consulta](build-query.md)

La barra de herramientas situada en la esquina superior derecha del lienzo proporciona opciones para manipular fácilmente los componentes de la consulta y navegar por el lienzo:

* **Modo de selección múltiple**: seleccione varios componentes de filtrado para copiarlos y pegarlos en la ubicación que elija.
* **Rotar**: cambie el lienzo verticalmente.
* **Ajustar a pantalla**: adapta el nivel de zoom del lienzo a la pantalla.
* **Alejar** / **Acercar**: Aleja o acerca en el lienzo.
* **Mostrar mapa**: abre una instantánea del lienzo que muestra tu ubicación actual.

### El panel Propiedades de la regla {#rule-properties}

En el lado derecho, el panel **[!UICONTROL Propiedades de regla]** proporciona información sobre la consulta. Permite realizar varias operaciones para comprobar la consulta y asegurarse de que se adapta a sus necesidades. Este panel se muestra al crear una consulta para crear una audiencia. [Aprenda a comprobar y validar su consulta](build-query.md#check-and-validate-your-query)