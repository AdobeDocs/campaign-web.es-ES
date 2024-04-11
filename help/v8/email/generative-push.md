---
audience: end-user
title: Notificación push con el asistente de IA en Campaign
description: Introducción al asistente de IA en Campaign
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: f249a73e25857e65e200f3cbd9516206aab918f9
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 9%

---

# Generación de notificaciones push con el asistente de IA {#generative-push}

>[!BEGINSHADEBOX]

**Tabla de contenido**

* [Introducción al asistente de IA](generative-gs.md)
* [Generación de correo electrónico con el asistente de IA](generative-content.md)
* [Generación de SMS con el asistente de IA](generative-sms.md)
* **[Generación de notificaciones push con el asistente de IA](generative-push.md)**

>[!ENDSHADEBOX]


El asistente de IA puede ayudarle a optimizar el impacto de sus envíos sugiriendo contenido diferente que es más probable que resuene en su audiencia.

Con el asistente de IA, el contenido se puede elevar a nuevas alturas. Por ejemplo, se puede utilizar para lo siguiente:

* **Resumir**: condense el contenido largo en resúmenes sucintos para las notificaciones push. Vaya directamente al grano y asegúrese de que los destinatarios capten el mensaje clave al instante.
* **Elaborado**: Amplíe los temas de las notificaciones push y proporcione detalles y contexto adicionales para una mejor comprensión.
* **Simplificar idioma**: haga que las notificaciones push sean accesibles para una audiencia más amplia utilizando un lenguaje claro y conciso.
* **Reformular**: evite la repetición haciendo que el asistente de IA reformule el mensaje de diferentes maneras
* **Cambiar tono**: cambie el tono emocional de las notificaciones push. Tanto si desea que suene informativo, lúdico o urgente, el asistente de IA puede adaptar el mensaje en consecuencia.

>[!NOTE]
>
>Antes de empezar a utilizar esta capacidad, lea la información relacionada [Protecciones y limitaciones](generative-gs.md#guardrails-and-limitations).

En el siguiente ejemplo, aprovecharemos el asistente de IA para crear mensajes atractivos para crear una experiencia del cliente más atractiva.

1. Después de crear y configurar la entrega de notificaciones push, haga clic en **[!UICONTROL Editar contenido]**.

   Para obtener más información sobre cómo configurar la entrega push, consulte [esta página](../push/create-push.md).

1. Rellene el **[!UICONTROL Detalles básicos]** para su envío. Una vez finalizado, haga clic en **[!UICONTROL Editar contenido]**.

1. Personalice la notificación push según sea necesario. [Más información](../push/content-push.md)

1. Acceda a la **[!UICONTROL Mostrar asistente de IA]** menú.

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. Ajuste el contenido describiendo lo que desea generar en la variable **[!UICONTROL Preguntar]** field.

   Si busca ayuda para crear el indicador, acceda al **[!UICONTROL Biblioteca de mensajes]** que proporciona una amplia gama de ideas rápidas para mejorar las entregas.

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. Habilite la **[!UICONTROL Mejorar con el contexto actual]** para que el asistente de IA personalice el nuevo contenido en función de su envío, nombre de envío y audiencia seleccionada.

   >[!IMPORTANT]
   >
   > El mensaje siempre debe estar vinculado a un contexto específico cargando un recurso de marca o habilitando **[!UICONTROL Mejora del contenido actual]** opción.

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. Seleccionar **[!UICONTROL Cargar recurso de marca]** para añadir cualquier recurso de marca que contenga contenido que pueda proporcionar contexto adicional, utilice el asistente de IA.

1. Elija el campo que desea generar: **[!UICONTROL Título]**, **[!UICONTROL Subtítulo]** o **[!UICONTROL Mensaje]**.

1. Seleccione el **[!UICONTROL Estrategia de comunicación]** que mejor se adapte a sus necesidades. Esto afectará al tono y al estilo del texto generado.

1. Elija la **[!UICONTROL Idioma]** y **[!UICONTROL Tono]** que desea que tenga el texto generado. Esto garantizará que el texto sea apropiado para su audiencia y propósito.

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. Una vez que la solicitud esté lista, haga clic en **[!UICONTROL Generar]**.

1. Examine el contenido generado **[!UICONTROL Variaciones]** y haga clic en **[!UICONTROL Aplicar]** una vez encontrado el contenido adecuado.

   Clic **[!UICONTROL Previsualizar]** para ver una versión en pantalla completa de la variación seleccionada.

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. Inserte campos de personalización para personalizar el contenido push en función de los datos de perfiles. [Más información sobre la personalización de contenido](../personalization/personalize.md)

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

1. Después de definir el contenido del mensaje, haga clic en **[!UICONTROL Simular contenido]** para controlar el procesamiento y comprobar la configuración de personalización con perfiles de prueba. [Más información](../preview-test/preview-content.md)

   ![](assets/push-genai-7.png){zoomable=&quot;yes&quot;}

1. Una vez definido el contenido, la audiencia y la programación, estará listo para preparar la entrega push. [Más información](../monitor/prepare-send.md)

