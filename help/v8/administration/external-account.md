---
title: Administrar cuenta externa
description: Obtenga información sobre cómo configurar cuentas externas
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 2%

---

# Cuentas externas específicas de la campaña {#external-account}

Siga los pasos a continuación para configurar las opciones de la cuenta según el tipo de cuenta externa seleccionada.

## Correos electrónicos rechazados (POP3) {#bounce}

La cuenta externa Rebote de correos electrónicos especifica la cuenta POP3 externa que se utiliza para conectarse al servicio de correo electrónico. Todos los servidores configurados para el acceso POP3 pueden recibir el correo electrónico devuelto.

![Captura de pantalla que muestra los campos de configuración de cuenta externa de correos rechazados (POP3).](assets/external_account_bounce.png)

Para configurar la cuenta externa **[!UICONTROL Correos rechazados (POP3)]**, rellene los campos siguientes:

* **[!UICONTROL Servidor]**: URL del servidor POP3.

* **[!UICONTROL Puerto]** - número de puerto de conexión POP3 (el puerto predeterminado es 110).

* **[!UICONTROL Cuenta]** - Nombre del usuario.

* **[!UICONTROL Contraseña]** - Contraseña de la cuenta de usuario.

* **[!UICONTROL Cifrado]** - Tipo de cifrado elegido, que incluye:
   * De forma predeterminada (POP3 si puerto 110, POP3S si puerto 995).
   * POP3 que cambia a SSL después de enviar un STARTTLS.
   * POP3 no seguro (puerto 110 de forma predeterminada).
   * POP3 secure above SSL (puerto 995 de forma predeterminada).

* **[!UICONTROL Función]** - Seleccione **[!UICONTROL Correo electrónico entrante]** para configurar la cuenta para recibir correos electrónicos entrantes o **[!UICONTROL enrutador de SOAP]** para administrar solicitudes de SOAP.

>[!IMPORTANT]
>
>Antes de configurar la cuenta externa POP3 con Microsoft OAuth 2.0, primero debe registrar la aplicación en Azure Portal. Para obtener más información, consulte [esta página](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app){target=_blank}.

Para configurar un POP3 externo con Microsoft OAuth 2.0, marque la opción Microsoft OAuth 2.0 y rellene los campos siguientes:

* **[!UICONTROL inquilino de Azure]**

  Azure ID (o ID de directorio (inquilino)) se encuentra en la lista desplegable de Essentials de la descripción general de la aplicación en el portal de Azure.

* **[!UICONTROL ID de cliente de Azure]**

  El ID de cliente (o el ID de aplicación (cliente)) se pueden encontrar en la lista desplegable Essentials de la descripción general de la aplicación en el portal de Azure.

* **[!UICONTROL Secreto de cliente de Azure]**

  El ID de secreto de cliente se puede encontrar en la columna Secretos de cliente del menú Certificados y secretos de la aplicación en el portal de Azure.

* **[!UICONTROL URL de redireccionamiento de Azure]**

  La URL de redireccionamiento se encuentra en el menú Autenticación de la aplicación en el portal de Azure. Debe finalizar con la siguiente sintaxis nl/jsp/oauth.jsp, p. ej. `https://redirect.adobe.net/nl/jsp/oauth.jsp`.

El acceso a Internet es necesario para la instalación y para utilizar el botón Probar conexión en la consola del cliente. Después de la configuración, el proceso de inMail puede comunicarse con los servidores de Microsoft sin Internet.

Después de introducir las diferentes credenciales, puede hacer clic en Configurar la conexión para finalizar la configuración de la cuenta externa.

## Enrutamiento {#routing}

Para configurar una cuenta externa específica para envíos externos, siga los pasos a continuación.

1. Cree una cuenta externa. [Más información](create-external-account.md)

1. Seleccione el tipo **[!UICONTROL Routing]**.

   ![Captura de pantalla que muestra la selección del tipo de cuenta externa de enrutamiento.](assets/external-account-routing.png){zoomable="yes"}

1. Seleccione el canal deseado y haga clic en **[!UICONTROL Crear]**.

1. En la sección de la cuenta externa **[!UICONTROL Detalles]**, **[!UICONTROL Externo]** está seleccionado de forma predeterminada como **[!UICONTROL Modo de envío]**.

   ![Captura de pantalla que muestra la configuración del modo de envío para las cuentas externas de enrutamiento.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >En este momento, **[!UICONTROL External]** es el único modo disponible.

1. Para gestionar el proceso después de la ejecución de la entrega, externalícelo a un flujo de trabajo de posprocesamiento. Cree un flujo de trabajo con una actividad [Señal externa](../workflows/activities/external-signal.md) y selecciónela en el campo **[!UICONTROL Procesamiento posterior]**.

   ![Captura de pantalla que muestra la configuración del campo de procesamiento posterior para las cuentas externas de enrutamiento.](assets/external-account-post-processing.png){zoomable="yes"}

1. En el campo **[!UICONTROL Actividad]**, edite el nombre de la actividad de flujo de trabajo de posprocesamiento que se muestra en los registros. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## Instancia de ejecución {#instance-exec}

Si tiene una arquitectura segmentada, identifique las instancias de ejecución asociadas a la instancia de control y establezca conexiones entre ellas. Las plantillas de mensajes transaccionales se implementan en la instancia de ejecución.

![Captura de pantalla que muestra los campos de configuración de cuenta externa de la instancia de ejecución.](assets/external_account_exec.png)

Para configurar la cuenta externa **[!UICONTROL Execution instance]**:

* **[!UICONTROL URL]**: URL del servidor donde está instalada la instancia de ejecución.

* **[!UICONTROL Cuenta]** - Nombre de la cuenta, que coincide con el Agente del centro de mensajes definido en la carpeta del operador.

* **[!UICONTROL Contraseña]**: contraseña de la cuenta tal como se define en la carpeta del operador.

* **[!UICONTROL Método]** - Elija entre servicio Web o acceso de datos federado (FDA).

  Para FDA, seleccione su cuenta de FDA. Tenga en cuenta que la conexión de Campaign a sistemas externos está restringida a usuarios avanzados y solo está disponible desde la consola del cliente. [Más información](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Crear flujo de trabajo de archivado]**: para cada instancia de ejecución registrada en el Centro de mensajes, independientemente de si tiene una o varias instancias, cree un flujo de trabajo de archivado independiente para cada cuenta externa asociada a la instancia de ejecución.
