---
audience: end-user
title: Adición de ofertas en los mensajes
description: Obtenga información sobre cómo añadir y enviar ofertas
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 23%

---

# Añadir ofertas a los mensajes {#offers-content}

Puede añadir ofertas a los envíos en la interfaz de usuario web de Adobe Campaign. Estas ofertas están disponibles en el menú de la izquierda **Ofertas**, que le permite acceder a la lista de ofertas. Todas estas ofertas son de solo lectura y deben crearse en la consola del cliente de Campaign utilizando el módulo **[!UICONTROL Interaction]**. Para obtener más información sobre interacción y cómo administrar un catálogo de ofertas en la consola, consulte la [documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=es){target="_blank"}.

Los pasos para enviar ofertas con una entrega son los siguientes:

1. [Configurar las ofertas que se van a proponer](#configure)
1. [Inserción de las ofertas en la entrega](#insert)

## Configurar las ofertas que se van a proponer {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Definir los parámetros de las ofertas"
>abstract="Configure qué ofertas deben proponerse a los destinatarios, definiendo un espacio de ofertas, opcionalmente una categoría y un tema, y especifique el número de ofertas que desea insertar en el envío."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Configuración avanzada de ofertas"
>abstract="Puede habilitar la exclusión de destinatarios para los que no haya suficientes ofertas aptas y elegir cómo se procesa el mensaje en caso de que una de las propuestas no exista."

Adobe Campaign permite responder en tiempo real durante una interacción a un contacto determinado proponiendo una o varias ofertas específicas. Estas ofertas pueden ser mensajes de comunicación sencillos, ofertas especiales sobre uno o varios productos o un servicio.

Para seleccionar las ofertas que desea añadir a la entrega, siga los pasos a continuación.

1. Haga clic en el botón **[!UICONTROL Configurar ofertas]** de la pantalla de edición de contenido de entrega.

   ![Captura de pantalla que muestra el botón de configuración de oferta en la pantalla de edición de contenido de entrega](assets/offer-setup.png){zoomable="yes"}

1. Configurar qué ofertas se deben proponer a los destinatarios.

   En primer lugar, seleccione el **[!UICONTROL espacio de ofertas]** que coincida con el entorno de ofertas. Aprenda a crear un espacio de ofertas en la [documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}.

   ![Captura de pantalla que muestra la selección del espacio de ofertas en el contenido de creación de ofertas](assets/offer-create-content.png){zoomable="yes"}

1. Para restringir la selección de ofertas del motor, seleccione la **[!UICONTROL Categoría de oferta]** específica en la que se ordenan las ofertas.

   Al seleccionar una carpeta, todas las subcarpetas se incluyen automáticamente y no se pueden eliminar. Tenga en cuenta que la interfaz [!DNL Campaign] no refleja este comportamiento.

   >[!NOTE]
   >
   >Si no se especifica ninguna categoría, el motor de ofertas tendrá en cuenta todas las ofertas contenidas en el entorno, a menos que se seleccione un **[!UICONTROL Tema de oferta]**.

1. (Opcional) Introduzca una temática para filtrar las categorías. Las temáticas son palabras clave definidas en sentido ascendente en las categorías. Actúan como un filtro y refinan el número de ofertas que se presentarán seleccionándolas en un conjunto de categorías.

1. Utilice el campo **[!UICONTROL Proposiciones]** para especificar el número de ofertas que desea insertar en la entrega.

1. Seleccione la opción **[!UICONTROL Excluir destinatarios no elegibles]** si es necesario.

   Esta opción permite activar o desactivar la exclusión de destinatarios para los que no haya suficientes ofertas aptas:

   * Si la opción está habilitada, los destinatarios que no tengan suficientes propuestas se excluyen del envío.
   * Si la opción está desactivada, estos destinatarios no se excluyen, pero no pueden tener el número solicitado de propuestas.

1. Si es necesario, seleccione la opción **[!UICONTROL Ocultar todo si no se selecciona ninguna oferta]**.

   Esta opción le permite elegir cómo se procesa el mensaje en caso de que una de las propuestas no exista:

   * Si la opción está activada, no se muestra la representación de la propuesta que falta y no aparece ningún contenido en el mensaje para esta propuesta.
   * Si la opción está desactivada, el mensaje en sí se cancela durante la entrega y los destinatarios ya no pueden recibir mensajes.

Una vez configuradas las ofertas para proponerlas en la entrega, puede insertarlas en el contenido de la entrega.

## Inserción de ofertas en la entrega {#insert}

Las ofertas se pueden agregar a la entrega mediante el [editor de expresiones](../personalization/gs-personalization.md#access). Se pueden insertar en la línea de asunto o en el cuerpo del envío.

>[!CAUTION]
>
>Antes de insertar una oferta en una entrega, asegúrese de tener [configurado qué ofertas proponer con esa entrega](#configure).

Para insertar una oferta mediante el editor de expresiones, siga los pasos a continuación.

1. Acceda a la línea de asunto o al contenido de cualquier entrega.

1. Coloque el cursor donde desee insertar la oferta y abra el editor de expresiones utilizando el icono de personalización.

   ![Captura de pantalla que muestra el icono de personalización usado para abrir el editor de expresiones](assets/offer-insert-perso-icon.png){zoomable="yes"}

1. Seleccione el menú **[!UICONTROL Proposiciones]**. Las propuestas disponibles se muestran en la lista.

   >[!NOTE]
   >
   >El número de propuestas se define al [configurar ofertas](#configure) para la entrega actual.

1. Defina cada propuesta utilizando los campos de personalización, las funciones de renderización o los atributos de oferta disponibles.

   ![Captura de pantalla que muestra una oferta insertada en el contenido de la entrega](assets/offer-inserted.png){zoomable="yes"}

   >[!NOTE]
   >
   >El número de propuestas disponibles depende de la forma en que se configure la visualización del motor y su orden depende de la prioridad de las ofertas. Obtenga más información en la [documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

1. Guarde los cambios.

1. Finalice el contenido, pruebe y realice la entrega. [Más información](gs-messages.md).

Ahora, cuando un destinatario recibe la entrega, se muestra la oferta correcta a ese perfil específico.