---
audience: end-user
title: Notificación push con el asistente de IA
description: Introducción al Asistente de IA
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 2%

---

# Generación de notificaciones push con el asistente de IA {#generative-push}

>[!IMPORTANT]
>
>Antes de empezar a usar esta capacidad, lea las [Protecciones y limitaciones](generative-gs.md#generative-guardrails) relacionadas.
>&#x200B;></br>
>
>Debe aceptar un [acuerdo de usuario](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) antes de usar el Asistente de IA en Adobe Campaign Web. Para obtener más información, póngase en contacto con su representante Adobe.

El asistente de IA ayuda a optimizar el impacto de las entregas sugiriendo contenido diferente que resuene en la audiencia.

En el siguiente ejemplo, el asistente de IA se aprovecha para crear mensajes atractivos para crear una experiencia del cliente más atractiva.

1. Después de crear y configurar su entrega de notificaciones push, haga clic en **[!UICONTROL Editar contenido]**.

   Para obtener más información sobre la configuración de su envío push, consulte [esta página](../push/create-push.md).

1. Acceda al menú **[!UICONTROL Mostrar asistente de IA]**.

   ![Captura de pantalla que muestra el menú Mostrar asistente de IA](assets/push-genai-1.png){zoomable="yes"}

1. Habilite la opción **[!UICONTROL Usar contenido original]** para el asistente de IA a fin de personalizar el nuevo contenido en función del contenido seleccionado.

1. Ajuste el contenido describiendo lo que desea generar en el campo **[!UICONTROL Preguntar]**.

   Si necesita ayuda para redactar el mensaje, acceda a la **[!UICONTROL Biblioteca de mensajes]**, que ofrece una amplia gama de ideas para mejorar los envíos.

   ![Captura de pantalla que muestra la interfaz de la biblioteca Prompt](assets/push-genai-2.png){zoomable="yes"}

1. Elija el campo que desea generar: **[!UICONTROL Título]**, **[!UICONTROL Subtítulo]**, **[!UICONTROL Mensaje]** o **[!UICONTROL Imagen]**.

1. Adapte el mensaje utilizando la opción **[!UICONTROL Configuración de texto]**:

   * **[!UICONTROL Estrategia de comunicación]**: elige el estilo de comunicación más adecuado para el texto generado.
   * **[!UICONTROL Tono]**: ajusta el tono de tu correo electrónico para que resuene en tu audiencia. Tanto si desea sonar informativo, lúdico o persuasivo, AI Assistant adapta el mensaje en consecuencia.

   ![Captura de pantalla que muestra las opciones de configuración de texto](assets/push-genai-3.png){zoomable="yes"}

1. Elija su **[!UICONTROL configuración de imagen]**:

   * **[!UICONTROL Tipo de contenido]**: Categorice la naturaleza del elemento visual y distinga entre distintas formas de representación visual, como fotografías, gráficos o arte.
   * **[!UICONTROL Intensidad visual]**: controla el impacto de la imagen ajustando su intensidad. Un ajuste más bajo (2) crea un aspecto más suave y restringido, mientras que un ajuste más alto (10) hace que la imagen sea más vibrante y visualmente potente.
   * **[!UICONTROL Iluminación]**: ajusta la iluminación de la imagen para dar forma a su atmósfera y resaltar elementos específicos.
   * **[!UICONTROL Composición]**: organice los elementos dentro del marco de la imagen.

   ![Captura de pantalla que muestra las opciones de configuración de imagen](assets/push-genai-4.png){zoomable="yes"}

1. En el menú **[!UICONTROL Brand assets]**, haga clic en **[!UICONTROL Cargar recurso de marca]** para agregar cualquier recurso de marca que contenga contenido que proporcione contexto adicional al Asistente de IA o seleccione uno cargado anteriormente.

   Los archivos cargados anteriormente están disponibles en la lista desplegable **[!UICONTROL Recursos de marca cargados]**. Cambie los recursos que desee incluir en la generación.

1. Una vez que la solicitud esté lista, haga clic en **[!UICONTROL Generar]**.

1. Examine las **[!UICONTROL variaciones]** generadas y haga clic en **[!UICONTROL Vista previa]** para ver una versión en pantalla completa de la variación seleccionada o en **[!UICONTROL Aplicar]** para reemplazar el contenido actual.

1. Haga clic en el icono de porcentaje para ver su **[!UICONTROL puntuación de alineación de marca]** e identificar cualquier desalineación con su marca.

   Más información sobre [puntuación de alineación de marca](../content/brands-score.md).

   ![](assets/push-genai-6.png){zoomable="yes"}

1. Vaya a la opción **[!UICONTROL Refinar]** en la ventana de **[!UICONTROL vista previa]** para obtener acceso a características de personalización adicionales:

   * **[!UICONTROL Usar como contenido de referencia]**: use la variante elegida como contenido de referencia para generar otros resultados.
   * **[!UICONTROL Reformular]**: reformula tu mensaje de diferentes maneras para mantener tu escritura fresca y atractiva para diversas audiencias.
   * **[!UICONTROL Use un lenguaje más sencillo]**: Simplifique su idioma para garantizar la claridad y accesibilidad para una audiencia más amplia.

   También puedes cambiar el **[!UICONTROL tono]** y la **[!UICONTROL estrategia de comunicación]** de tu texto.

   ![Captura de pantalla que muestra las opciones de refinamiento](assets/push-genai-5.png){zoomable="yes"}

1. Abra la pestaña **[!UICONTROL Alineación de marca]** para ver cómo se ajusta su contenido a las [directrices de marca](../content/brands.md).

1. Haz clic en **[!UICONTROL Seleccionar]** cuando encuentres el contenido apropiado.

1. Inserte campos de personalización para personalizar el contenido del correo electrónico en función de los datos del perfil. A continuación, haga clic en el botón **[!UICONTROL Simular contenido]** para controlar la renderización y comprobar la configuración de personalización con perfiles de prueba. [Más información](../preview-test/preview-content.md)

Al definir el contenido, la audiencia y la programación, prepare su envío push. [Más información](../monitor/prepare-send.md)