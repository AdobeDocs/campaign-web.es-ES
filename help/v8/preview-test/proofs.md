---
audience: end-user
title: Envío de pruebas
description: Documentación web de Campaign v8
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 28cada1d6b645bd6f0c365528c9302bf4b03ad65
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 2%

---

# Envío de pruebas {#send-proofs}

>[!NOTE]
>
>Esta documentación está en construcción y se actualiza con frecuencia. La versión final de este contenido estará lista en enero de 2023.

El envío de pruebas le permite validar su correo electrónico y comprobar varios elementos, como vínculos, vínculos de exclusión y páginas espejo, imágenes y detectar posibles errores.

Las pruebas se pueden enviar a dos tipos de destinatarios:

* **Perfiles y audiencias de prueba**: enviar pruebas a direcciones semilla, que son destinatarios adicionales de la base de datos que no forman parte del destinatario de correo electrónico,

* **Perfiles de sustitución**: envíe pruebas a una dirección de correo electrónico específica utilizando un perfil existente. Esto le permite colocarse en la posición de los perfiles y obtener una representación exacta del mensaje que recibirá el perfil.

## Seleccione los destinatarios de las pruebas {#recipients}

1. Acceda a la pantalla de creación de contenido de correo electrónico y haga clic en **[!UICONTROL Simular contenido]**.

1. Haga clic en el **[!UICONTROL Prueba]** a continuación, utilice el **[!UICONTROL Modo]** lista desplegable para elegir el tipo de destinatarios que recibirán las pruebas:

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Envío de pruebas a perfiles de prueba

1. Elija la **[!UICONTROL Uso de perfiles de prueba]** en el menú contextual.

1. Añada los perfiles de prueba que recibirán los correos electrónicos de prueba.

   También puede crear una audiencia para seleccionar perfiles de prueba en función de sus propios criterios utilizando la variable **[!UICONTROL Agregar audiencia de prueba]** botón.

   ![](assets/test-profiles-audience.png)

### Envío de pruebas a perfiles de sustitución

1. Elija la **[!UICONTROL Sustitución de destino]** en el menú contextual.

1. Añada las direcciones de correo electrónico que recibirán las pruebas.

   >[!NOTE]
   >
   >Puede especificar cualquier dirección de correo electrónico. Esto le permite enviar pruebas a cualquier usuario, incluso si no es usuario de Adobe Campaign V8.

1. Para cada dirección de correo electrónico, seleccione el perfil del destinatario que desea utilizar. También puede permitir que Adobe Campaign seleccione un perfil aleatorio del destinatario.

   ![](assets/substitution.png)

Una vez seleccionados los destinatarios de prueba, puede enviar el correo electrónico de prueba. [Aprenda a enviar pruebas](#send)

>[!NOTE]
>
>Si desea enviar el mensaje de correo electrónico final a los destinatarios de las pruebas, habilite la variable **[!UICONTROL Incluir población de prueba en el objetivo principal]** en.

## Envíe las pruebas {#send}

Para enviar las pruebas a los destinatarios seleccionados, haga clic en **[!UICONTROL Enviar correo electrónico de prueba]** a continuación, confirme la entrega.

![](assets/send-proof.png)

Una vez enviadas las pruebas, puede acceder a los registros dedicados desde el **[!UICONTROL Ver registro de correo electrónico de prueba]** botón. Estos registros le permiten acceder a las pruebas enviadas y a las estadísticas específicas relacionadas con el envío de la prueba.

![](assets/proof-log.png)

Envíe tantas pruebas como sea necesario hasta que haya finalizado el contenido de su envío. Una vez hecho esto, puede enviar el correo electrónico al destinatario principal. [Aprenda a preparar y enviar su correo electrónico](../monitor/prepare-send.md)
