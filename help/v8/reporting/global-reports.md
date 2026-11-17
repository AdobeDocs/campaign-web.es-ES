---
audience: end-user
title: Introducción a los informes globales
description: Comprender los informes globales
exl-id: e64d9765-f602-4fee-9923-a3665130c63a
TQID: 'https://experienceleague.adobe.com/UG5Dn-gdKdU1PfOUmCtoVzAjuYRG4pUPwGggZq2diiQ'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 62a8e2ac2a726b568e3c25b4e435d4de2f305b5f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 18%
---
# Introducción a los informes globales {#global-report-gs}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_global_report"
>title="Informe global"
>abstract="Los informes globales ofrecen una forma potente y eficaz de analizar el rendimiento de la campaña. Estos informes proporcionan una vista consolidada de las métricas clave de tráfico y participación de cada canal dentro de la campaña."

Los **informes globales** constituyen una herramienta eficaz que ofrece un resumen global consolidado de las métricas de tráfico y participación para cada canal dentro de la instancia de Campaign. Estos informes constan de varios widgets, cada uno de los cuales ofrece una perspectiva distinta sobre el rendimiento de la campaña o el envío.

Los indicadores clave de rendimiento (KPI) se actualizan cada hora, lo que garantiza perspectivas actualizadas. De forma predeterminada, los filtros de datos abarcan los últimos 30 días, lo que ofrece una perspectiva actual y relevante del rendimiento de sus campañas y envíos.

La lista completa de informes y las métricas asociadas para cada canal están disponibles en las siguientes páginas:

* [Informes globales de correo electrónico](global-report-email.md)
* [Informes globales de SMS](global-report-sms.md)
* [Informes globales push](global-report-push.md)
* [Informes globales de correo directo](global-report-direct.md)

## Administrar el tablero de informes {#manage-reports}

Para acceder y administrar sus informes globales, siga estos pasos:

1. Vaya al menú **[!UICONTROL Informes]** dentro de la sección **[!UICONTROL Informes]**.

1. En el menú de la izquierda, seleccione un informe de la lista y navegue por la pestaña para mostrar los datos de cada canal.

   ![Captura de pantalla que muestra el menú izquierdo y las pestañas para navegar por los datos de cada canal](assets/global_report_manage_3.png){zoomable="yes"}

1. En el tablero, elija **Inicio** y **[!UICONTROL Hora de finalización]** para segmentar datos específicos.

   ![Captura de pantalla que muestra el panel con opciones para seleccionar la hora de inicio y finalización para la segmentación de datos](assets/global_report_manage_1.png){zoomable="yes"}

1. En el campo **[!UICONTROL Seleccionar carpeta]**, seleccione si desea segmentar envíos o campañas desde una carpeta específica.

   ![Captura de pantalla que muestra el campo de la carpeta de selección para seleccionar envíos o campañas](assets/global_report_manage_2.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Agregar reglas]** para empezar a crear consultas y filtrar mejor los datos de informes. [Aprenda a utilizar el modelador de consultas](../query/query-modeler-overview.md).

1. Entre las **[!UICONTROL URL y los flujos de clics]**, elija los **[!UICONTROL vínculos más visitados]** o el **[!UICONTROL período de tiempo]**.

   Las opciones de **[!UICONTROL Ver por]** permiten filtrar por direcciones URL, etiquetas o categorías.

## Informes del canal LINE {#line-reports}

A continuación, se describen los informes disponibles para el canal LINE.

### Información general sobre el envío {#line-delivery-overview}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_line_deliveries_overview"
>title="Resumen del envío de LINE"
>abstract="Ver mensajes para enviar, mensajes enviados y errores de entrega para LINE."

El informe **[!UICONTROL Resumen de entrega]** muestra los mensajes que se van a enviar, los mensajes enviados y los errores de entrega de LINE.

### Público objetivo {#line-targeted-audience}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_line_targeted_audience"
>title="Audiencia objetivo de LINE"
>abstract="Vea la audiencia a la que se dirige el envío LINE y los resultados de envío resultantes."

El gráfico y la tabla **[!UICONTROL Audiencia objetivo]** muestran la audiencia objetivo del envío LINE y los resultados de envío resultantes.

### Estadísticas de envío {#line-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_line_delivery_stats"
>title="Estadísticas de envío de LINE"
>abstract="Vea los resultados clave de entrega de los mensajes de LINE, incluidos los mensajes que se van a enviar, los mensajes enviados y los errores de entrega."

El gráfico y la tabla **[!UICONTROL Delivery statistics]** muestran los resultados clave de entrega de los mensajes de LINE, incluidos los mensajes que se van a enviar, los mensajes enviados y los errores de entrega.

### Causas de exclusión {#line-exclusions}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_line_exclusions"
>title="Causas de exclusión de LINE"
>abstract="Vea por qué se excluyeron los perfiles objetivo del envío de LINE, como la elegibilidad, la validación o las reglas de configuración."

El gráfico y la tabla **[!UICONTROL Causas de exclusión]** muestran por qué se excluyeron los perfiles objetivo de la entrega LINE, como la elegibilidad, la validación o las reglas de configuración.

### Rendimiento del envío {#line-delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_line"
>title="Rendimiento de entrega de LINE"
>abstract="Ver la tasa de envío de mensajes de LINE a lo largo del tiempo."

El informe **[!UICONTROL Rendimiento de entrega]** muestra la velocidad de envío de los mensajes de LINE a lo largo del tiempo.
