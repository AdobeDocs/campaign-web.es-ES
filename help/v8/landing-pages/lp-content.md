---
title: Definición del contenido específico de la página de aterrizaje
description: Aprenda a diseñar contenido específico de páginas de aterrizaje en Campaign Web
feature: Landing Pages
exl-id: 6ca3c8c1-3633-4e3f-a9a1-f46ae27c5c8a
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1248'
ht-degree: 12%

---

# Definición del contenido específico de la página de aterrizaje {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Usar componentes de contenido"
>abstract="Los componentes de contenido son marcadores de posición de contenido vacíos que se pueden utilizar para crear el diseño de una página de aterrizaje. Para definir contenido específicos que permitan a los usuarios seleccionar y enviar sus opciones, utilice el componente de formulario."

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="Definición de la configuración de la página principal"
>abstract="El Página principal se muestra inmediatamente a los usuarios después de hacer clic en el vincular de su página de aterrizaje, por ejemplo, desde una correo electrónico o un sitio web."

Puede editar el contenido de cualquier Página de sus página de aterrizaje.

El primer Página, que se muestra inmediatamente a los usuarios después de hacer clic en el vincular del página de aterrizaje, ya se ha rellenado previamente con el componente](#use-form-component) de formulario específico del [página de aterrizaje para el plantilla<!-- to enable users to select and submit their choices--> seleccionado.

El contenido de las **[!UICONTROL páginas de Confirmación]**, **[!UICONTROL Error]** y **[!UICONTROL Caducidad]** también está precargado. Editar ellos según sea necesario.

También puede definir [estilos para su página de aterrizaje](#lp-form-styles).

Para diseñar aún más sus página de aterrizaje contenido:

* Utilice los mismos componentes que se utilizaron para diseñar una correo electrónico. [Más información](../email/content-components.md#add-content-components)

* Añada contenido condicional a sus páginas de aterrizaje del mismo modo que para un correo electrónico. [Más información](../personalization/conditions.md#condition-condition-builder)

  >[!AVAILABILITY]
  >
  >Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

## Uso del componente del formulario {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="Definir los campos del componente de formulario"
>abstract="Defina cómo verán y enviarán sus opciones los destinatarios desde la página de aterrizaje."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Qué sucede al hacer clic en el botón"
>abstract="Defina lo que sucederá cuando los usuarios envíen el formulario de página de aterrizaje."

Para definir contenido específicos que permitan a los usuarios seleccionar y enviar sus opciones desde el página de aterrizaje, edite el componente Formulario ****. Siga los pasos a continuación.

1. El componente **[!UICONTROL Formulario]** específico para la página de aterrizaje ya se muestra en el lienzo de la plantilla seleccionada.

   >[!NOTE]
   >
   >El componente **[!UICONTROL Form]** solo se puede usar una vez en la misma página.

1. Selecciónelo. La **[!UICONTROL pestaña contenido]** formulario se muestra en la paleta derecha para que pueda editar los distintos campos del formulario.

   ![Componente de formulario mostrado en el lienzo](assets/lp-form-component.png){zoomable="yes"}

   >[!NOTE]
   >
   >Cambie al **[!UICONTROL pestaña Estilos]** en cualquier momento para editar los estilos de su componente de formulario contenido. [Más información](#lp-form-styles)

1. Expanda el primer campo de texto, si lo hubiera, o agregue uno con el **[!UICONTROL botón añadir]** . En la **[!UICONTROL sección Campo de texto 1]** , edite el tipo de campo, el campo de base de datos que desea actualizar, la etiqueta y el texto que se muestra dentro del campo antes de que los usuarios especifiquen un valor.

   ![Configuración de campo de texto en el componente de formulario](assets/lp-form-text-field.png){zoomable="yes"}

1. Marque la opción Hacer que el **[!UICONTROL formulario sea obligatorio]** si es necesario. En ese caso, el página de aterrizaje solo se puede enviar si el usuario ha rellenado este campo.

   >[!NOTE]
   >
   >Si no se rellena un campo obligatorio, aparece un mensaje de error cuando el usuario envía la página.

1. Expanda la casilla de verificación si existe o agregue una con el botón **[!UICONTROL Agregar]**. Seleccione si esa casilla de verificación debe actualizar un servicio o un campo de la base de datos.

   ![Configuración de casilla de verificación en el componente del formulario](assets/lp-form-checkbox.png){zoomable="yes"}

   Si seleccionas **[!UICONTROL Suscripción y servicios]**, selecciona un [servicio](../audience/manage-services.md) de la lista y elige entre las dos opciones siguientes:

   * **[!UICONTROL Suscribirse si está marcado]**: los usuarios deben marcar la casilla para dar su consentimiento (inclusión).
   * **[!UICONTROL Cancelar suscripción si está marcada]**: los usuarios deben marcar la casilla para eliminar su consentimiento (exclusión).

   Si selecciona **[!UICONTROL Campo]**, seleccione un campo del lista](../get-started/attributes.md) de [atributos y elija entre las dos opciones siguientes:

   * **[!UICONTROL Sí, si se selecciona]**.
   * **[!UICONTROL No, si se selecciona]**.

1. Eliminar y agregue tantos campos (como campos de texto, botones de opción, casillas de verificación, listas desplegables, etc.) como sea necesario.

1. Una vez que se hayan agregado o actualizado todos los campos, haga clic en **[!UICONTROL Llamar a la acción]** para expandir la sección correspondiente. Permite definir el comportamiento del botón en el componente **[!UICONTROL Form]**. [Descubra cómo](#define-actions-on-form-submission)

   ![Configuración de llamada a la acción en el componente de formulario](assets/lp-call-to-action.png){zoomable="yes"}

1. Guarde el contenido para volver a las [propiedades de la página de aterrizaje](create-lp.md#create-landing-page).

### Definir acciones al enviar el formulario {#define-actions-on-form-submission}

1. Defina lo que sucede al hacer clic en el botón:

   * **[!UICONTROL Página]** de confirmación: de forma predeterminada, el usuario se redirige al **[!UICONTROL Página de confirmación]** establecido para el página de aterrizaje actual.

   * **[!UICONTROL Redirigir URL]**: Introduzca el URL de la Página a la que se redirige a los usuarios.

   * **[!UICONTROL Página de aterrizaje]**: seleccione otra página de aterrizaje a la que redirigir a los usuarios. Asegúrese de configurar los página de aterrizaje seleccionados en consecuencia.

1. Para realizar actualizaciones adicionales al enviar el formulario, seleccione **[!UICONTROL Actualizaciones adicionales]** y seleccione el elemento que desee actualizar:
   * Un [servicio](../audience/manage-services.md) de suscripción: defina si desea aceptar o rechazar usuarios al enviar el formulario. Al diseñar un correo electrónico, si define un vínculo de tipo **[!UICONTROL Página de aterrizaje]** a esta página de aterrizaje, el servicio seleccionado se utiliza automáticamente. [Más información sobre cómo insertar enlaces](../email/message-tracking.md)

     >[!NOTE]
     >
     >Si desea utilizar varios servicios con este página de aterrizaje, utilice el **[!UICONTROL Servicio desde URL]** opción que se describe a continuación.

   * El canal - la dirección correo electrónico utilizada al rellenar el formulario.
   * Todos los canales: al enviar el formulario, los usuarios optan por participar o no (dependiendo del plantilla seleccionado) para/desde todas las comunicaciones de su marca en todos los canales.
   * Un campo de la base de datos: seleccione un campo de los atributos lista y defina si debe establecerse como verdadero o falso al enviar el formulario.

   ![Configuración de actualizaciones adicionales en el componente de formulario](assets/lp-form-additionnal-updates.png){zoomable="yes"}

1. Seleccione la opción **[!UICONTROL Servicio de la URL]** para permitir que la página de aterrizaje se use en varios servicios, por lo que es dinámica. Defina si desea incluir o excluir usuarios al enviar el formulario.

   >[!AVAILABILITY]
   >
   >Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

   ![Servicio desde la configuración de URL en el componente de formulario](assets/lp-form-service-from-url.png){zoomable="yes"}

   Al diseñar una correo electrónico, si define una **[!UICONTROL vincular de tipo Página]** de aterrizaje para este página de aterrizaje, puede seleccionar cualquier servicio del lista. A continuación, puede seleccionar otros servicios al definir otros vínculos a este página de aterrizaje. [Más información sobre cómo insertar enlaces](../email/message-tracking.md)

   ![Enviar vincular correo electrónico a la configuración página de aterrizaje](assets/email-link-to-landing-page.png){zoomable="yes"}

1. Enviar un mensaje al enviar su página de aterrizaje. [Obtenga más información aquí](#lp-message)

### Enviar un mensaje después del envío {#lp-message}

>[!AVAILABILITY]
>
>Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

Para enviar un mensaje de confirmación automáticamente después del envío de un página de aterrizaje, seguir estos pasos:

1. En la sección **[!UICONTROL LLAMADA A LA ACCIÓN]**, marque la opción **[!UICONTROL Enviar correo electrónico de confirmación]**.

1. En la lista desplegable asociada, elija la plantilla de mensaje transaccional que debe enviarse.

![Configuración de correo electrónico de confirmación en el componente del formulario](assets/lp-confirmation.png){zoomable="yes"}

## Definir estilos de formulario de una página de aterrizaje {#lp-form-styles}

1. Para modificar los estilos de su componente de formulario contenido, cambie en cualquier momento al **[!UICONTROL pestaña Estilos]** .

1. La **[!UICONTROL sección Campo]** de texto se expande de forma predeterminada. Permite editar el aspecto de los campos de texto, como el fuente de etiqueta, la posición de la etiqueta, el color de fondo del campo o la borde de campo.

   ![Configuración de estilo de campo de texto](assets/lp-text-styles.png){zoomable="yes"}

1. Expanda la **[!UICONTROL sección Casilla]** de verificación para definir el aspecto de las casillas de verificación y el texto correspondiente. Por ejemplo, ajuste la familia y el tamaño del fuente, o el color de la borde de la casilla de verificación.

   ![Configuración de estilo de casilla de verificación](assets/lp-checkbox-style.png){zoomable="yes"}

1. Expanda y edite cualquier otra sección correspondiente a otros campos que haya agregado (botón de opción, lista desplegable, fecha y hora, etc.) al formulario.

1. Expanda la sección **[!UICONTROL Llamada a la acción]** para modificar el aspecto del botón en el formulario de componente. Por ejemplo, cambie la fuente, agregue un borde, edite el color de la etiqueta al pasar el ratón por encima o ajuste la alineación del botón.

   ![Configuración del estilo de llamada a la acción](assets/lp-call-to-action-style.png){zoomable="yes"}

   Vista previa algunos de los ajustes, como botón color de etiqueta al pasar el ratón por encima, mediante el **[!UICONTROL botón Simular contenido]** . [Más información](create-lp.md#test-landing-page)

1. Guarde los cambios.