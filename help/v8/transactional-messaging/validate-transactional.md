---
audience: end-user
title: Validación de mensajes transaccionales
description: Obtenga información sobre cómo validar un mensaje transaccional en la interfaz de usuario web de Campaign
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 1%

---

# Validación de mensajes transaccionales

Durante o después de crear el mensaje transaccional, es posible que desee validar el contenido mediante una muestra de datos.

## Simular contenido {#simulate-content}

Siga estos pasos para simular el contenido del mensaje:

* Asegúrese de que la ruta de personalización del contenido del mensaje coincida con el ejemplo de contexto. En el ejemplo siguiente, para mostrar el nombre del perfil de prueba, use la ruta de acceso *rtEvent.ctx.basicDetails.firstName*.

  Puede modificar el contenido del mensaje o el ejemplo de contexto para que se alineen.

  ![Captura de pantalla que muestra la verificación de las rutas de personalización en el contenido del mensaje](assets/validate-verification.png){zoomable="yes"}

* Haga clic en el botón **[!UICONTROL Simular contenido]** para obtener una vista previa del mensaje transaccional con los datos introducidos en la muestra de contexto.

  ![Captura de pantalla que muestra el botón Simular contenido y la funcionalidad de vista previa](assets/validate-simulate.png){zoomable="yes"}

  Después de revisar el contenido, haz clic en el botón **[!UICONTROL Cerrar]**.

* Asegúrese de hacer clic en el botón **[!UICONTROL Volver a publicar]** si ha realizado cambios en el contenido.

## Enviar prueba

Para probar y experimentar el mensaje transaccional tal como se entregaría a través del canal elegido, como correo electrónico, SMS o notificaciones push, utilice la función de prueba.

En la [ventana de contenido de simulación](#simulate-content), haga clic en el botón **[!UICONTROL Enviar revisión]**.

![Captura de pantalla que muestra el botón Enviar prueba en la ventana de contenido de simulación](assets/transactional-proof.png){zoomable="yes"}

En la nueva ventana que aparece, introduzca la dirección de correo electrónico o el número de teléfono, según el canal, donde desee recibir la prueba. Después de ingresar la dirección deseada, haz clic en los botones **[!UICONTROL Enviar revisión]** y **[!UICONTROL Confirmar]**. Esta acción envía un ejemplo del mensaje transaccional, lo que garantiza que todas las personalizaciones, el contenido dinámico y el formato aparezcan correctamente como lo harían los usuarios finales.

![Captura de pantalla que muestra la funcionalidad Enviar prueba y el proceso de confirmación](assets/transactional-sendproof.png){zoomable="yes"}

Este paso es esencial para identificar cualquier problema potencial antes de publicar el mensaje transaccional.