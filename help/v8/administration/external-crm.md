---
title: Administrar cuenta externa
description: Obtenga información sobre cómo configurar cuentas externas de CRM
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 3%

---

# Cuenta externa de CRM {#external-crm}

Utilice una cuenta externa de tipo CRM para conectar Adobe Campaign con una base de datos de terceros.

Los ajustes de configuración de esta cuenta externa dependen del motor de base de datos específico al que se conecte. En las secciones siguientes se proporcionan instrucciones detalladas de configuración para cada base de datos admitida.

## Microsoft Dynamics CRM

La cuenta externa Microsoft Dynamics CRM permite conectar la instancia de Campaign a la base de datos externa Microsoft Dynamics CRM.

En la interfaz de usuario web de Adobe Campaign, configure la cuenta externa de Microsoft Dynamics CRM.

1. [Cree su cuenta externa](external-account.md) y seleccione **[!UICONTROL Base de datos externa]** como **[!UICONTROL Tipo]** de su cuenta externa y Microsoft Dynamics CRM como **[!UICONTROL Tipo de proveedor]**.

1. Haga clic en **[!UICONTROL Crear]**.

1. Para configurar la cuenta externa **[!UICONTROL Microsoft Dynamics CRM]**, rellene los campos siguientes:

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Microsoft Dynamics CRM.](assets/crm-microsoft-1.png)

   +++ Para el tipo de OAuth de CRM: Credenciales de contraseña

   * **[!UICONTROL Servidor]**: escriba la dirección URL del servidor de Microsoft CRM.

     Para localizar la URL de Microsoft CRM Server, inicie sesión en su cuenta de Microsoft Dynamics CRM, seleccione Dynamics 365 y, a continuación, abra la aplicación. La dirección URL del servidor se muestra en la barra de direcciones del explorador, por ejemplo:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Cuenta]**: especifique la cuenta usada para iniciar sesión en Microsoft CRM.

   * **[!UICONTROL Contraseña]**: escriba la contraseña asociada a la cuenta especificada.

   * **[!UICONTROL Identificador de cliente]**: escriba el identificador de cliente encontrado en el portal de administración de Microsoft Azure.

   * **[!UICONTROL CRM version]**: Elija Dynamics CRM 365 CRM version.

   +++

   </br>

   +++ Para el tipo de autenticación de CRM: Certificado

   * **[!UICONTROL Servidor]**: escriba la dirección URL del servidor de Microsoft CRM.

     Para localizar la URL de Microsoft CRM Server, inicie sesión en su cuenta de Microsoft Dynamics CRM, seleccione Dynamics 365 y, a continuación, abra la aplicación. La dirección URL del servidor se muestra en la barra de direcciones del explorador, por ejemplo:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Clave privada(codificada en Base64)]**: proporcione la clave privada codificada en formato Base64.

     Para ello, puede utilizar la ayuda de un codificador Base64 o utilizar la línea de comandos `base64 -w0 private.key` para Linux.

   * **[!UICONTROL Identificador de clave personalizada]**: escriba el identificador de clave personalizada usado para su certificado.

   * **[!UICONTROL ID de clave]**: escriba el ID de clave asociado con el certificado.

   * **[!UICONTROL Identificador de cliente]**: escriba el identificador de cliente encontrado en Microsoft Azure Management

   * **[!UICONTROL CRM version]**: Elija Dynamics CRM 365 CRM version.

   +++

1. Después de configurar la conexión, acceda al **[!UICONTROL Asistente para la configuración de Microsoft CRM]** para generar la lista de tablas de Microsoft CRM.

   Haga clic en **[!UICONTROL Siguiente]** para seleccionar las tablas necesarias.

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Microsoft Dynamics CRM.](assets/crm-microsoft-2.png)

1. Seleccione las tablas de Microsoft CRM que desea recuperar o agregue una tabla remota especificando **[!UICONTROL Table label]** y **[!UICONTROL Table internal name]**; a continuación, habilite la opción **[!UICONTROL Selected]**.

   Haga clic en **[!UICONTROL Next]**.

1. Haga clic en **[!UICONTROL Iniciar]** para empezar a crear el esquema de Microsoft CRM basado en las tablas seleccionadas.

1. Siga las instrucciones que aparecen en pantalla para insertar páginas del historial de marketing y la administración de suscripciones de Adobe Campaign directamente en Microsoft Dynamics CRM.

1. Haga clic en **[!UICONTROL Mostrar direcciones URL del historial de marketing]** para ver las direcciones URL para integrar páginas del historial de marketing o en **[!UICONTROL Mostrar direcciones URL para suscripciones de posibles clientes]** para ver las direcciones URL para integrar páginas de Administración de suscripción.

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Microsoft Dynamics CRM.](assets/crm-microsoft-3.png)

1. Haga clic en **[!UICONTROL Guardar]** una vez que su cuenta externa de Microsoft CRM esté configurada.

1. Una vez creada la cuenta externa, puede hacer clic en **[!UICONTROL Sincronizar enumeraciones...]** para sincronizar las enumeraciones automáticamente desde Microsoft CRM a la interfaz de usuario web de Adobe Campaign.

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Microsoft CRM CRM.](assets/crm-microsoft-4.png)

1. Seleccione la enumeración de Adobe Campaign que coincida con la enumeración de Microsoft CRM.

   Para reemplazar valores de Adobe Campaign con valores de Microsoft CRM, habilite la opción **[!UICONTROL Reemplazar]**.

## Salesforce {#salesforce}

Para configurar la cuenta externa de Salesforce para que funcione con Adobe Campaign, debe proporcionar los siguientes detalles:

1. [Cree su cuenta externa](external-account.md) y seleccione **[!UICONTROL Base de datos externa]** como **[!UICONTROL Tipo]** de su cuenta externa y Salesforce.com como **[!UICONTROL Tipo de proveedor]**.

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Salesforce.](assets/crm-salesforce-1.png)

1. Haga clic en **[!UICONTROL Crear]**.

1. Para configurar la cuenta externa **[!UICONTROL Salesforce]**, rellene los campos siguientes:

   * **[!UICONTROL Tipo de autenticación de CRM]**: **[!UICONTROL Credenciales de contraseña]** o **[!UICONTROL Credenciales]**

   * **[!UICONTROL Cuenta]**: Cuenta utilizada para iniciar sesión en Salesforce CRM.

   * **[!UICONTROL Contraseña]**: escriba la contraseña asociada a la cuenta especificada.

   * **[!UICONTROL Token de seguridad]**: escriba el token de seguridad de Salesforce asociado a la cuenta.

   * **[!UICONTROL Versión de API]**: Elija la versión 49.

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Salesforce.](assets/crm-salesforce-2.png)

1. Abra el **[!UICONTROL Asistente para la configuración de Salesforce CRM]** para generar la lista de tablas de Salesforce CRM y haga clic en **[!UICONTROL Siguiente]**.

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Salesforce CRM.](assets/crm-salesforce-3.png)

1. Seleccione las tablas de Salesforce que desee recuperar o agregue una tabla remota escribiendo **[!UICONTROL Table label]** y **[!UICONTROL Table internal name]**; a continuación, habilite la opción **[!UICONTROL Selected]**.

   Haga clic en **[!UICONTROL Next]**.

1. Haga clic en **[!UICONTROL Iniciar]** para empezar a crear el esquema de Salesforce CRM basado en las tablas seleccionadas.

1. Haga clic en **[!UICONTROL Asistente para la creación de vínculos de Salesforce...]** para generar los vínculos web en Salesforce.

   A continuación, haga clic en **[!UICONTROL Siguiente]** para recuperar los vínculos web de **Posibles clientes** y **Contactos** de Salesforce.

1. Seleccione los vínculos que desea exportar a la lista de vínculos web de Salesforce.

1. Siga las instrucciones que aparecen en pantalla para insertar las páginas **Historial de marketing** y **Administración de suscripciones** de la interfaz de usuario web de Adobe Campaign en Salesforce CRM.

1. Haga clic en **[!UICONTROL Guardar]** una vez que su cuenta externa de Salesforce CRM esté configurada.

1. Una vez creada la cuenta externa, puede hacer clic en **[!UICONTROL Sincronizar enumeraciones...]** para sincronizar las enumeraciones automáticamente de Salesforce a la interfaz de usuario web de Adobe Campaign.

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Salesforce CRM.](assets/crm-salesforce-4.png)

1. Seleccione la enumeración Adobe Campaign que coincida con la enumeración Salesforce.

   Para reemplazar valores Adobe Campaign por valores Salesforce, habilite la opción **[!UICONTROL Reemplazar]**.

   ![Captura de pantalla que muestra los campos de configuración de cuenta externa de Salesforce CRM.](assets/crm-salesforce-5.png)

