---
audience: end-user
product: campaign
title: Trabajo con plantillas de contenido
description: Aprenda a crear plantillas para reutilizar contenido en Adobe Campaign correos electrónicos
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '1085'
ht-degree: 12%

---

# Trabajo con plantillas de contenido {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Plantillas de contenido"
>abstract="Para lograr un proceso de diseño acelerado y mejorado, puede crear plantillas de envío independientes con el fin de reutilizar fácilmente el contenido personalizado en Adobe Campaign. Estas plantillas de contenido se pueden diseñar desde cero, en función de las plantillas integradas o personalizadas, crear a partir de un contenido existente o importar al editor de plantillas de contenido."

Para un proceso de diseño acelerado y mejorado, puede crear plantillas independientes para reutilizar fácilmente el contenido personalizado en [!DNL Adobe Campaign]. Estas plantillas de contenido se pueden diseñar desde cero, en función de plantillas integradas o personalizadas, a partir de contenido existente o importadas en el editor de plantillas de contenido.

Esta funcionalidad permite a los usuarios orientados a contenido trabajar en plantillas independientes, de modo que los usuarios de marketing pueden reutilizarlas y adaptarlas dentro de sus propias campañas de correo electrónico.

>[!NOTE]
>
>Actualmente, solo se admiten las plantillas de contenido **email**.

## Plantillas de contenido de acceso {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Edite el contenido de la plantilla"
>abstract="Haga clic en el botón **Editar contenido** para actualizar el contenido con el Diseñador de correo electrónico."

Para acceder al lista de plantilla de contenido, vaya al **[!UICONTROL menú Administración de]** contenido > **[!UICONTROL Plantillas]** de contenido en el carril izquierdo.

![Las plantilla de contenido lista panel muestran las plantillas disponibles](assets/content-template-list.png){zoomable="yes"}

Este panel muestra todas las plantillas de contenido disponibles en forma de lista. Puede filtrar una [carpeta](../get-started/permissions.md#folders) específica mediante la lista desplegable o agregar reglas mediante [modelador de consultas](../query/query-modeler-overview.md).

![plantilla de contenido lista filtros para carpetas y reglas](assets/content-template-list-filters.png){zoomable="yes"}

Desde la lista, puede editar, duplicado o eliminar las plantillas de contenido existentes. Utilice el botón de la sección superior para crear una plantilla contenido.

### plantilla contenido en modo de solo lectura {#template-readonly}

Se pueden aplicar derechos de acceso a contenido plantillas.

Si no tiene permisos de edición para un plantilla contenido concreto, el plantilla contenido se muestra en **modo** de solo lectura. En este caso, el **[!UICONTROL botón contenido]** Editar se reemplaza por el **[!UICONTROL Ver contenido]** botón, lo que le permite vista el plantilla sin realizar ningún cambio.

![Modo de solo lectura para plantillas de contenido](assets/template-readonly.png){zoomable="yes"}

Como se muestra a continuación, todos los iconos de funciones están desactivados, lo que limita la interacción únicamente a la visualización.

![vista de solo lectura de plantillas de contenido](assets/template-readonly-view.png){zoomable="yes"}

## Crear plantillas de contenido {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Diseño de plantilla de contenido"
>abstract="Diseñe la plantilla de contenido del correo electrónico."

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Selección de plantilla de contenido"
>abstract="Seleccione la plantilla de contenido de correo electrónico."

Las plantillas de contenido se pueden crear [guardando un correo electrónico existente como plantilla](#save-as-template) o desde la lista de plantillas de correo electrónico, a través del botón **Crear plantilla de contenido**, [como se detalla a continuación](#create-template-from-scratch).

Una vez guardado, puede usar esta plantilla al generar cualquier [correo electrónico](../email/create-email.md) dentro de [!DNL Adobe Campaign]. [Descubra cómo](use-email-templates.md)

>[!NOTE]
>
>* Los cambios realizados en contenido plantillas no se propagan a los correos electrónicos.
>
>* Del mismo modo, cuando se utilizan plantillas en un correo electrónico, las modificaciones que realice en los contenido de correo electrónico no afectarán a las contenido utilizadas anteriormente plantilla.

### Creación de una nueva plantilla de contenido {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Defina las propiedades de la plantilla"
>abstract="Defina las propiedades de la plantilla de contenido de correo electrónico para recuperarla fácilmente cuando sea necesario."

Para crear una nueva plantilla de contenido desde el panel de plantillas de contenido, siga estos pasos:

1. Examinar al contenido plantilla lista desde las **[!UICONTROL plantillas]** de contenido > **[!UICONTROL contenido]** a la izquierda carril.

1. Seleccione **[!UICONTROL Crear plantilla]**.

   ![Crear contenido plantilla botón en panel](assets/content-template-create.png){zoomable="yes"}

1. Introduzca la etiqueta y las propiedades plantilla. Puede seleccionar la carpeta en la que desee tienda el plantilla. De forma predeterminada, contenido plantillas se guardan en una carpeta dedicada del Adobe Campaign jerarquía: **[!UICONTROL Explorer]** > **[!UICONTROL plantillas de recursos]** > **[!UICONTROL >****de]** contenido. Más información sobre las carpetas de [este Página](../get-started/permissions.md#folders)

   ![Pantalla de detalles de plantilla para etiquetas y propiedades](assets/content-template-details.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Crear]** y elija cómo desea diseñar su plantilla de las diferentes opciones:

   * [Diseñe su contenido desde cero](create-email-content.md) a través de la interfaz del Diseñador de correo electrónico.
   * [Code o copiar y pegar HTML](code-content.md) sin procesar directamente en el Diseñador de correo electrónico.
   * [Importar contenido](existing-content.md) HTML existente de un archivo o una carpeta .zip.
   * Utilice contenido existente de una lista de plantillas integradas o personalizadas. En esta sección](use-email-templates.md) se describen [los pasos para utilizar un plantilla contenido en una correo electrónico.

   ![Opciones de Email Designer para crear plantillas](assets/email_designer-templates.png){zoomable="yes"}

1. Se muestra el Diseñador de correo electrónico. Editar su contenido según sea necesario, de la misma manera que lo haría para cualquier correo electrónico, de acuerdo con la opción que seleccionó. Aprenda a utilizar el Diseñador de correo electrónico en [esta sección](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Una vez que la plantilla esté lista, haz clic en **[!UICONTROL Guardar]**.

   Si es necesario, haga clic en la flecha situada junto al nombre del plantilla para volver a la pantalla Detalles ]**y editar los**[!UICONTROL  plantilla.

   ![Guardar y vuelva a la pantalla de detalles](assets/content-template-save-back.png){zoomable="yes"}

El plantilla está disponible en las plantillas ]**de**[!UICONTROL  contenido lista. [Más información](#access-templates)

Ahora puede usar este plantilla para versión nuevas contenido. Está disponible en el **[!UICONTROL pestaña Plantillas]** guardadas del Diseñador de correo electrónico. [Descubra cómo](use-email-templates.md)

### Guardar contenido de correo electrónico como plantilla {#save-as-template}

Una vez que [diseñe un correo electrónico](create-email-content.md), puede guardar este contenido como una plantilla para reutilizarla en el futuro. Las plantillas guardadas están disponibles para todos los usuarios de su entorno de Adobe Campaign.

Para guardar un contenido de correo electrónico como plantilla, siga los pasos a continuación:

1. En el diseñador de correo electrónico, haga clic en el **[!UICONTROL botón Más]** en la parte superior derecha de la pantalla.

1. Seleccione **[!UICONTROL Guardar como contenido plantilla]** en el menú desplegable.

   ![Guardar como opción de plantilla de contenido en el diseñador de correo electrónico](assets/email_designer-save-template.png){zoomable="yes"}

1. Introduzca un nombre para esta plantilla y guárdela.

   ![Escriba el nombre de la plantilla guardada](assets/email_designer-template-name.png){zoomable="yes"}

La plantilla se guardará y se mostrará en la lista **[!UICONTROL Plantillas de contenido]**. Se convierte en una plantilla de contenido independiente a la que se puede acceder, editar y eliminar como cualquier otro elemento de la lista. [Más información](#access-manage-templates)

Ahora puede utilizar esta plantilla para crear contenido nuevo. Está disponible en el **[!UICONTROL pestaña Plantillas]** guardadas del Diseñador de correo electrónico. [Descubra cómo](use-email-templates.md)

![Se guardaron plantilla en Email Designer](assets/email_designer-saved-template.png){zoomable="yes"}

>[!NOTE]
>
>Cualquier cambio en esa nueva plantilla no se propaga al correo electrónico de donde proviene. Del mismo modo, cuando el contenido original se edita dentro de ese correo electrónico, el nuevo plantilla no se modifica.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->

## Modificación de una plantilla de contenido {#modify-delete}

Para actualizar una plantilla de contenido existente, siga estos pasos:

1. Desde la lista de contenido plantillas, haga clic en la etiqueta de la plantilla para modificarla.

1. Haga clic en el **[!UICONTROL botón contenido Editar]** para actualizar el contenido con el Diseñador](get-started-email-designer.md) de [correo electrónico.

![Editar contenido opción plantilla](assets/content-template-edition.png){zoomable="yes"}

>[!NOTE]
>
>Los cambios realizados en contenido plantillas no se propagan a correos electrónicos con esta plantilla contenido.

## Eliminar una contenido plantilla {#content-delete}

Existen dos formas de eliminar una plantilla de contenido:

* En la lista de contenido plantillas, haga clic en el botón de puntos suspensivos y, a continuación, seleccione **Eliminar**.

  ![Eliminar un plantilla de contenido del panel](assets/content-template-list-delete.png){zoomable="yes"}

* En la propia plantilla de contenido, haz clic en el **botón Más** y, a continuación, selecciona **Eliminar**.

>[!NOTE]
>
>La eliminación de un plantilla contenido no afecta a las entregas creadas con este plantilla.

## Duplicar un plantilla contenido {#content-duplicate}

Existen dos formas de duplicar una plantilla de contenido:

* En la lista de plantillas de contenido, haga clic en el botón de puntos suspensivos y, a continuación, seleccione **Duplicar**.

* En la propia plantilla de contenido, haga clic en el botón **Más** y, a continuación, seleccione **Duplicar**.

En ambos casos, confirme la duplicación para crear la nueva plantilla de contenido. La etiqueta de la nueva plantilla de contenido es **Copia de`<label of the initial campaign>`**. Vaya a la configuración de la plantilla para actualizar esta etiqueta.