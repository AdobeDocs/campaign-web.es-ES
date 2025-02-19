---
audience: end-user
title: Trabajo con reglas empresariales (tipologías)
description: Aprenda a trabajar con tipologías y reglas de tipología para controlar, filtrar y monitorizar la entrega de envíos.
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 10%

---

# Trabajo con reglas empresariales (tipologías) {#typologies}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Reglas empresariales"
>abstract="Ahora puede crear tipologías y reglas de tipología en la interfaz de usuario web de Adobe Campaign. Las tipologías permiten controlar, filtrar y priorizar la entrega de envíos."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"


>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="Tipologías y reglas de tipología"
>abstract="Las tipologías le permiten estandarizar las prácticas comerciales en todas las entregas. Una tipología es una colección de reglas de tipología que le permiten controlar, filtrar y priorizar la entrega de envíos. Los perfiles que coinciden con los criterios dentro de las reglas de tipología quedan excluidos de los públicos de envío en la fase de preparación."

## Acerca de las tipologías

Las tipologías le permiten estandarizar las prácticas comerciales en todas las entregas. Una **tipología** es una colección de **reglas de tipología** que le permiten controlar, filtrar y priorizar la entrega de envíos. Los perfiles que coinciden con los criterios dentro de las reglas de tipología quedan excluidos de los públicos de envío en la fase de preparación.

Las tipologías garantizan que las entregas siempre contengan determinados elementos (como un vínculo de baja o una línea de asunto) o reglas de filtrado para excluir grupos de los destinatarios deseados (como suscriptores que se han dado de baja, competidores o clientes que no sean fieles).

Se puede acceder a las tipologías a través del menú **[!UICONTROL Administración]** > **[!UICONTROL Reglas de negocio]**. Desde esta pantalla, puede acceder a todas las tipologías y reglas de tipología existentes o crear otras nuevas basadas en sus necesidades.

![](assets/business-rules-list.png)

>[!NOTE]
>
>La lista **[!UICONTROL Reglas de tipología]** muestra todas las reglas existentes creadas hasta el momento en la interfaz de usuario web o la consola de cliente. Sin embargo, solo se pueden crear las reglas **Control** y **Filtrado** en la interfaz de usuario web. Para crear otros tipos de reglas de tipología, como Reglas de presión o de capacidad, utilice la consola del cliente de Campaign v8. [Aprenda a crear reglas de tipología en la consola del cliente](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

Los pasos principales para aplicar tipologías a los mensajes son los siguientes:

1. [Crear una tipología](#typology).
1. [Crear reglas de tipología](#typology-rules).
1. [Reglas de tipología de referencia en la tipología](#add-rules).
1. [Aplicar la tipología a un mensaje](#message).

## Creación de una tipología {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="Propiedades de la tipología"
>abstract="Defina las propiedades de la tipología y expanda la sección **[!UICONTROL Opciones adicionales]** para acceder a la configuración avanzada. Utilice el campo **[!UICONTROL afinidad de IP]** para asociar afinidades de IP con tipologías. Esto le permite controlar mejor el tráfico SMTP saliente, definiendo qué direcciones IP específicas se pueden utilizar para cada afinidad."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="Afinidad de IP"
>abstract="La administración de afinidades con direcciones IP permite un mejor control del tráfico SMTP de salida mediante la asociación de distintas direcciones IP con cada tipo de tráfico en función de la tipología de su acción de envío."

Para crear una tipología, siga estos pasos:

1. Vaya al menú **[!UICONTROL Reglas de negocio]** y, a continuación, seleccione la pestaña **[!UICONTROL Tipología]**.

1. Haga clic en el botón **[!UICONTROL Crear tipología]** e introduzca una **[!UICONTROL Etiqueta]** para la tipología.

1. Expanda la sección **[!UICONTROL Opciones adicionales]** para definir la configuración avanzada, como el nombre interno de la tipología, la carpeta de almacenamiento y la descripción.

   ![](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >El campo **[!UICONTROL afinidad de IP]** le permite asociar afinidades de IP con tipologías. Esto le permite controlar mejor el tráfico SMTP saliente, definiendo qué direcciones IP específicas se pueden utilizar para cada afinidad.  Por ejemplo, puede utilizar una afinidad por país o subdominio. A continuación, puede crear una tipología por país y vincular cada afinidad a la tipología correspondiente.

1. Haga clic en **[!UICONTROL Crear]** para confirmar la creación de la tipología.

La tipología abre los detalles abiertos. Desde esta pantalla, puede hacer referencia directamente a las reglas de tipología existentes. También puede crear nuevas reglas de tipología y hacer referencia a ellas en la tipología más adelante:
* [Aprenda a crear una regla de tipología](#add-rules)
* [Obtenga información sobre cómo hacer referencia a reglas en una tipología](#add-rules)

## Creación de una regla de tipología {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="Propiedades de la regla de tipología"
>abstract="Defina las propiedades de la regla de tipología. Las reglas de **Control** verifican la calidad y validez del mensaje previo al envío, mientras que las reglas de **Filtrado** excluyen segmentos de la audiencia de destino según criterios específicos.<br/><br/>También puede cambiar el orden de ejecución de la regla para administrar la secuencia en la que se ejecutarán las reglas de tipología cuando se ejecuten varias reglas del mismo tipo durante la misma fase de procesamiento de mensajes."

Para crear una regla de tipología, vaya al menú **[!UICONTROL Reglas de negocio]** y luego seleccione la pestaña **[!UICONTROL Reglas de tipología]**.

Haga clic en el botón **[!UICONTROL Crear regla de tipología]** y siga los pasos detallados a continuación.

### Definición de las propiedades de la regla de tipología {#properties}

Defina las propiedades de la regla de tipología:

1. Escriba una **[!UICONTROL Etiqueta]** para la regla.

   ![](assets/business-rules-control-rule.png)

1. Seleccione el **[!UICONTROL Tipo]** de la regla de tipología:

   * **Control**: garantiza la calidad del mensaje y la validez antes del envío (por ejemplo, visualización de caracteres, longitud de SMS, formato de dirección, acortamiento de URL). Se crean mediante una interfaz de script para definir una lógica compleja para las comprobaciones y modificaciones de contenido.

   * Las reglas de **filtrado** excluyen segmentos de la audiencia de destino según criterios específicos (por ejemplo: edad, ubicación, país, números de teléfono). Estas reglas están vinculadas a una dimensión objetivo.

   >[!NOTE]
   >
   >Por ahora, solo se pueden crear reglas de tipología de **Control** y **Filtrado** desde la interfaz de usuario web. Para crear otros tipos de reglas, utilice la consola Cliente. [Aprenda a crear reglas de tipología en la consola del cliente](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

1. Seleccione un **[!UICONTROL canal]** para asociarlo a la regla.

1. Desactive la opción **[!UICONTROL Active]** si no desea que la regla esté activa justo después de crearla.

1. Defina la regla **[!UICONTROL Execution order]**.

   De forma predeterminada, el orden de las reglas de tipología se establece en 50. Puede adaptar este valor para gestionar la secuencia en la que se ejecutan las reglas de tipología cuando se ejecutan varias reglas del mismo tipo durante la misma fase de procesamiento de mensajes. Por ejemplo, una regla de filtrado con un orden de ejecución de 20 se ejecuta antes que una regla de filtrado con un orden de ejecución de 30.

1. Expanda la sección **[!UICONTROL Opciones adicionales]** para obtener acceso a la configuración avanzada, como el nombre interno de la regla, el almacenamiento de carpetas y la descripción.

1. En el caso de las reglas de control, hay dos reglas adicionales disponibles en las opciones adicionales. Permiten especificar cuándo se debe aplicar la regla y su nivel de alerta:

   * **[!UICONTROL Fase]**: este campo le permite especificar en qué punto del ciclo de vida de la entrega se aplicará la regla. Seleccione el valor que se aplicará en la lista desplegable **[!UICONTROL Fase]**. Expanda la sección siguiente para obtener más detalles sobre los valores posibles.

   +++Fases de reglas de control:

   **[!UICONTROL Al principio del destino]**: Para evitar que el paso de personalización se ejecute en caso de errores, puede aplicar la regla de control aquí.

   **[!UICONTROL Después del direccionamiento]**: Si necesita conocer el volumen del destino para aplicar la regla de control, seleccione esta fase. Por ejemplo, la regla de control Check proof size se aplica después de cada fase de objetivos: esta regla evita la personalización de los mensajes si hay demasiados destinatarios de prueba.

   **[!UICONTROL Al comienzo de la personalización]**: esta fase debe estar seleccionada si el control afecta a la aprobación de la personalización de mensajes. La personalización del mensaje se lleva a cabo durante la fase de análisis.

   **[!UICONTROL Al final del análisis]**:Cuando una comprobación requiera que se complete la personalización de mensajes, seleccione esta fase.

+++

   * **[!UICONTROL Nivel]**: esta opción le permite especificar el nivel de alerta para la regla. Expanda la sección siguiente para obtener más información.

   +++Niveles de reglas de control:

   **[!UICONTROL Error]**: detenga la preparación del mensaje.

   **[!UICONTROL Advertencia]**: mostrar una advertencia en los registros de preparación.

   **[!UICONTROL Información]**: muestra información en los registros de preparación.

   <!--**[!UICONTROL Status]**:-->

   **[!UICONTROL Detallado]**: muestra información en los registros del servidor.

+++

### Creación del contenido de la regla {#build}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="Filtrado"
>abstract="Las reglas de **filtrado** excluyen segmentos de la audiencia de destino según criterios específicos (por ejemplo: edad, ubicación, país, números de teléfono). Seleccione la dimensión de segmentación de la regla de tipología y haga clic en el botón **[!UICONTROL Agregar reglas]** para acceder al modelador de consultas y generar la regla."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="Código"
>abstract="Las reglas de **Control** verifican la calidad y validez del mensaje previo al envío (por ejemplo: visualización de caracteres, longitud de SMS, formato de dirección, acortamiento de URL). Se crean mediante código JavaScript."

Una vez definidas las propiedades de la regla de tipología, puede generar el contenido de la regla.

* Para **Reglas de control**, haga clic en el botón **Editar código** e introduzca la lógica para la regla con JavaScript. En el ejemplo siguiente, se crea una regla para mostrar una advertencia en los registros si el destino está vacío.

  ![](assets/business-rules-code.png)

* Para **Reglas de filtrado**, seleccione la dimensión de segmentación y haga clic en el botón **[!UICONTROL Agregar reglas]** para definir los criterios de filtrado con el [modelador de consultas](../query/query-modeler-overview.md).

  ![](assets/business-rules-query.png)

Cuando la regla esté lista, haga clic en el botón **[!UICONTROL Crear]** para crear la regla de tipología. Ahora puede hacer referencia a la regla en una tipología para aplicarla a los mensajes.

## Reglas de tipología de referencia en una tipología {#add-rules}

Para hacer referencia a una o varias reglas en una tipología, siga estos pasos:

1. Vaya a la pestaña **[!UICONTROL Tipología]** y abra la tipología en la que desee hacer referencia a las reglas.

1. Seleccione la pestaña **[!UICONTROL Reglas de tipología]** y haga clic en el botón **[!UICONTROL Agregar reglas de tipología&#39;]**.

   ![](assets/business-rules-reference.png)

1. Seleccione una o varias reglas de tipología para asociarlas a la tipología y confirmarlas.

   ![](assets/business-rules-typology-save.png)

1. Haga clic en **[!UICONTROL Guardar]**.

Ahora puede aplicar la tipología a los mensajes. Una vez finalizado, todas las reglas de tipología seleccionadas se ejecutarán para realizar las comprobaciones definidas.

## Aplicación de tipologías a mensajes {#message}

Para aplicar una tipología a un mensaje o a una plantilla de mensaje, debe seleccionar la tipología en la configuración del mensaje. [Aprenda a configurar las opciones de envío](../advanced-settings/delivery-settings.md#typology)

![](assets/business-rules-apply.png)

Una vez realizadas, las reglas de tipología incluidas en ella se ejecutan para comprobar la validez de la entrega durante la preparación del mensaje. Los perfiles que coinciden con los criterios dentro de una regla de tipología se excluyen de las audiencias de envío.
