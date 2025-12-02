---
audience: end-user
title: Contenido generativo
description: Obtenga información sobre cómo generar imágenes con el asistente de IA
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 2%

---

# Generación de imágenes con el asistente de IA {#generative-image}

>[!IMPORTANT]
>
>Antes de empezar a usar esta capacidad, lea las [Protecciones y limitaciones](generative-gs.md#generative-guardrails) relacionadas.
></br>
>
>Debe aceptar un [acuerdo de usuario](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} antes de usar el Asistente de IA en Adobe Campaign Web. Para obtener más información, póngase en contacto con su representante Adobe.

Utilice el asistente de IA en Adobe Campaign Web para crear contenido visual atractivo que mejore los mensajes en el correo electrónico, las páginas de aterrizaje y las notificaciones push. El asistente de IA le ayuda a generar y optimizar imágenes, lo que garantiza que el contenido sea visualmente atractivo y esté alineado con la marca.

## Para correo electrónico y páginas de destino {#email-web-channels}

El asistente de IA puede generar experiencias visuales completas para sus envíos de correo electrónico y páginas de aterrizaje. Esta capacidad le permite producir imágenes de marca y que llamen la atención y que resuenen con la audiencia en puntos de contacto digitales.

### Acceso y configuración {#access-configure}

Para empezar a generar imágenes con el asistente de IA, primero configure la entrega y abra el editor de contenido. Siga los pasos a continuación para preparar su espacio de trabajo y acceder al panel Asistente de IA.

1. Cree y configure su envío:

   * **Correo electrónico**: Después de crear y configurar tu envío de correo electrónico, haz clic en **[!UICONTROL Editar contenido]**. [Más información](../email/create-email-content.md)
   * **Página de aterrizaje**: Después de crear y configurar la página de aterrizaje, haga clic en **[!UICONTROL Editar contenido]**. [Más información](../landing-pages/create-lp.md)

1. Seleccione el recurso que desea cambiar con el Asistente de IA y acceda al menú **[!UICONTROL Asistente de IA]**.

   ![Captura de pantalla que muestra la selección de componentes de texto en Adobe Campaign Web](assets/image-genai-1.png){zoomable="yes"}

### Generar contenido {#generate-content}

1. Habilite la opción **[!UICONTROL Estilo de referencia]** para que el Asistente de IA personalice el nuevo contenido en función del contenido seleccionado.

1. Seleccione su **[!UICONTROL marca]** para asegurarse de que el contenido generado por IA se ajuste a las especificaciones de su marca. [Más información](brands.md) sobre marcas.

1. Ajuste el contenido describiendo lo que desea generar en el campo **[!UICONTROL Preguntar]**.

   Si necesita ayuda para redactar el mensaje, acceda a la **[!UICONTROL Biblioteca de mensajes]**, que ofrece una amplia gama de ideas para mejorar los envíos. [Más información sobre las prácticas recomendadas para los mensajes](ai-assistant-prompting-guide.md)

   ![Captura de pantalla que muestra la biblioteca de mensajes para la generación de imágenes en Adobe Campaign Web](assets/image-genai-2.png){zoomable="yes"}

1. Adapte el mensaje utilizando la opción **[!UICONTROL Configuración de imagen]**:

   * **[!UICONTROL Proporción de aspecto]**: determine la anchura y la altura del recurso. Elija entre proporciones comunes, como 16:9, 4:3, 3:2 o 1:1, o indique un tamaño personalizado.
   * **[!UICONTROL Tipo de contenido]**: Categorice la naturaleza del elemento visual y distinga entre distintas formas de representación visual, como fotografías, gráficos o arte.
   * **[!UICONTROL Intensidad visual]**: controla el impacto de la imagen ajustando su intensidad. Un ajuste más bajo (2) crea un aspecto más suave, mientras que un ajuste más alto (10) hace que la imagen sea más vibrante.
   * **[!UICONTROL Color y tono]**: ajusta el aspecto general de los colores y el estado de ánimo o atmósfera transmitidos.
   * **[!UICONTROL Iluminación]**: modifique la iluminación de la imagen para dar forma a su atmósfera y resaltar elementos específicos.
   * **[!UICONTROL Composición]**: organice los elementos dentro del marco de la imagen.

     ![Captura de pantalla que muestra las opciones de configuración de imagen en Adobe Campaign Web](assets/image-genai-4.png){zoomable="yes"}

1. En el menú **[!UICONTROL Contenido de referencia]**, haga clic en **[!UICONTROL Cargar archivo]** para agregar cualquier recurso de marca que contenga contenido que pueda proporcionar un asistente de IA de contexto adicional o seleccione uno cargado anteriormente.

   Los archivos cargados anteriormente están disponibles en la lista desplegable **[!UICONTROL Contenido de referencia cargado]**. Simplemente, cambie los recursos que desee incluir en la generación.

1. Una vez que esté satisfecho con la configuración de la solicitud, haga clic en **[!UICONTROL Generar]**.

### Refinamiento y finalización {#refine-finalize}

Después de generar variaciones de imagen, puede revisar los resultados, comprobar la alineación de la marca y seleccionar la mejor opción para el contenido.

1. Examine las **[!UICONTROL variaciones]** generadas.

1. Haga clic en el icono de porcentaje para ver su **[!UICONTROL puntuación de alineación de marca]** e identificar cualquier desalineación con su marca.

   Más información sobre [puntuación de alineación de marca](../content/brands-score.md).

   ![](assets/image-genai-3.png){zoomable="yes"}

1. Haz clic en **[!UICONTROL Vista previa]** para ver una versión en pantalla completa de la variación seleccionada o en **[!UICONTROL Aplicar]** para reemplazar el contenido actual.

1. Elija **[!UICONTROL Generar]** similar si desea ver imágenes relacionadas con esta variante.

1. Abra la pestaña **[!UICONTROL Alineación de marca]** para ver cómo se ajusta su contenido a las [directrices de marca](../content/brands.md).

1. Haz clic en **[!UICONTROL Seleccionar]** cuando encuentres el contenido apropiado.

1. Después de definir el contenido del mensaje, haga clic en el botón **[!UICONTROL Simular contenido]** para controlar la representación y comprobar la configuración de personalización con perfiles de prueba. [Más información](../preview-test/preview-content.md)

1. Revise y active el contenido:
   * **Correo electrónico**: Una vez que haya definido el contenido, la audiencia y la programación, estará listo para preparar su envío de correo electrónico. [Más información](../monitor/prepare-send.md)
   * **Página de aterrizaje**: Una vez que la página de aterrizaje esté lista, puede publicarla para que esté disponible para usarla en un mensaje. [Más información](../landing-pages/create-lp.md)

## Para canales móviles {#mobile-channels}

El asistente de IA le permite generar imágenes atractivas para las notificaciones push, lo que le ayuda a crear comunicaciones móviles visualmente atractivas que capturan la atención y resuenan en su audiencia.

### Acceso y configuración {#mobile-access-configure}

Para empezar a generar imágenes para notificaciones push con el asistente de IA, configure primero el envío y abra el asistente de IA.

1. Después de crear y configurar su entrega de notificaciones push, haga clic en **[!UICONTROL Editar contenido]**. [Más información](../push/create-push.md)

1. Acceda al menú **[!UICONTROL Mostrar asistente de IA]**.

   ![Captura de pantalla que muestra el menú Mostrar asistente de IA](assets/push-img-1.png){zoomable="yes"}

### Generar contenido {#mobile-generate-content}

Después de acceder a AI Assistant, puede ajustar la configuración de generación para crear imágenes que se alineen con su marca y apoyen sus objetivos.

1. Seleccione su **[!UICONTROL marca]** para asegurarse de que el contenido generado por IA se ajuste a las especificaciones de su marca. [Más información](brands.md) sobre marcas.

1. Ajuste el contenido describiendo lo que desea generar en el campo **[!UICONTROL Preguntar]**.

   Si está buscando ayuda para crear su mensaje, acceda a la **[!UICONTROL Biblioteca de mensajes]**, que proporciona una amplia gama de ideas para mejorar sus campañas. [Más información sobre las prácticas recomendadas para los mensajes](ai-assistant-prompting-guide.md)

   ![Asistente de IA con campo de solicitud y opciones](assets/push-img-2.png){zoomable="yes"}

1. Seleccione **[!UICONTROL Image]** para generar solamente recursos.

1. Elija su **[!UICONTROL configuración de imagen]**:

   * **[!UICONTROL Tipo de contenido]**: Categorice la naturaleza del elemento visual y distinga entre distintas formas de representación visual, como fotografías, gráficos o arte.
   * **[!UICONTROL Intensidad visual]**: controla el impacto de la imagen ajustando su intensidad. Un ajuste más bajo (2) crea un aspecto más suave y restringido, mientras que un ajuste más alto (10) hace que la imagen sea más vibrante y visualmente potente.
   * **[!UICONTROL Iluminación]**: ajusta la iluminación de la imagen para dar forma a su atmósfera y resaltar elementos específicos.
   * **[!UICONTROL Composición]**: organice los elementos dentro del marco de la imagen.

     ![Captura de pantalla que muestra las opciones de configuración de imagen](assets/push-img-3.png){zoomable="yes"}

1. En el menú **[!UICONTROL Contenido de referencia]**, haga clic en **[!UICONTROL Cargar archivo]** para agregar cualquier recurso de marca que contenga contenido que pueda proporcionar un asistente de IA de contexto adicional o seleccione uno cargado anteriormente.

   Los archivos cargados anteriormente están disponibles en la lista desplegable **[!UICONTROL Contenido de referencia cargado]**. Simplemente, cambie los recursos que desee incluir en la generación.

1. Una vez que la solicitud esté lista, haga clic en **[!UICONTROL Generar]**.

### Refinamiento y finalización {#mobile-refine-finalize}

Después de generar variaciones de imagen para los mensajes móviles, puede ajustar los resultados para asegurarse de que cumplen con sus requisitos exactos.

1. Después de la generación, examine **[!UICONTROL Variaciones]**.

1. Haga clic en el icono de porcentaje para ver su **[!UICONTROL puntuación de alineación de marca]** e identificar cualquier desalineación con su marca.

   Más información sobre [puntuación de alineación de marca](../content/brands-score.md).

   ![](assets/push-img-4.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Vista previa]** para examinar las **[!UICONTROL variaciones]**.

1. Abra la pestaña **[!UICONTROL Alineación de marca]** para ver cómo se ajusta su contenido a las [directrices de marca](brands.md).

1. Haga clic en **[!UICONTROL Seleccionar]** cuando encuentre el contenido apropiado.

Una vez definido el contenido, la audiencia y la programación, prepare la entrega push. [Más información](../monitor/prepare-send.md)
