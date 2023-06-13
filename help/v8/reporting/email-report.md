---
audience: end-user
title: Informes de envío de correo electrónico
description: Obtenga información sobre cómo acceder y utilizar los informes de envío por correo electrónico
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 39%

---

# Informe de envío de correo electrónico {#email-report}

El **Informe de envío de correo electrónico** ofrece información y datos completos específicos del canal de correo electrónico. Proporciona información detallada sobre el rendimiento, la eficacia y los resultados de sus envíos individuales, lo que le proporciona una visión general completa.

## Resumen de envíos {#delivery-summary-email}

* **[!UICONTROL Estadísticas de audiencia de destinatario inicial]** La tabla muestra datos relativos a los destinatarios:

  ![](assets/reporting_email_1.png){align="left" zoomable="yes"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Audiencia inicial]**: Número total de destinatarios objetivo.

   * **[!UICONTROL Para enviar]**: Número total de mensajes que desea enviar después del análisis de envío.

   * **[!UICONTROL Exclusión]**: Número total de mensajes excluidos del destinatario enviado.
+++

* **[!UICONTROL Estadísticas de envío]** La tabla detalla el éxito de su envío.

  ![](assets/reporting_email_2.png){align="left"}

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Mensaje enviado]**: Número total de mensajes que desea enviar después del análisis de envío.

   * **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

   * **[!UICONTROL Errores]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

   * **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

+++

* **[!UICONTROL Causas de exclusión]** el gráfico y la tabla muestran el desglose por regla de mensajes rechazados durante el análisis.

  ![](assets/reporting_email_3.png){align="center"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Usuario desconocido]**: Tipo de error generado durante la entrega para indicar que la dirección de correo electrónico no es válida.

   * **[!UICONTROL Dominio no válido]**: Tipo de error generado al realizar una entrega para indicar que el dominio de la dirección de correo electrónico es incorrecto o no existe.

   * **[!UICONTROL Buzón lleno]**: Tipo de error generado después de cinco intentos de entrega para indicar que la bandeja de entrada de los destinatarios contiene demasiados mensajes.

   * **[!UICONTROL Cuenta deshabilitada]**: Tipo de error generado al realizar una entrega para indicar que la dirección ya no existe.

   * **[!UICONTROL Rechazado]**: Tipo de error generado cuando el IAP (Proveedor de acceso a Internet) rechaza una dirección, por ejemplo, al aplicar una regla de seguridad (software antispam).

   * **[!UICONTROL Inalcanzable]**: Tipo de error que se produce en la cadena de distribución de mensajes: incidencia en la retransmisión SMTP, dominio temporalmente inaccesible, etc.

   * **[!UICONTROL Sin conexión]**: Tipo de error que indica que el teléfono móvil de los destinatarios está apagado o desconectado de la red en el momento de la entrega.

+++

## Rendimiento del envío {#delivery-throughtput}

Este informe presenta información detallada sobre el rendimiento de entrega de toda la plataforma en un periodo de tiempo especificado. La métrica principal utilizada para medir la velocidad de entrega de mensajes es el número de mensajes enviados por hora.

## Estadísticas de difusión {#broadcast-statistics}

* **[!UICONTROL Estadísticas de difusión]** contiene los datos disponibles de los posibles errores encontrados con cada dominio.

  ![](assets/reporting_email_4.png){align="center"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Correos electrónicos procesados]**: Número total de mensajes procesados por el servidor de envío.

   * **[!UICONTROL Entregado]**: porcentaje del número de mensajes procesados correctamente comparado con el número total de mensajes procesados.

   * **[!UICONTROL Rechazos graves]**: porcentaje del número de rechazos &quot;graves&quot; y errores permanentes, como una dirección de correo electrónico incorrecta, comparado con el número total de mensajes procesados.

   * **[!UICONTROL Rechazos leves]**: porcentaje del número de rechazos &quot;leves&quot;, errores temporales como una bandeja de entrada llena, comparado con el número total de mensajes procesados

   * **[!UICONTROL Aperturas]**: porcentaje del número de destinatarios objetivo que abrieron un mensaje al menos una vez comparado con el número de mensajes procesados correctamente.

   * **[!UICONTROL Clics]**: porcentaje del número de personas que hizo clic en una entrega al menos una vez comparado con el número de mensajes procesados correctamente.

   * **[!UICONTROL Baja de suscripciones]**: porcentaje del número de clics en un vínculo de baja de suscripción comparado con el número de mensajes procesados correctamente.
+++

## Rechazos y no entregables {#non-deliverables-email}

* **[!UICONTROL Desglose de errores por tipo]** y **[!UICONTROL Desglose de errores por dominio]** Las tablas y los gráficos contienen los datos disponibles para detectar posibles errores encontrados con cada dominio.

  Los errores que se muestran en este informe activan el proceso de cuarentena. Para obtener más información sobre la administración de la cuarentena, consulte [Administración de cuarentena](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=es)

  ![](assets/campaign_report_email_6.png)

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Usuario desconocido]**: Tipo de error generado durante la entrega para indicar que la dirección de correo electrónico no es válida.

   * **[!UICONTROL Dominio no válido]**: Tipo de error generado al realizar una entrega para indicar que el dominio de la dirección de correo electrónico es incorrecto o no existe.

   * **[!UICONTROL Buzón lleno]**: Tipo de error generado después de cinco intentos de entrega para indicar que la bandeja de entrada de los destinatarios contiene demasiados mensajes.

   * **[!UICONTROL Cuenta deshabilitada]**: Tipo de error generado al realizar una entrega para indicar que la dirección ya no existe.

   * **[!UICONTROL Rechazado]**: Tipo de error generado cuando el IAP (Proveedor de acceso a Internet) rechaza una dirección, por ejemplo, al aplicar una regla de seguridad (software antispam).

   * **[!UICONTROL Inalcanzable]**: Tipo de error que se produce en la cadena de distribución de mensajes: incidencia en la retransmisión SMTP, dominio temporalmente inaccesible, etc.

   * **[!UICONTROL Sin conexión]**: Tipo de error que indica que el teléfono móvil de los destinatarios está apagado o desconectado de la red en el momento de la entrega.

+++

## Indicadores de seguimiento {#tracking-indicators-email}

* **[!UICONTROL Estadísticas de envío]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre los datos disponibles para los correos electrónicos enviados.

  ![](assets/reporting_email_5.png){align="center"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

   * **[!UICONTROL Aperturas distintas]**: Número total de destinatarios objetivo que abrieron un mensaje al menos una vez.

   * **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

   * **[!UICONTROL Clics en el vínculo de no participación]**: Número de clics en el vínculo de baja de suscripción.

   * **[!UICONTROL Clicks on the mirror link]** : número de clics en el vínculo a la página espejo.

   * **[!UICONTROL Estimation of forwards]** : estimación del número de correos electrónicos reenviados por los destinatarios objetivo.
+++

* **[!UICONTROL Tasa de apertura y clics]** La tabla muestra datos relativos a los destinatarios.

  ![](assets/reporting_email_6.png){align="center"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Enviado]**: Número total de mensajes enviados.

   * **[!UICONTROL Complaints]** : número de mensajes de este dominio que el destinatario ha notificado como no deseados.

   * **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

   * **[!UICONTROL Clicks]** : número de destinatarios objetivo diferentes que hicieron clic en el mismo entrega al menos una vez.

   * **[!UICONTROL Raw reactivity]** : porcentaje del número de destinatarios que hicieron clic en una entrega al menos una vez comparado con el número de destinatarios que abrieron una entrega al menos una vez.
+++

## URL y flujos de clics {#url-email}

* **[!UICONTROL URL y flujos de clics]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre las direcciones URL en las que más se hizo clic durante una entrega.

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

* **[!UICONTROL Actividades de usuario]** muestra el desglose de aperturas y clics en forma de gráfico. Puede elegir el periodo de tiempo para los datos de destino: último día, hora o 30 minutos.

  ![](assets/reporting_email_10.png){align="center"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

+++

## Estadísticas de seguimiento {#tracking-statistics}

* **[!UICONTROL Estadísticas de seguimiento]** El gráfico proporciona estadísticas sobre aperturas y clics. Tiene la opción de seleccionar el lapso de tiempo específico para los datos de destino.

  ![](assets/reporting_email_11.png){align="center"}

  +++ Obtenga más información sobre las métricas de informes de envío de correo electrónico.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

+++

## Desglose de aperturas {#breakdown-opens}

Este informe muestra el desglose de aperturas por sistema operativo, dispositivo y navegador durante el periodo correspondiente. Para cada categoría se utilizan dos gráficos. El primero muestra estadísticas relacionadas con las aperturas en un ordenador y en dispositivos móviles. El segundo muestra estadísticas relacionadas únicamente con las aperturas en dispositivos móviles.
Tiene la flexibilidad de cambiar de **[!UICONTROL Corrección y móvil]** para segmentar exclusivamente **[!UICONTROL Solo móvil]** para una segmentación más precisa.

![](assets/reporting_email_13.png){align="center"}

## Hotclicks {#hotclicks}

Este informe muestra el contenido del mensaje (HTML o texto) con el porcentaje de clics en los vínculos, por cada vínculo. Los bloques personalizados, los vínculos de cancelación de suscripción, los vínculos de páginas espejo y los vínculos de ofertas se tienen en cuenta en el total de clics acumulados, pero no se muestran en el informe.

![](assets/reporting11.png)
