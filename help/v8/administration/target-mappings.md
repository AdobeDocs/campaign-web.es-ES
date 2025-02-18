---
title: Administrar asignaciones de destino
description: Obtenga información sobre cómo administrar las asignaciones de destino.
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 4%

---

# Administrar asignaciones de destino {#target-mappings}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_list"
>title="Asignaciones de destino "
>abstract="Asignaciones de destino"

## Acerca de las asignaciones de destino {#about}

Cada canal de comunicación utiliza una asignación de destino predeterminada para dirigirse a sus destinatarios. Por ejemplo, de forma predeterminada, las plantillas de envíos de correo electrónico y SMS tienen como destino **[!UICONTROL Destinatarios]**. El destino de mapeo utiliza los campos de la tabla **nms:recipient.** Para las notificaciones push, la asignación de destino predeterminada es **Aplicaciones del suscriptor (nms:appSubscriptionRcp)**, que está vinculada a la tabla de destinatarios.

Se puede acceder a las asignaciones de destino desde el menú **[!UICONTROL Administración]** > **[!UICONTROL Asignaciones de destino]**. Desde esta pantalla, puede acceder a los detalles de cada asignación de destino o crear nuevas asignaciones de destino para adaptarlas a sus necesidades.

![](assets/target-mappings-list.png)

Para obtener más información sobre las asignaciones de destino integradas proporcionadas con Adobe Campaign, consulte la [documentación de la consola del cliente de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=es){target="_blank"}.

## Creación de una asignación de destino {#create-mapping}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_properties"
>title="Propiedades de asignación de destinatario"
>abstract="La sección **[!UICONTROL Propiedades]** le permite definir la configuración genérica para la asignación de destino y la población de destino."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_mapping"
>title="Asignación de destinatario"
>abstract="La sección **[!UICONTROL Mapping]** permite identificar qué atributos del esquema de la asignación de destino se utilizarán para los distintos campos de direcciones de envío."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_denylist"
>title="Lista de bloqueados de asignación de destinatario"
>abstract="Lista de bloqueados de asignación de destinatario"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_storage"
>title="Almacenamiento de asignación de destinatario"
>abstract="La sección **[!UICONTROL Almacenamiento]** le permite identificar dónde se deben almacenar los registros."

Para crear una nueva asignación de destino, acceda al menú **[!UICONTROL Administración]** > **[!UICONTROL Asignaciones de destino]**. Haga clic en el botón **[!UICONTROL Crear asignación]** y luego siga los pasos detallados en las secciones a continuación.

1. En la sección **[!UICONTROL Propiedades]**, escriba una **[!UICONTROL Etiqueta]** para la asignación de destino.

1. Expanda la sección **[!UICONTROL Opciones adicionales]** para definir la configuración avanzada, como el nombre interno, la carpeta de almacenamiento y la descripción de la asignación de destino.

1. Seleccione la población objetivo. Puede:

   * **[!UICONTROL Usar la dimensión de segmentación directamente]**: seleccione la dimensión a la que se va a destinar directamente desde la lista de dimensiones disponibles.
   * **[!UICONTROL Usar datos vinculados]**: esta opción le permite comenzar desde una dimensión de segmentación (por ejemplo, suscripciones) y, a continuación, cambiar a la dimensión de segmentación a la que desee destinar (por ejemplo, destinatarios).

   ![](assets/target-mappings-properties.png)

1. Si la dimensión seleccionada no la está utilizando ya una asignación de destino existente, es necesario crear los esquemas para almacenar los registros. Para ello, hay opciones adicionales disponibles en la sección **[!UICONTROL Almacenamiento]**. Expanda la sección siguiente para obtener más detalles.

   +++Opciones de almacenamiento para nuevas dimensiones de segmentación

   1. **[!UICONTROL Espacio de nombres]**: identifique el espacio de nombres que se utilizará para crear los registros.
   1. **[!UICONTROL Sufijo del esquema de extensión]**: proporcione un sufijo para el nuevo esquema.

      En el ejemplo siguiente, el nombre del broadlog será &quot;cusbroadlogSupplier&quot;.

      ![](assets/target-mappings-new.png)

   1. **[!UICONTROL Registros de envío]**: active las opciones de esta sección para enriquecer los registros de envío con un campo de código de segmento o con un campo que contenga la dirección IP de envío. Por ejemplo, puede guardar un código de segmento calculado durante el flujo de trabajo en los registros de envío para refinar el objetivo más adelante. Esto le permite segmentar perfiles que tengan este código de segmento específico.

   1. **[!UICONTROL Exclusiones]**: especifique cómo desea almacenar los registros de exclusiones.

   1. **[!UICONTROL Registros de seguimiento]**: active la opción **[!UICONTROL Generar un esquema para el seguimiento]** para generar un esquema de almacenamiento para los registros de seguimiento

+++

1. Utilice la sección **[!UICONTROL Mapping]** para identificar qué atributos del esquema de la asignación de destino se utilizarán en cada campo de dirección de entrega. Para cada campo, seleccione el atributo que desee asignar. También puede crear una expresión para identificar el campo. Por ejemplo, puede aplicar una función menor al atributo de dirección.

   ![](assets/target-mappings-mapping.png)

1. Cuando la asignación de destino esté lista, haga clic en el botón **[!UICONTROL Crear]**. El sistema crea automáticamente la asignación de destino y todos los esquemas relacionados para los registros.

Una vez creada la asignación de destino, se muestran dos secciones adicionales en la pantalla:

* **[!UICONTROL Inclusión en la lista de bloqueados de]**: esta sección le permite identificar los atributos del esquema de la asignación de destino que se utilizarán para las listas de bloqueados de la.

  ![](assets/target-mappings-denylisting.png)

* **[!UICONTROL Almacenamiento]**: esta sección le permite identificar las tablas que se utilizarán para almacenar registros.

  ![](assets/target-mappings-storage.png)

   * **[!UICONTROL Esquema del mensaje]**: identifica el esquema que se va a utilizar para almacenar los registros de envío.
   * **[!UICONTROL Mensajes excluidos]**: esta sección especifica cómo administrar el almacenamiento de los registros de envío y exclusión.

      * **[!UICONTROL Almacenar exclusiones y mensajes en la misma tabla]**
      * **[!UICONTROL Almacenar solo mensajes]**: no almacene exclusiones.
      * **[!UICONTROL Almacenar exclusiones y mensajes en tablas independientes]**: seleccione el esquema que se utilizará para almacenar los registros de exclusión en el campo **[!UICONTROL Esquema de rechazo]**.

   * **[!UICONTROL Registros de seguimiento]**: elige dónde almacenar los registros de seguimiento y el origen de tráfico predeterminado.
   * **[!UICONTROL Campos adicionales]**: Esta sección le permite especificar una lista de campos adicionales para almacenar en los registros de envío. Estos campos pueden almacenar de forma permanente información sobre miembros individuales del público objetivo (p. ej., `recipient/@firstName`) o almacenar datos adicionales calculados durante el flujo de trabajo (p. ej. `[targetData/@offeCode]`)

     Para ello, seleccione **[!UICONTROL Agregar campo]**. Identifique la información que desee guardar en el campo **[!UICONTROL Source]** y el atributo que se utilizará en los registros de envío para guardar esta información en el campo **[!UICONTROL Destino]**.

     ![](assets/target-mappings-additional.png){width="50%" zoomable="yes"}
