---
title: Establecimiento de objetivos y filtrado de dimensiones
description: Obtenga más información acerca de las dimensiones de segmentación y filtrado en la IU web de Adobe Campaign
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 17%

---

# Establecimiento de objetivos y filtrado de dimensiones {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Seleccionar la dimensión de segmentación"
>abstract="La dimensión de segmentación permite definir la población a la que se dirige la operación: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. De forma predeterminada, en el caso de los correos electrónicos y SMS, el destinatario se selecciona en la tabla integrada Destinatarios. Para las notificaciones push, la dimensión de destino predeterminada son las aplicaciones del suscriptor."

La dimensión de segmentación, también conocida como asignación de destino, es el tipo de datos que administra una operación. Define la población objetivo, como perfiles, beneficiarios de contratos, operadores o suscriptores. La dimensión de filtrado permite aplicar filtros a la población objetivo haciendo referencia a criterios relacionados sin cambiar la dimensión de segmentación principal.

## Dimensiones de segmentación {#targeting}

La dimensión de segmentación de un flujo de trabajo se define mediante la primera actividad **[!UICONTROL Generar audiencia]** y se utiliza en todas las actividades subsiguientes hasta el final del flujo de trabajo. Por ejemplo, al consultar perfiles desde la base de datos, la transición saliente contiene datos de tipo &quot;destinatario&quot;, que se transmiten a la siguiente actividad.

Cambiar la dimensión de segmentación en un flujo de trabajo mediante [Cambiar actividad de dimensión](../workflows/activities/change-dimension.md). Esto permite consultar la base de datos en una tabla específica, como compras o suscripciones, y luego cambiar la dimensión de segmentación a Destinatarios para realizar envíos a los perfiles correspondientes.

Al seleccionar una dimensión de segmentación (en la configuración del flujo de trabajo o en actividades como **Generar audiencia**, **Reconciliación** o **Cambiar dimensión**), se muestra una lista de esquemas utilizados con frecuencia de forma predeterminada. Para mostrar todos los esquemas disponibles, active el botón **[!UICONTROL Mostrar todos los esquemas]**. La selección de opciones se guarda para cada usuario.

![Captura de pantalla que muestra la interfaz de la dimensión de segmentación con el botón &quot;Mostrar todos los esquemas&quot; habilitado.](assets/targeting-dimension-show-all.png){zoomable="yes"}

De forma predeterminada, las plantillas de entrega de correo electrónico y SMS se dirigen a perfiles. Su dimensión de destino utiliza los campos de la tabla **nms:recipient**. Para las notificaciones push, la dimensión de destino predeterminada es **Subscriber applications nms:appSubscriptionRcp**, que está vinculada a la tabla de destinatarios.

Utilice otras asignaciones de destino integradas en flujos de trabajo y envíos, como se muestra a continuación:

| Nombre | Usar para enviar a | Esquema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Destinatarios | Perfiles/destinatarios (tabla de destinatarios integrada) | nms:recipient |
| Visitantes | Visitantes cuyos perfiles se recopilaron mediante recomendación (marketing viral para ex) | mns:visitor |
| Suscripciones | Perfiles suscritos a un servicio informativo, como un boletín informativo | nms:subscription |
| Suscripciones de visitantes | Visitantes suscritos a un servicio informativo | nms:visitorSub |
| Operadores | Operadores de Adobe Campaign | nms:operator |
| Archivo externo | Envío a través de un archivo que contiene toda la información necesaria | No hay ningún esquema vinculado, no se ha introducido ningún destino |
| Aplicaciones del suscriptor | Perfiles suscritos a una aplicación | nms:appSubscriptionRcp |

Además, cree nuevas asignaciones de destino basadas en necesidades específicas. Realice esta operación únicamente desde la consola del cliente. Obtenga más información en la [documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=es#new-mapping){target="_blank"}.

## Filtrado de dimensiones {#filtering}

La dimensión de segmentación permite definir la población a la que se dirige la operación: destinatarios, beneficiarios de contratos, operadores, suscriptores, etc. La dimensión de filtrado permite aplicar filtros a esta población haciendo referencia a datos relacionados sin cambiar la dimensión de segmentación principal. Por ejemplo, puede seleccionar la población en función de criterios específicos como titulares de contrato o suscriptores a boletines informativos.

Las dimensiones de filtrado solo están disponibles en la actividad **Generar audiencia**.

Para seleccionar clientes que han tenido una póliza de seguro de vida durante más de 5 años, elija lo siguiente:

* Dimensión de segmentación: **Clients**
* Dimensión de filtrado: **Titular del contrato**.

Puede definir las condiciones de filtrado dentro de la actividad **Generar audiencia**. Consulte [esta página](../workflows/activities/build-audience.md).

Durante la selección de la dimensión de destino, solo se muestran en la interfaz las dimensiones de filtrado compatibles. Estas dos dimensiones deben estar relacionadas, por lo que el contenido de la lista de dimensiones de filtrado depende de la dimensión de segmentación seleccionada en el primer campo.
