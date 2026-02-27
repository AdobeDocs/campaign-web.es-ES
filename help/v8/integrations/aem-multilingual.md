---
audience: end-user
title: Creación de correos electrónicos multilingües con Adobe Experience Manager
description: Obtenga información sobre cómo crear envíos de correo electrónico multilingües con copias de idioma de Adobe Experience Manager en Campaign Web.
feature: Email
topic: Content Management
role: User
level: Intermediate
exl-id: 6fc6ff43-ac7f-46c7-aa1a-9489ffc45423
source-git-commit: 3a5121a4dca59532e1aada49c26de6ece1a58e4b
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 2%

---

# Creación de correos electrónicos multilingües con Adobe Experience Manager {#aem-multilingual}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Experience Manager live y copias de idioma"
>abstract="Ahora puede acceder al idioma de Adobe Experience Manager y a las Live Copies directamente en Campaign. La actualización de contenido en tiempo real elimina la sincronización manual para flujos de trabajo optimizados en varios idiomas."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

La integración de Adobe Experience Manager le permite crear envíos de correo electrónico multilingües utilizando copias de idioma de Adobe Experience Manager. Esto le permite administrar variantes de contenido en diferentes idiomas y enviar correos electrónicos personalizados en función de las preferencias de idioma del destinatario.

## Requisitos previos {#prerequisites}

Antes de crear un envío multilingüe de correo electrónico, asegúrese de lo siguiente:

* Acceso a una instancia de Adobe Experience Manager configurada para la integración de la interfaz web de Adobe Campaign.
* Contenido de Adobe Experience Manager con copias de idioma ya creadas y aprobadas. Obtenga más información acerca del Asistente para copia de idioma en [Documentación de Adobe Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)
* Plantilla de envíos de correo electrónico configurada para recibir contenido de Adobe Experience Manager. Consulte los pasos detallados en la sección [Habilitar el modo multilingüe](#enable-multilingual).

## Creación de una entrega multilingüe

Para crear un envío multilingüe de correo electrónico, primero debe habilitar la opción multilingüe en la configuración de envío. El sistema detecta automáticamente las copias de idioma disponibles y le permite elegir cuáles añadir.

### Habilitar modo multilingüe {#enable-multilingual}

Cree una nueva entrega y active la opción multilingüe en la configuración avanzada.

1. En el menú **[!UICONTROL Envíos]**, haga clic en **[!UICONTROL Crear envío]**.

   ![](assets/lg-copy-1.png)

1. Seleccione la plantilla **[!UICONTROL Email delivery with AEM content]** y haga clic en **[!UICONTROL Crear entrega]**.

   ![](assets/lg-copy-2.png)

1. Introduzca una etiqueta para la entrega y configure la audiencia. [Más información](../email/create-email.md)

1. Acceda a su envío **[!UICONTROL Configuración]** y luego vaya a la sección **[!UICONTROL Avanzadas]**.

1. Habilite la opción **[!UICONTROL Habilitar AEM multilingüe]**.

   ![](assets/lg-copy-3.png)

1. Asegúrese de que:

   * **[!UICONTROL El modo de edición de contenido]** está establecido en **[!UICONTROL AEM]**.
   * Se seleccionó la cuenta externa **[!UICONTROL External account]** de Adobe Experience Manager correcta.

1. Haga clic en **[!UICONTROL Guardar y cerrar]**.

### Crear variantes de contenido {#create-variants}

Seleccione el contenido de Adobe Experience Manager y elija las variantes de idioma que desea incluir en el envío.

1. Haga clic en **[!UICONTROL Editar contenido]**.

1. Seleccione **[!UICONTROL Crear variante de contenido]**.

   ![](assets/lg-copy-4.png)

1. Seleccione el contenido de Adobe Experience Manager de la lista.

   ![](assets/lg-copy-5.png)

1. El sistema detecta todas las copias de idioma asociadas con el contenido seleccionado (relación principal-secundario). Por ejemplo, si el contenido de Adobe Experience Manager tiene variantes en francés, alemán e italiano, todas las variantes están disponibles para su selección.

   Seleccione las variantes de idioma que desee incluir en el envío.

   ![](assets/lg-copy-6.png)

1. Haga clic en **[!UICONTROL Save]**.

1. Revise las variantes de idioma en el editor de contenido. Ahora puede [administrar cada variante de forma individual](#manage-variants) o continuar con [el envío](../monitor/prepare-send.md).

   ![](assets/lg-copy-7.png)

## Administrar variantes de idioma {#manage-variants}

Después de crear variantes de contenido, puede administrarlas directamente en la entrega:

1. Para establecer un idioma predeterminado, acceda al menú avanzado de la variante que haya elegido y seleccione **[!UICONTROL Establecer como predeterminado]**. El idioma predeterminado se utiliza cuando la preferencia de idioma de un perfil no está establecida o no coincide con ninguna variante disponible.

   Haga clic en **[!UICONTROL Eliminar]** para eliminar cualquier variante de su envío.

   ![](assets/lg-copy-8.png)

1. En el menú avanzado Variantes de contenido, haga clic en **[!UICONTROL Administrar configuraciones regionales]** para agregar otras configuraciones regionales a su envío.

   ![](assets/lg-copy-9.png)

1. Seleccione copias de idioma adicionales para incluir más variantes y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/lg-copy-11.png)

1. Si el contenido se actualiza en Adobe Experience Manager, haga clic en **[!UICONTROL Actualizar contenido de AEM]** para sincronizar todas las variantes con la última versión.

   ![](assets/lg-copy-10.png)

1. Haga clic en **[!UICONTROL Desvincular contenido de AEM]** si desea editar contenido directamente en Campaign o romper el vínculo con Adobe Experience Manager.

   >[!CAUTION]
   >
   >Después de desvincularlo, no puede actualizar el contenido de Adobe Experience Manager ni crear nuevas variantes. El contenido se vuelve independiente de Adobe Experience Manager.
