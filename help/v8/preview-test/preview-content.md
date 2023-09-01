---
audience: end-user
title: Previsualización del contenido de envío
description: Obtenga información sobre cómo previsualizar el contenido de la entrega con la IU web de Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Beta"
source-git-commit: 95d44fa2c44a346aad3aab1962e84917532cc966
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 10%

---


# Previsualización del contenido de envío {#preview-content}

Utilice el [!DNL Campaign] capacidad de simulación de contenido para previsualizar el contenido del mensaje antes de enviarlo. Esto permite controlar la personalización y comprobar cómo se muestra a los destinatarios.

Para obtener una vista previa del contenido del envío, siga los pasos a continuación.

1. Vaya a la pantalla de edición de contenido del envío.

   <!--email [Edit content](../content/edit-content.md) screen or to the [Email Designer](../content/get-started-email-designer.md).-->

1. Haga clic en **[!UICONTROL Simular contenido]** botón.

   ![](assets/simulate-button.png)

1. Para seleccionar los perfiles que se utilizarán para previsualizar el contenido personalizado, utilice:

   * **[!UICONTROL Añadir perfil(es) de prueba]** para previsualizar envíos de correo electrónico y SMS

   * **[!UICONTROL Añadir suscriptor(es)]** para previsualizar notificaciones push

1. Puede combinar perfiles y perfiles de prueba para previsualizar el mensaje de correo electrónico o SMS.

   * La pestaña **[!UICONTROL Perfiles de prueba]** incluye todas las direcciones semilla, que son destinatarios adicionales y ficticios de la base de datos.

     >[!NOTE]
     >
     >Los perfiles de prueba se pueden crear en [!DNL Campaign] consola en la **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Direcciones semilla]** carpeta. Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.

   * La pestaña **[!UICONTROL Perfiles]** incluye todos los destinatarios almacenados en la carpeta **[!UICONTROL Perfiles y destinatarios]** de la consola de [!DNL Campaign] Obtenga más información en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}.

   ![](assets/simulate-select-profiles.png)

1. Clic **[!UICONTROL Seleccionar]** para confirmar la selección.

   En el panel derecho del formulario se muestra una vista previa del contenido de la entrega **[!UICONTROL Simular]** pantalla. Los elementos personalizados se sustituyen por los datos del perfil seleccionado en el panel izquierdo.

   ![](assets/simulate-preview.png)

1. Si ha añadido varios perfiles, puede cambiar entre ellos en la lista para previsualizar el contenido de envío correspondiente. También puede agregar más perfiles de prueba y borrar la selección utilizando los botones correspondientes del panel izquierdo.

1. Para las entregas por correo electrónico, puede ajustar la **[!UICONTROL Nivel de zoom]** y previsualice el contenido en el escritorio o dispositivo móvil mediante el icono dedicado en la esquina superior derecha.

1. Desde el **[!UICONTROL Simular]** pantalla también puede:
   * Envío de entregas de prueba a destinatarios específicos para su validación: [Más información](test-deliveries.md)
   * Acceso a los registros de los envíos de prueba enviados: [Más información](test-deliveries.md#access-proofs)
   * Solo para correo electrónico, compruebe la renderización del contenido del mensaje en clientes de correo electrónico populares: [Más información](email-rendering.md)



