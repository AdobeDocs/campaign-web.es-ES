---
title: Administrar cuenta externa
description: Obtenga información sobre cómo configurar cuentas externas
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 14%

---

# Administración de cuentas externas {#external-accounts}

>[!AVAILABILITY]
>
>* Actualmente, las cuentas externas solo están disponibles para las instancias de correos rechazados (POP3), Enrutamiento y Ejecución. En el futuro se agregarán tipos de cuenta adicionales.
>
>* Las cuentas externas no admitidas creadas en la consola de Adobe Campaign están visibles en la interfaz de usuario web, pero no se pueden editar ni acceder a ellas.

Adobe Campaign incluye un conjunto de cuentas externas preconfiguradas para facilitar la integración con varios sistemas. Si necesita conectarse a plataformas adicionales o personalizar las conexiones para adaptarlas al flujo de trabajo, ahora puede crear fácilmente nuevas cuentas externas mediante la interfaz de usuario web para satisfacer sus necesidades específicas y garantizar transferencias de datos sin problemas.

## Creación de una cuenta externa {#create-ext-account}

Para crear una nueva cuenta externa, siga los pasos a continuación. La configuración detallada depende del tipo de cuenta externa. [Más información](#campaign-specific)

1. En el menú del panel izquierdo, seleccione **[!UICONTROL Cuentas externas]** en **[!UICONTROL Administración]**.

1. Haga clic en **[!UICONTROL Crear cuenta externa]**.

   ![](assets/external_account_create_1.png)

1. Escriba su **[!UICONTROL Etiqueta]** y seleccione la cuenta externa **[!UICONTROL Tipo]**.

   >[!NOTE]
   >
   >La configuración para los tipos específicos de campaña se detalla en [esta sección](#campaign-specific).

   ![](assets/external_account_create_2.png)

1. Haga clic en **[!UICONTROL Crear]**.

1. En la lista desplegable **[!UICONTROL Opciones adicionales]**, puede cambiar la ruta de acceso **[!UICONTROL Nombre interno]** o **[!UICONTROL Carpeta]** si es necesario.

   ![](assets/external_account_create_3.png)

1. Habilite la opción **[!UICONTROL Exportado automáticamente en paquetes]** si desea que los datos que administra esta cuenta externa se exporten automáticamente. <!--Exported where??-->

   ![](assets/external_account_create_exported.png)

1. En la sección **[!UICONTROL Detalles]**, configure el acceso a la cuenta especificando las credenciales según el tipo de cuenta externa elegida. [Más información](#bounce)

1. Haga clic en **[!UICONTROL Probar conexión]** para comprobar que la configuración es correcta.

1. Desde el menú **[!UICONTROL Más...]**, puede duplicar o eliminar su cuenta externa.

   ![](assets/external_account_create_4.png)

1. Una vez completada la configuración, haz clic en **[!UICONTROL Guardar]**.

## Cuentas externas específicas de la campaña {#campaign-specific}

Según el tipo de cuenta externa que haya seleccionado, siga los pasos a continuación para configurar las opciones de la cuenta.

### Correos rechazados (POP3) {#bounce}

>[!AVAILABILITY]
>
> Actualmente, OAuth 2.0 no es compatible.

La cuenta externa Rebote de correos electrónicos especifica la cuenta POP3 externa que se utiliza para conectarse al servicio de correo electrónico. Todos los servidores configurados para el acceso POP3 pueden recibir el correo electrónico devuelto.

![](assets/external_account_bounce.png)

Para configurar la cuenta externa **[!UICONTROL Correos rechazados (POP3)]**, rellene los campos siguientes:

* **[!UICONTROL Servidor]** - URL del servidor POP3

* **[!UICONTROL Puerto]** - número de puerto de conexión POP3 (el puerto predeterminado es 110)

* **[!UICONTROL Cuenta]** - Nombre del usuario

* **[!UICONTROL Contraseña]** - Contraseña de la cuenta de usuario

* **[!UICONTROL Cifrado]** - Tipo de cifrado elegido entre:

   * De forma predeterminada (POP3 si es el puerto 110, POP3S si es el puerto 995)
   * POP3 que cambia a SSL después del envío de STARTTLS
   * POP3 no seguro (puerto 110 de forma predeterminada)
   * POP3 seguro sobre SSL (puerto 995 por defecto)

* SOAP SOAP **[!UICONTROL Función]** - Correo electrónico entrante, cuando la cuenta externa está configurada para recibir correos electrónicos entrantes o enrutadores de, para gestionar solicitudes de.

### Enrutamiento {#routing}

Para configurar una cuenta externa específica que se utilizará en los envíos externos, siga los pasos a continuación.

1. Cree una cuenta externa. [Más información](../administration/external-account.md#create-ext-account)

1. Seleccione el tipo **[!UICONTROL Routing]**.

   ![](assets/external-account-routing.png){zoomable="yes"}

1. Seleccione el canal deseado y haga clic en **[!UICONTROL Crear]**.

1. En la sección de la cuenta externa **[!UICONTROL Detalles]**, **[!UICONTROL Externo]** está seleccionado de forma predeterminada como **[!UICONTROL Modo de envío]**.

   ![](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Actualmente **[!UICONTROL External]** es el único modo disponible.

1. Para gestionar el proceso después de la ejecución de la entrega, puede externalizarlo a un flujo de trabajo de posprocesamiento. Para ello, debe crear un flujo de trabajo con una actividad [Señal externa](../workflows/activities/external-signal.md) y seleccionarla en el campo **[!UICONTROL Procesamiento posterior]**.

   ![](assets/external-account-post-processing.png){zoomable="yes"}

1. En el campo **[!UICONTROL Actividad]**, puede editar el nombre de la actividad de flujo de trabajo de posprocesamiento que se mostrará en los registros. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->


### Instancia de ejecución {#instance-exec}

Si tiene una arquitectura segmentada, debe identificar las instancias de ejecución asociadas con la instancia de control y establecer conexiones entre ellas. Las plantillas de mensajes transaccionales se implementan en la instancia de ejecución.

![](assets/external_account_exec.png)

Para configurar la cuenta externa **[!UICONTROL Execution instance]**:

* **[!UICONTROL URL]**

  URL del servidor en el que está instalada la instancia de ejecución.

* **[!UICONTROL Cuenta]**

  El nombre de la cuenta debe coincidir con el Agente del centro de mensajes definido en la carpeta del operador.

* **[!UICONTROL Contraseña]**

  Contraseña de la cuenta tal como se define en la carpeta del operador.

* **[!UICONTROL Método]**

  Elija entre servicio web o acceso de datos federado (FDA).
En el caso del método FDA, seleccione su cuenta de FDA. Tenga en cuenta que la conexión de Campaign a sistemas externos está restringida a usuarios avanzados y solo está disponible desde la consola del cliente. [Más información](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Crear flujo de trabajo de archivado]**

  Para cada instancia de ejecución registrada en el Centro de mensajes, independientemente de si tiene una o varias instancias, debe crear un flujo de trabajo de archivado independiente para cada cuenta externa asociada con la instancia de ejecución.
