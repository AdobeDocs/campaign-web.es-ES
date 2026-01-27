---
audience: end-user
title: Creación de experimentos de contenido
description: Aprenda a crear experimentos de contenido en la web de Adobe Campaign
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '1121'
ht-degree: 2%

---

# Creación de experimentos de contenido {#content-experiment}

## Acerca de los experimentos de contenido {#about-content-experiment}

Los experimentos de contenido en la web de Adobe Campaign le permiten definir varias variantes de envío de pruebas A/B para medir cuál ofrece el mejor rendimiento para la audiencia de destino. Puede variar el contenido, el asunto o el remitente de la entrega para probar diferentes versiones y determinar qué variante produce los mejores resultados.

Puede realizar pruebas A/B en varios elementos de correo electrónico, como:

* **Línea de asunto**: pruebe distintas líneas de asunto de correo electrónico para ver cuál genera la tasa de apertura más alta
* **Nombre del remitente**: experimente con diferentes combinaciones de remitente
* **Contenido del cuerpo del correo electrónico**: cree varias versiones de contenido para identificar cuál ofrece la mejor tasa de pulsaciones

>[!NOTE]
>
>* Actualmente, los experimentos de contenido solo están disponibles para el canal de correo electrónico.
>* Las pruebas A/B no son compatibles con los mensajes transaccionales.
>* Máximo de 3 tratamientos (variantes) por experimento.

## Creación de un experimento de contenido {#create-content-experiment}

Para añadir un experimento de contenido a la entrega de correo electrónico, siga estos pasos:

1. Cree una entrega por correo electrónico o abra uno existente. [Aprenda a crear un correo electrónico](create-email.md)

1. En la página de propiedades de la entrega de correo electrónico, haga clic en el botón **[!UICONTROL Crear experimento]** ubicado en la sección **[!UICONTROL Contenido]**.

   ![Captura de pantalla que muestra el botón Crear experimento en las propiedades de correo electrónico](assets/ab-testing-1.png){zoomable="yes"}

## Configuración del experimento {#configure-experiment}

Configure el experimento mediante las siguientes secciones:

![Captura de pantalla que muestra la configuración del experimento](assets/ab-testing-2.png){zoomable="yes"}

### Configuración del público {#audience-settings}

Defina el porcentaje de la población objetivo que recibirá las variantes del experimento.

Introduzca un valor para establecer el tamaño de la audiencia. Representa la proporción de destinatarios que recibirán una de las variantes del experimento durante la fase de prueba.

* **Mínimo**: 1%
* **Máximo**: 100%
* **Predeterminado**: 10%

La audiencia restante (90 % de forma predeterminada) recibirá la variante ganadora una vez que finalice el experimento y se determine un ganador.

Por ejemplo, con una audiencia de 10 000 destinatarios y un tamaño de audiencia del 10 %, se seleccionarán aleatoriamente 1000 destinatarios para participar en el experimento. Los 9000 destinatarios restantes recibirán la variante ganadora una vez finalizado el experimento.

### Estrategia ganadora {#winning-strategy}

Seleccione la métrica que se utilizará para determinar la variante ganadora:

* **[!UICONTROL Mejor tasa de apertura]** (predeterminada): la variante con el porcentaje más alto de aperturas por correo electrónico gana
* **[!UICONTROL Mejor tasa de clics]**: la variante con el porcentaje más alto de clics en el correo electrónico gana
* **[!UICONTROL Tasa más baja de bajas]**: gana la variante con el porcentaje más bajo de bajas

El sistema realiza un seguimiento automático de estas métricas durante el experimento y calcula qué variante ofrece el mejor rendimiento según el criterio seleccionado.

### Método de envío ganador {#sending-method}

Defina cuánto tiempo debe ejecutarse el experimento y seleccione el método de envío:

1. Introduzca el valor de duración en horas. El experimento se ejecutará durante este período antes de determinar la variante ganadora.

   * **Mínimo**: 3 horas
   * **Máximo**: 240 horas (10 días)
   * **Predeterminado**: 24 horas

   >[!NOTE]
   >
   >Asegúrese de que la duración del experimento sea lo suficientemente larga como para recopilar datos significativos. Una duración corta puede no proporcionar suficiente relevancia estadística, especialmente para métricas como la tasa de pulsaciones que pueden tardar más en acumularse.

1. Elija cómo se debe enviar la variante ganadora a la población restante:

   * **[!UICONTROL Envío automático]** activado: el sistema envía automáticamente la variante ganadora a la audiencia restante una vez que finaliza el experimento.
   * Se desactivó el envío automático **[!UICONTROL 1&rbrace;: debe hacer clic manualmente en el botón]** Enviar **[!UICONTROL para enviar la variante ganadora después de revisar los resultados del experimento.]**

Si ninguna variante logra resultados significativamente mejores que las demás al final del experimento, el sistema envía la primera variante a la población restante. Consulte esta [sección](#send-deliveries).

## Definición de los tratamientos de contenido {#define-content}

Después de guardar la configuración del experimento, se crea un primer tratamiento de forma predeterminada. Ahora necesita añadir sus otros tratamientos (hasta tres) y definir su contenido específico.

1. En las propiedades de la entrega, haga clic en **[!UICONTROL Editar contenido]**. Los tratamientos se muestran en el lado izquierdo.

   ![Captura de pantalla que muestra el panel de experimentos de contenido](assets/ab-testing-3.png){zoomable="yes"}

1. Haga clic en el botón **[!UICONTROL Agregar tratamiento]** y defina su nombre. Repita esta operación para todos los tratamientos que necesite agregar. A continuación, puede cambiar su nombre, duplicarlos y eliminarlos.

1. Haga clic en cada tratamiento y personalice los siguientes elementos:

   * **Nombre del remitente**: personalice de quién parece proceder el correo electrónico
   * **Línea de asunto**: escriba una línea de asunto única para cada tratamiento
   * **Cuerpo del correo electrónico**: Diseñe distintas versiones del contenido con el Designer de correo electrónico

   ![Captura de pantalla que muestra varios tratamientos](assets/ab-testing-4.png){zoomable="yes"}

1. Para obtener una vista previa de cada tratamiento, haga clic en el mismo y luego en **[!UICONTROL Simular contenido]**.

## Inicie el experimento y supervise los resultados {#validate-start}

Una vez que haya definido todos los tratamientos de contenido, puede validar e iniciar el experimento.

1. En las propiedades de la entrega, haga clic en **[!UICONTROL Revisar y enviar]** y, a continuación, haga clic en **[!UICONTROL Preparar]**.

1. A continuación, haga clic en **[!UICONTROL Iniciar experimentación]** para iniciar la prueba A/B.

   ![Captura de pantalla que muestra el botón Iniciar experimentación](assets/ab-testing-5.png){zoomable="yes"}

1. Una vez que se esté ejecutando el experimento, monitorice las diferentes métricas que se muestran en el panel de envío.

Mientras se ejecuta el experimento, puede hacer clic en **[!UICONTROL Dejar de enviar]** para finalizar el experimento. También puedes decidir enviar manualmente antes del final del experimento haciendo clic en **[!UICONTROL Seleccionar y enviar al ganador]**.

>[!NOTE]
>
>Los resultados se actualizan casi en tiempo real a medida que los destinatarios interactúan con el correo electrónico. Sin embargo, es posible que los resultados tempranos no tengan relevancia estadística; se recomienda esperar hasta que la duración del experimento esté completa antes de tomar decisiones finales.

## Realización de las entregas {#send-deliveries}

El envío se puede realizar automática o manualmente, según lo que haya elegido en la configuración del **[!UICONTROL método de envío ganador]**. Consulte esta [sección](#sending-method).

### Envío automático {#automatic-sending}

Para el envío automático, el sistema analiza los resultados en función de su estrategia ganadora y determina el tratamiento ganador. El tratamiento ganador se envía automáticamente a la audiencia restante. Si no aparece ningún ganador claro, se elige la primera variante.

### Envío manual {#manual-sending}

Si configuraste el envío manual, revisa los resultados cuando finalice el experimento y haz clic en **[!UICONTROL Enviar]** para enviar el tratamiento ganador. Si no ha aparecido ningún ganador claro, el primer tratamiento se selecciona de forma predeterminada, pero puede elegir uno diferente.

## Ver resultados finales {#final-results}

Una vez finalizado el experimento y enviada la entrega por completo, puede acceder a informes completos:

1. En el panel de envío, haga clic en **[!UICONTROL Informes]**.

1. Vaya a la pestaña del informe **[!UICONTROL Experimentos]** para mostrar las métricas clave de rendimiento de cada tratamiento.

## Prácticas recomendadas {#best-practices}

Al crear experimentos de contenido, tenga en cuenta las siguientes recomendaciones:

* **Probar un elemento a la vez**: para obtener resultados más claros, pruebe las variaciones de un solo elemento (por ejemplo, solo línea de asunto o solo contenido) en lugar de varios elementos simultáneamente.

* **Elija la duración apropiada**: Deje tiempo suficiente para que la relevancia estadística:
   * Para las pruebas de tasa de apertura: 12-24 horas suele ser suficiente
   * Para las pruebas de tasa de clics: puede que se necesiten entre 24 y 48 horas o más
   * Las audiencias más grandes pueden requerir menos tiempo, mientras que las más pequeñas pueden necesitar más

* **Cambiar el tamaño de la audiencia** correctamente:
   * Asegúrese de que la audiencia del experimento (el porcentaje asignado a las pruebas) sea lo suficientemente grande como para generar resultados significativos
   * Directrices generales: Mínimo de 1.000 destinatarios por tratamiento para obtener resultados fiables

* **Realizar pruebas con regularidad pero no de forma excesiva**: llevar a cabo experimentos en campañas importantes, pero evitar probar cada envío para enfocar los recursos en decisiones impactantes.

* **Documente sus aprendizajes**: Mantenga registros de los resultados de los experimentos para informar futuras estrategias de campañas.

## Temas relacionados {#related-topics}

* [Creación de su primer correo electrónico](create-email.md)
* [Configurar el contenido del correo electrónico](edit-content.md)
* [Previsualización y envío de un correo electrónico](../monitor/prepare-send.md)
* [Informes de envío de correo electrónico](../reporting/email-report.md)
