---
title: Cuenta externa
description: Obtenga información sobre cómo configurar cuentas externas
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: bca2b133968d9392098e9b8b76d65e44d7e84645
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 27%

---

# Configuración de cuentas externas {#external-accounts}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Cuentas externas"
>abstract="Ahora puede conectarse a plataformas adicionales o personalizar las conexiones para adaptarlas al flujo de trabajo y crear fácilmente nuevas cuentas externas para satisfacer sus necesidades específicas y garantizar las transferencias de datos."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"


>[!AVAILABILITY]
>
> Tenga en cuenta que las cuentas externas actualmente solo están disponibles para correos rechazados (POP3) y la instancia de ejecución, con tipos de cuenta adicionales que se añadirán en el futuro.
> Las cuentas externas no admitidas creadas en la consola de Adobe Campaign están visibles en la interfaz de usuario web, pero no se pueden editar ni acceder a ellas.

Adobe Campaign incluye un conjunto de cuentas externas preconfiguradas para facilitar la integración con varios sistemas. Si necesita conectarse a plataformas adicionales o personalizar las conexiones para adaptarlas al flujo de trabajo, ahora puede crear fácilmente nuevas cuentas externas mediante la interfaz de usuario web para satisfacer sus necesidades específicas y garantizar transferencias de datos sin problemas.

## Creación de una cuenta externa {#create-ext-account}

Para crear una nueva cuenta externa, siga los pasos a continuación. La configuración detallada depende del tipo de cuenta externa.

1. En el menú del panel izquierdo, seleccione **[!UICONTROL Cuentas externas]** en **[!UICONTROL Administración]**.

1. Haga clic en **[!UICONTROL Crear cuenta externa]**.

   ![](assets/external_account_create_1.png)

1. Escriba su **[!UICONTROL Etiqueta]** y seleccione su Cuenta externa **[!UICONTROL Tipo]**.

   ![](assets/external_account_create_2.png)

1. Haga clic en **[!UICONTROL Crear]**.

1. Desde la lista desplegable **[!UICONTROL Opciones avanzadas]**, puede cambiar la ruta de acceso **[!UICONTROL Nombre interno]** o **[!UICONTROL Carpeta]** si es necesario.

   ![](assets/external_account_create_3.png)

1. Habilite **[!UICONTROL Exportado automáticamente]** si desea que los datos administrados por esta cuenta externa se exporten automáticamente.

1. Configure el acceso a la cuenta especificando las credenciales según el tipo de cuenta externa elegida.

1. Haga clic en **[!UICONTROL Probar la conexión]** para comprobar que la configuración es correcta

1. En el menú **[!UICONTROL Más...]**, duplique o elimine la cuenta externa.

   ![](assets/external_account_create_4.png)

1. Una vez completada la configuración, haz clic en **[!UICONTROL Guardar]**.

## Cuentas externas específicas de la campaña {#campaign-specific}

### Correos rechazados (POP3) {#bounce}

>[!AVAILABILITY]
>
> Actualmente, OAuth 2.0 no es compatible.

La cuenta externa Rebote de correo electrónico especifica la cuenta POP3 externa que se utiliza para conectarse al servicio de correo electrónico. Todos los servidores configurados para el acceso POP3 pueden recibir el correo electrónico devuelto.

![](assets/external_account_bounce.png)

Para configurar la cuenta externa **[!UICONTROL Bounce mails (POP3)]**:

* **[!UICONTROL Servidor]**

  URL del servidor POP3

* **[!UICONTROL Puerto]**

  Número de puerto de conexión POP3 (el puerto predeterminado es 110)

* **[!UICONTROL Cuenta]**

  Nombre del usuario

* **[!UICONTROL Contraseña]**

  Contraseña de cuenta de usuario

* **[!UICONTROL Cifrado]**

  Tipo de cifrado elegido entre:

   * De forma predeterminada (POP3 si es el puerto 110, POP3S si es el puerto 995)
   * POP3 que cambia a SSL después del envío de STARTTLS
   * POP3 no seguro (puerto 110 de forma predeterminada)
   * POP3 seguro sobre SSL (puerto 995 por defecto)

* **[!UICONTROL Función]**

  SOAP SOAP Correo electrónico entrante, cuando la cuenta externa está configurada para recibir correos electrónicos entrantes, o enrutador de, para gestionar solicitudes de.

### Instancia de ejecución{#instance-exec}

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
