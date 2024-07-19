---
audience: end-user
title: Previsualización del contenido de envío
description: Obtenga información sobre cómo previsualizar el contenido de la entrega con la interfaz de usuario web de Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 1%

---


# Vista previa del contenido del mensaje. {#preview-content}

Utilice la funcionalidad de simulación de contenido [!DNL Campaign] para obtener una vista previa del contenido del mensaje antes de enviarlo. Esto permite controlar la personalización y comprobar cómo se muestra a los destinatarios.

Para obtener una vista previa del contenido del envío, siga los pasos a continuación.

1. Vaya a la pantalla de edición de contenido de su envío o a [Email Designer](../email/get-started-email-designer.md).

1. Haga clic en el botón **[!UICONTROL Simular contenido]**.

   ![](assets/simulate-button.png){zoomable="yes"}

1. Seleccione los perfiles que desea utilizar para previsualizar el contenido. Para ello, haga clic en el botón **[!UICONTROL Agregar perfil(es) de prueba]** (para correo electrónico y SMS) o en el botón **[!UICONTROL Agregar suscriptor(es)]** (para notificaciones push).

1. Puede combinar perfiles y perfiles de prueba para previsualizar el mensaje de correo electrónico o SMS.

   * La ficha **[!UICONTROL Perfiles de prueba]** enumera todos los perfiles de prueba, que son destinatarios adicionales y ficticios de la base de datos. [Aprenda a trabajar con perfiles de prueba](../audience/test-profiles.md)

   * La ficha **[!UICONTROL Perfiles]** enumera todos los perfiles almacenados en la base de datos. [Aprenda a trabajar con perfiles](../audience/about-recipients.md)

   ![](assets/simulate-select-profiles.png){zoomable="yes"}

1. Al examinar el perfil de prueba o las listas de perfiles, puede utilizar filtros para restringir la búsqueda. Por ejemplo, puede definir una regla para buscar todos los perfiles de prueba con el estado **[!UICONTROL Candidato]**. [Aprenda a agregar reglas mediante el modelador de consultas](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Seleccionar]** para confirmar la selección.

   Se mostrará una vista previa del contenido de la entrega en el panel derecho de la pantalla **[!UICONTROL Simular]**. Los elementos personalizados se sustituyen por los datos del perfil seleccionado en el panel izquierdo.

   ![](assets/simulate-preview.png){zoomable="yes"}

1. Si ha añadido varios perfiles, puede cambiar entre ellos en la lista para previsualizar el contenido de envío correspondiente. También puede agregar más perfiles de prueba y borrar la selección utilizando los botones correspondientes del panel izquierdo.

1. Para las entregas por correo electrónico, puede ajustar el **[!UICONTROL nivel de zoom]** y previsualizar el contenido en el escritorio o en el dispositivo móvil mediante el icono dedicado en la esquina superior derecha.

1. Desde la pantalla **[!UICONTROL Simular]** también puede:
   * Enviar pruebas a destinatarios específicos para su validación: [Más información](test-deliveries.md)
   * Acceder a los registros de las pruebas enviadas: [Más información](test-deliveries.md#access-test-deliveries)
   * Solo para correo electrónico, compruebe la representación del contenido del mensaje en clientes de correo electrónico populares: [Más información](email-rendering.md)



