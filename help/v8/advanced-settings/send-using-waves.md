---
audience: end-user
title: Envío mediante olas
description: Obtenga más información sobre la configuración de envíos en Campaign Web
feature: Email
exl-id: d4cd5fe5-f9ac-44ac-a961-ae45131aeb3e
source-git-commit: e5a17ad1f8316d201dc3b4bc6ce20d61aea7a9c9
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 42%

---

# Envío mediante olas {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="División de los envíos en varios lotes"
>abstract="En lugar de enviar grandes volúmenes de mensajes al mismo tiempo, defina olas para dividir los envíos en varios lotes. Se pueden configurar varias olas del mismo tamaño o definir un calendario para que se envíen las distintas olas."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Definición del tamaño de cada ola"
>abstract="Debe introducir un tamaño para todas las olas que vaya a añadir. Introduzca un valor numérico (número de mensajes para cada ola) o un porcentaje (0-100 %)."

Para equilibrar la carga, puede dividir los envíos de correo electrónico en varios lotes. Configure el número de lotes y su proporción con respecto a todo el envío, así como el intervalo entre dos olas.

>[!NOTE]
>
>Solo se puede definir el tamaño y el retraso entre dos olas consecutivas. No se pueden ajustar los criterios de selección de destinatarios para cada ola.

Para realizar envíos mediante olas, siga los pasos a continuación.

1. Abra [configuración de envío](delivery-settings.md#retries).

1. Vaya a la sección **[!UICONTROL Envío]**.

1. Seleccione la opción **[!UICONTROL Enviar usando múltiples ondas]**.

1. Para configurar las olas, se puede:

   * [Programar varias olas del mismo tamaño](#waves-same-size)
   * [Programar las olas de acuerdo con un calendario](#waves-calendar)

1. Prepare y realice la entrega de la forma habitual. [Más información](../msg/gs-deliveries.md)

   >[!CAUTION]
   >
   >Asegúrese de que las últimas olas no superen la fecha límite de entrega definida en la pestaña [Validez](delivery-settings.md#validity); de lo contrario, es posible que algunos mensajes no se envíen. Una regla de control de tipología específica, **[!UICONTROL Verificación de programación de ondas]**, garantiza que la última ola se programe antes del límite de validez de la entrega. Obtenga más información sobre las reglas de control en la [documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=es).
   >
   >Al configurar las últimas olas, se debe dejar un margen suficiente para realizar reintentos. [Más información](delivery-settings.md#retries)

1. Para supervisar tus envíos, ve a [registros de envío](../monitor/delivery-logs.md). Se pueden ver los envíos que ya se han realizado en las olas procesadas (**[!UICONTROL Enviar]** estado) y las que se envían en las olas restantes (estado **[!UICONTROL Pendiente]**).

## Programar varias olas del mismo tamaño {#waves-same-size}

Si selecciona esta opción, todas las olas tienen el mismo tamaño (excepto la última) y el retardo entre cada ola es siempre el mismo.

![](assets/waves-same-size.png){zoomable="yes"}

* Especifique el tamaño de todas las olas en las que divide la entrega. Puede introducir un porcentaje o un valor numérico. Solo la última ola puede variar en tamaño, ya que debe incluir el número restante de mensajes.

  Por ejemplo, si escribe **[!UICONTROL 30%]** en el campo **[!UICONTROL Tamaño de las olas]**, las tres primeras olas representan el 30% de todos los mensajes incluidos en la entrega y la cuarta representa el 10% restante.

* En la sección **[!UICONTROL Intervalo]**, especifique el retardo entre el inicio de dos olas consecutivas. Por ejemplo, si escribe **[!UICONTROL 2 días]**, la primera ola comienza inmediatamente, la segunda ola comenzará en dos días, la tercera ola en cuatro días, etc.

Un caso de uso común para utilizar varias olas del mismo tamaño es con un centro de llamadas involucrado. Al administrar una campaña de lealtad por teléfono, su organización tiene una capacidad limitada para procesar la cantidad de llamadas a los suscriptores.

Al usar olas, restringimos el número de mensajes a 20 por día, es decir, la capacidad de procesamiento diaria de un centro de llamadas.

Para ello, seleccione la opción **[!UICONTROL Programar múltiples ondas del mismo tamaño]**. Escriba **[!UICONTROL 20]** como tamaño de olas y **[!UICONTROL 1 día]** en el campo **[!UICONTROL Intervalo]**.

![](assets/waves-call-center.png){zoomable="yes"}

## Programar las olas de acuerdo con un calendario {#waves-calendar}

Si selecciona esta opción, debe definir el día y la hora de inicio de cada ola que envíe, así como el tamaño de cada ola.

* En los campos **[!UICONTROL Iniciar]**, especifique el retardo entre el inicio de dos olas consecutivas.

* En la columna **[!UICONTROL Tamaño]**, introduzca un número fijo o un porcentaje.

Añada tantas olas como desee. Puede reordenarlos según sus necesidades.

>[!NOTE]
>
>Si utiliza porcentajes, el total de todas las olas no debe superar el 100%.

En el ejemplo siguiente, la primera ola representa el 25 % del número total de mensajes incluidos en la entrega y se inicia inmediatamente. Las dos olas siguientes completan la entrega y se establecen para comenzar a intervalos de seis horas.

![](assets/waves-calendar.png){zoomable="yes"}

Un caso de uso común para utilizar varias olas según un calendario es durante el proceso de aceleración.

Cuando se envían correos electrónicos utilizando una plataforma nueva, los proveedores de servicios de Internet (ISP) sospechan de las direcciones IP desconocidas. Si se envían, de repente, grandes volúmenes de correos electrónicos, los ISP suelen marcarlos como correo no deseado.

Para evitar que se lo considere correo no deseado, puede aumentar progresivamente el volumen enviado mediante el uso de olas. Esto debería garantizar un desarrollo uniforme de la fase de inicio y permitir reducir la velocidad total de direcciones no válidas.

Para hacer esto, seleccione la opción **[!UICONTROL Programar ondas según un calendario]**. Por ejemplo, defina la primera ola en 10 %, la segunda en 15 %, la tercera en 20 %, etc.

![](assets/waves-ramp-up.png){zoomable="yes"}
