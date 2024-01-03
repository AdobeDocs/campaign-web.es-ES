---
audience: end-user
title: Previsualización del contenido de envío
description: Obtenga información sobre cómo previsualizar el contenido de la entrega con la IU web de Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Disponibilidad limitada"
source-git-commit: 6dcdfae8aa6d6346fc02217db77a96cf6d219fdc
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 1%

---


# Previsualización del contenido de envío {#preview-content}

Utilice el [!DNL Campaign] capacidad de simulación de contenido para previsualizar el contenido del mensaje antes de enviarlo. Esto permite controlar la personalización y comprobar cómo se muestra a los destinatarios.

Para obtener una vista previa del contenido del envío, siga los pasos a continuación.

1. Vaya a la pantalla de edición de contenido de su envío o a la [Diseñador de correo electrónico](../content/get-started-email-designer.md).

1. Haga clic en **[!UICONTROL Simular contenido]** botón.

   ![](assets/simulate-button.png)

1. Para seleccionar los perfiles que se utilizarán para previsualizar el contenido personalizado, utilice:

   * **[!UICONTROL Añadir perfil(es) de prueba]** para previsualizar envíos de correo electrónico y SMS

   * **[!UICONTROL Añadir suscriptor(es)]** para previsualizar notificaciones push

1. Puede combinar perfiles y perfiles de prueba para previsualizar el mensaje de correo electrónico o SMS.

   * El **[!UICONTROL Perfiles de prueba]** La pestaña enumera todas las direcciones semilla que son destinatarios adicionales y ficticios de la base de datos.

     ![](assets/simulate-select-profiles.png)

     >[!NOTE]
     >
     >Los perfiles de prueba se pueden crear desde el **[!UICONTROL Administración de clientes]** > **[!UICONTROL Perfiles]** menú. [Más información](../audience/test-profiles.md#create-test-profiles)

   * El **[!UICONTROL Perfiles]** enumera todos los destinatarios almacenados en la **[!UICONTROL Perfiles y objetivos]** carpeta desde el [!DNL Campaign] consola. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}.

     >[!NOTE]
     >
     >También puede ver y administrar perfiles desde la pestaña correspondiente de la interfaz de usuario web de Campaign. [Más información](../audience/about-recipients.md)

1. Clic **[!UICONTROL Seleccionar]** para confirmar la selección.

   En el panel derecho del formulario se muestra una vista previa del contenido de la entrega **[!UICONTROL Simular]** pantalla. Los elementos personalizados se sustituyen por los datos del perfil seleccionado en el panel izquierdo.

   ![](assets/simulate-preview.png)

1. Si ha añadido varios perfiles, puede cambiar entre ellos en la lista para previsualizar el contenido de envío correspondiente. También puede agregar más perfiles de prueba y borrar la selección utilizando los botones correspondientes del panel izquierdo.

1. Para las entregas por correo electrónico, puede ajustar la **[!UICONTROL Nivel de zoom]** y previsualice el contenido en el escritorio o dispositivo móvil mediante el icono dedicado en la esquina superior derecha.

1. Desde el **[!UICONTROL Simular]** pantalla también puede:
   * Envío de entregas de prueba a destinatarios específicos para su validación: [Más información](test-deliveries.md)
   * Acceso a los registros de los envíos de prueba enviados: [Más información](test-deliveries.md#access-test-deliveries)
   * Solo para correo electrónico, compruebe la renderización del contenido del mensaje en clientes de correo electrónico populares: [Más información](email-rendering.md)



