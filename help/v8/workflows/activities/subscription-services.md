---
audience: end-user
title: Uso de la actividad Servicios de suscripción
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo Servicios de suscripción
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 0e5b5e916309b2a337ac86f3741bcb83237b3fad
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 18%

---

# Servicios de suscripción {#subscription-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Actividad Servicios de suscripción"
>abstract="La actividad Servicios de suscripción permite suscribirse o cancelar la suscripción en varios perfiles de un servicio en una sola acción."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Parámetros generales del servicio de suscripción"
>abstract="Elija el servicio deseado y elija la acción que desea realizar (suscribirse o cancelar la suscripción). Active la opción **Enviar un mensaje de confirmación** para notificar a la población que se ha suscrito o ha cancelado la suscripción del servicio seleccionado."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Generar una transición saliente"
>abstract="Alterne la opción **Generar una transición saliente** para añadir una transición después de la actividad."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_additionalinfo"
>title="Más información"
>abstract="Más información"

El **Servicios de suscripción** la actividad es una **Administración de datos** actividad. Permite crear o eliminar una suscripción a un servicio informativo para la población especificada en la transición.

## Configure la actividad Subscription services {#subscription-services-configuration}

Siga estos pasos para configurar el **Servicios de suscripción** actividad:

1. Añadir un **Servicios de suscripción** en el flujo de trabajo. Puede utilizar esta actividad después de segmentar perfiles o importar un archivo con datos identificados.

1. Seleccione el servicio para el que desea administrar las suscripciones mediante una de las siguientes opciones:

   * **[!UICONTROL Seleccione un servicio específico]**: Seleccione manualmente un servicio utilizando **[!UICONTROL Servicio]** field.

   * **[!UICONTROL Desde transición entrante]**: utilice el servicio especificado en la transición entrante. Por ejemplo, puede importar un archivo que especifique el servicio que se va a administrar para cada línea. El servicio en el que se realiza la operación se selecciona dinámicamente para cada perfil.

   ![](../assets/workflow-subscription-service.png)

1. Seleccione la operación que desea realizar: **Suscribirse** o **Cancelar suscripción**.

   Si el servicio se define en la transición entrante, puede elegir cómo recuperar esta operación:

   * **Seleccione un tipo de operación específico**: Seleccione manualmente la operación que desea realizar (**Suscribirse** o **Cancelar suscripción**)

   * **Seleccionar un tipo de operación de una ruta de transición entrante**: seleccione la columna de los datos de entrada que especifica la operación que se realizará para cada registro. Por ejemplo, puede importar un archivo que especifique la operación que se va a realizar para cada línea en una columna &quot;operación&quot;.

     Aquí solo se pueden seleccionar campos booleanos o enteros. Asegúrese de que los datos que contienen la operación que se va a realizar coinciden con este formato. Por ejemplo, si está cargando datos desde una actividad de Cargar archivo, compruebe que ha establecido correctamente el formato de la columna que contiene la operación en **[!UICONTROL Cargar archivo]** actividad. Se presenta un ejemplo en [esta sección](#uc2).

     >[!CAUTION]
     >
     >De forma predeterminada, si selecciona esta opción, la variable **Servicios de suscripción** La actividad espera tener una definición de vínculo a **Servicios (nms)** configuradas en el flujo de trabajo. Para ello, asegúrese de haber configurado un vínculo de reconciliación en una **Actividad de enriquecimiento** en el flujo de trabajo. Hay disponible un ejemplo que muestra cómo utilizar esta opción [aquí](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Para notificar a los destinatarios que se han suscrito o dado de baja del servicio seleccionado, cambie el **[!UICONTROL Enviar un mensaje de confirmación]** opción activada. El contenido de esta notificación se define en una plantilla de envío asociada al servicio de información.

1. Si utiliza datos de una transición entrante, se debe crear un **[!UICONTROL Información adicional]** se muestra esta sección, que le permite especificar los datos y el origen de la suscripción para cada registro. Puede dejar esta sección vacía, en cuyo caso no se definirá ninguna fecha ni ningún origen al ejecutar el flujo de trabajo.

   * Si los datos de entrada contienen una columna que indica la fecha de suscripción del perfil al servicio, puede seleccionarla en la **[!UICONTROL Fecha]** field.

   * En el **[!UICONTROL Ruta de origen]** , defina el origen de la suscripción. Puede establecerlo en uno de los campos de los datos de entrada o en un valor constante de su elección marcando la variable **[!UICONTROL Establecer una constante como origen]** opción.

   ![](../assets/workflow-subscription-service-additional.png)

1. Para añadir una transición saliente después de la actividad, cambie el **[!UICONTROL Generación de una transición saliente]** opción activada.

## Ejemplos {#example}

### Suscripción de una audiencia a un servicio específico {#uc1}

Este flujo de trabajo siguiente muestra cómo suscribir una audiencia a un servicio existente.

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL Crear audiencia]** la actividad se dirige a una audiencia existente.

* A **[!UICONTROL Servicios de suscripción]** La actividad de permite seleccionar el servicio al que se deben suscribir los perfiles.

### Actualización de varios estados de suscripción de un archivo {#uc2}

El flujo de trabajo siguiente muestra cómo importar un archivo que contiene perfiles y actualizar su suscripción a varios servicios especificados en el archivo.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Cargar archivo]** La actividad de carga un archivo CSV que contiene los datos y define la estructura de las columnas importadas. Las columnas &quot;servicio&quot; y &quot;operación&quot; especifican el servicio que se va a actualizar y la operación que se va a realizar (suscripción o baja).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Como ha visto, la operación se especifica en el archivo como “sub” o “unsub”. El sistema espera que un valor **booleano** o **entero** reconozca la operación que se va a realizar: “0” para cancelar la suscripción y “1” para suscribirse. Para hacer coincidir este requisito:
   * El **Tipo de datos** para la columna &quot;operación&quot; se establece en entero.
   * A **Reasignación de valores** debe realizarse para que coincidan los valores &quot;sub&quot; y &quot;unsub&quot; con los valores &quot;1&quot; y &quot;0&quot;.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Si el archivo ya utiliza “0” y “1” para identificar la operación, no es necesario volver a asignar esos valores. Solo asegúrese de que la columna se procesa como **Booleano** o **Entero** en las columnas del archivo de ejemplo.

* A **[!UICONTROL Reconciliación]** La actividad identifica los datos del archivo como pertenecientes a la dimensión de perfil de la base de datos de Adobe Campaign. El **email** del archivo coincide con el campo **email** del recurso de perfil.

  ![](../assets/workflow-subscription-service-uc2-reconciliation.png)

* Un **[!UICONTROL Enriquecimiento]** La actividad de crea un vínculo de reconciliación a la tabla &quot;Servicios (nms)&quot;, con una unión simple entre la columna &quot;servicio&quot; del archivo cargado y el campo &quot;nombre interno&quot; de los servicios en la base de datos.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Servicios de suscripción]** identifica los servicios que se van a actualizar como procedentes de la transición.

  El **[!UICONTROL Tipo de operación]** se identifica como proveniente de **operación** del archivo. Aquí solo se pueden seleccionar los campos booleano o entero. Si la columna del archivo que contiene la operación que se va a realizar no aparece en la lista, asegúrese de que ha configurado correctamente el formato de columna en la **[!UICONTROL Cargar archivo]** actividad de, tal como se explicó anteriormente en este ejemplo.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
