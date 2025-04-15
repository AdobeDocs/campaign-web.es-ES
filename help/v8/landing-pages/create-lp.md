---
title: Creación de una página de aterrizaje
description: Aprenda a configurar y publicar una página de aterrizaje en Campaign Web
feature: Landing Pages
exl-id: d4a49048-5ab1-4b69-9e12-1ffa235c51f4
source-git-commit: bd938c3e2046123a9a9c6b64890bf41d0c272d4d
workflow-type: tm+mt
source-wordcount: '1731'
ht-degree: 21%

---


# Creación y publicación de páginas de destino {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Creación y administración de páginas de destino"
>abstract="Adobe Campaign le permite crear, diseñar y compartir páginas de destino para dirigir a sus usuarios a páginas web en línea donde puede administrar casos de uso de Adquisición, suscripción/baja y lista de denegación, basados en plantillas integradas."

La interfaz de Campaign usuario web permite crear, diseñar y publicar páginas de aterrizaje. Después de la publicación, puede insertar un vincular en el formulario en un envío. Cuando los destinatarios hacen clic en ese vincular, se les dirige al página de aterrizaje correspondiente.

[!DNL Adobe Campaign] Incluye cuatro plantillas para administrar los siguientes casos de uso: **Adquisición**, **suscripción**, **baja** y **lista** de denegación. [Más información](lp-use-cases.md)

## Páginas de aterrizaje de Access {#access-landing-pages}

Para acceder al lista de página de aterrizaje, seleccione **[!UICONTROL Administración de]** contenido > **[!UICONTROL Páginas]** de destino en el menú de la izquierda.

![Captura de pantalla que muestra los inventario de las páginas de aterrizaje en la interfaz web de Campaign.](assets/lp-inventory.png){zoomable="yes"}

El **[!UICONTROL inventario Páginas]** de aterrizaje muestra todos los elementos creados. Puede filtrarlos mediante el **[!UICONTROL botón filtros]** Mostrar.

* Puede filtrar los elementos que ha creado o modificado.
* Puede restringir los resultados a una carpeta específica [mediante el lista desplegable o agregar reglas mediante el modelador](../query/query-modeler-overview.md) consulta[](../get-started/permissions.md#folders).

![Captura de pantalla que muestra las opciones de filtro en el inventario de páginas de destino.](assets/lp-inventory-filter.png){zoomable="yes"}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>No se pueden mostrar ni editar páginas de aterrizaje creadas desde la consola del cliente (formularios web) en la interfaz de Campaign Web usuario. Obtenga más información en la documentación](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html?lang=es){target="_blank"} de la consola Campaign[.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Puede duplicado o eliminar un página de aterrizaje. Haga clic en los puntos suspensivos junto a un página de aterrizaje para seleccionar la acción deseada.

## Creación de una página de aterrizaje {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definición de las propiedades de la página de aterrizaje"
>abstract="Rellene los campos de propiedades como la etiqueta y modifique el esquema si es necesario. Además, puede editar el nombre interno, cambiar la carpeta donde se almacena la página de aterrizaje y proporcionar una descripción."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Defina el contenido de cada página"
>abstract="Ajuste el contenido de cada página que forma parte de esta página de aterrizaje, como el propio formulario, la página de confirmación que se muestra al enviar el formulario o la página a la que se dirige a los usuarios en caso de que se produzca un error."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Programación de la página de aterrizaje"
>abstract="Defina una fecha de inicio y una fecha de finalización para la página de aterrizaje. Cuando la página llega al final del periodo de validez, el formulario ya no está disponible. En su lugar, se muestra la página **Caducidad**."

>[!CONTEXTUALHELP]
>id="acw_landingpages_preload"
>title="Definir opciones de precarga"
>abstract="Cuando la opción **Rellene previamente los datos a los que se hace referencia en el formulario** está seleccionada, si el visitante de la página de aterrizaje coincide con un perfil de la base de datos, la información del perfil se precarga automáticamente en el formulario. Con la opción **Autorizar ausencia de ID** seleccionada, cualquier visitante, incluidos los usuarios anónimos, puede acceder a la página de aterrizaje."

<!--With the **Skip preloading if no ID** option selected, each profile entered will be added to the database after approval of the form."-->

>[!CONTEXTUALHELP]
>id="acw_landingpages_storage"
>title="Definir opciones de almacenamiento"
>abstract="La sección de precarga le permite indicar cómo buscar el registro que se actualiza en la base de datos."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

To create a landing page, follow these steps:

1. En la inventario Páginas de **[!UICONTROL aterrizaje, haga clic en**[!UICONTROL  Crear página de aterrizaje ]**.]**

   ![Captura de pantalla que muestra el Crear página de aterrizaje botón.](assets/lp-create-button.png){zoomable="yes"}

1. Seleccione una plantilla:
   * **[!UICONTROL Adquisición]**: este es el plantilla predeterminado para las páginas de aterrizaje, que le permite capturar y actualizar perfil datos.
   * **[!UICONTROL Suscripción]**: use esta plantilla para permitir que los usuarios se suscriban a un [servicio](../audience/manage-services.md) específico.
   * **[!UICONTROL Unsubscription]**: This template can be used in a delivery sent to the subscribers of a service to allow them to unsubscribe from this [service](../audience/manage-services.md).
   * **[!UICONTROL Denylist]**: This template should be used when a profile clicks on an opt-out link in a delivery and no longer wants to be contacted.

   ![Screenshot showing the landing page templates.](assets/lp-templates.png){zoomable="yes"}

   >[!NOTE]
   >
   >Learn how to implement the different use cases corresponding to each template in [this page](lp-use-cases.md).

1. Haga clic en **[!UICONTROL Crear]**.

1. Rellene los campos Propiedades ****, como la etiqueta.

   De forma predeterminada, las páginas de destino se almacenan en la **[!UICONTROL carpeta de aplicaciones]** web. Para cambiarla, vaya a la ubicación deseada en las **[!UICONTROL Opciones]** adicionales. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders).

   También puede configurar el captcha para proteger su página de aterrizaje. [Más información aquí](#captcha).

   ![Captura de pantalla que muestra la sección página de aterrizaje propiedades.](assets/lp-properties.png){zoomable="yes"}

1. In the **[!UICONTROL Data preload]** section, the following options are available:

   * Cuando la opción **[!UICONTROL Rellene previamente los datos a los que se hace referencia en el formulario]** está seleccionada, si el visitante de la página de aterrizaje coincide con un perfil de la base de datos, la información del perfil se precarga automáticamente en el formulario. The user just has to fill in the missing fields and update the existing values if needed. This allows merging data for existing profiles instead of creating duplicates.

     >[!NOTE]
     >
     >Esta opción está seleccionada de forma predeterminada para todas las página de aterrizaje plantillas.

   * La **[!UICONTROL opción Autorizar la ausencia de ID]** permite que cualquier visitante acceda al página de aterrizaje. Unselecting this option prevents anonymous visitors from using it, meaning that only identified users can access and submit the form.

     >[!AVAILABILITY]
     >
     >This capability is in Limited Availability (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

     For the **[!UICONTROL Acquisition]** and **[!UICONTROL Subscription]** templates, this option is selected by default. For the **[!UICONTROL Unsubscription]** and **[!UICONTROL Denylist]** templates, this option is unselected by default and cannot be modified.

1. A landing page can have subsequent pages. To add pages, browse the **[!UICONTROL Pages]** section, and click the **[!UICONTROL Edit content]** button for each page that you want to design for this landing page. The content of each page is already pre-filled. Editar ellos según sea necesario. [Más información](lp-content.md).

   ![Captura de pantalla que muestra la sección de páginas del editor de página de aterrizaje.](assets/lp-pages.png){zoomable="yes"}

1. En la **[!UICONTROL sección Almacenamiento]** , la **[!UICONTROL opción Actualizar el registro]** precargado está seleccionada de forma predeterminada. Permite actualizar los perfiles almacenados en la base de datos a través del página de aterrizaje. La casilla de precarga le permite indicar cómo buscar el registro que se actualiza en la base de datos.

   También puede elegir entre los campos en el contexto actual del página de aterrizaje, aquellos que se utilizarán para encontrar los perfil correspondientes en la base de datos. Para ello, anule la selección de la **[!UICONTROL opción Actualizar el registro]** precargado y marque los campos deseados en **[!UICONTROL Opciones de reconciliación]**.

   ![Captura de pantalla que muestra las opciones de almacenamiento para el página de aterrizaje.](assets/lp-storage.png){zoomable="yes"}

1. **[!UICONTROL Crear datos]** adicionales para tienda datos internos cuando se envía la página de aterrizaje. Estos datos no son visibles para los usuarios que visita el Página. Solo se tienen en cuenta los valores constantes.

   >[!AVAILABILITY]
   >
   >Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

   ![Captura de pantalla que muestra la sección de datos adicionales.](assets/lp-additional-data.png){zoomable="yes"}

1. Puede definir una fecha de inicio y una fecha de finalización para la página de aterrizaje. Seleccione **[!UICONTROL Habilitar programación]** y establezca las fechas.

   ![Captura de pantalla que muestra las opciones de programación del página de aterrizaje.](assets/lp-schedule.png){zoomable="yes"}

   * El página de aterrizaje se publica automáticamente en la fecha y hora de inicio especificadas.

     >[!NOTE]
     >
     >Si no se define ninguna fecha de inicio, la página de aterrizaje se activa en cuanto se publica.

   * Cuando el Página llega a la fecha de finalización, el formulario ya no está disponible. En su lugar, se muestra la página **[!UICONTROL Caducidad]**.

     >[!NOTE]
     >
     >Por motivos de seguridad y rendimiento de la plataforma, Adobe Systems recomienda establecer una fecha de finalización.

1. Haga clic en **[!UICONTROL Revisar y publicar]**.

Una vez que defina todos los ajustes y [diseñe](lp-content.md) todas las páginas, puede [prueba](#test-landing-page) y [publicar](#publish-landing-page) sus página de aterrizaje como se detalla a continuación.

## Proteja su página de aterrizaje con un captcha {#captcha}

>[!AVAILABILITY]
>
>Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que usan **Adobe Campaign v8.7.2 actualizado con la última versión de corrección**, y no se puede implementar en ningún otro entorno.

La configuración de un captcha le ayuda a proteger la página de aterrizaje del spam y los abusos.

Para usarlo, vaya a las **[!UICONTROL Propiedades]** de su página de aterrizaje.
En **[!UICONTROL Opciones adicionales]** también. Active la opción **[!UICONTROL Habilitar solución captcha adicional]**.

![Captura de pantalla que muestra la opción Habilitar solución captcha adicional](assets/lp-properties-captcha.png){zoomable="yes"}

Para comprobar la configuración del captcha, haga clic en el botón **[!UICONTROL Revisar y publicar]** y en **[!UICONTROL Simular contenido]**. Al enviar el formulario, verá el widget captcha funcionando durante la validación como se muestra a continuación.

![Captura de pantalla del widget captcha](assets/lp-captcha.png){zoomable="yes"}

>[!NOTE]
>
>El widget captcha en Adobe Campaign v8 es ALTCHA y funciona en modo flotante. Aparece durante la validación y desaparece una vez completado el proceso.


## Prueba de la página de aterrizaje {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulación de la página de aterrizaje"
>abstract="Puede ver una vista previa de la página de aterrizaje en la interfaz de usuario web de Campaign o abrirla en una nueva pestaña del explorador web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Previsualizar y probar la página de aterrizaje"
>abstract="Una vez que haya definido la configuración y el contenido de la página de aterrizaje, puede utilizar perfiles de prueba para previsualizarlos."

Una vez definida la configuración y los contenido de página de aterrizaje, puede utilizar perfiles de prueba para previsualización. Si ha insertado [contenido](../personalization/gs-personalization.md) personalizados, podrá comprobar cómo se muestra este contenido en el página de aterrizaje, utilizando prueba perfil datos.

>[!CAUTION]
>
>Debe tener prueba perfiles disponibles para poder previsualización los mensajes y enviar pruebas. [Más información sobre prueba perfiles](../audience/test-profiles.md)

To test your landing page, follow these steps:

1. Después de hacer clic en **[!UICONTROL Revisar y publicar]**, seleccione el botón **[!UICONTROL Simular contenido]** del panel de página de aterrizaje para acceder a la selección del perfil de prueba.

   ![Captura de pantalla del botón Simular contenido](assets/lp-simulate-content.png){zoomable="yes"}

1. En la pantalla **[!UICONTROL Simular]**, seleccione uno o más perfiles de prueba.

   Los pasos para seleccionar perfiles de prueba son los mismos que al probar un mensaje. Se detallan en la sección [Previsualizar y probar](../preview-test/preview-test.md).

1. Al probar una página de aterrizaje dinámica (con la opción **[!UICONTROL Servicio de la URL]** seleccionada - [más información](../landing-pages/create-lp.md#define-actions-on-form-submission)

1. Seleccione **[!UICONTROL Abrir vista previa]** para probar la página de aterrizaje.

   ![Captura de pantalla del botón Abrir vista previa](assets/lp-open-preview.png){zoomable="yes"}

1. La vista previa de la página de aterrizaje se abrirá en una nueva pestaña. Los elementos personalizados se sustituyen por los datos de perfil de prueba seleccionados.

   Si seleccionó la opción **[!UICONTROL Rellenar previamente con los datos a los que se hace referencia en el formulario]** en la configuración de la página de aterrizaje, los campos del formulario se rellenarán automáticamente previamente con los datos del perfil de prueba correspondientes.<!--TBC-->

   ![Example of a delivery](assets/lp-preview.png){zoomable="yes"}

1. Select other test profiles to preview the rendering for each variant of your landing page.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Publicar la página de aterrizaje {#publish-landing-page}

Once your landing page is ready and validated, publish it to make it available for use in a delivery using the corresponding button.

Una vez publicado:

* The landing page is added to the landing page list with the **[!UICONTROL Published]** status. It is now live and ready to be referenced in your contents.

* You can copy-paste the **[!UICONTROL Landing page URL]** that is displayed on top of the page into a web browser to preview your landing page.

>[!CAUTION]
>
>Para probar o aprovechar al máximo la página de aterrizaje, no puede copiar y pegar este vínculo directamente en un explorador web o en los envíos. Instead, use the [Simulate content](#test-landing-page) function to test it, and follow the steps described in [this section](lp-use-cases.md) to make proper use of your landing page.

![Screenshot showing the Landing Page URL](assets/lp-published.png){zoomable="yes"}

You can monitor your landing page impacts through logs<!--and specific reports-->. Haga clic en el **[!UICONTROL botón Registros]** .