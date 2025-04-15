---
audience: end-user
title: Correo electrónico informes de envío
description: Aprenda a acceder y utilizar correo electrónico informes de envío
exl-id: 2a0bd3e9-5d75-47c8-bd6a-b3e0b1ce0a01
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 38%

---

# Informe de envío de correo electrónico {#email-report}

El **informe** envío correo electrónico ofrece perspectivas completas y datos específicos del correo electrónico canal. Proporciona información detallada sobre el rendimiento, la eficacia y los resultados de sus envíos individuales, lo que le proporciona una visión general completa.

## Resumen de envíos {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Envío de creación de informes"
>abstract="La pestaña **Envío** dentro del informe proporciona una perspectiva detallada de las interacciones de los visitantes con los envíos y cualquier posible error que hayan encontrado."

### Población de público destinatario inicial {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Población de público destinatario inicial"
>abstract="El gráfico **Población de público destinatario inicial** muestra datos relativos a los destinatarios y los mensajes, en función de los resultados de la preparación de envíos."

El **[!UICONTROL gráfico de población]** del destino inicial muestra los datos relativos a los destinatarios. Las métricas se calculan durante la preparación envío y muestran: el audiencia inicial, el número de mensajes a enviar y el número de destinatarios excluidos.

![Captura de pantalla de un gráfico que muestra datos](assets/reporting_email_1.png){zoomable="yes"}

Sitúe el ratón encima de una porción del gráfico para mostrar el número exacto.

![Captura de pantalla de un gráfico con el ratón encima de una porción para mostrar el número exacto](assets/reporting_email_1.1.png){zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL audiencia]** inicial: número total de destinatarios objetivo.

* **[!UICONTROL Para entregar]**: número total de mensajes a enviar después de envío preparación.

* **[!UICONTROL Exclusión]**: número total de destinatarios excluidos de la población destino.
+++

### Estadísticas de envío {#email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Estadísticas de envío"
>abstract="El gráfico **Estadísticas de envío** detalla el éxito de su envío y los errores que se han producido."

El **[!UICONTROL gráfico de estadísticas]** de entrega detalla el éxito de su envío. Las métricas se detallan a continuación.

![Captura de pantalla de un gráfico que muestra los detalles de las estadísticas envío](assets/reporting_email_2.png){zoomable="yes"}

+++Más información sobre el correo electrónico campaña métricas de informes.

* **[!UICONTROL Enviar mensaje enviados]**: número total de mensajes que se enviarán después de envío preparación.

* **[!UICONTROL Correcto]**: número de mensajes procesados correctamente en relación con el número de mensajes que desea enviar.

* **[!UICONTROL Errores]**: número total de errores acumulados durante los envíos y el procesamiento automático de rechazos en relación con el número de mensajes que se van a enviar.

* **[!UICONTROL Nuevo cuarentenas]**: número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio inválido) en relación con el número de mensajes que se van a enviar.

+++

### Causas de exclusión  {#email-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Causas de exclusión de entrega"
>abstract="El gráfico y la tabla **Causas de exclusión** muestran el desglose por regla de mensajes rechazados durante la preparación del envío."

El **[!UICONTROL gráfico y la tabla Causas de exclusión]** muestran el desglose por regla de mensajes rechazados durante la preparación del envío. Las reglas de exclusión se detallan en la documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank} de la [Campaign v8 (consola).

![Captura de pantalla del gráfico y la tabla Causas de exclusión](assets/reporting_email_3.png){zoomable="yes"}{align="center" zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Usuario desconocido]**: Error tipo generado durante la envío para indicar que la dirección correo electrónico es no válido.

* **[!UICONTROL Dominio]** no válido: Error tipo generado al enviar un envío para indicar que el dominio de la dirección del correo electrónico es incorrecto o no existe.

* **[!UICONTROL Buzón lleno]**: Error tipo generado después de cinco envío intenta indicar que la bandeja de entrada de los destinatarios contiene demasiados mensajes.

* **[!UICONTROL Cuenta desactivada]**: Error tipo generado al enviar una envío para indicar que la dirección ya no existe.

* **[!UICONTROL Rechazado]**: Error tipo generado cuando una dirección es rechazada por el IAP (Internet Access Provider), para instancia siguiendo el aplicación de un regla de seguridad (software antispam).

* **[!UICONTROL Inaccesible]**: Error tipo que aparece en la cadena de distribución de mensajes: problema en el relé SMTP, dominio temporalmente inaccesible, etc

* **[!UICONTROL sin conexión]**: Error tipo para indicar que el teléfono móvil de los destinatarios está apagado o desconectado de la red en el momento del envío.

+++

## Rendimiento del envío {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Rendimiento del envío"
>abstract="El informe **Rendimiento del envío** presenta información detallada sobre el rendimiento del envío de toda la plataforma en un período de tiempo especificado."

Este informe presenta información detallada sobre el rendimiento envío de toda la plataforma dentro de un periodo de tiempo específico. La métrica principal utilizada para medir la velocidad de envío de mensajes es el número de mensajes enviados por hora.

![Captura de pantalla del rendimiento del envío](assets/reporting_email_3.1.png){zoomable="yes"}{align="center" zoomable="yes"}


## Estadísticas de difusión {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Estadísticas de difusión"
>abstract="El informe **Estadísticas de difusión** contiene los datos disponibles sobre los posibles errores encontrados con cada dominio."

La **[!UICONTROL tabla de estadísticas]** de difusión contiene los datos disponibles de posibles errores encontrados con cada dominio. Las métricas se detallan a continuación.

![Captura de pantalla de las estadísticas de emisión](assets/reporting_email_4.png){zoomable="yes"}{align="center" zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Correos electrónicos]** procesados: número total de mensajes procesados por el servidor envío.

* **[!UICONTROL Entregados]**: porcentaje del número de mensajes procesados correctamente en comparación con el número total de mensajes procesados.

* **[!UICONTROL Rechazos duros: Porcentaje del número de rechazos &quot;duros&quot;, errores permanentes]**, como una dirección de correo electrónico incorrecta, en comparación con el número total de mensajes procesados.

* **[!UICONTROL Rechazos leves]**: Porcentaje del número de rechazos &quot;leves&quot;, errores temporales como un bandeja de entrada completo, en comparación con el número total de mensajes procesados

* **[!UICONTROL Aperturas]**: porcentaje del número de destinatarios objetivo que abrieron un mensaje al menos una vez en comparación con el número de mensajes procesados correctamente.

* **[!UICONTROL Clics]**: porcentaje del número de personas que hicieron clic en un envío al menos una vez en comparación con el número de mensajes procesados correctamente.

* **[!UICONTROL Bajas de suscripción]**: porcentaje del número de clics en una vincular de baja en comparación con el número de mensajes procesados correctamente.
+++

## Envíos que no se pueden entregar {#non-deliverables-email}

### Desglose de errores por tipo {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Desglose de errores por tipo"
>abstract="El gráfico **Desglose de errores por tipo** contiene los datos disponibles para cada tipo de error encontrado: usuario desconocido, buzón lleno, dominio inválido y mucho más."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type_table"
>title="Desglose de errores por tipo"
>abstract="La tabla **Desglose de errores por tipo** proporciona un desglose completo de la ocurrencia de cada tipo de error."

La **[!UICONTROL tabla y el gráfico Desglose de errores por tipo]** contienen los datos disponibles para el tipo de error. Las métricas se detallan a continuación.

Los errores que se muestran en este informe activan el proceso de cuarentena. Para obtener más información sobre cuarentena administración, consulte [Campaign documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"} de v8 (consola del cliente).

![Captura de pantalla del breakdwon de errores por tipo](assets/campaign_report_email_6.png){zoomable="yes"}{align="left" zoomable="yes"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Usuario desconocido]**: Error tipo generado durante la envío para indicar que la dirección correo electrónico es no válido.

* **[!UICONTROL Dominio]** no válido: Error tipo generado al enviar un envío para indicar que el dominio de la dirección del correo electrónico es incorrecto o no existe.

* **[!UICONTROL Buzón lleno]**: Error tipo generado después de cinco envío intenta indicar que la bandeja de entrada de los destinatarios contiene demasiados mensajes.

* **[!UICONTROL Cuenta desactivada]**: Error tipo generado al enviar una envío para indicar que la dirección ya no existe.

* **[!UICONTROL Rechazado]**: Error tipo generado cuando una dirección es rechazada por el IAP (Internet Access Provider), para instancia siguiendo el aplicación de un regla de seguridad (software antispam).

* **[!UICONTROL Inaccesible]**: Error tipo que aparece en la cadena de distribución de mensajes: problema en el relé SMTP, dominio temporalmente inaccesible, etc

* **[!UICONTROL sin conexión]**: Error tipo para indicar que el teléfono móvil de los destinatarios está apagado o desconectado de la red en el momento del envío.

+++

### Desglose de errores por dominio {#email-delivery-breakdown-domain}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Desglose de errores por dominio"
>abstract="El gráfico **Desglose de errores por dominio** muestra los datos disponibles para cada tipo de error encontrado según cada dominio."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain_table"
>title="Desglose de errores por dominio"
>abstract="La tabla **Desglose de errores por dominio** proporciona un desglose completo de la ocurrencia de cada error según el dominio utilizado."

La tabla y el **[!UICONTROL gráfico Desglose de errores por dominio]** muestran los datos disponibles de posibles errores encontrados con cada dominio.

![Captura de pantalla del desglose de errores por dominio](assets/campaign_report_email_6.1.png){zoomable="yes"}{align="left" zoomable="yes"}

Haga clic en el icono situado junto al nombre de cada dominio para obtener más información.

![Captura de pantalla del desglose de errores por dominio con los detalles de cada dominio](assets/campaign_report_email_6.1.png){zoomable="yes"}{align="left" zoomable="yes"}

Las métricas disponibles son las mismas que para el [desglose de errores por tipo](#email-delivery-breakdown-type) descrito anteriormente.

## Indicadores de seguimiento {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Seguimiento de creación de informes"
>abstract="La pestaña **Seguimiento** dentro de su informe ofrece datos valiosos, incluido el comportamiento de los destinatarios por vínculo, el desglose de aperturas y clics, así como información detallada sobre las direcciones URL donde se hace clic con más frecuencia durante un envío."


### Estadísticas de envío  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Estadísticas de envío"
>abstract="El informe **Estadísticas de envío** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre los datos disponibles para los correos electrónicos enviados: éxito, aperturas, clics, etc."


El **[!UICONTROL informe de estadísticas]** de entrega proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre los datos disponibles para los correos electrónicos enviados. Las métricas se detallan a continuación.

![Captura de pantalla de las estadísticas de entrega](assets/reporting_email_5.png){zoomable="yes"}{align="center"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Correcto]**: número de mensajes procesados correctamente en relación con el número de mensajes que desea enviar.

* **[!UICONTROL Aperturas distintas]**: número total de destinatarios objetivo que abrieron un mensaje al menos una vez.

* **[!UICONTROL Aperturas]**: número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

* **[!UICONTROL Clics en el vínculo de no participación]**: número de clics en el vincular baja.

* **[!UICONTROL Clics en el vincular]** espejo: número de clics en el vincular al página espejo.

* **[!UICONTROL Estimación de reenvíos]**: Estimación del número de correos electrónicos reenviados por los destinatarios objetivo.
+++

### Tasa de clics y de aperturas {#email-tracking-click-through}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Tasa de clics y de aperturas"
>abstract="La tabla **Tasa de clics y de aperturas** muestra datos relativos ao engajamento dos recipients com a entrega."



La **[!UICONTROL tabla de tasa de]** clics y de apertura muestra los datos relativos a los destinatarios. Las métricas se detallan a continuación.

![Captura de pantalla de la tabla de tasas de clics y de apertura](assets/reporting_email_6.png){zoomable="yes"}{align="center"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Enviados]**: número total de mensajes enviados.

* **[!UICONTROL Quejas]**: Número de mensajes para este dominio que han sido reportados como indeseables por el destinatario.

* **[!UICONTROL Aperturas]**: número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

* **[!UICONTROL Clics]**: número de destinatarios objetivo diferentes que hicieron clic en el mismo envío al menos una vez.

* **[!UICONTROL Reacciones]** sin procesar: porcentaje del número de destinatario que hicieron clic en un envío al menos una vez en comparación con el número de destinatarios que abrieron un envío al menos una vez.
+++

## URL y flujos de clics {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL y flujos de clics"
>abstract="El informe de **URL y flujos de clics** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre las direcciones URL en las que se hizo clic con mayor frecuencia durante un envío."


El informe de **[!UICONTROL URL y flujos de clics]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre las direcciones URL en las que se hizo clic con mayor frecuencia durante un envío.

![Captura de pantalla del informe de URL y flujos de clics](assets/reporting_email_7.png){zoomable="yes"}{align="center"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Reactividad]**: Proporción del número de destinatarios objetivo que han hecho clic en un envío, en relación con el número estimado de destinatarios objetivo que han abierto un envío.

* **[!UICONTROL Clics distintos]**: número total de destinatarios distintos que hicieron clic en un envío al menos una vez.

* **[!UICONTROL Clics: número total de clics en los vínculos de los envíos]**.

* **[!UICONTROL Platform promedio]**: Esta tasa promedio, que se muestra debajo de cada tasa (reactividad, clics distintos y clics acumulados), se calcula para las entregas enviadas durante los seis meses anteriores. Solo se tienen en cuenta los envíos con la misma tipología y en el mismo canal. Se excluyen las pruebas.

+++

### Los 10 vínculos más visitados {#email-tracking-top10}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_top10"
>title="Los 10 vínculos más visitados"
>abstract="El gráfico y la tabla **Los 10 vínculos más visitados** contienen los datos disponibles sobre el comportamiento del destinatario por vínculo."


El gráfico y la tabla **[!UICONTROL Los 10 vínculos más visitados]** contienen los datos disponibles sobre el comportamiento del destinatario por vínculo.

![Captura de pantalla del gráfico de los 10 vínculos más visitados](assets/reporting_email_8.png){zoomable="yes"}{align="center"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Clics: número total de clics en los vínculos de los envíos]**.

* **[!UICONTROL Porcentaje]**: porcentaje de usuarios que interactuaron con el envío.

+++

### Desglose de los clics con el tiempo {#email-tracking-breakdown-over-time}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_click_breakdown"
>title="Desglose de los clics con el tiempo"
>abstract="El gráfico **Desglose de clics a lo largo del tiempo** muestra los datos disponibles del comportamiento del destinatario por vínculo."


El **[!UICONTROL gráfico Desglose de clics a lo largo del tiempo]** contiene los datos disponibles para destinatario comportamiento por vincular.

![Captura de pantalla del gráfico de desglose de clics a lo largo del tiempo](assets/reporting_email_9.png){zoomable="yes"}{align="center"}

## Actividades del usuario {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Actividades del usuario"
>abstract="El gráfico **Actividades de usuario** muestra el desglose de aperturas y clics en forma de gráfico. Puede elegir el período de tiempo para el que desea obtener los datos: último día, última hora o últimos 30 minutos."

El **[!UICONTROL informe Actividades del usuario]** muestra la desglose de aperturas y clics en forma de gráfico. Puede elegir el período de tiempo para el que desea obtener los datos: último día, última hora o últimos 30 minutos.

![Captura de pantalla del informe Actividades del usuario](assets/reporting_email_10.png){zoomable="yes"}{align="center"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Clics: número total de clics en los vínculos de los envíos]**.

* **[!UICONTROL Aperturas]**: número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

+++

## Estadísticas de seguimiento {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Estadísticas de seguimiento"
>abstract="El gráfico **Estadísticas de seguimiento** proporciona estadísticas sobre aperturas y clics. Tiene la opción de seleccionar el lapso de tiempo específico para los datos de segmentación."

El gráfico **[!UICONTROL Estadísticas de seguimiento]** proporciona estadísticas sobre aperturas y clics. Tiene la opción de seleccionar el lapso de tiempo específico para los datos de segmentación.

![Captura de pantalla del gráfico de estadísticas de seguimiento](assets/reporting_email_11.png){zoomable="yes"}{align="center"}

+++Obtenga más información sobre las métricas de informes de envío correo electrónico.

* **[!UICONTROL Clics: número total de clics en los vínculos de los envíos]**.

* **[!UICONTROL Aperturas]**: número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

+++

## Desglose de aperturas {#breakdown-opens}

### Desglose de aperturas por dispositivo {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Desglose por dispositivo"
>abstract="El informe **Desglose por dispositivo** muestra el desglose de las aperturas por dispositivo durante el período. Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y en dispositivos móviles. El segundo muestra el número exacto y el porcentaje para cada tipo de dispositivo."

El **informe Desglose por dispositivos** muestra el desglose de aperturas por dispositivos durante el período: equipos personales, Android dispositivos, Apple dispositivos u otros.

Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y en dispositivos móviles. El segundo muestra el número exacto y el porcentaje para cada tipo de dispositivo.

![Captura de pantalla del informe Desglose por dispositivos](assets/reporting_email_13.png){zoomable="yes"}{align="center"}


### Desglose de aperturas por sistema operativo {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Desglose por sistema operativo"
>abstract="El informe **Desglose por sistema operativo** muestra el desglose de las aperturas por sistema operativo durante el período correspondiente. El primer gráfico muestra las estadísticas relacionadas con las aperturas en un equipo y en dispositivos móviles. El segundo muestra el número exacto y el porcentaje de cada sistema operativo."

El **informe Desglose por sistema operativo** muestra el desglose de aperturas por sistema operativo durante el período: sistemas Windows, sistemas Android, sistemas iOS u otros.

Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y sistemas operativos móviles. El segundo muestra el número y el porcentaje exactos de cada sistema operativo.

![Captura de pantalla del informe Desglose por sistema operativo](assets/reporting_email_13.1.png){zoomable="yes"}{align="center"}

### Desglose de aperturas por explorador {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Desglose por explorador"
>abstract="El **Desglose por explorador** muestra el desglose de aperturas por explorador para el período. El primer gráfico muestra las estadísticas relacionadas con las aperturas en un equipo y en dispositivos móviles. El segundo muestra el número exacto y el porcentaje de cada explorador."

El **informe Desglose por explorador** muestra el desglose de aperturas por explorador: Cromo, Safari, Internet Explorer y más.

Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y sistemas operativos móviles. El segundo muestra el número exacto y el porcentaje de cada explorador.

![Captura de pantalla del desglose de aperturas por informe explorador](assets/reporting_email_13.2.png){zoomable="yes"}{align="center"}


## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Informe de clics interactivos"
>abstract="El informe de **clics interactivos** muestra el contenido del mensaje (HTML o texto) con el porcentaje de clics en cada vínculo. Los bloques de personalización, los vínculos baja, los vínculos de páginas espejo y los vínculos de ofertas se tienen en cuenta en el total de clics acumulados, pero no se muestran en el informe."

Este informe muestra el contenido del mensaje (HTML o texto) con el porcentaje de clics en los vínculos, por cada vínculo. Los bloques de personalización, los vínculos baja, los vínculos de páginas espejo y los vínculos de ofertas se tienen en cuenta en el total de clics acumulados, pero no se muestran en el informe.

![Captura de pantalla del informe Hotclicks](assets/reporting11.png){zoomable="yes"}