---
audience: end-user
title: Administrar recursos con Adobe Experience Manager as a Cloud Service
description: Obtenga información sobre cómo administrar contenido con Adobe Experience Manager as a Cloud Service
badge: label="Disponibilidad limitada"
source-git-commit: 6fd2fa72e482883802c96f0888ea79f2b16b7152
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 3%

---

# Administración de plantillas con [!DNL Adobe Experience Manager as a Cloud service]{#aem-assets}

## Introducción a [!DNL Adobe Experience Manager as a Cloud service]{#create-aem}

La integración de la interfaz web de Adobe Campaign con Adobe Experience Manager facilita la administración optimizada del contenido y los formularios de los envíos de correos electrónicos directamente en la plataforma de Adobe Experience Manager.

![](assets/do-not-localize/book.png)[Obtenga más información sobre Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Creación de una plantilla en [!DNL Adobe Experience Manager as a Cloud service]{#create-aem-template}

1. Navegue hasta su [!DNL Adobe Experience Manager] Cree una instancia de autor de y haga clic en Experiencia de Adobe en la esquina superior izquierda de la página. Elegir **[!UICONTROL Sites]** en el menú.

1. Acceso **[!UICONTROL Campañas > Nombre de la marca > Área principal > Nombre de la página]**.

1. Clic **[!UICONTROL Crear]** y seleccione **[!UICONTROL Página]** en el menú desplegable.

   ![](assets/aem_1.png)

1. Seleccione el **[!UICONTROL Correo electrónico de Adobe Campaign]** y asigne un nombre al boletín informativo.

   ![](assets/aem_2.png)

1. Personalice el contenido del correo electrónico añadiendo componentes como, por ejemplo, campos de personalización de Adobe Campaign. [Más información](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. Una vez que el correo electrónico esté listo, vaya a **[!UICONTROL Información de página]** y haga clic en **[!UICONTROL Iniciar flujo de trabajo]**.

   ![](assets/aem_3.png)

1. En la primera lista desplegable, seleccione **[!UICONTROL Aprobar Adobe Campaign]** como modelo de flujo de trabajo y haga clic en **[!UICONTROL Iniciar flujo de trabajo]**.

1. Aparecerá un aviso legal en la parte superior de la página que indica: `This page is subject to the workflow Approve for Adobe Campaign`. Clic **[!UICONTROL Completar]** junto al aviso legal para confirmar la revisión y haga clic en **[!UICONTROL Ok]**.

   ![](assets/aem_4.png)

1. Clic **[!UICONTROL Completar]** de nuevo y seleccione **[!UICONTROL Aprobación de newsletter]** en el **[!UICONTROL Paso siguiente]** menú desplegable.

El boletín ya está listo y sincronizado en Adobe Campaign.

## Importar una plantilla de Adobe Experience Manager as a Cloud Service{#aem-templates-perso}

Una vez que la plantilla de Experience Manager esté disponible en Adobe Campaign Web como plantilla de contenido, puede identificar e incorporar el contenido necesario para el correo electrónico, incluida la personalización.

1. En Campaign Web, desde el **[!UICONTROL Envíos]** , haga clic en **[!UICONTROL Creación de envíos]**.

1. En la ventana de plantilla de correo electrónico, seleccione la opción integrada **[!UICONTROL AEM Envío de correo electrónico con contenido de]** plantilla.

   ![](assets/aem_5.png)

1. Introduzca una **[!UICONTROL Etiqueta]** para el envío y configure opciones adicionales según sus necesidades:

   * **[!UICONTROL Nombre interno]**: asigne un identificador único a la entrega.

   * **[!UICONTROL Carpeta]**: almacene la entrega en una carpeta específica.

   * **[!UICONTROL Código de envío]**: utilice este campo para organizar los envíos en función de su propia convención de nombres.

   * **[!UICONTROL Descripción]**: especifique una descripción para la entrega.

   * **[!UICONTROL Naturaleza]**: especifique la naturaleza del correo electrónico con fines de clasificación.

1. Definir un **[!UICONTROL Audiencia]** a su correo electrónico. [Más información](../email/create-email.md#define-audience)

1. Clic **[!UICONTROL Editar contenido]**.

1. Desde el **[!UICONTROL Editar contenido]** , haga clic en **[!UICONTROL AEM Seleccionar contenido de la]**.

   ![](assets/aem_6.png)

1. AEM Navegue por la plantilla de y seleccione la que desea importar a Campaign Web.

   ![](assets/aem_8.png)

1. Si los cambios se realizan directamente en las plantillas en Adobe Experience Manager, simplemente seleccione **[!UICONTROL AEM Actualizar contenido de]** para tener la última versión de la plantilla.

1. Para eliminar la vinculación entre Experience Manager y Campaign o para personalizar aún más la plantilla de Experience Manager en el Diseñador de correo electrónico, haga clic en **[!UICONTROL AEM Desvincular contenido de la]**.

   ![](assets/aem_9.png)

1. Si ha añadido contenido personalizado a la plantilla de Experience Manager, haga clic en **[!UICONTROL Simular contenido]** para previsualizar cómo aparecerá en el mensaje mediante perfiles de prueba.

[Más información sobre la vista previa y los perfiles de prueba](../preview-test/preview-content.md)

1. Al ver la vista previa del mensaje, los elementos personalizados se sustituyen automáticamente por los datos correspondientes del perfil de prueba seleccionado.

   Si es necesario, se pueden añadir perfiles de prueba adicionales mediante la variable **[!UICONTROL Administración de perfiles de prueba]** botón.

La entrega ya está listo para realizarse.
