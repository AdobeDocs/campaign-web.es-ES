---
audience: end-user
title: Informes de envío de correo electrónico
description: Obtenga información sobre cómo acceder y utilizar los informes de envío por correo electrónico
badge: label="Beta"
source-git-commit: cc58e6bcf030885ba364df7dfd51de797117120c
workflow-type: tm+mt
source-wordcount: '2205'
ht-degree: 29%

---

# Informe de envío de correo electrónico {#email-report}

El **Informe de envío de correo electrónico** ofrece información y datos completos específicos del canal de correo electrónico. Proporciona información detallada sobre el rendimiento, la eficacia y los resultados de sus envíos individuales, lo que le proporciona una visión general completa.

## Resumen de envíos {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Informes que envían"
>abstract="él **Enviando** dentro del informe proporciona una perspectiva detallada de las interacciones de los visitantes con las entregas y cualquier posible error que hayan encontrado."

### Población de públicos destinatarios iniciales {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Población de públicos destinatarios iniciales"
>abstract="El **Población de destinatarios iniciales** El gráfico muestra datos relativos a los destinatarios y los mensajes, en función de los resultados de la preparación de envíos."

El **[!UICONTROL Población de destinatarios iniciales]** El gráfico muestra datos relativos a los destinatarios. Las métricas se calculan durante la preparación de la entrega y muestran: la audiencia inicial, el número de mensajes que se van a enviar y el número de destinatarios excluidos.

![](assets/reporting_email_1.png){width="50%" align="center" zoomable="yes"}

Pase el ratón sobre una parte del gráfico para ver el número exacto.

![](assets/reporting_email_1.1.png){width="50%" align="center" zoomable="yes"}


+++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

* **[!UICONTROL Audiencia inicial]**: Número total de destinatarios objetivo.

* **[!UICONTROL Para enviar]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Exclusión]**: Número total de destinatarios excluidos de la población objetivo.
+++

### Estadísticas de entrega {#email-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Estadísticas de entrega"
>abstract="El **Estadísticas de envío** El gráfico detalla el éxito de su envío y los errores que se han producido."


El **[!UICONTROL Estadísticas de envío]** el gráfico detalla el éxito de su envío. Las métricas se detallan a continuación.

![](assets/reporting_email_2.png){width="50%" align="center" zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

* **[!UICONTROL Mensaje enviado]**: Número total de mensajes que desea enviar después de la preparación de la entrega.

* **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Errores]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

* **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

+++

### Causas de exclusión  {#email-delivery-exclusions}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Estadísticas de entrega"
>abstract="El **Causas de exclusión** el gráfico y la tabla muestran el desglose por regla de mensajes rechazados durante la preparación de la entrega."


El **[!UICONTROL Causas de exclusión]** el gráfico y la tabla muestran el desglose por regla de mensajes rechazados durante la preparación de la entrega. Las reglas de exclusión se detallan en la sección [Documentación de Campaign v8 (consola)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/reporting_email_3.png){align="center" zoomable="yes"}

+++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

* **[!UICONTROL Usuario desconocido]**: Tipo de error generado durante la entrega para indicar que la dirección de correo electrónico no es válida.

* **[!UICONTROL Dominio no válido]**: Tipo de error generado al realizar una entrega para indicar que el dominio de la dirección de correo electrónico es incorrecto o no existe.

* **[!UICONTROL Buzón lleno]**: Tipo de error generado después de cinco intentos de entrega para indicar que la bandeja de entrada de los destinatarios contiene demasiados mensajes.

* **[!UICONTROL Cuenta deshabilitada]**: Tipo de error generado al realizar una entrega para indicar que la dirección ya no existe.

* **[!UICONTROL Rechazado]**: Tipo de error generado cuando el IAP (Proveedor de acceso a Internet) rechaza una dirección, por ejemplo, al aplicar una regla de seguridad (software antispam).

* **[!UICONTROL Inalcanzable]**: Tipo de error que se produce en la cadena de distribución de mensajes: incidencia en la retransmisión SMTP, dominio temporalmente inaccesible, etc.

* **[!UICONTROL No conectado]**: Tipo de error que indica que el teléfono móvil de los destinatarios está apagado o desconectado de la red en el momento de la entrega.

+++

## Rendimiento del envío {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Widget de rendimiento del envío"
>abstract="El **Rendimiento del envío** Este informe presenta información detallada sobre el rendimiento de entrega de toda la plataforma en un periodo de tiempo especificado."

Este informe presenta información detallada sobre el rendimiento de entrega de toda la plataforma en un periodo de tiempo especificado. La métrica principal utilizada para medir la velocidad de entrega de mensajes es el número de mensajes enviados por hora.

![](assets/reporting_email_3.1.png){align="center" zoomable="yes"}


## Estadísticas de difusión {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Widget de estadísticas de difusión"
>abstract="El **Estadísticas de difusión** El informe contiene los datos disponibles sobre los posibles errores encontrados con cada dominio."

El **[!UICONTROL Estadísticas de difusión]** contiene los datos disponibles de los posibles errores encontrados con cada dominio. Las métricas se detallan a continuación.

![](assets/reporting_email_4.png){align="center" zoomable="yes"}

+++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

* **[!UICONTROL Correos electrónicos procesados]**: Número total de mensajes procesados por el servidor de envío.

* **[!UICONTROL Entregado]**: porcentaje del número de mensajes procesados correctamente comparado con el número total de mensajes procesados.

* **[!UICONTROL Rechazos graves]**: porcentaje del número de rechazos &quot;graves&quot; y errores permanentes, como una dirección de correo electrónico incorrecta, comparado con el número total de mensajes procesados.

* **[!UICONTROL Rechazos leves]**: porcentaje del número de rechazos &quot;leves&quot;, errores temporales como una bandeja de entrada llena, comparado con el número total de mensajes procesados

* **[!UICONTROL Aperturas]**: porcentaje del número de destinatarios objetivo que abrieron un mensaje al menos una vez comparado con el número de mensajes procesados correctamente.

* **[!UICONTROL Clics]**: porcentaje del número de personas que hizo clic en una entrega al menos una vez comparado con el número de mensajes procesados correctamente.

* **[!UICONTROL Baja de suscripciones]**: porcentaje del número de clics en un vínculo de baja de suscripción comparado con el número de mensajes procesados correctamente.
+++

## Envíos que no se pueden entregar {#non-deliverables-email}

### Desglose de errores por tipo {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Desglose de errores por tipo"
>abstract="El **Desglose de errores por tipo** La tabla y el gráfico contienen los datos disponibles para cada tipo de error encontrado: usuario desconocido, buzón lleno, dominio no válido y más."

El **[!UICONTROL Desglose de errores por tipo]** La tabla y el gráfico contienen los datos disponibles para el tipo de error. Las métricas se detallan a continuación.

Los errores que se muestran en este informe activan el proceso de cuarentena. Para obtener más información sobre la administración de cuarentena, consulte [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=es){target="_blank"}.

![](assets/campaign_report_email_6.png){align="left" zoomable="yes"}

+++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

* **[!UICONTROL Usuario desconocido]**: Tipo de error generado durante la entrega para indicar que la dirección de correo electrónico no es válida.

* **[!UICONTROL Dominio no válido]**: Tipo de error generado al realizar una entrega para indicar que el dominio de la dirección de correo electrónico es incorrecto o no existe.

* **[!UICONTROL Buzón lleno]**: Tipo de error generado después de cinco intentos de entrega para indicar que la bandeja de entrada de los destinatarios contiene demasiados mensajes.

* **[!UICONTROL Cuenta deshabilitada]**: Tipo de error generado al realizar una entrega para indicar que la dirección ya no existe.

* **[!UICONTROL Rechazado]**: Tipo de error generado cuando el IAP (Proveedor de acceso a Internet) rechaza una dirección, por ejemplo, al aplicar una regla de seguridad (software antispam).

* **[!UICONTROL Inalcanzable]**: Tipo de error que se produce en la cadena de distribución de mensajes: incidencia en la retransmisión SMTP, dominio temporalmente inaccesible, etc.

* **[!UICONTROL No conectado]**: Tipo de error que indica que el teléfono móvil de los destinatarios está apagado o desconectado de la red en el momento de la entrega.

+++


### Desglose de errores por dominio {#email-delivery-breakdown-domain}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Desglose de errores por dominio"
>abstract="El **Desglose de errores por dominio** La tabla y el gráfico muestran los datos disponibles para cada tipo de error encontrado según cada dominio."


El **[!UICONTROL Desglose de errores por dominio]** La tabla y el gráfico muestran los datos disponibles para detectar los posibles errores encontrados con cada dominio.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Haga clic en el icono situado junto al nombre de cada dominio para ver los detalles.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Las métricas disponibles son las mismas que para el [Desglose de errores por tipo](#email-delivery-breakdown-type) descrito anteriormente.

## Indicadores de seguimiento {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Seguimiento de creación de informes"
>abstract="El **Seguimiento** dentro de su informe ofrece datos valiosos, incluido el comportamiento de los destinatarios por vínculo, el desglose de aperturas y clics, así como información detallada sobre las direcciones URL donde se hace clic con más frecuencia durante una entrega."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Widget de tasa de apertura y clics"
>abstract="El **Tasa de apertura y clics** La tabla muestra datos relativos a la participación de los destinatarios en el envío."

### Estadísticas de entrega  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Estadísticas de entrega"
>abstract="El **Estadísticas de envío** Este informe proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre los datos disponibles para los correos electrónicos enviados: éxito, aperturas, clics, etc."


El **[!UICONTROL Estadísticas de envío]** Este informe proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre los datos disponibles para los correos electrónicos enviados. Las métricas se detallan a continuación.

![](assets/reporting_email_5.png){align="center"}

+++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

* **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Aperturas distintas]**: Número total de destinatarios objetivo que abrieron un mensaje al menos una vez.

* **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

* **[!UICONTROL Clics en el vínculo de no participación]**: Número de clics en el vínculo de baja de suscripción.

* **[!UICONTROL Clicks on the mirror link]** : número de clics en el vínculo a la página espejo.

* **[!UICONTROL Estimation of forwards]** : estimación del número de correos electrónicos reenviados por los destinatarios objetivo.
+++

### Tasa de clics y de apertura {#email-tracking-click-through}

El **[!UICONTROL Tasa de apertura y clics]** La tabla muestra datos relativos a los destinatarios. Las métricas se detallan a continuación.

![](assets/reporting_email_6.png){align="center"}

+++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

* **[!UICONTROL Enviado]**: Número total de mensajes enviados.

* **[!UICONTROL Complaints]** : número de mensajes de este dominio que el destinatario ha notificado como no deseados.

* **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

* **[!UICONTROL Clicks]** : número de destinatarios objetivo diferentes que hicieron clic en el mismo entrega al menos una vez.

* **[!UICONTROL Raw reactivity]** : porcentaje del número de destinatarios que hicieron clic en una entrega al menos una vez comparado con el número de destinatarios que abrieron una entrega al menos una vez.
+++

## URL y flujos de clics {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="Widget de URL y flujos de clics"
>abstract="El **URL y flujos de clics** Este informe proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre las direcciones URL en las que se hizo clic con mayor frecuencia durante una entrega."

* El **[!UICONTROL URL y flujos de clics]** Este informe proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre las direcciones URL en las que se hizo clic con mayor frecuencia durante una entrega.

  ![](assets/reporting_email_7.png){align="center"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Reactivity]** : la proporción del número de destinatarios objetivo que han hecho clic en una entrega en relación con el número estimado de destinatarios objetivo que han abierto una entrega.

   * **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Platform average]** : la tasa promedio, mostrada debajo de cada tasa (reacción, distintos clics y clics acumulados), se calcula para los envíos realizados durante los seis meses anteriores. Solo se tienen en cuenta los envíos con la misma tipología y en el mismo canal. Se excluyen las pruebas.

+++

* **[!UICONTROL Los 10 vínculos más visitados]** el gráfico y la tabla contienen los datos disponibles sobre el comportamiento del destinatario por vínculo.

  ![](assets/reporting_email_8.png){align="center"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Porcentaje]**: porcentaje de usuarios que interactuaron con el envío.

+++

* **[!UICONTROL Desglose de los clics a lo largo del tiempo]** El gráfico contiene los datos disponibles sobre el comportamiento del destinatario por vínculo.

  ![](assets/reporting_email_9.png){align="center"}

## Actividades de usuario {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Widget de actividades de usuario"
>abstract="El **Actividades de usuario** El gráfico muestra el desglose de aperturas y clics en forma de gráfico. Puede elegir el periodo de tiempo para los datos de destino: último día, hora o 30 minutos."

El **[!UICONTROL Actividades de usuario]** Este informe muestra el desglose de aperturas y clics en forma de gráfico. Puede elegir el periodo de tiempo para los datos de destino: último día, hora o 30 minutos.

![](assets/reporting_email_10.png){align="center"}

+++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

* **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

* **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

+++

## Estadísticas de seguimiento {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Widget de estadísticas de seguimiento"
>abstract="El **Estadísticas de seguimiento** El gráfico proporciona estadísticas sobre aperturas y clics. Tiene la opción de seleccionar el lapso de tiempo específico para los datos de destino."

El **[!UICONTROL Estadísticas de seguimiento]** El gráfico proporciona estadísticas sobre aperturas y clics. Tiene la opción de seleccionar el lapso de tiempo específico para los datos de destino.

![](assets/reporting_email_11.png){align="center"}

+++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

* **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

* **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

+++

## Desglose de aperturas {#breakdown-opens}


### Desglose de aperturas por dispositivo {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Desglose por dispositivos"
>abstract="El **Desglose por dispositivo** Este informe muestra el desglose de las aperturas por dispositivo durante el periodo. Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y en dispositivos móviles. El segundo muestra el número exacto y el porcentaje para cada tipo de dispositivo."

El **Desglose por dispositivo** Este informe muestra el desglose de aperturas por dispositivo durante el periodo: equipos personales, dispositivos Android, dispositivos Apple u otros.

Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y en dispositivos móviles. El segundo muestra el número exacto y el porcentaje para cada tipo de dispositivo.

![](assets/reporting_email_13.png){align="center"}


### Desglose de aperturas por sistema operativo {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Desglose por sistema operativo"
>abstract="El **Desglose por sistema operativo** Este informe muestra el desglose de las aperturas por sistema operativo durante el periodo correspondiente. El primer gráfico muestra estadísticas relacionadas con las aperturas en un equipo y en dispositivos móviles. El segundo muestra el número exacto y el porcentaje de cada sistema operativo."

El **Desglose por sistema operativo** Este informe muestra el desglose de aperturas por sistema operativo durante el periodo: sistemas Windows, Android, iOS u otros.

Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y en sistemas operativos móviles. El segundo muestra el número exacto y el porcentaje de cada sistema operativo.

![](assets/reporting_email_13.1.png){align="center"}

### Desglose de aperturas por explorador {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Desglose por explorador"
>abstract="El **Desglose por explorador** muestra el desglose de aperturas por explorador para el periodo. El primer gráfico muestra estadísticas relacionadas con las aperturas en un equipo y en dispositivos móviles. El segundo muestra el número exacto y el porcentaje de cada explorador."

El **Desglose por explorador** Este informe muestra el desglose de aperturas por navegador: Chrome, Safari, Internet Explorer y más.

Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y en sistemas operativos móviles. El segundo muestra el número exacto y el porcentaje de cada explorador.

![](assets/reporting_email_13.2.png){align="center"}


## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Informe de clics interactivos"
>abstract="El **Hotclicks** presenta el contenido del correo electrónico (HTML o texto) con el porcentaje de clics en los vínculos, por cada vínculo. Los bloques personalizados, los vínculos de baja de suscripción, los vínculos de páginas espejo y los vínculos de ofertas se tienen en cuenta en el total de clics acumulados, pero no se muestran en el informe."

Este informe muestra el contenido del mensaje (HTML o texto) con el porcentaje de clics en los vínculos, por cada vínculo. Los bloques personalizados, los vínculos de baja de suscripción, los vínculos de páginas espejo y los vínculos de ofertas se tienen en cuenta en el total de clics acumulados, pero no se muestran en el informe.

![](assets/reporting11.png)
