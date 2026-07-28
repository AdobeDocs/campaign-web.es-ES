---
audience: end-user
title: Creación y administración de espacios de oferta
description: Obtenga información sobre cómo crear, configurar, implementar y previsualizar espacios de ofertas en Campaign Web
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: tm+mt
source-wordcount: 921
ht-degree: 0%

---

# Creación y administración de espacios de oferta {#offer-space}

Un **espacio de ofertas** define dónde y cómo se expone una oferta a un contacto: qué canal utiliza (correo electrónico, correo directo, SMS, web entrante, etc.), qué campos de contenido puede utilizar la oferta y cómo se crea la representación final. Un solo entorno puede contener varios espacios de oferta, uno para cada punto de exposición.

Un espacio de oferta no es un canal en sí mismo. Representa una ubicación específica en la que la oferta se muestra en un canal. Dos titulares en la misma página web suelen corresponder a dos espacios de oferta diferentes. Para ver el modelo conceptual completo, consulte la [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}.

## Creación o modificación de un espacio de oferta{#create-offer-space}

Los espacios de ofertas se almacenan en la carpeta del entorno de ofertas. Para examinar los espacios de ofertas disponibles en la plataforma, abra el **[!UICONTROL Explorador]**, navegue hasta el entorno de ofertas y seleccione la subcarpeta que los contiene.

![Captura de pantalla que muestra la lista del espacio de ofertas.](assets/offers-space.png){zoomable="yes"}

Desde allí, puede abrir un espacio de ofertas existente o crear uno nuevo haciendo clic en **[!UICONTROL Crear espacio de ofertas]**.

![Captura de pantalla que muestra la pantalla del espacio de ofertas.](assets/offers-space-1.png){zoomable="yes"}

### Definición de las propiedades {#properties}

Esta sección le permite:

* Escriba una **[!UICONTROL Etiqueta]** para el espacio de ofertas.
* Seleccione el **[!UICONTROL canal]** que coincida con el punto de exposición (correo electrónico, correo directo, SMS, web, etc.).
* Seleccione **[!UICONTROL Habilitar modo unitario]** si este espacio de oferta también debe admitir llamadas unitarias (en tiempo real, de una sola oferta) al motor de oferta, además de llamadas de entrega en masa.

### Definición de los campos de contenido {#content-fields}

Los campos de contenido enumeran los atributos que se pueden editar en el nivel de oferta y reutilizar mediante la función de renderización. El orden en que se agregan los campos al espacio de oferta impulsa el orden en que se exponen en la sección de la oferta **[!UICONTROL Contenido]**.

De manera predeterminada, cada oferta se envía con los siguientes campos de contenido predeterminados: **[!UICONTROL Título]**, **[!UICONTROL URL de destino]**, **[!UICONTROL URL de imagen]**, **[!UICONTROL contenido de HTML]** y **[!UICONTROL Contenido de texto]**. Puede ampliar esta lista con cualquier campo personalizado que necesite para el procesamiento, por ejemplo, **contenido corto**, **URL rastreada** o cualquier atributo agregado mediante la extensión de esquema.

Haga clic en **[!UICONTROL Agregar campo de contenido]** y, a continuación, seleccione el atributo que desee exponer desde el esquema de oferta, o haga clic en **[!UICONTROL Editar expresión]** para definir una expresión personalizada en su lugar.

>[!IMPORTANT]
>
>Para que un atributo personalizado se pueda editar desde la sección de la oferta **[!UICONTROL Contenido]**, el atributo también debe declararse en la sección **[!UICONTROL Contenido de la oferta]** del esquema [!DNL nms:offer]. Más información en [Trabajar con esquemas](../administration/schemas.md).

### Configuración de las funciones de renderización {#rendering}

Las funciones de renderización crean la representación de oferta final a partir de los campos de contenido. Puede elegir entre la renderización predeterminada (que simplemente genera el contenido tal cual) o una función personalizada que combine los campos con HTML, XML o texto.

Seleccione la pestaña **[!UICONTROL HTML rendering]**, **[!UICONTROL XML rendering]** o **[!UICONTROL Text rendering]** y habilite **[!UICONTROL Overload the rendering function]** para activarla.

Utilice el editor de expresiones para escribir la función de renderización. Puede hacer referencia a los campos de contenido definidos en el espacio, los atributos de oferta y cualquier función desde el [editor de expresiones](../query/expression-editor.md).

>[!NOTE]
>
>Si no se define ninguna función de renderización, el contenido de la oferta se devuelve tal cual con los atributos predeterminados. La función de renderización XML solo se puede usar cuando se selecciona **[!UICONTROL Habilitar modo unitario]** en el espacio de oferta.

### Configuración del almacenamiento y el estado de la propuesta {#storage}

Esta sección le permite controlar cómo se mantienen las propuestas generadas a través de este espacio y cómo evoluciona su estado a lo largo de su ciclo de vida:

* **[!UICONTROL Deshabilitar la inserción de propuestas]**: evita que las propuestas generadas a través de este espacio de oferta se inserten en la tabla de almacenamiento de propuestas.

* **[!UICONTROL Estado]** de la propuesta: estado aplicado a la propuesta en el momento en que el motor de oferta la devuelve (normalmente **[!UICONTROL Presentada]** para las entregas salientes).

* **[!UICONTROL Estado]** al aceptar: estado aplicado cuando el destinatario interactúa con la oferta (normalmente **[!UICONTROL Aceptado]**).

Los valores de estado disponibles coinciden con la lista utilizada por la consola de cliente. Para obtener más información, consulte [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#offer-proposition-statuses){target="_blank"} en la documentación de la consola.

<!--
>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.
-->

### Configuración avanzada {#advanced}

Esta sección le permite definir la **[!UICONTROL identificación de destino]**. Haga clic en **[!UICONTROL Agregar]** y seleccione uno o varios atributos de **[!UICONTROL Destinatario]** o haga clic en **[!UICONTROL Editar expresión]** para definir una expresión personalizada en su lugar. Esta configuración es opcional para un espacio de oferta básico. Para obtener toda la referencia y el comportamiento, consulte la [documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html){target="_blank"}.

Los espacios de ofertas creados en el **canal web entrante** también requieren que el sitio web se configure para mostrar la oferta y para llamar al motor de oferta. Esta integración se realiza en la consola del cliente; consulte [Presentar ofertas en tiempo real](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html){target="_blank"} y [Configurar la integración del motor de ofertas](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html){target="_blank"} en la documentación de Campaign v8.

## Implementación del espacio de ofertas {#deploy}

Se debe implementar un espacio de oferta antes de poder utilizarlo en una entrega. Guarde el espacio de ofertas y haga clic en **Implementar**. El estado de la implementación se refleja en el espacio de ofertas.

![Captura de pantalla que muestra la implementación de la oferta.](assets/offers-space-2.png){zoomable="yes"}

## Previsualización del espacio de oferta {#preview}

La previsualización permite simular cómo se selecciona y procesa una oferta para un destino determinado.

1. En el espacio de ofertas, selecciona la pestaña **[!UICONTROL Vista previa]** junto a **[!UICONTROL Información general]**.

   ![Captura de pantalla que muestra la vista previa de la oferta.](assets/offers-space-3.png){zoomable="yes"}

1. Seleccione un perfil de destino y ejecute la previsualización. Las ofertas coincidentes se devuelven con la representación producida por la función de renderización.

>[!NOTE]
>
>Si no se devuelve ninguna propuesta, compruebe las reglas de idoneidad de las ofertas y la configuración del espacio.

A continuación, [cree una oferta](create-offer.md) en el catálogo y asígnela a este espacio.
