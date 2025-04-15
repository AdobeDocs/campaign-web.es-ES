---
audience: end-user
title: Monitorización de los registros de envío
description: Obtenga información sobre cómo monitorizar los registros de envío
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 55%

---

# Monitorización de los registros de envío {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Registros de envío"
>abstract="Los registros de envío muestran los detalles del envío. Estos muestran los detalles del envío, los destinatarios que se han excluido y el porqué, así como la información de seguimiento de aperturas y clics."

Una vez preparada la envío y haga clic en Enviar **** botón, vaya a la registros de envío para comprobar las advertencias, los errores, el estado, las exclusiones y los datos seguimiento. Se puede acceder a estos registros directamente desde el panel de mensajes. Estos muestran los detalles del envío, los destinatarios que se han excluido y el porqué, así como la información de seguimiento de aperturas y clics.

Para ver los registros, acceda al panel del envío y haga clic en el botón **Registros**.

Las fichas disponibles son las siguientes:

* [Registros](#logs-tab)
* [Envíos](#deliveries-tab)
* [Exclusiones](#exclusion-tab)
* [Causas de exclusión](#exclusion-causes)
* [Direcciones URL rastreadas](#tracked-urls)
* [Seguimiento](#tracking)

## Registros {#logs-tab}

La pestaña **Registros** contiene todos los mensajes relacionados con los envíos y las pruebas. Los iconos específicos le permiten identificar los errores o las advertencias.

Se enumeran todos los pasos validación, advertencias y errores. Los iconos de color muestran el tipo de mensaje:

* El icono gris indica los mensajes informativos.
* El icono amarillo indica un error de procesamiento no crítico.
* El icono rojo indica un error de esencial que impide enviar el envío. Los errores críticos deben corregirse para que se envíe la envío.

![ Los registros pestaña que muestran validación pasos, advertencias y errores con iconos de colores que indican los tipos de mensajes.](assets/logs.png){zoomable="yes"}

## Envíos {#deliveries-tab}

La pestaña **Envío de registros** muestra el historial de cada ocurrencia del envío. La lista de los mensajes enviados y sus estados se almacena aquí. Permite ver el estado de envío de cada destinatario.

![ Los envíos pestaña muestran un historial de mensajes enviados y sus estados.](assets/logs2.png){zoomable="yes"}

## Exclusiones {#exclusion-tab}

La pestaña **Registros de exclusión** contiene todos los mensajes que se han excluido del destinatario y especifica el motivo de error del envío.

![Exclusiones pestaña enumerar mensajes excluidos y motivos de errores de envío.](assets/logs3.png){zoomable="yes"}

## Causas de exclusión {#exclusion-causes-tab}

La **pestaña causas de exclusión** muestra, para cada posible causa, el número de mensajes que se han excluido del destino.

![Las causas de exclusión pestaña muestran el número de mensajes excluidos por cada causa.](assets/logs4.png){zoomable="yes"}

## Direcciones URL rastreadas {#tracked-urls-tab}

El **pestaña de direcciones** URL rastreadas reagrupa las direcciones URL contenidas en los mensajes enviados, incluidos su tipo de URL y su URL de origen.

![Las direcciones URL rastreadas pestaña muestran las direcciones URL contenidas en los mensajes enviados, sus tipos y las direcciones URL de origen.](assets/logs5.png){zoomable="yes"}

## Seguimiento {#tracking-tab}

La pestaña **Seguimiento** enumera el historial de seguimiento de este envío. Este pestaña muestra seguimiento datos de los mensajes enviados, incluidas todas las direcciones URL sujetas a seguimiento por Adobe Campaign.

![El seguimiento pestaña que muestra el historial de seguimiento y los datos de los mensajes enviados.](assets/logs6.png){zoomable="yes"}

>[!NOTE]
>
>Si el seguimiento no está habilitado para un envío, no se muestra esta pestaña.