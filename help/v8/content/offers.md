---
audience: end-user
title: Envío de ofertas
description: Envío de ofertas
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Alfa"
source-git-commit: 4fbab5ddf2f1c69fbe27d214aa3e349075054c10
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 95%

---


# Envío de ofertas {#offers-content}

La web de Adobe Campaign versión 8 le permite enviar ofertas que se han creado en la consola con sus correos electrónicos mediante el uso del módulo **[!UICONTROL Interacción]**. Para obtener más información sobre la interacción y cómo administrar un catálogo de ofertas en la consola, consulte la [documentación de la versión 8 de Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=es){target="_blank"}.

Los pasos para enviar un correo electrónico son los siguientes:

1. [Configurar las ofertas que se van a proponer](#configure),
1. [Insertar las ofertas en el correo electrónico](#insert).

## Configurar las ofertas que se van a proponer {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Configuración de ofertas"
>abstract="Configurar qué ofertas se deben proponer a los destinatarios."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Configuración avanzada de ofertas"
>abstract="Configurar las opciones avanzadas en las ofertas."

1. Para seleccionar las ofertas que desea proponer en el correo electrónico, haga clic en el botón **[!UICONTROL Ofertas]** en la pantalla de edición del contenido del correo electrónico.

   ![](assets/setup-offers.png)

1. Configurar qué ofertas se deben proponer a los destinatarios. En primer lugar, seleccione el **[!UICONTROL espacio de ofertas]** que coincida con el entorno de la oferta.

   ![](assets/create-content-offers.png)

1. Para restringir la selección de ofertas del motor, seleccione la **[!UICONTROL Categoría de oferta]** específica en la que se ordenan las ofertas. Al seleccionar una carpeta, todas las subcarpetas se incluyen automáticamente y no se pueden eliminar. Tenga en cuenta que la IU de no refleja este comportamiento.

   Si no se especifica ninguna categoría, el motor de ofertas tendrá en cuenta todas las ofertas contenidas en el entorno, a menos que se seleccione un **[!UICONTROL Tema de oferta]**.

   >[!NOTE]
   >
   >Los temas son palabras clave que se definen de forma ascendente en las categorías. Estos actúan como un filtro y permiten refinar la cantidad de ofertas que se presentarán seleccionándolas de un conjunto de categorías.

1. Utilice el campo **[!UICONTROL Propuestas]** para especificar el número de ofertas que desea insertar en el correo electrónico.

1. Seleccione la opción **[!UICONTROL Excluir destinatarios no elegibles]** si es necesario.

   Esta opción permite activar o desactivar la exclusión de destinatarios para los que no haya suficientes ofertas elegibles.

   * Si la opción está habilitada, los destinatarios que no tengan suficientes propuestas se excluyen del envío.
   * Si la opción está deshabilitada, estos destinatarios no se excluyen, pero no pueden tener el número solicitado de propuestas.

1. Si es necesario, seleccione la opción **[!UICONTROL Ocultar todo si no se selecciona ninguna oferta]**.

   Esta opción le permite elegir cómo se procesará el mensaje en caso de que una de las propuestas no exista.

   * Cuando se habilita esta casilla, no se muestra la representación de la propuesta que falta, y no aparecerá ningún contenido en el mensaje para esta propuesta.
   * Si la opción está deshabilitada, el mensaje en sí se cancela durante el envío y los destinatarios ya no recibirán ningún mensaje.

Una vez configuradas las ofertas para proponerlas en el correo electrónico, puede insertarlas en el correo electrónico mediante el Editor de expresiones. [Aprenda a insertar ofertas en el correo electrónico](#insert)

## Inserción de ofertas en el correo electrónico {#insert}

Las ofertas se pueden añadir al correo electrónico mediante el Editor de expresiones. Pueden insertarse:

* En la línea de asunto del correo electrónico,
* En el cuerpo del correo electrónico, permitiendo la personalización en cualquier componente de contenido. [Aprenda a añadir componentes de contenido](content-components.md)

>[!NOTE]
>
>Antes de insertar una oferta, asegúrese de que haya [configurado qué ofertas proponer con el correo electrónico](#configure).

Para insertar una oferta mediante el Editor de expresiones, siga estos pasos:

1. Abra el Editor de expresiones y seleccione el menú **[!UICONTROL Propuestas]**.

   Las propuestas disponibles se muestran en la lista. El número de propuestas se define al configurar las ofertas que se van a proponer.

   ![](assets/offer-insertion.png)

1. Añada las propuestas al asunto o al cuerpo del correo electrónico utilizando los campos de personalización, las funciones de renderización o los atributos de oferta disponibles para cada propuesta.

   ![](assets/offer-inserted.png)
