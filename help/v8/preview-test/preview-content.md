---
audience: end-user
title: Previsualización del contenido de envío
description: Obtenga información sobre cómo previsualizar el contenido de la entrega con la interfaz de usuario web de Campaign
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 1%

---

# Vista previa del contenido del mensaje. {#preview-content}

Utilice la funcionalidad de simulación de contenido [!DNL Campaign] para obtener una vista previa del contenido del mensaje antes de enviarlo. Esta función le permite controlar la personalización y comprobar cómo se muestra el mensaje a los destinatarios.

Para obtener una vista previa del contenido del envío, siga estos pasos:

1. Vaya a la pantalla de edición de contenido de su envío o a [Email Designer](../email/get-started-email-designer.md).

1. Haga clic en el botón **[!UICONTROL Simular contenido]**.

   ![Imagen que muestra el botón Simular contenido](assets/simulate-button.png){zoomable="yes"}

1. Seleccione los perfiles que desea utilizar para obtener una vista previa del contenido. Para realizar esta acción, haga clic en el botón **[!UICONTROL Agregar perfiles de prueba]** (para correo electrónico y SMS) o en el botón **[!UICONTROL Agregar suscriptores]** (para notificaciones push).

1. Combine perfiles y perfiles de prueba para previsualizar el mensaje de correo electrónico o SMS.

   * La ficha **[!UICONTROL Perfiles de prueba]** enumera todos los perfiles de prueba, que son destinatarios adicionales y ficticios de la base de datos. [Aprenda a trabajar con perfiles de prueba](../audience/test-profiles.md).

   * La ficha **[!UICONTROL Perfiles]** enumera todos los perfiles almacenados en la base de datos. [Aprenda a trabajar con perfiles](../audience/about-recipients.md).

   ![Imagen que muestra la selección de perfiles](assets/simulate-select-profiles.png){zoomable="yes"}

1. Al examinar el perfil de prueba o las listas de perfiles, utilice filtros para restringir la búsqueda. Por ejemplo, defina una regla para buscar todos los perfiles de prueba con el estado **[!UICONTROL Candidato]**. [Aprenda a agregar reglas mediante el modelador de consultas](../query/query-modeler-overview.md).

   ![Imagen que muestra filtros aplicados a perfiles de prueba](assets/simulate-test-profile-filter.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Seleccionar]** para confirmar la selección.

   Aparecerá una vista previa del contenido de la entrega en el panel derecho de la pantalla **[!UICONTROL Simular]**. Los elementos personalizados se sustituyen por los datos del perfil seleccionado en el panel izquierdo.

   ![Imagen que muestra la vista previa del contenido del envío](assets/simulate-preview.png){zoomable="yes"}

1. Si se añaden varios perfiles, cambie entre ellos en la lista para previsualizar el contenido de envío correspondiente. Añada más perfiles de prueba o borre la selección utilizando los botones correspondientes del panel izquierdo.

1. Para las entregas por correo electrónico, ajusta el **[!UICONTROL nivel de zoom]** y previsualiza el contenido en un equipo de escritorio o dispositivo móvil mediante el icono dedicado en la esquina superior derecha.

1. En la pantalla **[!UICONTROL Simular]**, también puede:
   * Enviar pruebas a destinatarios específicos para su validación: [Más información](test-deliveries.md).
   * Acceda a los registros de las pruebas enviadas: [Más información](test-deliveries.md#access-test-deliveries).
   * Solo para correo electrónico, compruebe la representación del contenido del mensaje en clientes de correo electrónico populares: [Más información](email-rendering.md).