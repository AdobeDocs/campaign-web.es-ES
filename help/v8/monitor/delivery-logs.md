---
audience: end-user
title: Monitorización de registros de envío
description: Documentación web de Campaign v8
source-git-commit: 4ed89d326acd3b7d5d8f14bec68cceda3c8169fb
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 46%

---

# Monitorización de registros de envío {#delivery-logs}

>[!NOTE]
>
>Esta documentación está en construcción y se actualiza con frecuencia. La versión final de este contenido estará lista en enero de 2023.

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Registros de entregas"
>abstract="TBC"

Después de preparar y enviar un correo electrónico, los registros de envío le permiten verificar que no hay error. Se puede acceder a estos registros directamente desde el panel de mensajes. Muestran los detalles del envío, qué destinatario se ha excluido y por qué, así como la información de seguimiento como aperturas y clics.

Para ver los registros, haga clic en el botón **Registros** botón.

![](assets/logs.png)

Varias pestañas contienen información (si existe) sobre los registros de envío, los registros de exclusión, las causas de exclusión, los registros de seguimiento y las direcciones URL rastreadas.

**Los** ficha

La variable **Registros** contiene todos los mensajes relacionados con la entrega y las pruebas. Los iconos específicos le permiten identificar errores o advertencias.

Se muestran todos los pasos, advertencias y errores de validación. Los iconos de color muestran el tipo de mensaje:

* El icono gris indica un mensaje informativo.
* El icono amarillo indica un error de procesamiento no crítico.
* El icono rojo indica un error crítico que impide realizar el envío.

**Pestaña Entregas**

La variable **Entregas** ofrece un historial de cada ocurrencia de este envío. La lista de los mensajes enviados y sus estados se almacena aquí. Permite ver el estado de envío de cada destinatario.

**Exclusiones** ficha

La pestaña Exclusion logs enumera todos los mensajes que se han excluido del destinatario enviado y especifica el motivo del error de envío.

**Causas de exclusión** ficha

La variable **Causas de exclusión** muestra el volumen (en número de mensajes) de mensajes que se excluyeron del envío de destino.

**Direcciones URL rastreadas** ficha

La variable **Direcciones URL rastreadas** ficha

**Pestaña Seguimiento**

La pestaña **Tracking** enumera el historial de seguimiento de esta entrega. Esta pestaña muestra los datos de seguimiento de los mensajes enviados, es decir, todas las direcciones URL sobre las que Adobe Campaign realiza un seguimiento. Los datos de seguimiento se actualizan cada hora.

>[!NOTE]
>
>Si el seguimiento no está habilitado para una entrega, esta pestaña no se muestra.

Los datos de Tracking se interpretan en los informes de envío. Consulte esta sección.



