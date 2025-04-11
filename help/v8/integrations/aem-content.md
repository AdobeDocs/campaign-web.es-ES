---
audience: end-user
title: Administración de recursos con Adobe Experience Manager as a Cloud Service
description: Obtenga información sobre cómo administrar contenido con Adobe Experience Manager as a Cloud Service
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 5%

---

# Administrar plantillas con [!DNL Adobe Experience Manager as a Cloud Service]{#aem-assets}

## Introducción a [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

La integración de la interfaz web de Adobe Campaign con Adobe Experience Manager permite una administración optimizada del contenido y los formularios de los envíos de correos electrónicos directamente en la plataforma de Adobe Experience Manager.

![](assets/do-not-localize/book.png)[Más información en Adobe Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Crear una plantilla en [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem-template}

1. Vaya a la instancia de autor de [!DNL Adobe Experience Manager] y haga clic en Adobe Experience en la esquina superior izquierda de la página. Elija **[!UICONTROL Sitios]** en el menú.

1. Acceda a **[!UICONTROL Campañas > Nombre de su marca > Área principal > Nombre de su página]**.

1. Haga clic en **[!UICONTROL Crear]** y seleccione **[!UICONTROL Página]** en el menú desplegable.

   ![Captura de pantalla que muestra el botón &quot;Crear&quot; y la opción &quot;Página&quot; en el menú desplegable.](assets/aem_1.png)

1. Seleccione la plantilla **[!UICONTROL Adobe Campaign Email]** y asigne un nombre al boletín informativo.

   ![[Captura de pantalla que muestra el campo de nombre y selección de la plantilla &quot;Correo electrónico de Adobe Campaign&quot;.]](assets/aem_2.png)

1. Personalice el contenido del correo electrónico añadiendo componentes como, por ejemplo, campos de personalización de Adobe Campaign. [Más información](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. Una vez que el correo electrónico esté listo, vaya al menú **[!UICONTROL Información de la página]** y haga clic en **[!UICONTROL Iniciar flujo de trabajo]**.

   ![Captura de pantalla que muestra el menú &quot;Información de página&quot; y la opción &quot;Iniciar flujo de trabajo&quot;.](assets/aem_3.png)

1. En el primer menú desplegable, seleccione **[!UICONTROL Aprobar Adobe Campaign]** como modelo de flujo de trabajo y haga clic en **[!UICONTROL Iniciar flujo de trabajo]**.

1. Aparecerá un aviso de exención de responsabilidad en la parte superior de la página que indica `This page is subject to the workflow Approve for Adobe Campaign`. Haga clic en **[!UICONTROL Completar]** junto al aviso legal para confirmar la revisión y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

   ![Captura de pantalla que muestra el descargo de responsabilidad y el botón &quot;Completar&quot;.](assets/aem_4.png)

1. Vuelva a hacer clic en **[!UICONTROL Completar]** y seleccione **[!UICONTROL Aprobación de la newsletter]** en el menú desplegable **[!UICONTROL Siguiente paso]**.

El boletín ya está listo y sincronizado en Adobe Campaign.

## Importar una plantilla de Adobe Experience Manager as a Cloud Service{#aem-templates-perso}

Una vez que la plantilla de Experience Manager esté disponible en Adobe Campaign Web como plantilla de contenido, puede identificar e incorporar el contenido necesario para el correo electrónico, incluida la personalización.

1. En Campaign Web, en el menú **[!UICONTROL Envíos]**, haga clic en **[!UICONTROL Crear envío]**.

1. En la ventana de la plantilla de correo electrónico, seleccione la plantilla integrada **[!UICONTROL Email delivery with AEM content]**.

   ![Captura de pantalla que muestra la selección de plantilla &quot;Envío de correo electrónico con contenido de AEM&quot;.](assets/aem_5.png)

1. Escriba una **[!UICONTROL Etiqueta]** para la entrega y configure opciones adicionales según sus necesidades:

   * **[!UICONTROL Nombre interno]**: asignar un identificador único al envío.
   * **[!UICONTROL Carpeta]**: almacene el envío en una carpeta específica.
   * **[!UICONTROL Código de envío]**: utilice este campo para organizar los envíos según sus propias convenciones de nomenclatura.
   * **[!UICONTROL Descripción]**: especifique una descripción para la entrega.
   * **[!UICONTROL Naturaleza]**: especifique la naturaleza del correo electrónico con fines de clasificación.

1. Defina una **[!UICONTROL audiencia]** para su correo electrónico. [Más información](../email/create-email.md#define-audience)

1. Haga clic en **[!UICONTROL Editar contenido]**.

1. En el menú **[!UICONTROL Editar contenido]**, haga clic en **[!UICONTROL Seleccionar contenido de AEM]**.

   ![Captura de pantalla que muestra la opción &quot;Seleccionar contenido de AEM&quot; en el menú &quot;Editar contenido&quot;.](assets/aem_6.png)

1. Examine la plantilla de AEM y seleccione la que desea importar a Campaign Web.

   ![Captura de pantalla que muestra la interfaz de selección de plantillas de AEM.](assets/aem_8.png)

1. Tenga en cuenta que el contenido no se sincroniza automáticamente. Si los cambios se realizan directamente en las plantillas en Adobe Experience Manager, seleccione **[!UICONTROL Actualizar contenido de AEM]** para actualizar a la última versión de la plantilla.

1. Para eliminar la vinculación entre Experience Manager y Campaign o para personalizar aún más la plantilla de Experience Manager en el Diseñador de correo electrónico, haga clic en **[!UICONTROL Desvincular el contenido de AEM]**.

   ![Captura de pantalla que muestra la opción &quot;Desvincular contenido de AEM&quot;.](assets/aem_9.png)

1. Si agregó contenido personalizado a la plantilla de Experience Manager, haga clic en **[!UICONTROL Simular contenido]** para obtener una vista previa del aspecto que tendrá el mensaje mediante perfiles de prueba.

[Más información sobre la vista previa y los perfiles de prueba](../preview-test/preview-content.md)

1. Al ver la vista previa del mensaje, los elementos personalizados se sustituyen automáticamente por los datos correspondientes del perfil de prueba seleccionado.

   Si es necesario, agregue perfiles de prueba adicionales mediante el botón **[!UICONTROL Administrar perfiles de prueba]**.

La entrega ya está listo para realizarse.