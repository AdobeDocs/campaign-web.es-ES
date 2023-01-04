---
audience: end-user
title: Enviar ofertas
description: Enviar ofertas
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: bf55b13011f7d2bdafcc55b1b2539c4ce590dd85
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 5%

---

# Enviar ofertas {#offers-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Configuración de ofertas"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Configuración avanzada de ofertas"
>abstract="TBC"

>[!NOTE]
>
>Esta documentación está en construcción y se actualiza con frecuencia. La versión final de este contenido estará lista en enero de 2023.

La web de Adobe Campaign v8 le permite enviar con sus correos electrónicos ofertas que se han creado en la consola mediante el uso de **[!UICONTROL Interacción]** módulo. Para obtener más información sobre la interacción y cómo administrar un catálogo de ofertas en la consola, consulte la [Documentación de Campaign V8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html)

Los pasos para enviar ofertas con un correo electrónico son los siguientes:

1. [Configurar las ofertas que se van a proponer](#configure),
1. [Inserte las ofertas en el correo electrónico](#insert).

## Configurar las ofertas que se van a proponer {#configure}

Para seleccionar las ofertas que desea proponer en el correo electrónico, haga clic en el botón **[!UICONTROL Ofertas]** en la pantalla de edición de contenido del correo electrónico y, a continuación, configure las ofertas que desea proponer.

![](assets/create-content-offers.png)

1. Seleccione el **[!UICONTROL Espacio de oferta]** que coincida con el entorno de la oferta.

1. Para restringir la selección de ofertas del motor, seleccione una **[!UICONTROL Categoría de oferta]** en el que se ordenan las ofertas.

   Si no se especifica ninguna categoría, el motor de oferta tendrá en cuenta todas las ofertas contenidas en el entorno, a menos que se **[!UICONTROL Tema de oferta]** está seleccionado.

   >[!NOTE]
   >
   >Los temas son palabras clave definidas hacia arriba en las categorías. Actúan como un filtro y permiten refinar el número de ofertas que se presentarán seleccionándolas en un conjunto de categorías.

1. Utilice la variable **[!UICONTROL Propuestas]** para especificar el número de ofertas que desea insertar en el correo electrónico.

1. Seleccione la opción **[!UICONTROL Excluir destinatarios no elegibles]** si es necesario.

   esta opción permite activar o desactivar la exclusión de destinatarios para los que no haya suficientes ofertas aptas.

   * Si la opción está activada, los destinatarios que no tengan suficientes propuestas se excluirán de la entrega.
   * Si la opción está desactivada, estos destinatarios no se excluirán, pero no tendrán el número solicitado de propuestas.

1. Si es necesario, seleccione la **[!UICONTROL Ocultar todo si no se selecciona ninguna oferta]** .

   Esta opción le permite elegir cómo se procesará el mensaje en caso de que una de las propuestas no exista.

   * Si la opción está activada, la representación de la propuesta que falta no se muestra y no aparecerá ningún contenido en el mensaje para esta propuesta.
   * Si la opción está desactivada, el mensaje en sí se cancela durante la entrega y los destinatarios ya no reciben ningún mensaje.

Una vez configuradas las ofertas para proponerlas en el correo electrónico, puede insertarlas en el correo electrónico mediante el Editor de expresiones. [Aprenda a insertar ofertas en el correo electrónico](#insert)

## Inserción de ofertas en el correo electrónico {#insert}

Las ofertas se añaden a un correo electrónico mediante el Editor de expresiones. Pueden insertarse:

* en la línea de asunto del correo electrónico,
* en el cuerpo del correo electrónico permitiendo la personalización en cualquier componente de contenido. [Aprenda a añadir componentes de contenido](content-components.md)

>[!NOTE]
>
>Antes de insertar una oferta, asegúrese de que tiene [configurado qué ofertas proponer con el correo electrónico](#configure).

Para insertar una oferta mediante el Editor de expresiones, siga estos pasos:

1. Abra el Editor de expresiones y seleccione la opción **[!UICONTROL Propuestas]** para abrir el Navegador.

   Las propuestas disponibles se muestran en la lista. El número de propuestas se define al configurar las ofertas que se van a proponer.

   ![](assets/offer-insertion.png)

1. Añada las propuestas al asunto o al cuerpo del correo electrónico utilizando los campos de personalización, las funciones de renderización o los atributos de oferta disponibles para cada propuesta.

   ![](assets/offer-inserted.png)
