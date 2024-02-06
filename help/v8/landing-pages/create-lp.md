---
title: Creación de una página de aterrizaje
description: Obtenga información sobre cómo configurar y publicar una página de destino en Campaign Web
badge: label="Disponibilidad limitada"
source-git-commit: 7635ab284900c8a4cd5ceca5675e57dbedb39f3a
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 26%

---

# Creación y publicación de páginas de destino {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Creación y administración de páginas de destino"
>abstract="Adobe Campaign le permite crear, diseñar y compartir páginas de aterrizaje para dirigir a los usuarios a páginas web en línea donde puede administrar adquisiciones, suscripciones/bajas de suscripciones y casos de uso de listas de bloqueados, en función de plantillas integradas."

Adobe Campaign le permite crear, diseñar y compartir páginas de aterrizaje para dirigir a los usuarios a páginas web en línea donde puede administrar adquisiciones, suscripciones/bajas de suscripciones y casos de uso de listas de bloqueados, en función de plantillas integradas.

## Acceso a páginas de aterrizaje {#access-landing-pages}

Para acceder a la lista de página de aterrizaje, seleccione **[!UICONTROL Administración de campañas]** > **[!UICONTROL Páginas de aterrizaje]** en el menú de la izquierda.

![](assets/lp-inventory.png)

El **[!UICONTROL Páginas de aterrizaje]** inventory muestra todos los artículos creados. Puede filtrarlos con el **Mostrar filtros** botón. Puede restringir los resultados a un específico [carpeta](../get-started/permissions.md#folders) mediante la lista desplegable o agregue reglas utilizando la variable [modelador de consultas](../query/query-modeler-overview.md).

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>No puede mostrar ni editar páginas de destino creadas desde la consola del cliente en Campaign Web. Obtenga más información en la [Documentación de la consola de Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Puede duplicar o eliminar una página de aterrizaje. Haga clic en los tres puntos junto a una página de aterrizaje para seleccionar la acción deseada.

## Creación de una página de aterrizaje {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definición de las propiedades de la página de aterrizaje"
>abstract="Rellene los campos de propiedades como la etiqueta y modifique el esquema si es necesario. Además, puede editar el nombre interno, cambiar la carpeta donde se almacena la página de aterrizaje y proporcionar una descripción."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Definición del contenido de las páginas"
>abstract="Edite el contenido de cada página que forma parte de esta página de aterrizaje."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Programación de la página de aterrizaje"
>abstract="Puede definir una fecha de inicio y una fecha de finalización para la página de aterrizaje. Cuando la página haya caducado, se mostrará la página **Caducidad**."


>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definición de la configuración de la página principal"
>abstract="La página principal se muestra inmediatamente a los usuarios después de hacer clic en el vínculo a la página de aterrizaje, por ejemplo, desde un correo electrónico o un sitio web."

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Establecimiento de la página de aterrizaje de la suscripción"
>abstract="Una página de suscripción permite a los clientes suscribirse a un servicio."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png)-->

1. Desde el **[!UICONTROL Páginas de aterrizaje]** inventario, haga clic en **[!UICONTROL Crear página de aterrizaje]**.

   ![](assets/lp-create-button.png)

1. Seleccione una plantilla:
   * **[!UICONTROL Adquisición]**: Esta es la plantilla predeterminada para páginas de aterrizaje, que le permite capturar y actualizar datos de perfil.
   * **[!UICONTROL Suscripción]**: utilice esta plantilla para ofrecer suscripciones a un servicio.
   * **[!UICONTROL Baja]**: Esta plantilla se puede vincular desde un correo electrónico enviado a los suscriptores de un servicio para permitirles cancelar su suscripción.
   * **[!UICONTROL Lista de bloqueados de]**: esta plantilla debe utilizarse cuando un perfil ya no quiere que Campaign le siga contactando. Más información sobre la administración de lista de bloqueados de la

   ![](assets/lp-templates.png)

1. Haga clic en **[!UICONTROL Create]**.

1. Rellene los campos de propiedades como la etiqueta. De forma predeterminada, las páginas de aterrizaje se almacenan en **[!UICONTROL Aplicaciones web]** carpeta. Puede cambiarlo navegando a la ubicación deseada en la **[!UICONTROL Opciones adicionales]**. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. En el **[!UICONTROL Precarga de datos]** , las dos opciones siguientes están seleccionadas de forma predeterminada:

   * El **[!UICONTROL Rellene previamente los datos a los que se hace referencia en el formulario]** La opción permite precargar automáticamente los datos que coinciden con los campos de entrada y de combinación del formulario.

   * El **[!UICONTROL Omitir precarga si no hay ID]** La opción debe estar seleccionada si no desea actualizar los perfiles. En este caso, cada perfil introducido se añade a la base de datos después de la aprobación del formulario. Esta opción se utiliza, por ejemplo, cuando se publica el formulario en un sitio web.

1. En el **[!UICONTROL Páginas]** , haga clic en **[!UICONTROL Editar contenido]** para cada página que desee diseñar para esta página de aterrizaje. El contenido de cada página ya está rellenado previamente. Edítelos según sea necesario. [Más información](lp-content.md)

   ![](assets/lp-pages.png)

1. El **[!UICONTROL Actualización del registro cargado previamente]** está seleccionada de forma predeterminada. Si desea actualizar los perfiles almacenados en la base de datos a través de la página de aterrizaje, puede utilizar una casilla de precarga. La casilla de precarga permite indicar cómo buscar el registro que se actualiza en la base de datos. También puede elegir entre los campos del contexto actual de la página de aterrizaje, los que se utilizan para encontrar el perfil correspondiente en la base de datos.

   ![](assets/lp-storage-schedule.png)

1. Puede definir una fecha de inicio y una fecha de finalización para la página de aterrizaje. Seleccionar **[!UICONTROL Habilitar programación]** y fije las fechas. Cuando la página haya caducado, se mostrará la página **[!UICONTROL Caducidad]**.

1. Clic **[!UICONTROL Revisión y publicación]**.

Una vez configuradas y diseñadas todas las páginas, puede [prueba](#test-landing-page) y [publicar](#publish-landing-page) su página de aterrizaje.

## Prueba de la página de aterrizaje {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulación de la página de aterrizaje"
>abstract="Puede ver una vista previa de la página de aterrizaje en la interfaz de usuario web de Campaign o abrirla en una nueva pestaña del explorador web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Previsualizar y probar la página de aterrizaje"
>abstract="Una vez que haya definido la configuración y el contenido de la página de aterrizaje, puede utilizar perfiles de prueba para previsualizarlos."

Una vez definida la configuración y el contenido de la página de aterrizaje, puede utilizar perfiles de prueba para previsualizarlo. Si ha insertado [contenido personalizado](../personalization/gs-personalization.md), podrá comprobar cómo se muestra este contenido en la página de aterrizaje mediante los datos de perfil de prueba.

>[!CAUTION]
>
>Debe tener perfiles de prueba disponibles para poder previsualizar los mensajes y enviar pruebas. Obtenga información sobre cómo [creación de perfiles de prueba](../audience/test-profiles.md).

1. En la interfaz de la página de aterrizaje, haga clic en **[!UICONTROL Simular contenido]** para acceder a la selección del perfil de prueba.

   ![](assets/lp-simulate-content.png)

1. Desde el **[!UICONTROL Simular]** , seleccione uno o más perfiles de prueba.

   Los pasos para seleccionar perfiles de prueba son los mismos que al probar un mensaje. Se encuentran detalladas en la [Previsualización y prueba](../preview-test/preview-test.md) sección.

1. Seleccionar **[!UICONTROL Abrir vista previa]** para probar la página de aterrizaje.

   ![](assets/lp-open-preview.png)

1. La vista previa de la página de aterrizaje se abrirá en una nueva pestaña. Los elementos personalizados se sustituyen por los datos de perfil de prueba seleccionados.

   ![](assets/lp-preview.png)

1. Seleccione otros perfiles de prueba para previsualizar el procesamiento de cada variante de la página de aterrizaje.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Publicar la página de aterrizaje {#publish-landing-page}

Una vez que la página de aterrizaje esté lista, puede publicarla para que esté disponible para usarla en un mensaje.

Una vez publicada la página de aterrizaje, se añade a la lista de página de aterrizaje con el **[!UICONTROL Publicado]** estado. Ahora está activo y listo para usarse.

![](assets/lp-published.png)

Una vez publicado, puede copiar y pegar el **[!UICONTROL URL de página de aterrizaje]** que se muestra en la parte superior de la página en un explorador web.

Puede monitorizar el impacto de su página de aterrizaje a través de registros e informes específicos.
