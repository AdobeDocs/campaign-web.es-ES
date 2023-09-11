---
audience: end-user
title: Administración de permisos en la web de Campaign
description: Obtenga más información sobre los permisos en la versión 8 de la web de Campaign
badge: label="Beta"
source-git-commit: 5c7d60b3f59de2a5176a55d9556a3f1c6d2a7651
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---


# Acceso y permisos {#access-and-permissions}

El control de acceso puede restringir el acceso a objetos y datos de listas principales, como envíos, destinatarios o flujos de trabajo. Estas restricciones también se aplican en el árbol de navegación del Explorador. Además, necesita permisos para crear, eliminar, duplicar y editar objetos desde la interfaz de usuario. El control de acceso se administra en la consola del cliente. Todos los permisos de la web de Campaign se sincronizan con los permisos de la consola del cliente de Campaign. Solo los administradores de Campaign pueden definir y modificar permisos de usuario. Obtenga más información sobre los permisos de usuario en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html){target="_blank"}.

A medida que navega por la interfaz de usuario web de Campaign, puede acceder a datos, objetos y funcionalidades en función de sus permisos. Por ejemplo, si no tiene permisos de acceso a una carpeta, no podrá verla. Los permisos también afectan a la administración de objetos y datos. Sin permisos de escritura para una carpeta específica, no se puede crear una entrega en esa carpeta, aunque se pueda ver en la interfaz de usuario.

## Ver permisos {#view-permissions}

Desde el **Explorer**, puede examinar los permisos de cada carpeta. Estos permisos se establecen en la consola del cliente y se utilizan para organizar y controlar el acceso a los datos de Campaign.


Para ver los permisos de una carpeta, siga estos pasos:

1. Desde el **Explorer** menú de navegación de la izquierda, seleccione una carpeta.
1. Haga clic en los tres puntos de la esquina superior derecha y seleccione **Permisos de carpeta**.

   ![](assets/permissions-view-menu.png){width="70%" align="left" zoomable="yes"}

1. Compruebe los detalles en la pantalla, como se muestra a continuación:

   ![](assets/permissions-view-screen.png){width="70%" align="left" zoomable="yes"}

   Un grupo o un operador puede tener permisos de lectura, escritura o eliminación sobre los datos almacenados en la carpeta seleccionada.

   Si la variable **Propagación** está activada, todos los permisos definidos para una carpeta se aplican a todas sus subcarpetas. Estos permisos se pueden sobrecargar para cada subcarpeta.

   Si la variable **Carpeta del sistema** está activada, el acceso está permitido a todos los operadores, independientemente de sus permisos.

Obtenga más información acerca de los permisos de carpeta en [Documentación de Campaign v8 (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html){target="_blank"}.


## Trabajo con carpetas {#folders}

Puede crear, cambiar el nombre, reordenar y mover carpetas para organizar los componentes y los datos. También puede eliminar carpetas desde el mismo menú.

>[!CAUTION]
>
>Al eliminar una carpeta, también se eliminan todos los datos almacenados en ella.

Para crear una carpeta, siga estos pasos:

1. Desde el **Explorer** menú de navegación de la izquierda, seleccione una carpeta.
1. Haga clic en los tres puntos de la esquina superior derecha y elija **Crear nueva subcarpeta**.
1. Introduzca el nombre de la carpeta y guárdela.

   ![](assets/create-new-subfolder.png){width="70%" align="left" zoomable="yes"}

   La carpeta se agrega como una subcarpeta de la carpeta actual. Navegue hasta esa nueva carpeta para crear componentes directamente en ella. También puede crear un componente a partir de cualquier carpeta y guardarlo en esa nueva carpeta, desde el **Opciones adicionales** de las propiedades, como se muestra a continuación para una entrega:

   ![](assets/delivery-properties-folder.png){width="70%" align="left" zoomable="yes"}

