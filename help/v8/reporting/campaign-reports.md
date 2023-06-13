---
audience: end-user
title: Informes de campaña
description: Obtenga información sobre cómo acceder y utilizar los informes de campaña
badge: label="Alpha" type="Positive"
source-git-commit: 535ab4238c9937d716a20ac8019b44da091bdd6c
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 22%

---

# Informes de campaña {#campaign-reports}

El informe de campaña se divide en diferentes widgets que detallan el éxito y los errores de la campaña.

La página del informe de campaña se muestra con las siguientes pestañas:

* [Canal de correo electrónico](#email-channel)
* [Canal de SMS](#sms-channel)
* [Canal de Push](#push-channel)

Para acceder al informe de Campaign, haga clic en Reports en el panel de campañas.

![](assets/campaign_report_email_13.png)

## Canal de correo electrónico {#email-channel}

### Resumen de envíos {#delivery-summary-email}

* **[!UICONTROL Resumen de entrega]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de correo electrónico.

  ![](assets/campaign_report_email_1.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Total enviado]**: Número total de mensajes procesados durante el análisis de envío.

   * **[!UICONTROL Entregado]**: Número de mensajes enviados correctamente en relación con el número total de mensajes enviados.

   * **[!UICONTROL Devoluciones]**: Total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

   * **[!UICONTROL Aperturas distintas]**: Número total de destinatarios objetivo que abrieron un mensaje al menos una vez.

   * **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

+++

* **[!UICONTROL Estadísticas de audiencia de destinatario inicial]** La tabla muestra datos relativos a los destinatarios:

  ![](assets/campaign_report_email_2.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Audiencia inicial]**: Número total de destinatarios objetivo.

   * **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después del análisis de envío.

   * **[!UICONTROL Rechazado por reglas]**: Número total de direcciones ignoradas durante el análisis al aplicar las reglas: direcciones faltantes, en cuarentena, en la lista de bloqueados, etc.

+++

* **[!UICONTROL Estadísticas de ejecución]** La tabla detalla el éxito de su envío.

  ![](assets/campaign_report_email_3.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después del análisis de envío.

   * **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

   * **[!UICONTROL Errores]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

   * **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

+++

* **[!UICONTROL Estadísticas de reacción]** contiene los datos disponibles de la actividad de destinatario de su envío.

  ![](assets/campaign_report_email_4.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Aperturas distintas]**: Número total de destinatarios objetivo que abrieron un mensaje al menos una vez.

   * **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

   * **[!UICONTROL Baja de suscripciones]**: Número de destinatarios que hicieron clic en las bajas de suscripción durante el periodo correspondiente.

   * **[!UICONTROL Página espejo]**: número de destinatarios que hicieron clic en el vínculo de la página espejo.

   * **[!UICONTROL Reenvíos]**: número de destinatarios que hicieron clic y que reenviaron el correo electrónico.
+++

* **[!UICONTROL Flujos de clics generados]** La tabla muestra datos relativos a la interacción de los destinatarios con el envío.

  ![](assets/campaign_report_email_5.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Reactivity]** : la proporción del número de destinatarios objetivo que han hecho clic en una entrega en relación con el número estimado de destinatarios objetivo que han abierto una entrega.

+++

### Envíos que no se pueden entregar {#non-deliverables-email}

* **[!UICONTROL Desglose de errores por tipo]** y **[!UICONTROL Desglose de errores por dominio]** Las tablas y los gráficos contienen los datos disponibles para detectar posibles errores encontrados con cada dominio.

  ![](assets/campaign_report_email_6.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Errores]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

   * **[!UICONTROL Contribución]**:

   * **[!UICONTROL Desglose]**:

+++

### Indicadores de seguimiento {#tracking-indicators-email}

* **[!UICONTROL Estadísticas de envío]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre los datos disponibles para los correos electrónicos enviados.

  ![](assets/campaign_report_email_7.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

   * **[!UICONTROL Aperturas distintas]**: Número total de destinatarios objetivo que abrieron un mensaje al menos una vez.

   * **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

   * **[!UICONTROL Clics en el vínculo de no participación]**: Número de clics en el vínculo de baja de suscripción.

   * **[!UICONTROL Clicks on the mirror link]** : número de clics en el vínculo a la página espejo.

   * **[!UICONTROL Estimation of forwards]** : estimación del número de correos electrónicos reenviados por los destinatarios objetivo.
+++

* **[!UICONTROL Estadísticas de audiencia de destinatario inicial]** La tabla muestra datos relativos a los destinatarios.

  ![](assets/campaign_report_email_8.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Enviado]**: Número total de mensajes enviados.

   * **[!UICONTROL Complaints]** : número de mensajes de este dominio que el destinatario ha notificado como no deseados.

   * **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

   * **[!UICONTROL Clicks]** : número de destinatarios objetivo diferentes que hicieron clic en el mismo entrega al menos una vez.

   * **[!UICONTROL Raw reactivity]** : porcentaje del número de destinatarios que hicieron clic en una entrega al menos una vez comparado con el número de destinatarios que abrieron una entrega al menos una vez.
+++

### URL y flujos de clics {#url-email}

* **[!UICONTROL URL y flujos de clics]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre las direcciones URL en las que más se hizo clic durante una entrega.

  ![](assets/campaign_report_email_9.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Reactivity]** : la proporción del número de destinatarios objetivo que han hecho clic en una entrega en relación con el número estimado de destinatarios objetivo que han abierto una entrega.

   * **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

+++

* **[!UICONTROL Los 10 vínculos más visitados]** el gráfico y la tabla contienen los datos disponibles sobre el comportamiento del destinatario por vínculo.

  ![](assets/campaign_report_email_10.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Porcentaje]**: porcentaje de usuarios que interactuaron con el envío.

+++

* **[!UICONTROL Desglose de los clics a lo largo del tiempo]** El gráfico contiene los datos disponibles sobre el comportamiento del destinatario por vínculo.

  ![](assets/campaign_report_email_11.png)

### Actividades de usuario {#user-activities-email}

* **[!UICONTROL Actividades de usuario]** muestra el desglose de aperturas y clics en forma de gráfico.

  ![](assets/campaign_report_email_12.png)

  +++Obtenga más información sobre las métricas de informes de campañas de correo electrónico.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Opens]** : número de destinatarios objetivo diferentes para este dominio que han abierto un mensaje al menos una vez.

+++

## Canal de SMS {#sms-channel}

### Resumen de envíos {#delivery-summary-sms}

* **[!UICONTROL Resumen de entrega]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de SMS.

  +++Obtenga más información sobre las métricas de informes de campañas de SMS.

   * **[!UICONTROL Total enviado]**: Número total de mensajes procesados durante el análisis de envío.

   * **[!UICONTROL Entregado]**: Número de mensajes enviados correctamente en relación con el número total de mensajes enviados.

   * **[!UICONTROL Errores]**: Total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

   * **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

+++

* **[!UICONTROL Estadísticas de audiencia de destinatario inicial]** La tabla muestra datos relativos a los destinatarios:

  +++Obtenga más información sobre las métricas de informes de campañas de SMS.

   * **[!UICONTROL Audiencia inicial]**: Número total de destinatarios objetivo.

   * **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después del análisis de envío.

   * **[!UICONTROL Rechazado por reglas]**: Número total de direcciones ignoradas durante el análisis al aplicar las reglas: direcciones faltantes, en cuarentena, en la lista de bloqueados, etc.

+++

* **[!UICONTROL Estadísticas de ejecución]** La tabla detalla el éxito de su envío:

  +++Obtenga más información sobre las métricas de informes de campañas de SMS.

   * **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después del análisis de envío.

   * **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

   * **[!UICONTROL Errores]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

   * **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

+++

* **[!UICONTROL Flujos de clics generados]** La tabla muestra datos relativos a la interacción de los destinatarios con el envío:

  +++Obtenga más información sobre las métricas de informes de campañas de SMS.

   * **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Reactivity]** : la proporción del número de destinatarios objetivo que han hecho clic en una entrega en relación con el número estimado de destinatarios objetivo que han abierto una entrega.

+++

## Canal de Push {#push-channel}

### Resumen de envíos {#delivery-summary-push}

* **[!UICONTROL Resumen de entrega]** proporciona indicadores clave de rendimiento (KPI) que proporcionan información detallada sobre cómo los visitantes interactúan con el envío de notificaciones push.

  +++Obtenga más información sobre las métricas de informes de campañas push.

   * **[!UICONTROL Total enviado]**: Número total de mensajes procesados durante el análisis de envío.

   * **[!UICONTROL Entregado]**: Número de mensajes enviados correctamente en relación con el número total de mensajes enviados.

   * **[!UICONTROL Errores]**: Total de errores acumulados durante el envío y el procesamiento automático de devoluciones en relación con el número total de mensajes enviados.

   * **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

+++

* **[!UICONTROL Estadísticas de audiencia de destinatario inicial]** La tabla muestra datos relativos a los destinatarios:

  +++Obtenga más información sobre las métricas de informes de campañas push.

   * **[!UICONTROL Audiencia inicial]**: Número total de destinatarios objetivo.

   * **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después del análisis de envío.

   * **[!UICONTROL Rechazado por reglas]**: Número total de direcciones ignoradas durante el análisis al aplicar las reglas: direcciones faltantes, en cuarentena, en la lista de bloqueados, etc.

+++

* **[!UICONTROL Estadísticas de ejecución]** La tabla detalla el éxito de su envío:

  +++Obtenga más información sobre las métricas de informes de campañas push.

   * **[!UICONTROL Mensaje para enviar]**: Número total de mensajes que desea enviar después del análisis de envío.

   * **[!UICONTROL Correcto]**: Número de mensajes procesados correctamente en relación con el número de mensajes que se van a enviar.

   * **[!UICONTROL Errores]**: Número total de errores acumulados durante los envíos y el procesamiento automático de los rechazos en relación con el número de mensajes que se desea enviar.

   * **[!UICONTROL Nuevas cuarentenas]**: Número total de direcciones en cuarentena después de un envío fallido (usuario desconocido, dominio no válido) en relación con el número de mensajes que se van a enviar.

+++

* **[!UICONTROL Flujos de clics generados]** La tabla muestra datos relativos a la interacción de los destinatarios con el envío:

  +++Obtenga más información sobre las métricas de informes de campañas push.

   * **[!UICONTROL Clics distintos]**: Número total de destinatarios diferentes que hicieron clic en una entrega al menos una vez.

   * **[!UICONTROL Hacer clic]**: Número total de clics en los vínculos de las entregas.

   * **[!UICONTROL Reactivity]** : la proporción del número de destinatarios objetivo que han hecho clic en una entrega en relación con el número estimado de destinatarios objetivo que han abierto una entrega.

+++
