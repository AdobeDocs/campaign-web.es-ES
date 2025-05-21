---
audience: end-user
title: Uso de la actividad de flujo de trabajo Cambiar fuente de datos
description: Aprenda a utilizar la actividad del flujo de trabajo Cambiar fuente de datos
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 13%

---

# Cambio de la fuente de datos {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Cambio de la fuente de datos"
>abstract="La actividad **Cambiar fuente de datos** le permite seleccionar una fuente de datos diferente para la tabla de trabajo del flujo de trabajo."

La actividad **Cambiar fuente de datos** es una actividad **segmentación**. Esta actividad le permite cambiar la fuente de datos utilizada por la tabla de trabajo del flujo de trabajo. Esto proporciona más flexibilidad al permitirle administrar los datos en sus diferentes bases de datos y mejorar el rendimiento.

En los flujos de trabajo, los datos que pasan de una actividad a otra mediante transiciones se almacenan en una **Tabla de trabajo** temporal. De forma predeterminada, las tablas de trabajo se crean en la misma base de datos que el origen de los datos procesados. Por ejemplo, al consultar la tabla &quot;Perfiles&quot;, almacenada en la base de datos en la nube, se crea una tabla de trabajo en la misma base de datos en la nube.

En algunos casos, los datos no están disponibles en la base de datos actual o no son lo suficientemente eficientes como para realizar operaciones unitarias. Por lo tanto, es posible que deba forzar el flujo de trabajo para que utilice una base de datos diferente para realizar estas operaciones agregando una actividad **[!UICONTROL Cambiar fuente de datos]**.

Encontrará información detallada sobre la arquitectura de Campaign en la [documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html).

>[!IMPORTANT]
>
>Tenga en cuenta que las actividades **[!UICONTROL Cambiar dimensión]** y **[!UICONTROL Cambiar fuente de datos]** no deben agregarse en una fila. Si necesita usar ambas actividades consecutivamente, incluya una actividad **[!UICONTROL Enrichment]** entre ellas. Esto garantiza una ejecución adecuada y evita posibles conflictos o errores.

<!--

Let's say you want to send VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Configuración de la actividad Cambiar fuente de datos {#configure}

Siga estos pasos para configurar la actividad **Cambiar fuente de datos**:

![Captura de pantalla que muestra cómo agregar la actividad Cambiar fuente de datos a un flujo de trabajo.](../assets/workflow-change-data-source-add.png)

1. Agregue una actividad **Cambiar fuente de datos** a su flujo de trabajo.

1. Defina el origen de datos al que desea mover la tabla de trabajo:

   * **[!UICONTROL Base de datos de Campaign predeterminada (PostgreSQL)]**: use la base de datos local de Campaign predeterminada.
   * **[!UICONTROL Cuenta externa de FDA]**: use bases de datos de nube externas conectadas a Adobe Campaign mediante la capacidad de acceso de datos federado.

     >[!AVAILABILITY]
     >
     >La configuración de Campaign y la conexión a sistemas externos están restringidas a usuarios avanzados y solo están disponibles desde la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=es){target="_blank"}

1. Configure el flujo de trabajo para que realice las operaciones deseadas utilizando la nueva fuente de datos.

<!--
## Example {#example}

The workflow below illustrates the use case detailed earlier, sending VIP customers offer codes that they can redeem on our online store.

-->