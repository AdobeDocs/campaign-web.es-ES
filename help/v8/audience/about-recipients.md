---
title: Trabajo con destinatarios y audiencias
description: Aprenda a trabajar con destinatarios en Campaign Web
badge: label="Beta"
source-git-commit: 899d6306e1de90c4c9b38a30061f97fa72fe7123
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 21%

---


# Trabajo con destinatarios y audiencias {#about-recipients}

## ¿Qué son los destinatarios? {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Destinatarios"
>abstract="Un destinatario es un perfil dirigido a recibir mensajes enviados por Adobe Campaign. En Adobe Campaign, los destinatarios son los perfiles predeterminados a los que se dirigen los envíos (correos electrónicos, SMS). En esta lista, puede ver el perfil del destinatario en función de sus permisos. Utilice las opciones de filtrado para examinar esta lista. Puede editar y actualizar un pequeño conjunto de atributos del destinatario."

Un destinatario es un perfil dirigido a recibir mensajes enviados por Adobe Campaign. En Adobe Campaign, los destinatarios son los perfiles predeterminados a los que se dirigen los envíos (correos electrónicos, SMS, etc.). Los datos de destinatario almacenados en la base de datos permiten crear audiencias que reciban cualquier entrega dada y añadir datos de personalización en el contenido de la entrega. En la base de datos se almacenan otros tipos de perfiles. Están diseñados para diferentes usos: por ejemplo, se crean perfiles semilla para probar los envíos antes de enviarlos a la audiencia final.

Los destinatarios solo se pueden agregar desde la consola del cliente de Campaign. Sin embargo, se pueden ver en la web de Campaign, en la **Destinatarios** entrada del carril de navegación izquierdo. También puede editar los atributos del destinatario desde esa pantalla.

Para editar los datos del destinatario, haga clic en los tres puntos junto a su nombre y seleccione **Editar...**.

![Edición de un perfil de destinatario](assets/recipient-edit.png)

Puede actualizar un conjunto limitado de atributos, que son: nombre, apellidos, correo electrónico y número de teléfono.

![Actualización de un perfil de destinatario](assets/recipient-update.png)

>[!NOTE]
>
>Este formulario limitado de edición de perfiles solo se proporciona para pruebas de programas beta. Se mejorará en la versión futura. Permite al usuario añadir rápidamente una dirección de correo electrónico y un número de teléfono a cualquier perfil para que pueda probar los canales de correo electrónico y SMS y recibir los mensajes enviados.

Puede filtrar los destinatarios utilizando el campo de búsqueda, desde el **Mostrar filtros** botón.

También puede acceder a los destinatarios desde el **Explorer** vea, examine y cree carpetas y subcarpetas, y compruebe los permisos asociados.

![Lista de destinatarios de la vista del explorador](assets/recipients-from-explorer.png)

>[!NOTE]
>
>Según los permisos, es posible que no tenga acceso a la lista completa de destinatarios almacenados en la base de datos. Más información sobre los permisos en [esta sección](../get-started/permissions.md).

Además, puede administrar las suscripciones y bajas de sus destinatarios a servicios como los boletines informativos. [Descubra cómo trabajar con servicios de suscripción](manage-services.md)

Puede crear flujos de trabajo para deduplicar, enriquecer, combinar perfiles y crear audiencias. Obtenga más información en [esta sección](../workflows/gs-workflows.md).

## ¿Qué son las audiencias? {#audiences}

El público destinatario es el destinatario principal de su envío: los destinatarios que reciben los mensajes. El tipo de público destinatario depende de la asignación de destino definida en la plantilla de envíos. [Descubra qué es una plantilla de envíos](../msg/delivery-template.md).

Para definir la población de una audiencia, puede:

* [Crear nuevas audiencias](create-audience.md) desde el **[!UICONTROL Audiencias]** menú,
* [Seleccionar una audiencia existente](add-audience.md) se crea como una lista en la consola de cliente,
* [Seleccione un público destinatario de Adobe Experience Platform](aep-audience.md),
* [Cree un nuevo público destinatario con el generador de reglas definiendo y combinando criterios de filtrado,](segment-builder.md)
* [Uso de una audiencia de un archivo externo](file-audience.md). Esta opción solo está disponible para envíos de correo electrónico independientes y no se puede utilizar en envíos de campañas.

Al segmentar una audiencia, también puede definir lo siguiente **grupos de control** para evitar enviar mensajes a una parte de la audiencia y medir el impacto de las campañas. [Obtenga información sobre cómo establecer un grupo de control](control-group.md)

>[!NOTE]
>
>Al enviar mensajes en el contexto de un flujo de trabajo de campaña, la audiencia se define en una **Crear audiencia** actividad de flujo de trabajo. En este contexto, no se puede cargar un público destinatario de un archivo para un envío de correo electrónico, y el público destinatario se define solo en esta actividad dedicada. Obtenga información sobre cómo definir el público destinatario de su envío en un flujo de trabajo de campaña [en esta sección](../workflows/activities/build-audience.md)

## Dimensiones de segmentación {#targeting-dimensions}

La dimensión de segmentación es el tipo de datos que administra una operación. Permite definir la población objetivo: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc.

La dimensión de segmentación de un flujo de trabajo se define mediante la primera **[!UICONTROL Crear audiencia]** y se utiliza en todas las demás actividades hasta el final del flujo de trabajo. Por ejemplo, si realiza una consulta en los destinatarios de la base de datos, la transición saliente contendrá datos del tipo destinatario y se transmitirá a la siguiente actividad.

Tenga en cuenta que puede cambiar la dimensión de segmentación en un flujo de trabajo mediante una **[!UICONTROL Cambiar dimensión]** actividad. [Más información](../workflows/activities/change-dimension.md). Esto le permite, por ejemplo, consultar la base de datos en una tabla específica, como compras o suscripciones, y luego cambiar la dimensión de segmentación a Destinatarios para realizar envíos a los destinatarios correspondientes.

De forma predeterminada, las plantillas de envío de correo electrónico y SMS están segmentadas **[!UICONTROL Destinatarios]**. Por lo tanto, su dimensión de destino utiliza los campos del **nms:destinatario** tabla. Para las notificaciones push, la dimensión de destino predeterminada es **Aplicaciones del suscriptor nms:appSubscriptionRcp**, que está vinculado a la tabla de destinatarios.

También puede utilizar otras asignaciones de destino integradas en los flujos de trabajo y envíos que se enumeran a continuación:

| Name | Uso para | Esquema |
|---|---|---|
| Destinatarios | Envío a destinatarios (tabla de destinatarios integrada) | nms:recipient |
| Visitantes | Envío a los visitantes cuyos perfiles se hayan recopilado mediante recomendación (marketing viral) por ejemplo. | mns:visitor |
| Suscripciones | Envío a destinatarios suscritos a un servicio de información como un boletín informativo | nms:subscription |
| Suscripciones de visitantes | Envío a los visitantes que están suscritos a un servicio de información | nms:visitorSub |
| Operadores | Envío a los operadores de Adobe Campaign | nms:operator |
| Archivo externo | Envío a través de un archivo que contiene toda la información necesaria para la entrega | No hay ningún esquema vinculado, no se ha introducido ningún destino |
| Aplicaciones del suscriptor | Envío a destinatarios suscritos a una aplicación | nms:appSubscriptionRcp |

Además, puede crear una nueva asignación de destino según sus necesidades. Esto se realiza desde la consola del cliente. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
