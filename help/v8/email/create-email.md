---
audience: end-user
title: Crear el primer correo electrónico
description: Documentación web de Campaign v8
source-git-commit: cdddef89cda4fa39cee38e9d0171a6ea395537c7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 2%

---

# Enviar su primer correo electrónico {#first-email}

>[!NOTE]
>
>Esta documentación está en construcción y se actualiza con frecuencia. La versión final de este contenido estará lista en enero de 2023.

Este caso de uso detalla cómo crear su primer correo electrónico

En este ejemplo, programaremos el envío de un correo electrónico en una fecha específica a los clientes fieles de plata y oro. Este correo electrónico se diseñará con una plantilla de HTML predefinida de un archivo ZIP e incluirá la personalización mediante los atributos del perfil.

![](assets/delivery-list.png)

## Creación del correo electrónico {#create-email}

1. Cree un nuevo envío desde la **[!UICONTROL Entregas]** para abrir el Navegador.
1. Seleccione el **[!UICONTROL Correo electrónico]** canal y la plantilla que se va a utilizar y, a continuación, haga clic en **[!UICONTROL Crear]**.

   >[!NOTE]
   >
   >información sobre plantillas. información de comprobación en el documento V7

   ![](assets/channel-template.png)

1. Proporcione una etiqueta para la entrega y configure opciones adicionales según sus necesidades:

   * Nombre interno:
   * Carpeta:
   * Código del envío:
   * Descripción:
   * Naturaleza:

   compruebe qué configuración se define en la plantilla y menciónelas (descripción? carpeta, naturaleza?)

   ![](assets/email-properties.png)

   >[!NOTE]
   >
   >información sobre la configuración del envío, botón + vínculo a doc

## Creación del contenido del correo electrónico {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Cree el primer contenido de correo electrónico con el Diseñador de correo electrónico."
>abstract="Crear el primer contenido de correo electrónico"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Creación del contenido del correo electrónico"
>abstract="TBC"

1. Haga clic en el **[!UICONTROL Editar contenido]** para comenzar a crear el contenido del correo electrónico.

   Esta pantalla le permite configurar el contenido del correo electrónico y diseñarlo con el Diseñador de correo electrónico.

   ![](assets/edit-content.png)

   >[!NOTE]
   >
   >La información de correo electrónico Desde nombre y Desde está predefinida en la plantilla de correo electrónico seleccionada.
   >
   >De forma predeterminada, el seguimiento de correo electrónico está habilitado para las aperturas y los clics. Para desactivar estas opciones, desmarque las opciones de la sección Funciones opcionales .

1. Especifique el asunto del correo electrónico con el Editor de expresiones. [Obtenga información sobre cómo personalizar el contenido](../personalization/personalize.md)

   En este ejemplo, se desea personalizar la línea de asunto con el nombre de los perfiles.

   ![](assets/subject-line.png)

1. Añada un archivo adjunto al correo electrónico si es necesario. Aprenda a editar el contenido del correo electrónico

1. Haga clic en el **[!UICONTROL Editar cuerpo del correo electrónico]** para crear y diseñar el contenido del correo electrónico.

   Elija el método que desee utilizar para crear el contenido del correo electrónico. En este ejemplo, queremos importar un contenido de HTML existente.

   ![](assets/import-html.png)

1. Seleccione el HTML o el archivo ZIP que desea importar y haga clic en **[!UICONTROL Siguiente]**.

   Si la carpeta contiene recursos, elija la instancia y la carpeta donde deben almacenarse y haga clic en **[!UICONTROL Importar]**. (+ vínculo a doc en recursos?)

   ![](assets/import-folder.png)

1. Una vez importado el contenido, se muestra en el Diseñador de correo electrónico, lo que le permite editarlo si es necesario y añadir personalización.

   En este ejemplo, queremos añadir personalización en el título del correo electrónico. Para ello, seleccione el bloque de componentes y haga clic en **[!UICONTROL Añadir personalización]**.

   ![](assets/add-perso.png)

1. Una vez que el contenido esté listo, guárdelo y haga clic en la flecha para volver a la pantalla de creación del correo electrónico.

   ![](assets/save-content.png)

## Definición de la audiencia {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definición de la audiencia"
>abstract="TBC"

1. Haga clic en el **[!UICONTROL Seleccionar la audiencia]** a continuación, elija una audiencia existente o cree una nueva.

   En este ejemplo, queremos utilizar una audiencia existente dirigida a clientes que pertenezcan a los niveles de puntos de lealtad de oro y plata.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Las audiencias disponibles en la lista proceden de la instancia de Campaign V8 o de Adobe Experience Platform si la integración Destino / Fuentes se ha implementado en la instancia. Obtenga información sobre cómo seleccionar la audiencia de correo electrónico

1. Una vez seleccionada la audiencia, puede editar las reglas si es necesario. También puede establecer un grupo de control para analizar el comportamiento de los destinatarios de correo electrónico en comparación con el comportamiento de los perfiles que no estaban segmentados. Aprenda a trabajar con grupos de control

## Programe el envío {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Programe el envío"
>abstract="TBC"

Para programar el envío del correo electrónico, haga clic en Habilitar y especifique la fecha y la hora deseadas.

= confirm before sending, opción : qué sucede en la fecha programada: para confirmar el envío del mensaje?

![](assets/schedule.png)

## Previsualizar y probar el correo electrónico {#preview-test}

Una vez que el correo electrónico esté listo, puede obtener una vista previa y probarlo antes de iniciar su envío.

1. Haga clic en **[!UICONTROL Revisar para enviar]**. Se muestra una vista previa del correo electrónico, junto con todas las propiedades, audiencia y programación configuradas. Puede editar cualquiera de estos elementos mediante el botón de modificación.

   ![](assets/review-email.png)

1. Haga clic en el **[!UICONTROL Simular contenido]** para obtener una vista previa del correo electrónico y enviar pruebas.

1. En el área del lado izquierdo, seleccione los perfiles que desea utilizar para previsualizar el correo electrónico. Puede utilizar perfiles de destino o perfiles de prueba específicos.

1. Se muestra una previsualización del correo electrónico en el área derecha basada en el perfil seleccionado. Si ha añadido varios perfiles, puede cambiar entre cada uno de ellos para previsualizar el correo electrónico correspondiente.

   ![](assets/preview.png)

   >[!NOTE]
   >
   >Además, la variable **[!UICONTROL Procesar correo electrónico]** permite previsualizar el correo electrónico utilizando varios dispositivos o proveedores de correo. Obtenga información sobre cómo previsualizar el procesamiento de correo electrónico

1. Para enviar pruebas del correo electrónico, haga clic en el **[!UICONTROL Prueba]** a continuación, seleccione los perfiles que recibirán la prueba. En este ejemplo, deseamos enviar las pruebas a un perfil de prueba específico.

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >También puede probar los mensajes suplantando algunos de los perfiles de destino y enviando el mensaje de prueba a la dirección de correo electrónico que desee. Aprenda a utilizar Sustituir del modo de destino

1. Haga clic en **[!UICONTROL Enviar correo electrónico de prueba]** a continuación, confirme la entrega.

   Una vez enviadas las pruebas, puede comprobar su estado haciendo clic en el botón **[!UICONTROL Ver registro de correo electrónico de prueba]** botón.

## Enviar y supervisar el correo electrónico {#prepare-send}

Una vez que haya revisado y probado el correo electrónico, puede iniciar su preparación y enviarlo.

1. Haga clic en **[!UICONTROL Preparación]** para iniciar la preparación del mensaje.

   Puede realizar un seguimiento del progreso de la preparación en tiempo real, junto con estadísticas. Una vez finalizada la preparación, puede acceder a registros detallados para un análisis más detallado. Descubra cómo monitorizar las entregas

   ![](assets/preparation.png)

1. Una vez que el correo electrónico esté listo para enviarse, haga clic en **[!UICONTROL Enviar]** a continuación, confirme la entrega.

   Puede realizar un seguimiento de los envíos en tiempo real, junto con estadísticas. Además, la variable **[!UICONTROL Registros]** permite acceder a información detallada sobre el envío de correo electrónico. Descubra cómo monitorizar las entregas

   ![](assets/logs.png)

1. Una vez enviado el correo electrónico, puede acceder a los informes dedicados para realizar más análisis.

   ![](assets/reports.png)
