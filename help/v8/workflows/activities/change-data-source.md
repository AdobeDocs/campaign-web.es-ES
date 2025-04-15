---
audience: end-user
title: Usar el fuente de datos de cambio flujo de trabajo actividad
description: Aprenda a utilizar el actividad Change fuente de datos flujo de trabajo
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

La **actividad Change fuente de datos** es un **direccionamiento** actividad. Este actividad le permite cambiar el fuente de datos utilizado por la mesa de trabajo de su flujo de trabajo. Esto proporciona más flexibilidad al permitirle administrar datos en sus diferentes bases de datos y mejorar el rendimiento.

En flujos de trabajo, los datos transportados de una actividad a otra a través de transiciones se almacenan en una tabla **de trabajo temporal**. De forma predeterminada, las tablas de trabajo se crean en la misma base de datos que la fuente de los datos procesados. Por ejemplo, al consultar la tabla &quot;Perfiles&quot;, almacenada en la base de datos Cloud, se crea una tabla de trabajo en la misma base de datos Cloud.

En algunos casos, los datos no están disponibles en la base de datos actual o no son lo suficientemente eficientes como para realizar operaciones unitarias. Por lo tanto, es posible que deba forzar a la flujo de trabajo a utilizar una base de datos diferente para realizar estas operaciones agregando un **[!UICONTROL actividad de fuente de datos]** cambio.

Puede encontrar información detallada sobre Campaign arquitectura en [Campaign documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html) de la versión 8 (consola del cliente).

>[!IMPORTANT]
>
>Tenga en cuenta que las actividades Cambiar Dimension ]**y**[!UICONTROL  Cambiar fuente ]**de**[!UICONTROL  datos no deben agregarse en una fila. Si necesita utilizar ambas actividades consecutivamente, incluya una **[!UICONTROL actividad de enriquecimiento]** entre ellas. Esto garantiza una ejecución correcta y evita posibles conflictos o errores.

<!--

Let's say you want to send VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Configurar el cambio fuente de datos actividad {#configure}

Siga estos pasos para configurar el **actividad Change fuente de datos** :

![Captura de pantalla que muestra cómo agregar el actividad Change fuente de datos a un flujo de trabajo.](../assets/workflow-change-data-source-add.png)

1. añadir un **cambio fuente de datos** actividad a su flujo de trabajo.

1. Defina la fuente de datos hacia la que desee mover la tabla de trabajo:

   * **[!UICONTROL Base de datos de Campaign predeterminada (PostgreSQL):]** utilice la base de datos local Campaign predeterminada.
   * **[!UICONTROL FDA cuenta externa]**: utilice bases de datos externas en la nube conectadas a Adobe Campaign a través de acceso de datos federado capacidad.

     >[!AVAILABILITY]
     >
     >La configuración de Campaign y la conexión a sistemas externos están restringidas a usuarios avanzados y solo están disponibles desde la consola del cliente. [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=es){target="_blank"}

1. Configure su flujo de trabajo para realizar las operaciones deseadas con la nueva fuente de datos.

<!--
## Example {#example}

The workflow below illustrates the use case detailed earlier, sending VIP customers offer codes that they can redeem on our online store.

-->