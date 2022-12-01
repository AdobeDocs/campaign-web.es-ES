---
audience: end-user
title: Configuración avanzada
description: Documentación web de Campaign v8
source-git-commit: c90d8a5eff6169945d381f3250cb3e4d06194d31
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 34%

---

# Configuración avanzada {#advanced-settings}

>[!NOTE]
>
>Esta documentación está en construcción y se actualiza con frecuencia. La versión final de este contenido estará lista en enero de 2023.

Estos ajustes son parámetros técnicos de envío definidos en la plantilla de correo electrónico. Si desea modificar cualquiera de ellos para un envío específico, tenga cuidado.

## Configuración de entrega de correo electrónico {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

Todos los parámetros técnicos de envío de la plantilla.
Cambie solo los parámetros, no cree aquí.
Según los permisos, los practicantes no deben modificarlo, tenga cuidado. Comprobar y cambiar solo la regla de tipología -> resto definido en la plantilla

## Tipología {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipología"
>abstract="La tipología permite controlar, filtrar y monitorizar los envíos."

### Parámetro de presión {#pressure-parameter}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso del envío"
>abstract="El peso de la entrega le permite identificar las entregas de mayor prioridad dentro del marco de la gestión de presión. Los mensajes con mayor peso son prioritarios."

### Configuración de capacidad {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importancia del destinatario"
>abstract="TBC"


## Audiencia {#audience}

## Envío {#delivery}

### Reintentos {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Número máximo de reintentos"
>abstract="Si un mensaje falla debido a un error temporal, los reintentos se realizan durante la duración del envío."

## Aprobación {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Aprobación mode"
>abstract="Cada paso de una entrega puede estar sujeto a aprobación para garantizar una monitorización y un control completos de los distintos procesos."

## Validez {#validity}

### Período de validez {#validity-period}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Duración del envío"
>abstract="El campo Duración de la entrega permite introducir el límite de los reintentos de entrega global. Esto significa que Adobe Campaign envía los mensajes comenzando en la fecha de inicio y, a continuación, para los mensajes que devuelven solo un error se realizan reintentos normales y configurables hasta que se alcanza el límite de validez."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Vigencia de recursos"
>abstract="El campo Límite de validez se utiliza para los recursos cargados, principalmente para la página espejo y las imágenes. Los recursos de esta página son válidos durante un tiempo limitado."


### Seguimiento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Período de validez"
>abstract="Esta opción define la duración durante la cual se activará el seguimiento en las direcciones URL."














