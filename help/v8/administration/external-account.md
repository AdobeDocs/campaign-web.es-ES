---
title: Administrar cuenta externa
description: Obtenga información sobre cómo configurar cuentas externas
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 21%

---

# Administración de cuentas externas {#external-accounts}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Creación de cuentas externas"
>abstract="Como administrador de Campaign, ahora puede configurar nuevas conexiones con sistemas externos desde la interfaz de usuario web de Campaign. También puede ver, actualizar y administrar cuentas externas existentes."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

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

## Cuentas externas de integración de soluciones de Adobe

### Adobe Experience Cloud

Para conectarse a la consola de Adobe Campaign mediante un Adobe ID, debe configurar la cuenta externa de Adobe Experience Cloud (MAC).

![Captura de pantalla que muestra los campos de configuración de cuenta externa de Adobe Experience Cloud MAC.](assets/external-MAC.png)

* **[!UICONTROL Servidor IMS]**

  URL del servidor IMS. Asegúrese de que las instancias de ensayo y de producción indiquen el mismo punto final de producción IMS.

* **[!UICONTROL Ámbito de IMS]**

  Los ámbitos definidos aquí deben ser un subconjunto de los que proporciona IMS.

* **[!UICONTROL Identificador de cliente IMS]**

  ID de su cliente IMS.

* **[!UICONTROL Secreto de cliente IMS]**

  Credencial del secreto de su cliente IMS.

* **[!UICONTROL Callback server]**

  Acceso URL de su instancia de Adobe Campaign.

* **[!UICONTROL IMS organization ID]**

  ID de su organización. Para encontrar su ID de organización, consulte [esta página](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=es){target=_blank}.

* **[!UICONTROL Máscara de asociación]**

  Sintaxis que permitirá nombres de configuración en Enterprise Dashboard para sincronizar con los grupos en Adobe Campaign.

* **[!UICONTROL Servidor]**

  URL de su instancia de Adobe Experience Cloud.

* **[!UICONTROL Tenant]**

  Nombre su inquilino de Adobe Experience Cloud.

## Transferir datos a cuentas externas

### Amazon Simple Storage Service (S3) {#amazon-simple-storage-service--s3--external-account}

El conector de Amazon Simple Storage Service (S3) se puede utilizar para importar o exportar datos a Adobe Campaign. Se puede configurar en una actividad de flujo de trabajo. Para obtener más información, consulte [esta página](https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/design-workflows/transfer-file){target=_blank}.

![](assets/external-AWS.png)

Al configurar esta nueva cuenta externa, debe proporcionar los siguientes detalles:

* **[!UICONTROL AWS S3 Account Server]**

  La URL del servidor debe completarse de la siguiente manera:

  `  <S3bucket name>.s3.amazonaws.com/<s3object path>`


* **[!UICONTROL AWS access key ID]**

  Para saber dónde encontrar el ID de clave de acceso de AWS, consulte [esta página](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys).

* **[!UICONTROL Secret access key to AWS]**

  Para saber dónde encontrar la clave de acceso secreta a AWS, consulte [esta página](https://aws.amazon.com/fr/blogs/security/wheres-my-secret-access-key/).

* **[!UICONTROL AWS Region]**

  Para obtener más información sobre la región AWS, consulte esta [página](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/).

* La casilla de verificación **[!UICONTROL Use server side encryption]** permite almacenar el archivo en modo codificado S3.

Para saber dónde encontrar el ID de clave de acceso y la clave de acceso secreta, consulte la [documentación](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys) de los servicios web de Amazon.

### Azure Blob Storage {#azure-blob-external-account}

La cuenta externa **[!UICONTROL Azure Blob Storage]** se puede usar para importar o exportar datos a Adobe Campaign mediante una actividad de flujo de trabajo **[!UICONTROL Transferir archivo]**. Para obtener más información, consulte [esta sección](https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/design-workflows/transfer-file){target=_blank}.

![](assets/external-azure.png)

Para configurar la cuenta externa de **[!UICONTROL Azure]** para que funcione con Adobe Campaign, debe proporcionar los siguientes detalles:

* **[!UICONTROL Servidor]**

  URL del servidor de Azure Blob Storage.

* **[!UICONTROL Cifrado]**

  Tipo de cifrado elegido entre **[!UICONTROL None]** o **[!UICONTROL SSL]**.

* **[!UICONTROL Tecla de acceso]**

  Para saber dónde encontrar su **[!UICONTROL clave de acceso]**, consulte esta [página](https://docs.microsoft.com/en-us/azure/storage/common/storage-account-keys-manage?tabs=azure-portal).

## Hadoop

La cuenta externa Hadoop permite conectar la instancia de Campaign a la base de datos externa Hadoop. Puede obtener más información sobre Hadoop en [Documentación de la consola de Campaign V7](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/accessing-external-database/configure-fda/config-databases/configure-fda-hadoop){target=_blank}.

![Captura de pantalla que muestra la configuración de la cuenta externa de Hadoop.](assets/external-hadoop.png)

* **[!UICONTROL Servidor]**

  URL del servidor de almacenamiento de Hadoop.

* **[!UICONTROL Cuenta]**

  Nombre de la cuenta del servidor de Hadoop.
