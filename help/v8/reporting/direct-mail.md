---
audience: end-user
title: correo postal informes
description: Aprenda a acceder a los informes de correo postal y a utilizarlos
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 20%

---

# Informe de envíos de correo directo {#direct-mail-report}

El **informe envío de** correo postal proporciona información completa y datos específicos de su envío correo postal. Incluye información detallada sobre el rendimiento, la eficacia y los resultados de los partos individuales, ofreciendo una visión general completa.

## Resumen de envíos {#delivery-summary-direct-mail}

### Información general sobre el envío {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Información general sobre el envío"
>abstract="La **Información general de entrega** presenta métricas clave de rendimiento (KPI) que ofrecen información exhaustiva sobre la interacción de los visitantes con cada envío de correo directo. Las métricas se describen a continuación."

La **[!UICONTROL descripción general]** de la entrega proporciona información detallada sobre visitante interacciones con cada correo directo envío y muestra métricas clave de rendimiento (KPI) esenciales. Las métricas se describen a continuación.

![Gráfico de métricas de resumen de entrega que muestra los indicadores clave de rendimiento para correo directo envío.](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++Más información sobre métricas de información general de entrega.

* **[!UICONTROL Mensajes que se van a enviar]**: número total de mensajes procesados durante envío preparación.
* **[!UICONTROL Segmentado]**: número de perfiles de usuario que califican como perfiles destino para mensajes correo directo.
* **[!UICONTROL Para excluir]**: número de perfiles usuario excluidos de los perfiles objetivo que no recibirán mensajes de correo directo.
+++

### Población de público destinatario inicial {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="Población de público destinatario inicial"
>abstract="El gráfico **Población de público destinatario inicial** muestra datos relativos a los destinatarios y los mensajes, en función de los resultados de la preparación de envíos."

El **[!UICONTROL gráfico de población]** destino inicial muestra datos relacionados con los destinatarios. Las métricas se calculan durante la preparación de envío e incluyen el audiencia inicial, el número de mensajes que se van a enviar y el número de destinatarios excluidos.

![Gráfico de población del destino inicial que muestra el tamaño audiencia, los mensajes que se van a enviar y las exclusiones.](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

Pase el ratón sobre una parte del gráfico para ver el número exacto.

![vista detallado del gráfico de población del destino inicial con funcionalidad flotante.](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

+++Obtenga más información sobre correo postal envío métricas de informes.

* **[!UICONTROL audiencia]** inicial: número total de destinatarios objetivo.
* **[!UICONTROL Para entregar]**: número total de mensajes a enviar después de envío preparación.
* **[!UICONTROL Exclusión]**: número total de destinatarios excluidos de la población destino.
+++

### Estadísticas de envío {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="Estadísticas de envío"
>abstract="El gráfico **Estadísticas de envío** detalla el éxito de su envío de correo directo y los errores que se han producido."

El **[!UICONTROL gráfico de estadísticas]** de entrega proporciona una visión general del rendimiento envío y ofrece métricas detalladas para medir éxito y eficacia.

![Gráfico de estadísticas de entrega que muestra las tasas de éxito, los errores y las cuarentenas.](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++Obtenga más información sobre correo postal campaña métricas de informes.

* **[!UICONTROL Enviar mensaje enviados]**: número total de mensajes que se enviarán después de envío preparación.
* **[!UICONTROL Éxito]**: número de mensajes procesados correctamente en comparación con el número de mensajes que se van a enviar.
* **[!UICONTROL Errores]**: número total de errores acumulados durante los envíos y el procesamiento automático de rechazos en comparación con el número de mensajes que se van a enviar.
* **[!UICONTROL Nuevo cuarentenas]**: el número total de direcciones en cuarentena después de un envío fallido (por ejemplo, usuario desconocido, dominio inválido) en comparación con el número de mensajes que se van a enviar.
+++

### Causas de exclusión {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Causas de exclusión de entrega"
>abstract="El gráfico **Causas de exclusión** ilustra la distribución de mensajes rechazados durante la preparación de la entrega, clasificados por cada regla."

El **[!UICONTROL gráfico Causas de exclusión]** proporciona una desglose de motivos para el rechazo del mensaje durante envío preparación. Este desglose está organizado por varias reglas, que ofrecen una vista detallada de los factores que contribuyen a la exclusión de mensajes. Las reglas de exclusión se detallan en la documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank} de la [Campaign v8 (consola).

![Causas de exclusión Gráfico que muestra la distribución de mensajes rechazados por regla.](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++Más información sobre Causas de las métricas de exclusión.

* **[!UICONTROL Dirección en cuarentena]**: Error tipo generado cuando se coloca una dirección en cuarentena.
* **[!UICONTROL Dirección no especificada]**: Error tipo generado cuando no existe una dirección.
* **[!UICONTROL Dirección de mala calidad]**: Error tipo generado cuando la calificación de calidad de la dirección postal es demasiado baja.
* **[!UICONTROL Dirección en la lista de]** denegación: Error tipo generado cuando el destinatario se incluyó en la lista de denegación durante envío.
* **[!UICONTROL Doble]**: Error tipo generado cuando el destinatario se excluyó debido a valores de clave no únicos.
* **[!UICONTROL Control grupo]**: la dirección del destinatario forma parte del grupo de control.
* **[!UICONTROL Target de tamaño]** limitado: se ha alcanzado el tamaño máximo de envío para el destinatario.
+++

### Exclusiones {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Exclusiones"
>abstract="El gráfico **[!UICONTROL Exclusiones]** muestra un desglose detallado, por regla, de los mensajes rechazados durante el proceso de preparación de la entrega."

La **[!UICONTROL tabla Exclusiones proporciona un desglose detallado, categorizado por reglas específicas, de mensajes rechazados]** durante envío preparación. Este desglose ofrece una comprensión clara de las razones detrás de las exclusiones de mensajes.

![Tabla de exclusiones que muestra desglose detallados de mensajes rechazados por regla.](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

Las métricas disponibles son las mismas que para las [causas de exclusión](#direct-mail-delivery-exclusions) descritas anteriormente.