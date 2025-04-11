---
audience: end-user
title: Creación de una audiencia única para una entrega
description: Obtenga información sobre cómo crear una audiencia única para una entrega.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 13%

---

# Crear un público único {#one-time}

En esta sección se explica cómo crear una audiencia al crear una nueva entrega. En esta situación, los perfiles incluidos en la audiencia de envío se segmentan consultando la base de datos con el modelador de consultas. La audiencia resultante se utiliza una sola vez para este envío y no se guarda en la lista de audiencias.

Al definir el objetivo principal de una entrega, también puede:
* [Seleccione una audiencia existente](add-audience.md) de la lista **[!UICONTROL Audiencias]**.
* [Cargar una audiencia desde un archivo externo](file-audience.md) (solo para correos electrónicos).

Para crear una nueva audiencia única para una entrega, siga estos pasos:

1. En la sección **Público** del asistente de creación de envíos, haga clic en el botón **[!UICONTROL Seleccionar el público]**.

   [Captura de pantalla que muestra la sección Audiencia del asistente de creación de envíos con el botón Seleccionar audiencia resaltado](assets/segment-builder0.png){zoomable="yes"}

1. Seleccione **Crear su propio** para abrir el modelador de consultas. El modelador de consultas permite definir la población objetivo filtrando los datos contenidos en la base de datos. [Aprenda a utilizar el modelador de consultas](../query/query-modeler-overview.md).

   [Captura de pantalla que muestra la interfaz del modelador de consultas](assets/query-modeler.png){zoomable="yes"}

1. Una vez que la consulta esté lista, haga clic en **Confirmar** para usar la audiencia resultante como destinatario principal de la entrega.

   También puede establecer un grupo de control para medir el impacto de sus campañas. El grupo de control no recibe el mensaje. Esto le permite comparar el comportamiento de la población que recibió el mensaje con el comportamiento de los contactos que no lo hicieron. [Más información](control-group.md).