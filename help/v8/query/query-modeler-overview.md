---
audience: end-user
title: Trabajar con el modelador de consultas
description: Aprenda a trabajar con el modelador de consultas web de Adobe Campaign.
source-git-commit: 94350335df08ae9c24d88843c77554db1890ab4d
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 17%

---

# Trabajar con el modelador de consultas {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Modelador de consultas"
>abstract="Defina criterios de filtrado para los destinatarios o cualquier otra dimensión de segmentación de la base de datos. Aproveche el público de Adobe Experience Platform para delimitar aún más el público destinatario y maximizar el impacto de su campaña."

Adobe Campaign Web incluye un modelador de consultas que simplifica el proceso de filtrado de bases de datos para seleccionar destinos específicos según diversos criterios. Esto incluye el uso de expresiones avanzadas y operadores.

## Acceso al modelador de consultas

El modelador de consultas está disponible en todos los contextos en los que necesite definir reglas para filtrar los datos.

| Uso | Ejemplo |
|  ---  |  ---  |
| **Definir audiencias**: especifique la población a la que desea dirigirse en los mensajes o flujos de trabajo y cree nuevas audiencias adaptadas a sus necesidades sin esfuerzo. | ![](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **Personalizar actividades de flujo de trabajo**: aplique reglas dentro de las actividades de flujo de trabajo, como División y Reconciliación, para alinearse con los requisitos específicos. | ![](assets/access-workflow.png){width="200" align="center" zoomable="yes"} |
| **Filtros predefinidos**: Cree filtros predefinidos que sirvan de accesos directos durante varias operaciones de filtrado, tanto si trabaja con listas de datos como si forma la audiencia para una entrega. | ![](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **Filtrado de datos de informes**: Añada una regla para filtrar los datos mostrados en los informes. | ![](assets/access-reports.png){width="200" align="center" zoomable="yes"} |
| **Personalización de listas**: Cree reglas personalizadas para filtrar los datos mostrados en listas como destinatarios, envíos, listas, etc. | ![](assets/access-lists.png){width="200" align="center" zoomable="yes"} |



<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png)

 +++
-->


## Interfaz del modelador de consultas {#interface}

El modelador de consultas proporciona un lienzo central en el que puede agregar y combinar los diferentes componentes para crear la consulta.

En el lado derecho, el panel de propiedades de la regla proporciona información sobre la consulta. Le permite realizar varias operaciones para comprobar la consulta y asegurarse de que se adapta a sus necesidades. Obtenga información sobre cómo comprobar y validar la consulta

![](assets/query-interface.png)
