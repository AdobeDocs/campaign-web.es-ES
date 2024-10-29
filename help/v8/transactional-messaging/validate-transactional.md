---
audience: end-user
title: Validación de mensajes transaccionales
description: Obtenga información sobre cómo validar un mensaje transaccional en la interfaz de usuario web de Campaign
source-git-commit: e0d87d22d9712837f085f94f9d9ba63e96f36b36
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# Validación de mensajes transaccionales

Durante o después de crear el mensaje transaccional, es posible que desee validar el contenido mediante una muestra de datos.

## Simular contenido {#simulate-content}

Siga estos pasos para simular el contenido del mensaje:

* Asegúrese de que la ruta de personalización del contenido del mensaje coincida con el ejemplo de contexto. En el ejemplo siguiente, para mostrar el nombre del perfil de prueba, se utiliza la ruta de acceso *rtEvent.ctx.basicDetails.firstName*

  Puede cambiar el contenido del mensaje o el ejemplo de contexto para que se alineen.

  ![](assets/validate-verification.png){zoomable="yes"}

* Haga clic en el botón **[!UICONTROL Simular contenido]** para obtener una vista previa del mensaje transaccional con los datos introducidos en la muestra de contexto.

  ![](assets/validate-simulate.png){zoomable="yes"}

  Después de revisar el contenido, haz clic en el botón **[!UICONTROL Cerrar]**.

* No olvide hacer clic en el botón **[!UICONTROL Volver a publicar]** si ha realizado cambios en el contenido.

## Enviar prueba

Si desea probar y experimentar el mensaje transaccional tal como se entregaría a través del canal elegido (como correo electrónico, SMS o notificaciones push), puede utilizar la función de prueba.

En la [ventana de contenido de simulación](#simulate-content), haga clic en el botón **[!UICONTROL Enviar revisión]**.

![](assets/transactional-proof.png){zoomable="yes"}

En la nueva ventana que aparece, introduzca la dirección de correo electrónico (o el número de teléfono, según el canal) donde desea recibir la prueba. Una vez que hayas ingresado la dirección deseada, haz clic en **[!UICONTROL Enviar revisión]** y en **[!UICONTROL Confirmar]** botones. Esta acción le permite enviar una muestra del mensaje transaccional, asegurándose de que todas las personalizaciones, el contenido dinámico y el formato aparezcan correctamente como lo harían los usuarios finales.

![](assets/transactional-sendproof.png){zoomable="yes"}

Este es un paso esencial para identificar cualquier problema potencial antes de publicar el mensaje transaccional.
