---
audience: end-user
title: Administración de recursos con Adobe Experience Manager as a Cloud Service
description: Obtenga información sobre cómo administrar contenido con Adobe Experience Manager as a Cloud Service
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: 8e035bbf92914f17607a15c184ecf48f5c0efb13
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 3%

---

# Administrar plantillas con [!DNL Adobe Experience Manager as a Cloud Service]{#aem-assets}

## Introducción a [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

La integración de la interfaz web de Adobe Campaign con Adobe Experience Manager facilita la administración optimizada del contenido y los formularios de los envíos de correos electrónicos directamente en la plataforma de Adobe Experience Manager.

![](assets/do-not-localize/book.png)[Más información en Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Crear una plantilla en [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem-template}

1. Vaya a la instancia de autor de [!DNL Adobe Experience Manager] y haga clic en Experiencia de Adobe en la esquina superior izquierda de la página. Elija **[!UICONTROL Sitios]** en el menú.

1. Acceda a **[!UICONTROL Campañas > Nombre de su marca > Área principal > Nombre de su página]**.

1. Haga clic en **[!UICONTROL Crear]** y seleccione **[!UICONTROL Página]** en el menú desplegable.

   ![](assets/aem_1.png)

1. Seleccione la plantilla **[!UICONTROL Adobe Campaign Email]** y asigne un nombre al boletín informativo.

   ![](assets/aem_2.png)

1. Personalice el contenido del correo electrónico añadiendo componentes como, por ejemplo, campos de personalización de Adobe Campaign. [Más información](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. Una vez que el correo electrónico esté listo, vaya al menú **[!UICONTROL Información de la página]** y haga clic en **[!UICONTROL Iniciar flujo de trabajo]**.

   ![](assets/aem_3.png)

1. En la primera lista desplegable, seleccione **[!UICONTROL Aprobar Adobe Campaign]** como modelo de flujo de trabajo y haga clic en **[!UICONTROL Iniciar flujo de trabajo]**.

1. Aparecerá un aviso de exención de responsabilidad en la parte superior de la página que indica `This page is subject to the workflow Approve for Adobe Campaign`. Haga clic en **[!UICONTROL Completar]** junto al aviso legal para confirmar la revisión y haga clic en **[!UICONTROL Aceptar]**.

   ![](assets/aem_4.png)

1. Vuelva a hacer clic en **[!UICONTROL Completar]** y seleccione **[!UICONTROL Aprobación de la newsletter]** en la lista desplegable **[!UICONTROL Siguiente paso]**.

El boletín ya está listo y sincronizado en Adobe Campaign.

## Importar una plantilla de Adobe Experience Manager as a Cloud Service{#aem-templates-perso}

Una vez que la plantilla de Experience Manager esté disponible en Adobe Campaign Web como plantilla de contenido, puede identificar e incorporar el contenido necesario para el correo electrónico, incluida la personalización.

1. En Campaign Web, en el menú **[!UICONTROL Envíos]**, haga clic en **[!UICONTROL Crear envío]**.

1. AEM En la ventana de la plantilla de correo electrónico, seleccione la plantilla integrada **[!UICONTROL Entrega de correo electrónico con contenido de la plantilla]** de la lista de distribución de correo electrónico

   ![](assets/aem_5.png)

1. Escriba una **[!UICONTROL Etiqueta]** para la entrega y configure opciones adicionales según sus necesidades:

   * **[!UICONTROL Nombre interno]**: asigne un identificador único al envío.

   * **[!UICONTROL Carpeta]**: almacene la entrega en una carpeta específica.

   * **[!UICONTROL Código de envío]**: utilice este campo para organizar los envíos según sus propias convenciones de nomenclatura.

   * **[!UICONTROL Descripción]**: especifique una descripción para la entrega.

   * **[!UICONTROL Naturaleza]**: especifique la naturaleza del correo electrónico con fines de clasificación.

1. Defina una **[!UICONTROL audiencia]** en su correo electrónico. [Más información](../email/create-email.md#define-audience)

1. Haga clic en **[!UICONTROL Editar contenido]**.

1. AEM En el menú **[!UICONTROL Editar contenido]**, haga clic en **[!UICONTROL Seleccionar contenido]**.

   ![](assets/aem_6.png)

1. AEM Navegue por la plantilla de y seleccione la que desea importar a Campaign Web.

   ![](assets/aem_8.png)

1. Tenga en cuenta que el contenido no se sincroniza automáticamente. Si los cambios se realizan directamente en las plantillas en Adobe Experience Manager AEM, simplemente selecciona **[!UICONTROL Actualizar contenido de la plantilla]** para obtener la versión más reciente de tu plantilla.

1. Para eliminar la vinculación entre Experience Manager y Campaign o para personalizar aún más la plantilla de Experience Manager AEM en el Diseñador de correo electrónico, haga clic en **[!UICONTROL Desvincular contenido]**.

   ![](assets/aem_9.png)

1. Si agregó contenido personalizado a la plantilla de Experience Manager, haga clic en **[!UICONTROL Simular contenido]** para obtener una vista previa del aspecto que tendrá el mensaje mediante perfiles de prueba.

[Más información sobre la vista previa y los perfiles de prueba](../preview-test/preview-content.md)

1. Al ver la vista previa del mensaje, los elementos personalizados se sustituyen automáticamente por los datos correspondientes del perfil de prueba seleccionado.

   Si es necesario, se pueden agregar perfiles de prueba adicionales mediante el botón **[!UICONTROL Administrar perfiles de prueba]**.

La entrega ya está listo para realizarse.
