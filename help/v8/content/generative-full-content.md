---
audience: end-user
title: Contenido generativo
description: Obtenga información sobre cómo generar experiencias de contenido completas con AI Assistant en Journey Optimizer.
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1606'
ht-degree: 1%

---

# Generar contenido completo con el asistente de IA {#generative-full-content}

>[!IMPORTANT]
>
>Antes de empezar a usar esta capacidad, lea las [Protecciones y limitaciones](generative-gs.md#generative-guardrails) relacionadas.
></br>
>
>Debe aceptar un [acuerdo de usuario](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} antes de usar el Asistente de IA en Adobe Campaign Web. Para obtener más información, póngase en contacto con su representante Adobe.

Utilice el asistente de IA en la web de Adobe Campaign para generar experiencias de contenido completas en el correo electrónico, las páginas de aterrizaje y los canales de notificaciones push. El asistente de IA le ayuda a optimizar el impacto de sus envíos mediante la creación de contenido completo que resuene en su audiencia.

## Para correo electrónico y página de aterrizaje {#email-web-channels}

El asistente de IA puede producir experiencias de contenido completas para sus envíos de correo electrónico y páginas de aterrizaje, lo que genera texto e imágenes. Esta sólida funcionalidad le ayuda a crear contenido atractivo y de marca que se conecta con su audiencia en todos los puntos de contacto digitales.

### Acceso y configuración {#access-configure}

Antes de empezar a crear contenido con el asistente de IA, debe configurar la entrega y abrir el editor de contenido. Siga los pasos a continuación para preparar su espacio de trabajo y acceder al panel Asistente de IA.

1. Cree y configure su envío:

   * **Correo electrónico**: Después de crear y configurar tu envío de correo electrónico, haz clic en **[!UICONTROL Editar contenido]**. [Más información](../email/create-email-content.md)
   * **Página de aterrizaje**: Después de crear y configurar la página de aterrizaje, haga clic en **[!UICONTROL Editar contenido]**. [Más información](../landing-pages/create-lp.md)

1. Personalice el diseño según sea necesario y acceda al menú **[!UICONTROL Asistente de IA]**.

   ![Panel del asistente de IA que muestra la selección de marca y el campo de solicitud](assets/full-email-1.png){zoomable="yes"}

### Generar contenido {#generate-content}

Con el Asistente de IA abierto, ahora puede configurar los ajustes de generación para crear contenido que coincida con sus objetivos de marca y campaña. Personalice los parámetros de texto e imagen, añada recursos de marca y proporcione indicadores para guiar la IA en la generación de variaciones relevantes para su audiencia.

1. Seleccione su **[!UICONTROL marca]** para asegurarse de que el contenido generado por IA se ajuste a las especificaciones de su marca. [Más información](brands.md) sobre marcas.

1. Ajuste el contenido describiendo lo que desea generar en el campo **[!UICONTROL Preguntar]**.

   Si necesita ayuda para redactar el mensaje, acceda a la **[!UICONTROL Biblioteca de mensajes]**, que ofrece una amplia gama de ideas para mejorar los envíos. [Más información sobre las prácticas recomendadas para los mensajes](ai-assistant-prompting-guide.md)

   ![Captura de pantalla que muestra la biblioteca de mensajes en Adobe Campaign Web](assets/full-email-2.png){zoomable="yes"}

1. **Para correos electrónicos**, puede alternar las opciones **[!UICONTROL Línea de asunto]** y **[!UICONTROL Encabezado previo]** para incluirlas en la generación de variante.

1. Adapte el mensaje utilizando la opción **[!UICONTROL Configuración de texto]**:

   * **[!UICONTROL Estrategia de comunicación]**: elige el estilo de comunicación más adecuado para el texto generado.
   * **[!UICONTROL Idiomas]**: elige el idioma del contenido generado.
   * **[!UICONTROL Tono]**: Asegúrese de que el tono del correo electrónico resuene en la audiencia. Tanto si desea sonar informativo, lúdico o persuasivo, AI Assistant adapta el mensaje en consecuencia.

     ![Captura de pantalla que muestra las opciones de configuración de texto en Adobe Campaign Web](assets/full-email-4.png){zoomable="yes"}

1. Elija su **[!UICONTROL configuración de imagen]**:

   * **[!UICONTROL Tipo de contenido]**: Categorice la naturaleza del elemento visual y distinga entre distintas formas de representación visual, como fotografías, gráficos o arte.
   * **[!UICONTROL Intensidad visual]**: controla el impacto de la imagen ajustando su intensidad. Un ajuste más bajo (2) crea un aspecto más suave, mientras que un ajuste más alto (10) hace que la imagen sea más vibrante.
   * **[!UICONTROL Color y tono]**: ajusta el aspecto general de los colores y el estado de ánimo o atmósfera transmitidos.
   * **[!UICONTROL Iluminación]**: modifique la iluminación de la imagen para dar forma a su atmósfera y resaltar elementos específicos.
   * **[!UICONTROL Composición]**: organice los elementos dentro del marco de la imagen.

1. En el menú **[!UICONTROL Contenido de referencia]**, haga clic en **[!UICONTROL Cargar archivo]** para agregar cualquier recurso de marca que contenga contenido que pueda proporcionar un asistente de IA de contexto adicional o seleccione uno cargado anteriormente.

   Los archivos cargados anteriormente están disponibles en la lista desplegable **[!UICONTROL Contenido de referencia cargado]**. Simplemente, cambie los recursos que desee incluir en la generación.

   ![Captura de pantalla que muestra las opciones de configuración de marcas en Adobe Campaign Web](assets/full-email-3.png){zoomable="yes"}

1. Una vez que la solicitud esté lista, haga clic en **[!UICONTROL Generar]**.

### Refinamiento y finalización {#refine-finalize}

Después de generar variaciones de contenido, puede ajustar los resultados para asegurarse de que cumplan con sus requisitos exactos. Revise la alineación de la marca, ajuste el tono y el idioma, y prepare el contenido para su activación en la entrega.

1. Después de la generación, examine **[!UICONTROL Variaciones]**.

1. Haga clic en el icono de porcentaje para ver su **[!UICONTROL puntuación de alineación de marca]** e identificar cualquier desalineación con su marca.

   Más información sobre [puntuación de alineación de marca](brands-score.md).

   ![](assets/full-email-7.png){zoomable="yes"}

1. Haz clic en **[!UICONTROL Vista previa]** para ver una versión en pantalla completa de la variación seleccionada o en **[!UICONTROL Aplicar]** para reemplazar el contenido actual.

1. Vaya a la opción **[!UICONTROL Refinar]** en la ventana de **[!UICONTROL vista previa]** para obtener acceso a características de personalización adicionales:

   * **[!UICONTROL Reformular]**: vuelva a escribir el mensaje conservando su significado. Esta opción le ayuda a generar frases alternativas, mejorar el flujo o ajustar el estilo sin cambiar el mensaje principal.

   * **[!UICONTROL Use un lenguaje más sencillo]**: aproveche el Asistente para IA a fin de simplificar su lenguaje y garantizar la claridad y accesibilidad para una audiencia más amplia.

   * **[!UICONTROL Traducir]**: Simplifique su idioma para garantizar la claridad y accesibilidad para una audiencia más amplia.

   * **[!UICONTROL Cambiar tono]**: Ajuste el tono del mensaje para que coincida mejor con su estilo de comunicación, es decir, para que sea más amable, profesional, urgente o inspirador.

   * **[!UICONTROL Cambiar estrategia de comunicación]**: modifique el enfoque de mensajería en función de sus objetivos, como crear urgencia o enfatizar atractivo interesante.

     ![Refinar menú que muestra opciones](assets/full-email-5.png){zoomable="yes"}

1. Abra la pestaña **[!UICONTROL Alineación de marca]** para ver cómo se ajusta su contenido a las [directrices de marca](brands.md).

1. Haga clic en **[!UICONTROL Seleccionar]** cuando encuentre el contenido apropiado.

1. Inserte campos de personalización para personalizar el contenido en función de los datos de perfiles. A continuación, haga clic en el botón **[!UICONTROL Simular contenido]** para controlar la renderización y compruebe la configuración de personalización con perfiles de prueba. [Más información](../preview-test/preview-content.md)

1. Revise y active el contenido:
   * **Correo electrónico**: Una vez que haya definido el contenido, la audiencia y la programación, estará listo para preparar su envío de correo electrónico. [Más información](../monitor/prepare-send.md)
   * **Página de aterrizaje**: Una vez que la página de aterrizaje esté lista, puede publicarla para que esté disponible para usarla en un mensaje. [Más información](../landing-pages/create-lp.md)

## Para canales móviles {#mobile-channels}

AI Assistant también admite la generación de contenido para notificaciones push móviles, lo que le permite crear títulos, mensajes e imágenes atractivos para sus aplicaciones móviles. Esto le ayuda a mantener una comunicación coherente y de alta calidad en todos los puntos de contacto de los clientes, incluido el móvil.

### Acceso y configuración {#mobile-access-configure}

Para utilizar el asistente de IA para notificaciones push, configure primero la entrega push y abra el editor de contenido. Los pasos siguientes le guiarán a través de la preparación de su envío y el acceso a las herramientas del asistente de IA.

1. Después de crear y configurar su entrega de notificaciones push, haga clic en **[!UICONTROL Editar contenido]**.

   Para obtener más información sobre la configuración de su envío push, consulte [esta página](../push/create-push.md).

1. Personalice la notificación push según sea necesario. [Más información](../push/content-push.md)

1. Acceda al menú **[!UICONTROL Mostrar asistente de IA]**.

   ![Captura de pantalla que muestra el menú Mostrar asistente de IA](assets/push-genai-1.png){zoomable="yes"}

### Generar contenido {#mobile-generate-content}

Una vez que haya accedido al asistente de IA para notificaciones push, puede configurar los ajustes de generación para crear contenido móvil atractivo. Defina sus preferencias de texto e imagen, seleccione recursos de marca y utilice mensajes para generar variaciones de notificaciones push que involucren a los usuarios móviles.

1. Seleccione su **[!UICONTROL marca]** para asegurarse de que el contenido generado por IA se ajuste a las especificaciones de su marca. [Más información](brands.md) sobre marcas.

1. Ajuste el contenido describiendo lo que desea generar en el campo **[!UICONTROL Preguntar]**.

   Si está buscando ayuda para redactar el mensaje, acceda a la **[!UICONTROL Biblioteca de mensajes]**, que proporciona una amplia gama de ideas para mejorar su envío. [Más información sobre las prácticas recomendadas para los mensajes](ai-assistant-prompting-guide.md)

   ![Asistente de IA con campo de solicitud y opciones](assets/push-genai-2.png){zoomable="yes"}

1. Elija el campo que desea generar: **[!UICONTROL Título]**, **[!UICONTROL Subtítulo]**, **[!UICONTROL Mensaje]** y/o **[!UICONTROL Imagen]**.

1. Adapte el mensaje con la opción **[!UICONTROL Configuración de texto]**:

   * **[!UICONTROL Estrategia de comunicación]**: elige el estilo de comunicación más adecuado para el texto generado.
   * **[!UICONTROL Idiomas]**: elige el idioma del contenido generado.
   * **[!UICONTROL Tono]**: el tono de las notificaciones push debería interesar a la audiencia. Tanto si desea sonar informativo, lúdico o persuasivo, el asistente de IA puede adaptar el mensaje en consecuencia.

     ![Panel de configuración de texto para notificaciones push](assets/push-genai-3.png){zoomable="yes"}

1. Elija su **[!UICONTROL configuración de imagen]**:

   * **[!UICONTROL Tipo de contenido]**: Categorice la naturaleza del elemento visual y distinga entre distintas formas de representación visual, como fotografías, gráficos o arte.
   * **[!UICONTROL Intensidad visual]**: controla el impacto de la imagen ajustando su intensidad. Un ajuste más bajo (2) crea un aspecto más suave y restringido, mientras que un ajuste más alto (10) hace que la imagen sea más vibrante y visualmente potente.
   * **[!UICONTROL Iluminación]**: ajusta la iluminación de la imagen para dar forma a su atmósfera y resaltar elementos específicos.
   * **[!UICONTROL Composición]**: organice los elementos dentro del marco de la imagen.

     ![Configuración de imagen para notificaciones push](assets/push-genai-4.png){zoomable="yes"}

1. En el menú **[!UICONTROL Contenido de referencia]**, haga clic en **[!UICONTROL Cargar archivo]** para agregar cualquier recurso de marca que contenga contenido que pueda proporcionar un asistente de IA de contexto adicional o seleccione uno cargado anteriormente.

   Los archivos cargados anteriormente están disponibles en la lista desplegable **[!UICONTROL Contenido de referencia cargado]**. Simplemente, cambie los recursos que desee incluir en la generación.

1. Una vez que la solicitud esté lista, haga clic en **[!UICONTROL Generar]**.

### Refinamiento y finalización {#mobile-refine-finalize}

Después de revisar las variaciones de notificaciones push generadas, puede pulir el contenido a la perfección. Utilice herramientas de refinamiento para ajustar el idioma y el tono, verificar la alineación de la marca y personalizar el contenido antes de activar la campaña push.

1. Examine las **[!UICONTROL variaciones]** generadas.

1. Haga clic en el icono de porcentaje para ver su **[!UICONTROL puntuación de alineación de marca]** e identificar cualquier desalineación con su marca.

   Más información sobre [puntuación de alineación de marca](brands-score.md).

   ![Variaciones de notificaciones push generadas con puntuación de alineación de marca](assets/push-genai-6.png){zoomable="yes"}

1. Haga clic en **[!UICONTROL Vista previa]** para ver una versión en pantalla completa de la variación seleccionada o haga clic en **[!UICONTROL Aplicar]** para reemplazar el contenido actual.

1. Vaya a la opción **[!UICONTROL Refinar]** en la ventana de **[!UICONTROL vista previa]** para obtener acceso a características de personalización adicionales:

   * **[!UICONTROL Usar como contenido de referencia]**: use la variante elegida como contenido de referencia para generar otros resultados.
   * **[!UICONTROL Reformular]**: reformula tu mensaje de diferentes maneras para mantener tu escritura fresca y atractiva para diversas audiencias.
   * **[!UICONTROL Use un lenguaje más sencillo]**: Simplifique su idioma para garantizar la claridad y accesibilidad para una audiencia más amplia.
   * **[!UICONTROL Traducir]**: Simplifique su idioma para garantizar la claridad y accesibilidad para una audiencia más amplia.

   También puedes cambiar el **[!UICONTROL tono]** y la **[!UICONTROL estrategia de comunicación]** de tu texto.

   ![Refinar opciones para notificaciones push](assets/push-genai-5.png){zoomable="yes"}

1. Abra la pestaña **[!UICONTROL Alineación de marca]** para ver cómo se ajusta su contenido a las [directrices de marca](brands.md).

1. Haga clic en **[!UICONTROL Seleccionar]** cuando encuentre el contenido apropiado.

1. Inserte campos de personalización para personalizar el contenido del correo electrónico en función de los datos del perfil. A continuación, haga clic en el botón **[!UICONTROL Simular contenido]** para controlar la renderización y comprobar la configuración de personalización con perfiles de prueba. [Más información](../preview-test/preview-content.md)

Al definir el contenido, la audiencia y la programación, prepare su envío push. [Más información](../monitor/prepare-send.md)

## Vídeos explicativos {#video}

Aprenda a utilizar el asistente de IA para generar contenido, texto e imágenes completos de correo electrónico.

>[!VIDEO](https://video.tv.adobe.com/v/3428984)