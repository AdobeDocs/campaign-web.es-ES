---
audience: end-user
title: Previsualización del contenido del correo electrónico
description: Obtenga información sobre cómo previsualizar el contenido del correo electrónico con la IU de la web de Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha" type="Positive"
source-git-commit: 6671d4c18da5655d67b9fd30c05fd2e9052d000b
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 28%

---


# Previsualización del contenido del correo electrónico {#preview-content}

Utilice el [!DNL Campaign] capacidad de simulación de contenido para previsualizar el contenido del correo electrónico antes de enviarlo. Esto permite controlar la personalización y comprobar cómo se muestra a los destinatarios.

Para previsualizar el contenido del correo electrónico, siga los pasos a continuación.

1. Navegar al correo electrónico [Editar contenido](../content/edit-content.md) o a la [Diseñador de correo electrónico](../content/get-started-email-designer.md).

1. Haga clic en **[!UICONTROL Simular contenido]** botón.

   ![](assets/simulate-button.png)

1. Utilice el **[!UICONTROL Añadir perfil(es) de prueba]** para seleccionar los perfiles que se utilizarán para previsualizar el contenido personalizado.

1. Puede combinar perfiles y perfiles de prueba para previsualizar el correo electrónico.

   * La pestaña **[!UICONTROL Perfiles de prueba]** incluye todas las direcciones semilla, que son destinatarios adicionales y ficticios de la base de datos.

     >[!NOTE]
     >
     >Los perfiles de prueba se pueden crear en [!DNL Campaign] consola en la **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Direcciones semilla]** carpeta. Obtenga más información en [Documentación de Campaign v8 (consola)](https://experienceleague.corp.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   * La pestaña **[!UICONTROL Perfiles]** incluye todos los destinatarios almacenados en la carpeta **[!UICONTROL Perfiles y destinatarios]** de la consola de [!DNL Campaign] [Más información](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}

   ![](assets/simulate-select-profiles.png)

1. Clic **[!UICONTROL Seleccionar]** para confirmar la selección en ambas pestañas.

   En el panel derecho del mensaje se muestra una vista previa del correo electrónico **[!UICONTROL Simular]** pantalla. Los elementos personalizados se sustituyen por los datos del perfil seleccionado en el panel izquierdo.

   ![](assets/simulate-preview.png)

1. Si ha añadido varios perfiles, puede cambiar entre ellos en la lista para obtener una vista previa del contenido de correo electrónico correspondiente. También puede agregar más perfiles de prueba y borrar la selección utilizando los botones correspondientes del panel izquierdo.

1. Puede ajustar la variable **[!UICONTROL Nivel de zoom]** y previsualice el contenido en el escritorio o dispositivo móvil mediante el icono dedicado en la esquina superior derecha.

1. Desde el **[!UICONTROL Simular]** pantalla también puede:
   * Compruebe el procesamiento de correo electrónico en clientes de correo electrónico populares: [Más información](email-rendering.md)
   * Envío de correos electrónicos de prueba a destinatarios específicos para su validación: [Más información](proofs.md)



