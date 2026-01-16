---
audience: end-user
title: Administración de permisos en la interfaz de usuario web de Campaign
description: Más información sobre los permisos en la interfaz de usuario web de Campaign
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: 692a9badf72e465791e6f964d02753e7f1a25713
workflow-type: ht
source-wordcount: '296'
ht-degree: 100%

---

# Permisos {#permissions}

Cada usuario de Adobe Campaign tiene permisos y restricciones específicos en la aplicación. El usuario puede pertenecer a un grupo de operadores y heredar los permisos del grupo.

Según sus permisos, un operador puede hacer lo siguiente:

* Acceder a determinadas funciones
* Acceder a determinados datos
* Acceder a determinadas acciones (crear, modificar, eliminar)

Los procedimientos detallados para configurar los permisos en Adobe Campaign están disponibles en la [documentación de la versión 8 Adobe Campaign (consola)](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Permisos de las carpetas {#folder-permissions}

En función de sus derechos, puede ver y administrar permisos en las carpetas en la **[!UICONTROL Configuración de carpetas]**.

A continuación se muestra un ejemplo de una carpeta de envío:

![Ejemplo de configuración de carpetas en Adobe Campaign](assets/folder_settings.png){zoomable="yes"}

En la sección **[!UICONTROL Seguridad]** de la **[!UICONTROL Configuración de carpetas]**, puede ver y administrar (añadir o eliminar) operadores o grupos que tengan acceso a la carpeta.

![Ejemplo de configuración de seguridad de carpetas en Adobe Campaign](assets/folder_security.png){zoomable="yes"}

Puede hacer clic directamente en los permisos y cambiarlos entre **[!UICONTROL Permitido]** o **[!UICONTROL Denegado]**.

![Ejemplo de permisos denegados en la configuración de seguridad de carpetas](assets/folder_security_denied.png){zoomable="yes"}

>[!NOTE]
>
>No debería poder crear un objeto para el que no tenga al menos una carpeta con derechos de escritura.
>
>No necesita ser administrador para crear fragmentos, pero debe tener derechos de escritura en al menos una carpeta “Fragmento visual de contenido”. De lo contrario, no podrá crear un fragmento visual.

Si la opción **[!UICONTROL Propagar]** está habilitada, todos los permisos definidos para una carpeta se aplican a todas sus subcarpetas. Estos permisos pueden anularse para cada subcarpeta.

Si la opción **[!UICONTROL Carpeta del sistema]** está habilitada, el acceso está permitido a todos los operadores, independientemente de sus permisos.

También puede [administrar los permisos de las carpetas en la consola de Adobe Campaign](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Todos los permisos de la interfaz de usuario web de Campaign se sincronizan con los permisos de la consola del cliente de Campaign.