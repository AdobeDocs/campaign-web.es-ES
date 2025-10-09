---
audience: end-user
title: Configuración de un envío multilingüe
description: Obtenga información sobre cómo configurar un envío multilingüe
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 7%

---

# Configuración de un envío multilingüe {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Añadir idiomas"
>abstract="En esta pestaña, encontrará una lista de idiomas en los que se va a realizar el envío. Para añadir más idiomas, haga clic en el botón Añadir idioma o duplique otro idioma desde esta pestaña."

En la interfaz de usuario web de Campaign, puede configurar las entregas como multilingües, lo que le permite enviar mensajes en función del idioma preferido de un perfil. Cuando no se define ninguna preferencia, el mensaje se envía en el idioma predeterminado.

En un envío multilingüe, la administración de idiomas se basa en variantes. Cada variante representa un idioma. Durante la creación de la entrega, puede añadir varias variantes de idioma para que coincidan con el número de idiomas necesarios en el mensaje. También puede cambiar el idioma predeterminado en cualquier momento después de agregar estas variantes.

Actualmente, la capacidad multilingüe está disponible para correos electrónicos, notificaciones push y mensajes transaccionales.

>[!AVAILABILITY]
>
>Las notificaciones push multilingües, los mensajes transaccionales y los SMS solo están disponibles para un conjunto de organizaciones (disponibilidad limitada) y se implementarán globalmente en una versión futura. El servidor debe actualizarse a la versión 8.8.2 o posterior.

Para configurar envíos multilingües, siga estos pasos principales:

1. Agregar una variante de idioma [leer más](#add-variant)
1. Defina el contenido para cada variante [leer más](#define-content)
1. Administrar variantes de idioma, [leer más](#manage-variant)

## Añadir una variante de idioma{#add-variant}

Para crear variantes de idioma, siga estos pasos:

1. En el panel de entregas, haga clic en el icono de lápiz para acceder a la pantalla de edición de contenido de entrega y, a continuación, haga clic en **[!UICONTROL Añadir idioma]**.

   >[!IMPORTANT]
   >
   >El botón **[!UICONTROL Agregar idioma]** solo está disponible si la dimensión de destino contiene el esquema **Idioma**. Para obtener más información sobre esquemas y dimensiones de destino, consulte la [documentación detallada](../audience/targeting-dimensions.md).

   ![](assets/edit-content_2.png){zoomable="yes"}

1. En el menú desplegable **Agregar idioma**, seleccione el idioma que desee agregar y confirme la acción.

   El primer idioma que agregue se establecerá automáticamente como predeterminado y el contenido existente se convertirá en la versión predeterminada. Cuando se añaden idiomas adicionales, su contenido se copia inicialmente del idioma predeterminado.

   ![](assets/edit-content_3.png){zoomable="yes"}

   >[!NOTE]
   >
   >Los idiomas disponibles en esta lista dependen de los valores definidos por el atributo **Language** (valores como: system, user, dbenum, etc.). Obtenga más información acerca de la administración de la enumeración en esta [sección](../administration/enumerations.md).

1. Repita esta operación para agregar otros idiomas. El panel **[!UICONTROL Idiomas]**, a la izquierda, muestra la lista de idiomas que ha elegido, el número de idiomas y el idioma predeterminado.

   Por ejemplo, si ha elegido inglés, francés y sueco, puede ver estos 3 idiomas como se muestra a continuación:

   ![](assets/edit-content_9.png){zoomable="yes"}

   Para aprender a administrar las variantes de idioma, consulte esta [sección](#manage-variant).

## Definir el contenido para cada variante{#define-content}

Una vez configurados los idiomas, defina el contenido del envío para cada idioma.

1. En la pantalla de edición de contenido de entrega, seleccione un idioma en el panel **[!UICONTROL Idiomas]** que hay a la izquierda.

   ![](assets/edit-content_11.png){zoomable="yes"}

1. Defina el contenido del mensaje para este idioma. Obtenga más información en esta [sección](../msg/create-deliveries.md).

1. Repita esta operación para cada idioma.

<!--
>[!BEGINTABS]

>[!TAB Email delivery]

1. From the delivery content edition screen, choose a language and click the **[!UICONTROL Edit email body]** button. You can also hover over the email preview and select **[!UICONTROL Open email designer]**.

    ![](assets/edit-content_11.png){zoomable="yes"}

1. Define the content of your email for this language. [Read more](../email/get-started-email-designer.md#start-authoring)

1. Repeat this operation for each language.

>[!TAB SMS delivery]

1. From the delivery content edition screen, choose a language.

1. Edit the content of the SMS message for this language. [Read more](../sms/create-sms.md)

    ![](assets/edit-content_11-sms.png){zoomable="yes"}

1. Repeat this operation for each language.

>[!ENDTABS]

-->

Para obtener una vista previa del envío, haga clic en el botón **[!UICONTROL Simular contenido]** y seleccione perfiles. Asegúrese de que se muestra el contenido correcto para cada perfil.

![](assets/edit-content_5.png){zoomable="yes"}

## Administrar variantes de idioma{#manage-variant}

En el panel izquierdo, se muestra toda la información de la variante de idioma. Para eliminar todos los idiomas, haga clic en el botón Expandir y, a continuación, haga clic en **[!UICONTROL Eliminar todas las variantes]**.

![](assets/edit-content_13.png){zoomable="yes"}

En la lista de variantes de idioma, puede realizar las siguientes acciones:

* **Editar**: cambia el idioma mientras se mantiene el contenido asociado.
* **Establecer como predeterminado**: establezca el idioma como predeterminado. Cuando un perfil no tiene definido ningún idioma, el mensaje se envía en el idioma predeterminado.
* **Duplicate**: duplica el contenido definido para este idioma y elige una variante diferente.
* **Eliminar**: elimine la variante y su contenido asociado.

![](assets/edit-content_13-sms.png){zoomable="yes"}

