---
audience: end-user
product: campaign
title: Trabajo con plantillas de contenido
description: Learn how to create templates to reuse content in Adobe Campaign emails
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 0b85b5a4b6eff4fdb9835a0d1ccb5d0a86c103a0
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 17%

---

# Trabajo con plantillas de contenido {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Plantillas de contenido"
>abstract="Para lograr un proceso de diseño acelerado y mejorado, puede crear plantillas de envío independientes con el fin de reutilizar fácilmente el contenido personalizado en Adobe Campaign. Estas plantillas de contenido se pueden diseñar desde cero, en función de las plantillas integradas o personalizadas, crear a partir de un contenido existente o importar al editor de plantillas de contenido."

[!DNL Adobe Campaign] Estas plantillas de contenido se pueden diseñar desde cero, en función de las plantillas integradas o personalizadas, crear a partir de un contenido existente o importar al editor de plantillas de contenido.

This functionality enables content-oriented users to work on standalone templates so that marketing users can reuse and adapt them inside their own email campaigns.

>[!NOTE]
>
>****

## Plantillas de contenido de acceso {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Edite el contenido de la plantilla"
>abstract="Haga clic en el botón **Editar contenido** para actualizar el contenido con el Diseñador de correo electrónico."

Para acceder a la lista de plantillas de contenido, vaya al menú **[!UICONTROL Administración de contenido]** > **[!UICONTROL Plantillas de contenido]** desde el carril izquierdo.

![](assets/content-template-list.png){zoomable="yes"}

Este panel muestra todas las plantillas de contenido disponibles en forma de lista. Puede filtrar una [carpeta](../get-started/permissions.md#folders) específica mediante la lista desplegable o agregar reglas mediante [modelador de consultas](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png){zoomable="yes"}

Desde la lista, puede editar, duplicar o eliminar plantillas de contenido existentes. Utilice el botón de la sección superior para crear una plantilla de contenido.

### Plantilla de contenido en modo de solo lectura {#template-readonly}

Los derechos de acceso se pueden aplicar a las plantillas de contenido.

Si no tiene permisos de edición para una plantilla de contenido determinada, esta se mostrará en **modo de solo lectura**. En este caso, el botón **[!UICONTROL Editar contenido]** se reemplaza con el botón **[!UICONTROL Ver contenido]**, lo que le permite ver la plantilla sin realizar ningún cambio.

![](assets/template-readonly.png){zoomable="yes"}

Como se muestra a continuación, todos los iconos de funciones están desactivados, lo que limita la interacción únicamente a la visualización.

![](assets/template-readonly-view.png){zoomable="yes"}

## Crear plantillas de contenido {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Diseño de plantilla de contenido"
>abstract="Diseñe la plantilla de contenido del correo electrónico."

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Selección de plantilla de contenido"
>abstract="Seleccione la plantilla de contenido de correo electrónico."

Las plantillas de contenido se pueden crear [guardando un correo electrónico existente como plantilla](#save-as-template) o de la lista de plantillas de correo electrónico, mediante el botón **Crear plantilla de contenido**, [como se detalla a continuación](#create-template-from-scratch).

[](../email/create-email.md)[!DNL Adobe Campaign] [Descubra cómo](use-email-templates.md)

>[!NOTE]
>
>* Changes made to content templates are not propagated to emails.
>
>* Similarly, when templates are used in an email, any edits you make to your email content do not impact the previously used content template.

### Creación de una nueva plantilla de contenido {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Defina las propiedades de la plantilla"
>abstract="Defina las propiedades de la plantilla de contenido de correo electrónico para recuperarlas fácilmente cuando sea necesario."

Para crear una nueva plantilla de contenido desde el panel de plantillas de contenido, siga estos pasos:

1. Vaya a la lista de plantillas de contenido desde el carril izquierdo de **[!UICONTROL Administración de contenido]** > **[!UICONTROL Plantillas de contenido]**.

1. Seleccione **[!UICONTROL Crear plantilla]**.

   ![](assets/content-template-create.png){zoomable="yes"}

1. Introduzca la etiqueta de plantilla y las propiedades. Puede seleccionar la carpeta en la que desea almacenar la plantilla. De manera predeterminada, las plantillas de contenido se almacenan en una carpeta específica de la jerarquía de Adobe Campaign: **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Templates]** > **[!UICONTROL Content templates]**. Más información sobre las carpetas de [esta página](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Crear]** y elija cómo desea diseñar la plantilla a partir de las distintas opciones:

   * [Diseñe su contenido desde cero](create-email-content.md) a través de la interfaz de Designer de correo electrónico.

   * [Codifique o copie y pegue el HTML sin procesar](code-content.md) directamente en el Designer de correo electrónico.

   * [Importe contenido existente del HTML](existing-content.md) desde un archivo o una carpeta .zip.

   * Utilice contenido existente de una lista de plantillas integradas o personalizadas. [](use-email-templates.md)

   ![](assets/email_designer-templates.png){zoomable="yes"}

1. The Email Designer displays. Edit your content as needed, the same way you would do for any email, according to the option you selected. [](get-started-email-designer.md)

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. ****

   ****

   ![](assets/content-template-save-back.png){zoomable="yes"}

**** [Más información](#access-templates)

Ahora puede usar esta plantilla para generar un nuevo contenido: está disponible en la pestaña **[!UICONTROL Plantillas guardadas]** de Email Designer. [Descubra cómo](use-email-templates.md)

### Guardar contenido de correo electrónico como plantilla {#save-as-template}

Una vez que [diseñó un correo electrónico](create-email-content.md), puede guardar este contenido como una plantilla para reutilizarlo en el futuro. Las plantillas guardadas están disponibles para todos los usuarios de su entorno de Adobe Campaign.

Para guardar un contenido de correo electrónico como plantilla, siga los pasos a continuación:

1. En el diseñador de correo electrónico, haga clic en el botón **[!UICONTROL Más]** en la parte superior derecha de la pantalla.

1. Seleccione **[!UICONTROL Guardar como plantilla de contenido]** en el menú desplegable.

   ![](assets/email_designer-save-template.png){zoomable="yes"}

1. Introduzca un nombre para esta plantilla y guárdela.

   ![](assets/email_designer-template-name.png){zoomable="yes"}

La plantilla se guardará y se mostrará en la lista **[!UICONTROL Plantillas de contenido]**. Se convierte en una plantilla de contenido independiente a la que se puede acceder, editar y eliminar como cualquier otro elemento de la lista. [Más información](#access-manage-templates)

**** [Descubra cómo](use-email-templates.md)

![](assets/email_designer-saved-template.png){zoomable="yes"}


>[!NOTE]
>
>Any change to that new template is not propagated to the email it comes from. Similarly, when the original content is edited within that email, the new template is not modified.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->


## Modify a content template {#modify-delete}

To update an existing content template, follow these steps:

1. From the list of content templates, click on the label of the template to modify to edit it.

1. ****[](get-started-email-designer.md)

![](assets/content-template-edition.png){zoomable="yes"}

>[!NOTE]
>
>Changes made to content templates are not propagated to emails using this content template.

## Delete a content template {#content-delete}

You have two ways to delete a content template:

* ****

  ![Eliminar una plantilla de contenido del tablero](assets/content-template-list-delete.png)

* en la propia plantilla de contenido, haga clic en el botón **Más** y seleccione **Eliminar**


>[!NOTE]
>
>La eliminación de una plantilla de contenido no afecta a los envíos creados con esta plantilla.


## Duplicación de una plantilla de contenido {#content-duplicate}

Existen dos formas de duplicar una plantilla de contenido:

* en la lista de plantillas de contenido, haga clic en el botón de puntos suspensivos y seleccione **Duplicate**

* en la propia plantilla de contenido, haga clic en el botón **Más** y, a continuación, seleccione **Duplicar**

En ambos casos, confirme la duplicación para crear la nueva plantilla de contenido. La etiqueta de la nueva plantilla de contenido es **Copia de`<label of the initial campaign`**. Vaya a la configuración de la plantilla para actualizar esta etiqueta.

