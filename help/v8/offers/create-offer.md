---
audience: end-user
title: Creación y publicación de una oferta
description: Obtenga información sobre cómo crear, configurar, aprobar e implementar una oferta en Campaign Web
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 7bd09b83112efb99c90884b7da21a5e9a5c76b6c
workflow-type: tm+mt
source-wordcount: 1057
ht-degree: 2%

---

# Creación y publicación de una oferta {#create-offer}

Una **oferta** es una propuesta individual con su propio período de elegibilidad, filtro de destinatario, peso y contenido. Las ofertas se organizan en el catálogo de ofertas a través de **categorías** y se presentan a los destinatarios a través de **espacio de ofertas**.

Antes de crear una oferta, asegúrese de que el entorno de la oferta está configurado y de que se publica al menos un espacio de oferta. Obtenga más información en [Configurar un entorno de ofertas](offer-environment.md) y [Crear y administrar espacios de ofertas](offer-space.md).

## Acceso al catálogo de ofertas {#access}

Para examinar y crear ofertas, seleccione **[!UICONTROL Ofertas]** en el carril de navegación izquierdo. La lista muestra las ofertas existentes. Utilice el campo de búsqueda, el selector de carpetas o el [modelador de consultas](../query/query-modeler-overview.md) para filtrar la lista.

![Captura de pantalla que muestra el catálogo de ofertas.](assets/offers-offer.png){zoomable="yes"}

Haz clic en el nombre de una oferta para abrirla y editarla, o usa los tres puntos que hay junto a ella para **[!UICONTROL Duplicarla]** o **[!UICONTROL Eliminarla]**.

## Creación de una oferta {#create}

Para crear una oferta nueva:

1. En la lista de ofertas, haga clic en **[!UICONTROL Crear oferta]**.

1. Seleccione la **[!UICONTROL plantilla]** desde la que crear la oferta (por ejemplo, una oferta en blanco o una plantilla de oferta anónima).

   ![Captura de pantalla que muestra la creación de la oferta.](assets/offers-offer-1.png){zoomable="yes"}

1. Escriba una **[!UICONTROL Etiqueta]** y, opcionalmente, asigne la oferta a un operador usando **[!UICONTROL Asignado a]** o escriba un **[!UICONTROL Código de oferta]**.

1. Expanda **[!UICONTROL Opciones adicionales]** para editar el **[!UICONTROL nombre interno]** generado automáticamente, seleccione la **[!UICONTROL categoría]** en la que está almacenada la oferta o agregue una descripción. Este paso es opcional.

1. Expanda **[!UICONTROL Aprobaciones]** para asignar aprobadores a los grupos **[!UICONTROL Aprobación de elegibilidad]** y **[!UICONTROL Aprobación de contenido]**. Este paso es opcional.

1. Expanda **[!UICONTROL Opciones personalizadas]** para rellenar los campos adicionales que su organización haya agregado al esquema de ofertas. Los campos que se muestran en esta sección varían de una instancia de Campaign a otra. Este paso es opcional.

1. Haga clic en **[!UICONTROL Crear]**. Se muestra la pantalla de configuración completa.

   ![Captura de pantalla que muestra la pantalla Configuración de oferta.](assets/offers-offer-2.png){zoomable="yes"}

### Definición de la idoneidad {#eligibility}

Esta sección le permite controlar cuándo y a quién se puede presentar la oferta. Estas son las opciones disponibles:

* **[!UICONTROL Horario]**: establezca las fechas de inicio y finalización entre las cuales se puede presentar la oferta.

  >[!NOTE]
  >
  >Se tienen en cuenta las intersecciones del periodo de elegibilidad con la categoría principal: incluso si el propio calendario de la oferta es más amplio, la oferta solo se presenta mientras que su categoría principal también es elegible.

* **[!UICONTROL Filtros en el destino]** — Haga clic en **[!UICONTROL Crear filtro]** para abrir el generador de reglas y restringir la oferta a una audiencia específica. Deje el filtro vacío para que la oferta sea apta para toda la audiencia del entorno. Para reutilizar un **filtro predefinido** declarado a nivel de plataforma, consulte la [documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html){target="_blank"}. Los filtros predefinidos se crean desde la consola del cliente.

* **[!UICONTROL Administración de la ponderación de la oferta]** — Haga clic en **[!UICONTROL Mostrar ponderación de la oferta]** y luego en **[!UICONTROL Agregar ponderación]** para influir en la prioridad de la oferta cuando varias ofertas sean elegibles al mismo tiempo. Cada ponderación tiene una fecha de inicio, una fecha de finalización y un filtro opcional.

>[!NOTE]
>
>El motor de oferta clasifica las ofertas aptas por peso descendente y devuelve primero las propuestas con peso más alto. La lógica de selección (denominada **arbitraje**) también tiene en cuenta las reglas de elegibilidad y las ponderaciones configuradas en la categoría principal y en el entorno. Obtenga más información acerca del principio de arbitraje en la [Documentación de Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

### Definición del contenido {#content}

En la oferta, seleccione la ficha **[!UICONTROL Contenido]**. Esta pestaña define los valores que expondrá la función de renderización.

1. Complete los atributos predeterminados: **[!UICONTROL Title]**, **[!UICONTROL Destination URL]**, **[!UICONTROL Image URL]** y cualquier atributo personalizado declarado en el esquema de la oferta.

1. Use el [editor de expresiones](../query/expression-editor.md) para personalizar los valores con datos de perfil, atributos de oferta o campos de propuesta.

1. Para las cargas de HTML y de texto, haga clic en **[!UICONTROL Editar contenido]** para abrir el editor de contenido. Puede diseñar el contenido desde cero, codificar su propio HTML o importar el HTML existente, opcionalmente a partir de una plantilla de ejemplo.

>[!IMPORTANT]
>
>Los atributos disponibles en la sección **[!UICONTROL Content]** dependen del esquema [!DNL nms:offer]. Para exponer atributos personalizados, amplíe el esquema y selecciónelos en la sección **[!UICONTROL Contenido de la oferta]**. Más información en [Trabajar con esquemas](../administration/schemas.md).

## Previsualización de la oferta {#preview}

Puede obtener una vista previa de la oferta antes de enviarla.

1. En la oferta, seleccione la ficha **[!UICONTROL Vista previa]** junto a **[!UICONTROL Información general]**.

   ![Captura de pantalla que muestra la vista previa de la oferta.](assets/offers-offer-3.png){zoomable="yes"}

1. Seleccione un perfil de destino y, si procede, el espacio de oferta en el que se debe ejecutar la vista previa.

   La función de renderización definida en el espacio de oferta se aplica al contenido de la oferta y se muestra la representación resultante.

>[!NOTE]
>
>Si la previsualización devuelve un error o ningún contenido, compruebe la función de renderización del espacio de oferta, las reglas de idoneidad de la oferta y que se rellenan todos los campos de contenido requeridos.

## Aprobación e implementación de la oferta {#approve-deploy}

Las ofertas no están disponibles inmediatamente en los envíos: pasan por un ciclo de aprobación e implementación.

1. En la descripción general de la oferta, haga clic en **[!UICONTROL Aprobación]**.

   ![Captura de pantalla que muestra la aprobación de la oferta.](assets/offers-offer-4.png){zoomable="yes"}

1. Apruebe **[!UICONTROL Elegibilidad]** y **[!UICONTROL Contenido]**. El contenido se puede aprobar por espacio de oferta, por lo que puede aprobarlo para un espacio de oferta mientras deja otros pendientes.

1. Una vez concedidas ambas aprobaciones, haga clic en **[!UICONTROL Implementar]** para publicar la oferta en el entorno en vivo.

1. Actualice la vista de ofertas para confirmar que la representación de **[!UICONTROL Live]** está actualizada.

<!--
>[!NOTE]
>
>Once deployed, the design offer's status resets to **[!UICONTROL Being edited]** — its normal draft status, not a sign that someone is actively editing it. This just means the design offer is ready to accept further changes, which would then need to go through a new approval and deployment cycle. The live representation itself remains untouched until that happens.
-->

>[!CAUTION]
>
>La aprobación de la idoneidad y el contenido de una oferta son dos acciones distintas. Una oferta se puede aprobar parcialmente (solo contenido, por ejemplo) y permanecer no disponible para su envío hasta que se conceda también la aprobación de idoneidad.

## Monitorización del panel de ofertas {#dashboard}

La pestaña de la oferta **[!UICONTROL Información general]** resume el estado de la oferta en las tarjetas **[!UICONTROL Propiedades]**, **[!UICONTROL Contenido]** y **[!UICONTROL Elegibilidad]**, con un icono de lápiz en cada una para volver a la edición. Una tarjeta **[!UICONTROL Representation]** enumera todos los espacios de ofertas a los que está vinculada la oferta, junto con su estado de diseño actual.

![Captura de pantalla que muestra el panel de ofertas.](assets/offers-offer-5.png){zoomable="yes"}

Haga clic en **[!UICONTROL Registros]** para obtener acceso a los registros de implementación o en el menú **··** (**[!UICONTROL Más]**) para **[!UICONTROL Duplicar]** o **[!UICONTROL Eliminar]** la oferta.

Una vez que una oferta está activa, la modificación de cualquier configuración cambia la oferta de diseño a un estado editable. La representación en directo permanece intacta hasta el siguiente ciclo de aprobación e implementación.

## Uso de la oferta en una entrega {#use-in-delivery}

Cuando la oferta está activa, se puede seleccionar desde cualquier entrega orientado al espacio de oferta coincidente. Aprenda a configurar ofertas en una entrega de [Agregar ofertas a sus mensajes](../msg/offers.md).

Para obtener la integración de la entrega saliente completa, incluido cómo se crea la llamada al motor y cómo se aplica el seguimiento a los vínculos de oferta, consulte las [ofertas de documentación de Campaign v8 en las entregas salientes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-send-offers.html){target="_blank"}.

