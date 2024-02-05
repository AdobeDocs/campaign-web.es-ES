---
audience: end-user
title: Envío mediante olas
description: Obtenga más información sobre la configuración de envíos en Campaign Web
badge: label="Disponibilidad limitada"
source-git-commit: 1d3e2ccbf4db5eb23531351572a4400754982e2d
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 81%

---


# Envío mediante olas {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Definición de olas"
>abstract="Defina olas para dividir los envíos en varios lotes en lugar de enviar grandes volúmenes de mensajes al mismo tiempo."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Tamaño de la ola"
>abstract="El tamaño de la ola es obligatorio. Introduzca un valor numérico (número de mensajes) o un porcentaje (0-100 %) en el campo de tamaño."

Para equilibrar la carga, se pueden dividir los envíos en varios lotes. Configure el número de lotes y su proporción con respecto a todo la entrega.

>[!NOTE]
>
>Solo se puede definir el tamaño y el retraso entre dos olas consecutivas. No se pueden configurar los criterios de selección de destinatarios para cada ola.

1. Abra el [configuración de envío](delivery-settings.md#retries) y vaya a la **[!UICONTROL Envío]** pestaña.
1. Seleccione la opción **[!UICONTROL Send using multiple waves]** y haga clic en el vínculo **[!UICONTROL Define waves...]**

1. Para configurar las olas, se puede:

   * **[!UICONTROL Programar varias olas del mismo tamaño]**. Por ejemplo, si se introduce **[!UICONTROL 30%]** en el campo correspondiente, cada ola representa el 30 % de los mensajes incluidos en la entrega, excepto el último, que representa el 10 % de los mensajes.

     En el **[!UICONTROL Intervalo]** , especifique el retardo entre el inicio de dos olas consecutivas. Por ejemplo, si se introduce **[!UICONTROL 2d]**, la primera ola comienza inmediatamente, la segunda ola comienza en dos días, la tercera ola en cuatro días, etc.

   * **[!UICONTROL Programar olas según un calendario]**.

     En la columna **[!UICONTROL Comenzar]**, especifique el retardo entre el inicio de dos olas consecutivas. En la columna **[!UICONTROL Tamaño]**, introduzca un número fijo o un porcentaje.

     En el siguiente ejemplo, la primera ola representa el 25 % del número total de mensajes incluidos en la entrega y se inicia inmediatamente. Las dos olas siguientes completan la entrega y se establecen para comenzar a intervalos de seis horas.

     Una regla de control de tipología específica, **[!UICONTROL Comprobación de programación de olas]**, garantiza que la última ola se programe antes del límite de validez del envío. Las tipologías de campaña y sus reglas se configuran en la variable **[!UICONTROL Tipología]** de la configuración de entrega. Obtenga más información sobre las reglas de control en la [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html)

     >[!IMPORTANT]
     >
     >Asegúrese de que las últimas olas no superen la fecha límite de entrega, que se define en la pestaña **[!UICONTROL Validez]**. De lo contrario, es posible que algunos mensajes no se envíen. [Más información](delivery-settings.md#validity)
     >
     >Al configurar las últimas olas, se debe dejar un margen suficiente para realizar reintentos. [Más información](delivery-settings.md#retries)

1. Para supervisar sus envíos, vaya a [registros de envío](../monitor/delivery-logs.md).

Se pueden ver los envíos que ya se han realizado en las olas procesadas (**[!UICONTROL Enviar]** estado) y las que se envían en las olas restantes (estado **[!UICONTROL Pendiente]**).

Los siguientes dos ejemplos son los casos más comunes para usar varias olas.

* **Durante el proceso de aceleración**

  Cuando se envían correos electrónicos utilizando una plataforma nueva, los proveedores de servicios de Internet (ISP) sospechan de las direcciones IP desconocidas. Si se envían, de repente, grandes volúmenes de correos electrónicos, los ISP suelen marcarlos como correo no deseado.

  Para evitar que se lo considere correo no deseado, puede aumentar progresivamente el volumen enviado mediante el uso de olas. Esto debería garantizar un desarrollo uniforme de la fase de inicio y permitir reducir la velocidad total de direcciones no válidas.

  Para hacer esto, seleccione la opción **[!UICONTROL Programar ondas según un calendario]**. Por ejemplo, defina la primera ola en 10 %, la segunda en 15 % y así sucesivamente.

* **Campañas que implican un centro de llamadas**

  Al administrar una campaña de lealtad por teléfono, su organización tiene una capacidad limitada para procesar la cantidad de llamadas a los suscriptores.

  Al usar olas, restringimos el número de mensajes a 20 por día, es decir, la capacidad de procesamiento diaria de un centro de llamadas.

  Para ello, seleccione la opción **[!UICONTROL Programar múltiples ondas del mismo tamaño]**. Introducir **[!UICONTROL 20]** como tamaño de la onda y **[!UICONTROL 1d]** en el campo **[!UICONTROL Periodo]**.