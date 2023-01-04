---
audience: end-user
title: Añadir una audiencia
description: Documentación web de Campaign v8
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: a572ac51db2ef79dc45afe2504aeb8476314bbfc
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 5%

---

# Seleccionar una audiencia {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Seleccionar una audiencia existente"
>abstract="Las audiencias se definen en la consola Adobe Campaign v8. Si tiene una integración de Adobe Experience Platform disponible, también debería poder ver las audiencias definidas por Platform."

>[!NOTE]
>
>Esta documentación está en construcción y se actualiza con frecuencia. La versión final de este contenido estará lista en enero de 2023.

En esta sección se explica cómo seleccionar una audiencia existente al definir la población objetivo de una entrega de correo electrónico. Si desea crear una audiencia nueva, consulte esta [sección](segment-builder.md).

1. En el **Audiencia** del asistente de creación de envíos, haga clic en el botón **[!UICONTROL Seleccionar la audiencia]** botón.

   ![](assets/create-audience.png)

1. Choose **[!UICONTROL Seleccionar la audiencia]** para usar una audiencia existente. Para crear una nueva audiencia para usarla en este correo electrónico, elija **Cree sus propios**. Consulte esta [sección](segment-builder.md).

   Esta pantalla muestra todas las audiencias existentes definidas en la consola de Adobe Campaign o en Adobe Experience Platform.

   ![](assets/create-audience2.png)

1. Elija una audiencia y haga clic en **Select**.

1. Haga clic en **Editar reglas** si desea restringir la audiencia.

   ![](assets/create-audience3.png)

1. Con el generador de segmentos, puede enriquecer la audiencia con filtros adicionales o combinando distintas audiencias. Consulte esta [sección](segment-builder.md).

   ![](assets/create-audience4.png)

1. Haga clic en **Save**.

También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibirá el mensaje. Esto le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de contactos que no lo hicieron. Consulte [sección](control-group.md).