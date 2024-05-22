---
audience: end-user
title: Monitorización de los registros de envío
description: Obtenga información sobre cómo monitorizar los registros de envío
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 71%

---

# Monitorización de los registros de envío {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Registros de envío"
>abstract="Los registros de envío muestran los detalles del envío. Estos muestran los detalles del envío, los destinatarios que se han excluido y el porqué, así como la información de seguimiento de aperturas y clics."

Una vez preparada la entrega y haciendo clic en el botón **Enviar** , vaya a los registros de envío para comprobar las advertencias, los errores, el estado, las exclusiones y los datos de seguimiento. Se puede acceder a estos registros directamente desde el panel de mensajes. Estos muestran los detalles del envío, los destinatarios que se han excluido y el porqué, así como la información de seguimiento de aperturas y clics.

Para ver los registros, acceda al panel del envío y haga clic en el botón **Registros**.

Las pestañas disponibles son las siguientes:

* [Registros](#logs-tab)
* [Envíos](#deliveries-tab)
* [Exclusiones](#exclusion-tab)
* [Causas de exclusión](#exclusion-causes)
* [Direcciones URL rastreadas](#tracked-urls)
* [Seguimiento](#tracking)

## Registros {#logs-tab}

La pestaña **Registros** contiene todos los mensajes relacionados con los envíos y las pruebas. Los iconos específicos le permiten identificar los errores o las advertencias.

Se muestran todos los pasos, advertencias y errores de validación. Los iconos de color muestran el tipo de mensaje:

* El icono gris indica los mensajes informativos.
* El icono amarillo indica un error de procesamiento no crítico.
* El icono rojo indica un error crítico que impide realizar el envío. Deben corregirse los errores críticos para que se realice la entrega.

![](assets/logs.png){zoomable="yes"}


## Envíos {#deliveries-tab}

La pestaña **Envío de registros** muestra el historial de cada ocurrencia del envío. La lista de los mensajes enviados y sus estados se almacena aquí. Permite ver el estado de envío de cada destinatario.

![](assets/logs2.png){zoomable="yes"}

## Exclusiones {#exclusion-tab}

La pestaña **Registros de exclusión** contiene todos los mensajes que se han excluido del destinatario y especifica el motivo de error del envío.

![](assets/logs3.png){zoomable="yes"}

## Causas de exclusión {#exclusion-causes-tab}

El **Causas de exclusión** La pestaña muestra, por cada causa posible, el número de mensajes que se han excluido del destinatario.

![](assets/logs4.png){zoomable="yes"}

## Direcciones URL rastreadas {#tracked-urls-tab}

El **URL seguidas** reagrupa las direcciones URL contenidas en los mensajes enviados, incluido su tipo de dirección URL y la dirección URL de origen.

![](assets/logs5.png){zoomable="yes"}

## Seguimiento {#tracking-tab}

La pestaña **Seguimiento** enumera el historial de seguimiento de este envío. Esta pestaña muestra los datos de seguimiento de los mensajes enviados, es decir, todas las direcciones URL sobre las que Adobe Campaign realiza un seguimiento.


![](assets/logs6.png){zoomable="yes"}

>[!NOTE]
>
>Si el seguimiento no está habilitado para un envío, no se muestra esta pestaña.