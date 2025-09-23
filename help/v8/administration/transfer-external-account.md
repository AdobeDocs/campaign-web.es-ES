---
title: Administrar cuenta externa
description: Obtenga información sobre cómo configurar cuentas externas
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 29%

---

# Transferir datos a cuentas externas {#transfer-external-account}

## Amazon Simple Storage Service (S3) {#amazon-simple-storage-service--s3--external-account}

El conector de Amazon Simple Storage Service (S3) se puede utilizar para importar o exportar datos a Adobe Campaign. Se puede configurar en una actividad de flujo de trabajo. Para obtener más información, consulte [esta página](https://experienceleague.adobe.com/es/docs/campaign-web/v8/wf/design-workflows/transfer-file){target=_blank}.

![Captura de pantalla que muestra los campos de configuración de cuenta externa de Amazon Simple Storage Service S3.](assets/external-AWS.png)

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

## Azure Blob Storage {#azure-blob-external-account}

La cuenta externa **[!UICONTROL Azure Blob Storage]** se puede usar para importar o exportar datos a Adobe Campaign mediante una actividad de flujo de trabajo **[!UICONTROL Transferir archivo]**. Para obtener más información, consulte [esta sección](https://experienceleague.adobe.com/es/docs/campaign-web/v8/wf/design-workflows/transfer-file){target=_blank}.

![Captura de pantalla que muestra los campos de configuración de cuenta externa de Azure Blob Storage.](assets/external-azure.png)

Para configurar la cuenta externa de **[!UICONTROL Azure]** para que funcione con Adobe Campaign, debe proporcionar los siguientes detalles:

* **[!UICONTROL Servidor]**

  URL del servidor de Azure Blob Storage.

* **[!UICONTROL Cifrado]**

  Tipo de cifrado elegido entre **[!UICONTROL None]** o **[!UICONTROL SSL]**.

* **[!UICONTROL Tecla de acceso]**

  Para saber dónde encontrar su **[!UICONTROL clave de acceso]**, consulte esta [página](https://docs.microsoft.com/en-us/azure/storage/common/storage-account-keys-manage?tabs=azure-portal).

## SFTP

La cuenta externa SFTP permite configurar y probar el acceso a un servidor fuera de Adobe Campaign.

![Captura de pantalla que muestra los campos de configuración de la cuenta externa SFTP.](assets/ext-account-sftp.png)

Para configurar la cuenta externa **[!UICONTROL SFTP]**, rellene los campos siguientes:

* **[!UICONTROL Servidor]**

  Introduzca el nombre o la dirección del servidor SFTP.

* **[!UICONTROL Puerto]**

  Especifique el número de puerto de la conexión SFTP. El puerto predeterminado es 22.

* **[!UICONTROL Cuenta]**

  Introduzca el nombre de usuario utilizado para conectarse al servidor SFTP.

* **[!UICONTROL Contraseña]**

  Introduzca la contraseña de la cuenta SFTP.

* **[!UICONTROL Tipo de autenticación SFTP]**

  Elija el método para autenticarse con el servidor SFTP. Las opciones incluyen:

   * **[!UICONTROL Contraseña]**: realice la autenticación con la contraseña de la cuenta.

   * **[!UICONTROL Clave pública]**: realice la autenticación mediante un par de claves SSH (clave privada y pública).

Si se selecciona la autenticación de **[!UICONTROL clave pública]**, deben rellenarse los siguientes campos:

* **[!UICONTROL Archivo de clave privada]**

  Especifique el archivo de clave SSH privada utilizado para la autenticación.

* **[!UICONTROL Archivo de clave pública]**

  Especifique la clave SSH pública correspondiente registrada en el servidor SFTP.

* **[!UICONTROL Frase de contraseña de clave SSH]**

  Introduzca la frase de contraseña para descifrar la clave privada si está protegida.

## HTTP

La cuenta externa HTTP permite configurar y probar el acceso a un servidor fuera de Adobe Campaign.

![Captura de pantalla que muestra los campos de configuración de cuenta externa HTTP.](assets/ext-account-http.png)

Para configurar la cuenta externa **[!UICONTROL HTTP]**, rellene los campos siguientes:

* **[!UICONTROL Servidor]**

  Introduzca el nombre o la dirección del servidor HTTP.

* **[!UICONTROL Puerto]**

  Especifique el número de puerto de la conexión HTTP. El puerto predeterminado es 80.

* **[!UICONTROL Cuenta]**

  Introduzca el nombre de usuario para la autenticación.

* **[!UICONTROL Contraseña]**

  Introduzca la contraseña asociada a la cuenta de usuario.

* **[!UICONTROL Tipo de autenticación SFTP]**

  Seleccione el tipo de autenticación para la conexión. Las opciones incluyen:

   * Contraseña
   * Clave pública

Si está usando la autenticación de **[!UICONTROL clave pública]**, en el menú **[!UICONTROL Autenticación de clave pública]**, introduzca los valores necesarios para:

* **[!UICONTROL Contraseña]**: La frase de contraseña que protege la clave privada, si corresponde.

* **[!UICONTROL Clave privada]**: La clave privada utilizada para autenticar la cuenta de Snowflake.



## FTP

La cuenta externa de FTP permite configurar y probar el acceso a un servidor fuera de Adobe Campaign.

![Captura de pantalla que muestra los campos de configuración de cuenta externa de FTP.](assets/ext-account-ftp.png)

Para configurar la cuenta externa **[!UICONTROL FTP]**, rellene los campos siguientes:

* **[!UICONTROL Servidor]**

  Introduzca el nombre o la dirección del servidor FTP.

* **[!UICONTROL Puerto]**

  Especifique el número de puerto de la conexión FTP. El puerto predeterminado es 21.

* **[!UICONTROL Cuenta]**

  Introduzca el nombre de usuario para la autenticación.

* **[!UICONTROL Contraseña]**

  Introduzca la contraseña asociada a la cuenta de usuario.

* **[!UICONTROL Cifrado]**

  Seleccione el tipo de cifrado para la conexión. Las opciones incluyen:

   * De forma predeterminada
   * POP3 + STARTTLS
   * POP3 no seguro
   * POP3 secure