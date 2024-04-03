---
audience: end-user
title: Uso de la actividad de flujo de trabajo Cambiar fuente de datos
description: Aprenda a utilizar la actividad del flujo de trabajo Cambiar fuente de datos
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 27%

---

# Cambio de la fuente de datos {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Cambio de la fuente de datos"
>abstract="Utilice la nueva actividad de segmentación del flujo de trabajo Cambiar fuente de datos para cambiar la fuente de datos utilizada por la tabla de trabajo del flujo de trabajo. Esta actividad proporciona más flexibilidad al permitirle administrar datos en sus diferentes bases de datos y mejorar los rendimientos."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Cambio de la fuente de datos"
>abstract="La actividad **Cambiar fuente de datos** le permite seleccionar una fuente de datos diferente para la tabla de trabajo del flujo de trabajo."

El **Cambiar fuente de datos** la actividad es una **segmentación** actividad. Esta actividad le permite cambiar la fuente de datos utilizada por la tabla de trabajo del flujo de trabajo. Esto proporciona más flexibilidad al permitirle administrar los datos en sus diferentes bases de datos y mejorar el rendimiento.

En los flujos de trabajo, los datos que pasan de una actividad a otra a través de transiciones se almacenan en un **Tabla de trabajo**. De forma predeterminada, las tablas de trabajo se crean en la misma base de datos que el origen de los datos procesados. Por ejemplo, al consultar la tabla &quot;Perfiles&quot;, almacenada en la base de datos en la nube, se crea una tabla de trabajo en la misma base de datos en la nube.

En algunos casos, los datos no están disponibles en la base de datos actual o no son lo suficientemente eficientes como para realizar operaciones unitarias. Por lo tanto, es posible que tenga que forzar el flujo de trabajo para que utilice una base de datos diferente para realizar estas operaciones añadiendo una **[!UICONTROL Cambiar fuente de datos]** actividad.

Encontrará información detallada sobre la arquitectura de Campaign en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html)

<!--

Let's say you want to send to your  VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Configuración de la actividad Cambiar fuente de datos {#configure}

Siga estos pasos para configurar el **Cambiar dimensión** actividad:

![](../assets/workflow-change-data-source-add.png)

1. Añadir un **Cambiar fuente de datos** a su flujo de trabajo.

1. Defina el origen de datos al que desea mover la tabla de trabajo:

   * **[!UICONTROL Base de datos de Campaign predeterminada (PostgreSQL)]**: utilice la base de datos local predeterminada de Campaign.
   * **[!UICONTROL Cuenta externa de FDA]**: utilice bases de datos de nube externas conectadas a Adobe Campaign mediante la función de acceso de datos federado.

     >[!AVAILABILITY]
     >
     >La configuración de Campaign y la conexión a sistemas externos están restringidas a usuarios avanzados y solo están disponibles desde la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=es){target="_blank"}

1. Configure el flujo de trabajo para que realice las operaciones deseadas utilizando la nueva fuente de datos.

<!--
## Example {#example}

The workflow belows illustrates the use case detailed earlier, i.e. sending VIP customers offer codes that they can redeem on our online store.

-->
