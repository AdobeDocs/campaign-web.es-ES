---
title: Creación de un perfil
description: Obtenga información sobre cómo crear un perfil en Campaign Web.
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 48%

---

# Creación de un perfil {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Detalles básicos"
>abstract="Esta sección ofrece detalles básicos del perfil. Para modificar cualquier información, realice los cambios directamente en el campo correspondiente y haga clic en el botón **Guardar**, situado en la esquina superior derecha de la pantalla."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Información de contacto"
>abstract="Esta sección ofrece detalles sobre la información de contacto del perfil. Para modificar cualquier información, realice los cambios directamente en el campo correspondiente y haga clic en el botón **Guardar**, situado en la esquina superior derecha de la pantalla."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Dirección"
>abstract="Esta sección ofrece detalles sobre la dirección postal del perfil y la calidad de la dirección. Para modificar cualquier información, realice los cambios directamente en el campo correspondiente y haga clic en el botón **Guardar**, situado en la esquina superior derecha de la pantalla."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Detalles de la cuenta"
>abstract="Esta sección ofrece información sobre los detalles de la cuenta del perfil. Para modificar cualquier información, realice los cambios directamente en el campo correspondiente y haga clic en el botón **Guardar**, situado en la esquina superior derecha de la pantalla."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Ya no se puede contactar"
>abstract="Esta sección ofrece detalles sobre las preferencias de contacto del perfil. Para modificar cualquier información, realice los cambios directamente en el campo correspondiente y haga clic en el botón **Guardar**, situado en la esquina superior derecha de la pantalla."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Campos personalizados"
>abstract="Los campos personalizados son atributos específicos adaptados a sus necesidades que se han configurado para su instancia. Para modificar cualquier información, realice los cambios directamente en el campo correspondiente y haga clic en el botón **Guardar**, situado en la esquina superior derecha de la pantalla."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Otros"
>abstract="Esta sección proporciona atributos integrados adicionales. Para modificar cualquier información, realice los cambios directamente en el campo correspondiente y haga clic en el botón **Guardar**, situado en la esquina superior derecha de la pantalla."

Para crear un perfil, siga estos pasos:

1. Vaya a **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]** y haga clic en **[!UICONTROL Crear perfil]** en la esquina superior derecha de la pantalla.

1. Se muestra la lista de atributos disponibles para el perfil, organizados en diferentes secciones detalladas en la siguiente tabla.

   ![](assets/create-profile.png){zoomable="yes"}

   | Sección Atributos | Descripción |
   |  ---  |  ---  |
   | **Detalles básicos** | Información básica sobre el perfil, como el nombre o la fecha de nacimiento.<br/>De forma predeterminada, los perfiles se almacenan en **[!UICONTROL Destinatarios]** carpeta. Puede cambiarlo navegando a la ubicación deseada. [Aprenda a trabajar con carpetas](../get-started/permissions.md#folders) |
   | **Información de contacto** | La información de contacto del perfil, como la dirección de correo electrónico o el número de teléfono. |
   | **Dirección** | La dirección postal del perfil. Esta sección también proporciona una evaluación de la calidad de la dirección. La dirección de un perfil se considera válida si se especifican los campos &quot;Apellidos&quot;, &quot;Ciudad&quot; y &quot;Código postal&quot;. |
   | **Detalles de la cuenta** | Información sobre la cuenta del perfil, como su estado o número de cuenta. |
   | **Ya no se puede contactar** | Las preferencias de contacto del perfil. Cuando se selecciona cualquiera de estas opciones, el perfil se encuentra en la lista de bloqueados de la.<br/>Por ejemplo, si el destinatario hace clic en un vínculo para darse de baja de un boletín, esta información se agrega a los datos de contacto. Este destinatario ya no está dirigido a los canales seleccionados. Obtenga más información sobre la administración de cuarentena en [Documentación de Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"} |
   | **Campos personalizados** | Si se han configurado campos personalizados, estos se muestran en esta sección. Los campos personalizados son atributos adicionales añadidos a **[!UICONTROL Perfiles]** mediante la consola de Adobe Campaign. Obtenga más información en la [Documentación de Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html){target="_blank"} |
   | **Otros** | Atributos integrados adicionales. |

1. Una vez configurado el perfil, haga clic en **[!UICONTROL Crear]** para guardarlo en la base de datos.

   Una vez finalizado, puede editar el perfil en cualquier momento abriéndolo en la lista de perfiles. [Obtenga información sobre cómo explorar los detalles de los perfiles](profile-view.md)
