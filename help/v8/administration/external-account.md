---
title: Administrar cuenta externa
description: Obtenga información sobre cómo configurar cuentas externas
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# Administración de cuentas externas {#external-accounts}

>[!AVAILABILITY]
>
>* Actualmente, las cuentas externas solo están disponibles para correos rechazados (POP3), enrutamiento y la instancia de ejecución. Los tipos de cuenta adicionales se agregarán más adelante.
>
>* Las cuentas externas no admitidas creadas en la consola de Adobe Campaign están visibles en la interfaz de usuario web, pero no se pueden editar ni acceder a ellas.

Adobe Campaign incluye cuentas externas preconfiguradas para facilitar la integración con varios sistemas. Para conectarse a plataformas adicionales o personalizar conexiones para adaptarse al flujo de trabajo, cree nuevas cuentas externas mediante la interfaz de usuario web. Esto garantiza transferencias de datos sin problemas.

## Creación de una cuenta externa {#create-ext-account}

Para crear una nueva cuenta externa, siga los pasos a continuación. La configuración detallada depende del tipo de cuenta externa. [Más información](#campaign-specific)

1. En el menú del panel izquierdo, seleccione **[!UICONTROL Cuentas externas]** en **[!UICONTROL Administración]**.

1. Haga clic en **[!UICONTROL Crear cuenta externa]**.

   ![Captura de pantalla que muestra la opción de crear una cuenta externa en la interfaz de usuario web.](assets/external_account_create_1.png)

1. Escriba su **[!UICONTROL Etiqueta]** y seleccione la cuenta externa **[!UICONTROL Tipo]**.

   >[!NOTE]
   >
   >La configuración para los tipos específicos de campaña se detalla en [esta sección](#campaign-specific).

   ![Captura de pantalla que muestra campos para ingresar la etiqueta y seleccionar el tipo de cuenta externa.](assets/external_account_create_2.png)

1. Haga clic en **[!UICONTROL Crear]**.

1. En la lista desplegable **[!UICONTROL Opciones adicionales]**, cambie la ruta de acceso **[!UICONTROL Nombre interno]** o **[!UICONTROL Carpeta]** si es necesario.

   ![Captura de pantalla que muestra opciones adicionales para la configuración de nombre interno y ruta de carpeta.](assets/external_account_create_3.png)

1. Habilite la opción **[!UICONTROL Exportado automáticamente en paquetes]** para exportar automáticamente los datos administrados por esta cuenta externa. <!--Exported where??-->

   ![Captura de pantalla que muestra la opción para habilitar la exportación automática en paquetes.](assets/external_account_create_exported.png)

1. En la sección **[!UICONTROL Detalles]**, configure el acceso a la cuenta especificando las credenciales según el tipo de cuenta externa elegida. [Más información](#bounce)

1. Haga clic en **[!UICONTROL Probar conexión]** para comprobar que la configuración es correcta.

1. En el menú **[!UICONTROL Más...]**, duplique o elimine la cuenta externa.

   ![Captura de pantalla que muestra el menú Más con opciones para duplicar o eliminar la cuenta externa.](assets/external_account_create_4.png)

1. Una vez completada la configuración, haz clic en **[!UICONTROL Guardar]**.

## Cuentas externas específicas de la campaña {#campaign-specific}

Según el tipo de cuenta externa que haya seleccionado, siga los pasos a continuación para configurar las opciones de la cuenta.

### Correos electrónicos rechazados (POP3) {#bounce}

>[!AVAILABILITY]
>
> Actualmente, OAuth 2.0 no es compatible.

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

### Enrutamiento {#routing}

Para configurar una cuenta externa específica para envíos externos, siga los pasos a continuación.

1. Cree una cuenta externa. [Más información](../administration/external-account.md#create-ext-account)

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

### Instancia de ejecución {#instance-exec}

Si tiene una arquitectura segmentada, identifique las instancias de ejecución asociadas a la instancia de control y establezca conexiones entre ellas. Las plantillas de mensajes transaccionales se implementan en la instancia de ejecución.

![Captura de pantalla que muestra los campos de configuración de cuenta externa de la instancia de ejecución.](assets/external_account_exec.png)

Para configurar la cuenta externa **[!UICONTROL Execution instance]**:

* **[!UICONTROL URL]**: URL del servidor donde está instalada la instancia de ejecución.

* **[!UICONTROL Cuenta]** - Nombre de la cuenta, que coincide con el Agente del centro de mensajes definido en la carpeta del operador.

* **[!UICONTROL Contraseña]**: contraseña de la cuenta tal como se define en la carpeta del operador.

* **[!UICONTROL Método]** - Elija entre servicio Web o acceso de datos federado (FDA).

  Para FDA, seleccione su cuenta de FDA. Tenga en cuenta que la conexión de Campaign a sistemas externos está restringida a usuarios avanzados y solo está disponible desde la consola del cliente. [Más información](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Crear flujo de trabajo de archivado]**: para cada instancia de ejecución registrada en el Centro de mensajes, independientemente de si tiene una o varias instancias, cree un flujo de trabajo de archivado independiente para cada cuenta externa asociada a la instancia de ejecución.