---
title: Creación de una página de destino
description: Obtenga información sobre cómo configurar y publicar una página de destino en Campaign Web
feature: Landing Pages
exl-id: d4a49048-5ab1-4b69-9e12-1ffa235c51f4
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '1731'
ht-degree: 26%

---


# Creación y publicación de páginas de destino {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="Creación y administración de páginas de destino"
>abstract="Adobe Campaign le permite crear, diseñar y compartir páginas de destino para dirigir a los usuarios a las páginas web en línea en las que puede administrar la adquisición, suscripción o baja e incluir en la lista de bloqueados los casos de uso, en función de las plantillas integradas."

La interfaz de usuario web de Campaign permite crear, diseñar y publicar páginas de destino. Después de la publicación, puede insertar un vínculo al formulario en una entrega. Cuando los destinatarios hacen clic en ese vínculo, se les dirige a la página de aterrizaje correspondiente.

[!DNL Adobe Campaign] incluye cuatro plantillas para administrar los siguientes casos de uso: **adquisición**, **suscripción**, **baja** y **lista de bloqueados de la suscripción**. [Más información](lp-use-cases.md)

## Acceso a páginas de aterrizaje {#access-landing-pages}

Para acceder a la lista de páginas de aterrizaje, seleccione **[!UICONTROL Administración de contenido]** > **[!UICONTROL Páginas de aterrizaje]** en el menú de la izquierda.

![Captura de pantalla que muestra el inventario de páginas de aterrizaje en la interfaz web de Campaign.](assets/lp-inventory.png){zoomable="yes"}

El inventario **[!UICONTROL Páginas de aterrizaje]** muestra todos los elementos creados. Puede filtrarlos con el botón **[!UICONTROL Mostrar filtros]**.

* Puede filtrar los elementos que ha creado o modificado.
* Puede restringir los resultados a una [carpeta](../get-started/permissions.md#folders) específica usando la lista desplegable o agregar reglas usando [modelador de consultas](../query/query-modeler-overview.md).

![Captura de pantalla que muestra las opciones de filtro en el inventario de páginas de aterrizaje.](assets/lp-inventory-filter.png){zoomable="yes"}

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>No puede mostrar ni editar páginas de destino creadas desde la consola del cliente (formularios web) en la interfaz de usuario web de Campaign. Obtenga más información en la [documentación de la consola de Campaign](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html?lang=es){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

Puede duplicar o eliminar una página de aterrizaje. Haga clic en los puntos suspensivos junto a una página de aterrizaje para seleccionar la acción deseada.

## Creación de una página de destino {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="Definición de las propiedades de la página de destino"
>abstract="Rellene los campos de propiedades como la etiqueta y modifique el esquema si es necesario. Además, puede editar el nombre interno, cambiar la carpeta donde se almacena la página de destino y proporcionar una descripción."

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="Defina el contenido de cada página"
>abstract="Ajuste el contenido de cada página que forma parte de esta página de destino, como el propio formulario, la página de confirmación que se muestra al enviar el formulario o la página a la que se dirige a los usuarios en caso de que se produzca un error."

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="Programación de la página de destino"
>abstract="Defina una fecha de inicio y una fecha de finalización para la página de destino. Cuando la página llega al final del periodo de validez, el formulario ya no está disponible. En su lugar, se muestra la página **Caducidad**."

>[!CONTEXTUALHELP]
>id="acw_landingpages_preload"
>title="Definir opciones de precarga"
>abstract="Cuando la opción **Rellene previamente los datos a los que se hace referencia en el formulario** está seleccionada, si el visitante de la página de destino coincide con un perfil de la base de datos, la información del perfil se precarga automáticamente en el formulario. Con la opción **Autorizar ausencia de ID** seleccionada, cualquier visitante, incluidos los usuarios anónimos, puede acceder a la página de destino."

<!--With the **Skip preloading if no ID** option selected, each profile entered will be added to the database after approval of the form."-->

>[!CONTEXTUALHELP]
>id="acw_landingpages_storage"
>title="Definir opciones de almacenamiento"
>abstract="La sección de precarga le permite indicar cómo buscar el registro que se actualiza en la base de datos."

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png){zoomable="yes"}-->

Para crear una página de aterrizaje, siga estos pasos:

1. En el inventario de **[!UICONTROL Páginas de aterrizaje]**, haga clic en **[!UICONTROL Crear página de aterrizaje]**.

   ![Captura de pantalla que muestra el botón Crear página de aterrizaje.](assets/lp-create-button.png){zoomable="yes"}

1. Seleccione una plantilla:
   * **[!UICONTROL Adquisición]**: Esta es la plantilla predeterminada para páginas de aterrizaje, que le permite capturar y actualizar datos de perfil.
   * **[!UICONTROL Suscripción]**: use esta plantilla para permitir que los usuarios se suscriban a un [servicio](../audience/manage-services.md) específico.
   * **[!UICONTROL Baja]**: esta plantilla se puede usar en una entrega enviada a los suscriptores de un servicio para permitirles cancelar su suscripción a este [servicio](../audience/manage-services.md).
   * **[!UICONTROL Lista de bloqueados de]**: esta plantilla debe usarse cuando un perfil hace clic en un vínculo de no participación en una entrega y ya no quiere que se le contacte.

   ![Captura de pantalla que muestra las plantillas de página de aterrizaje.](assets/lp-templates.png){zoomable="yes"}

   >[!NOTE]
   >
   >Aprenda a implementar los diferentes casos de uso correspondientes a cada plantilla en [esta página](lp-use-cases.md).

1. Haga clic en **[!UICONTROL Crear]**.

1. Rellene los campos **[!UICONTROL Propiedades]** como la etiqueta.

   De manera predeterminada, las páginas de destino se almacenan en la carpeta **[!UICONTROL Aplicaciones web]**. Puede cambiarlo si busca la ubicación deseada en **[!UICONTROL Opciones adicionales]**. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders).

   También puede configurar el captcha para proteger la página de aterrizaje. [Más información aquí](#captcha).

   ![Captura de pantalla que muestra la sección de propiedades de la página de aterrizaje.](assets/lp-properties.png){zoomable="yes"}

1. En la sección **[!UICONTROL Carga previa de datos]**, están disponibles las siguientes opciones:

   * Cuando la opción **[!UICONTROL Rellene previamente los datos a los que se hace referencia en el formulario]** está seleccionada, si el visitante de la página de destino coincide con un perfil de la base de datos, la información del perfil se precarga automáticamente en el formulario. El usuario solo tiene que rellenar los campos que faltan y actualizar los valores existentes si es necesario. Esto permite combinar datos para perfiles existentes en lugar de crear duplicados.

     >[!NOTE]
     >
     >Esta opción está seleccionada de forma predeterminada para todas las plantillas de página de aterrizaje.

   * La opción **[!UICONTROL Autorizar ausencia de ID]** permite que cualquier visitante acceda a la página de aterrizaje. Si se anula la selección de esta opción, se impide que los visitantes anónimos la utilicen, lo que significa que solo los usuarios identificados pueden acceder al formulario y enviarlo.

     >[!AVAILABILITY]
     >
     >Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

     Para las plantillas **[!UICONTROL Acquisition]** y **[!UICONTROL Subscription]**, esta opción está seleccionada de forma predeterminada. Para las plantillas **[!UICONTROL Baja]** y **[!UICONTROL Lista de bloqueados de la suscripción]**, esta opción no está seleccionada de forma predeterminada y no se puede modificar.

1. Una página de aterrizaje puede tener páginas posteriores. Para agregar páginas, examine la sección **[!UICONTROL Páginas]** y haga clic en el botón **[!UICONTROL Editar contenido]** para cada página que desee diseñar para esta página de aterrizaje. El contenido de cada página ya está rellenado previamente. Edítelos según sea necesario. [Más información](lp-content.md).

   ![Captura de pantalla que muestra la sección de páginas del editor de páginas de aterrizaje.](assets/lp-pages.png){zoomable="yes"}

1. En la sección **[!UICONTROL Storage]**, la opción **[!UICONTROL Update the preloaded record]** está seleccionada de forma predeterminada. Permite actualizar los perfiles almacenados en la base de datos a través de la página de aterrizaje. La casilla de precarga le permite indicar cómo buscar el registro que se actualiza en la base de datos.

   También puede elegir entre los campos del contexto actual de la página de aterrizaje, los que se utilizan para encontrar el perfil correspondiente en la base de datos. Para ello, anule la selección de la opción **[!UICONTROL Actualizar el registro precargado]** y marque los campos deseados en **[!UICONTROL Opciones de reconciliación]**.

   ![Captura de pantalla que muestra las opciones de almacenamiento de la página de aterrizaje.](assets/lp-storage.png){zoomable="yes"}

1. Cree **[!UICONTROL datos adicionales]** para almacenar datos internos cuando se envíe la página de aterrizaje. Estos datos no son visibles para los usuarios que visitan la página. Solo se tienen en cuenta los valores constantes.

   >[!AVAILABILITY]
   >
   >Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

   ![Captura de pantalla que muestra la sección de datos adicionales.](assets/lp-additional-data.png){zoomable="yes"}

1. Puede definir una fecha de inicio y una fecha de finalización para la página de destino. Seleccione **[!UICONTROL Habilitar la programación]** y establezca las fechas.

   ![Captura de pantalla que muestra las opciones de programación de la página de aterrizaje.](assets/lp-schedule.png){zoomable="yes"}

   * La página de aterrizaje se publica automáticamente en la fecha y la hora de inicio especificadas.

     >[!NOTE]
     >
     >Si no se define ninguna fecha de inicio, la página de aterrizaje se activa en cuanto se publica.

   * Cuando la página alcanza la fecha de finalización, el formulario ya no está disponible. En su lugar, se muestra la página **[!UICONTROL Caducidad]**.

     >[!NOTE]
     >
     >Por motivos de seguridad y de rendimiento de la plataforma, Adobe recomienda establecer una fecha de finalización.

1. Haga clic en **[!UICONTROL Revisar y publicar]**.

Una vez que haya definido toda la configuración y [diseñado](lp-content.md) todas las páginas, podrá [probar](#test-landing-page) y [publicar](#publish-landing-page) su página de aterrizaje como se detalla a continuación.

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


## Prueba de la página de destino {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="Simulación de la página de destino"
>abstract="Puede ver una vista previa de la página de destino en la interfaz de usuario web de Campaign o abrirla en una nueva pestaña del explorador web."

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="Previsualizar y probar la página de destino"
>abstract="Una vez que haya definido la configuración y el contenido de la página de destino, puede utilizar perfiles de prueba para previsualizarlos."

Una vez definida la configuración y el contenido de la página de aterrizaje, puede utilizar perfiles de prueba para previsualizarlo. Si ha insertado [contenido personalizado](../personalization/gs-personalization.md), podrá comprobar cómo se muestra este contenido en la página de aterrizaje mediante los datos del perfil de prueba.

>[!CAUTION]
>
>Debe tener perfiles de prueba disponibles para poder previsualizar los mensajes y enviar pruebas. [Más información sobre los perfiles de prueba](../audience/test-profiles.md)

Para probar la página de aterrizaje, siga estos pasos:

1. Después de hacer clic en **[!UICONTROL Revisar y publicar]**, seleccione el botón **[!UICONTROL Simular contenido]** del panel de página de aterrizaje para acceder a la selección del perfil de prueba.

   ![Captura de pantalla del botón Simular contenido](assets/lp-simulate-content.png){zoomable="yes"}

1. En la pantalla **[!UICONTROL Simular]**, seleccione uno o más perfiles de prueba.

   Los pasos para seleccionar perfiles de prueba son los mismos que al probar un mensaje. Se detallan en la sección [Previsualizar y probar](../preview-test/preview-test.md).

1. Al probar una página de aterrizaje dinámica (con la opción **[!UICONTROL Servicio de la URL]** seleccionada - [más información](../landing-pages/create-lp.md#define-actions-on-form-submission)

1. Seleccione **[!UICONTROL Abrir vista previa]** para probar la página de aterrizaje.

   ![Captura de pantalla del botón Abrir vista previa](assets/lp-open-preview.png){zoomable="yes"}

1. La vista previa de la página de aterrizaje se abrirá en una nueva pestaña. Los elementos personalizados se sustituyen por los datos de perfil de prueba seleccionados.

   Si seleccionó la opción **[!UICONTROL Rellenar previamente con los datos a los que se hace referencia en el formulario]** en la configuración de la página de aterrizaje, los campos del formulario se rellenarán automáticamente previamente con los datos del perfil de prueba correspondientes.<!--TBC-->

   ![Ejemplo de envío](assets/lp-preview.png){zoomable="yes"}

1. Seleccione otros perfiles de prueba para previsualizar el procesamiento de cada variante de la página de aterrizaje.

<!--Can you preview Confirmation/Error/Expiration pages?-->

## Publicar la página de destino {#publish-landing-page}

Una vez que la página de aterrizaje esté lista y validada, publíquela para que esté disponible para su uso en una entrega con el botón correspondiente.

Una vez publicado:

* La página de aterrizaje se agrega a la lista de páginas de aterrizaje con el estado **[!UICONTROL Publicado]**. Ahora está activo y listo para que se le haga referencia en su contenido.

* Puede copiar y pegar la **[!UICONTROL dirección URL de la página de aterrizaje]** que se muestra en la parte superior de la página en un explorador web para previsualizar la página de aterrizaje.

>[!CAUTION]
>
>Para probar o aprovechar al máximo la página de destino, no puede copiar y pegar este vínculo directamente en un explorador web o en los envíos. En su lugar, use la función [Simular contenido](#test-landing-page) para probarla y siga los pasos descritos en [esta sección](lp-use-cases.md) para usar correctamente su página de aterrizaje.

![Captura de pantalla que muestra la URL de la página de aterrizaje](assets/lp-published.png){zoomable="yes"}

Puede monitorizar el impacto de su página de aterrizaje mediante los registros <!--and specific reports-->. Haga clic en el botón **[!UICONTROL Registros]**.