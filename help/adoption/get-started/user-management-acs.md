---
title: Migración de usuarios técnicos a la consola de Adobe Developer
description: Obtenga información sobre cómo migrar la administración de acceso de usuarios de Campaign Standard a Campaign V8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: 31befa42b04bef1a2777df9f2bd494481ccf67cd
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 2%

---

# Administración de acceso de usuario de Campaign Standard a Campaign V8 {#user-management-acs}

Tanto Adobe Campaign Standard como Adobe Campaign V8 permiten a los usuarios definir y administrar permisos para distintos usuarios/operadores. Estos permisos constan de derechos específicos que conceden a los usuarios acceso a varias funciones del producto. Sin embargo, los dos productos utilizan enfoques e implementaciones diferentes para administrar el acceso de los usuarios.

En Adobe Campaign Standard y Campaign V8 se utilizan los siguientes conceptos para lograr la administración del acceso de los usuarios:

| Campaign Standard | Campaign V8 |
|---------|----------|
| Usuario | Operador |
| Función | Derecho con nombre |
| Grupo de seguridad | Grupo de operadores |
| Entidades organizativas | Permiso de carpeta |

## Enfoque de migración del grupo de seguridad al grupo de operadores

>[!CAUTION]
>
>Las capacidades de estas funciones/derechos asignados pueden variar en la implementación, lo que podría causar problemas de autorización (por ejemplo, elevación de privilegios o interrupciones en la funcionalidad). Recomendamos a los usuarios que revisen estas asignaciones después de la transición para garantizar un control de acceso adecuado. [Más información sobre los permisos](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

En la tabla siguiente se describe el método de migración para grupos de funciones de usuario al realizar la transición de Adobe Campaign Standard a Campaign V8. En Campaign Standard, se usa un **grupo de seguridad**, denominado **grupo de operadores** en Campaign V8, para asignar un conjunto de funciones a un usuario. Aunque algunos grupos de operadores/grupos de seguridad están disponibles de forma predeterminada, los usuarios pueden crear grupos nuevos o modificar los existentes si es necesario.

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **Terminología**  | Grupo de seguridad | Grupo de operadores |

Tanto en Adobe Campaign Standard como en Campaign V8, **los grupos de seguridad** y **los grupos de operadores** están asignados a perfiles de producto en Admin Console. Si desea asignar un **grupo de seguridad** o **grupo de operadores** a un usuario, puede vincular el **perfil de producto** correspondiente en Admin Console. Esta asociación se sincroniza cuando el usuario inicia sesión. [Más información sobre el perfil del producto](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Grupo de seguridad de Campaign Standard** | **Grupo de operadores de Campaign V8** |
|----------|---------|
| Administradores | Administradores |
| Supervisores de envío | Administradores |
| Supervisores de flujo de trabajo | Supervisores de flujo de trabajo  |

## Enfoque de migración de funciones de usuario a derechos asignados

>[!CAUTION]
>
>Durante la migración de Adobe Campaign Standard a Campaign V8, los usuarios con la función **Modelo de datos** pero no la función **Administración** obtendrán automáticamente acceso a **Administración**, ya que la creación de esquemas en Campaign V8 requiere derechos de administración. Para evitarlo, quite la función **Modelo de datos** antes de la migración.

En Adobe Campaign Standard, el término **función de usuario** se denomina **derecho asignado** en Campaign V8. La tabla siguiente describe la terminología utilizada para **Derechos asignados** en Campaign V8 correspondientes a **Funciones de usuario** en Campaign Standard.

| **Función de usuario de Campaign Standard** | **Campaña V8 con nombre correcto** | **Descripción**  |
|----------|---------|---------|
| Administración | Administración | El usuario con derecho de administración tiene acceso completo a la instancia. |
| Modelo de datos  | Administración | El derecho para ejecutar publicaciones y crear recursos personalizados. Funcionalidad relacionada con la creación de esquemas disponible para el administrador en Campaign V8.  |
| Entrega  | Administration  | Derecho a aprobar los envíos analizados previamente.  |
| Exportar | Exportar | Derecho a exportar datos.  |
| Acceso a archivos  | Acceso a archivos  | Derecho a aprobar los envíos analizados previamente.  |
| Importación genérica  | Importar  | Derecho para importar datos genéricos |
| Preparación de envíos | Preparación de envíos | Derecho a crear, modificar, preparar y eliminar entregas.  |
| Ejecución de script SQL | Ejecución de script SQL | Derecho a ejecutar cualquier comando SQL directamente en la base de datos. |
| Inicio de entregas  | Inicio de entregas  | Derecho a aprobar los envíos analizados previamente.  |
| Ejecución de comandos del sistema | Ejecución del programa | Derecho a ejecutar comandos del sistema en el servidor. |
| Flujo de trabajo | Flujo de trabajo | Derecho para administrar la ejecución de flujos de trabajo: inicio, parada, pausa, etc. |

## Enfoque de migración desde la unidad organizativa

>[!CAUTION]
>
>Las unidades organizativas en Adobe Campaign Standard sin **All (all)** como elemento principal directo o indirecto no se migrarán a Campaign V8.
></br>
>A los usuarios de varios grupos de seguridad se les asigna la unidad organizativa del grupo de seguridad de mayor clasificación. Si varios grupos tienen unidades de nivel superior paralelas, el inicio de sesión está restringido en Campaign Standard, pero concede un acceso más amplio en Campaign v8 después de la migración, lo que podría escalar los privilegios. Para evitarlo, evite asignar usuarios a grupos de seguridad con unidades organizativas paralelas.

En Adobe Campaign Standard, la **unidad organizativa** t está asignada al modelo de jerarquía **Folder** existente en Campaign V8 para mantener un control de acceso similar. [Más información sobre la administración de carpetas](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **Terminología**  | Entidades organizativas | Carpeta |

## Enfoque de migración del programa

En la versión 8 de Campaign, **los programas** se representan como **carpetas**. Campaign V8 permite la creación de carpetas y restringir el acceso a ellas.

Mediante **Grupos** y **Derechos asignados**, se puede otorgar acceso a **Operadores** a **Carpetas** específicas dentro de la jerarquía de navegación, con la capacidad de asignar permisos de lectura, escritura y eliminación. [Más información sobre la administración de carpetas](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Dado que un **Programa** se trata como una **Carpeta** en Campaign V8, su acceso se puede administrar de la misma manera que cualquier otra carpeta. Después de la migración, los administradores de Campaign Standard pueden seguir estos pasos:

1. Desde el explorador, haga clic con el botón derecho en cualquier carpeta y seleccione **[!UICONTROL Propiedades...]**.

1. Vaya a la ficha **[!UICONTROL Seguridad]**.

1. Modifique los permisos del grupo de operadores según el modelo de acceso deseado. 

## Asignación de perfil de producto para acceder a las API de REST 

Para acceder a las API transaccionales desde la instancia de ejecución en Campaign V8, se requiere un nuevo **perfil de producto**, además de los perfiles de producto **Administrador** y **Centro de mensajes**. Este nuevo **perfil de producto** se agregará a las cuentas técnicas existentes o creadas previamente en Campaign Standard.

Después de la migración, los usuarios de Campaign Standard deben revisar sus **asignaciones de perfiles de producto** y asignar el **perfil de producto** correspondiente si no desean vincular sus **cuentas técnicas** al perfil de producto **Administrador**. Para integraciones futuras, recomendamos usar la versión 8 de Campaign **ID de inquilino** en la **URL de REST** en lugar de la versión anterior de Campaign Standard **ID de inquilino**.

## Migración del acceso a los recursos integrados de Campaign para los operadores de Campaign Standard

Los operadores migrados de Campaign Standard tendrán acceso de lectura a recursos integrados específicos en la versión 8 de Campaign.

## Grupos y funciones de seguridad no migrados {#non-migrated-groups-roles}

A continuación se muestra una lista de funciones de Campaign Standard que no se han transferido:

* Cuenta de retransmisión predeterminada 

* Push del centro de mensajes 

A continuación se muestra una lista de asignaciones de grupos de seguridad de Campaign Standard que no se han transferido.

* Agentes del centro de mensajes

* Agentes push del centro de mensajes

* Administradores de aplicaciones de Adobe Experience Manager

* Cuenta de retransmisión

Tenga en cuenta que las funciones personalizadas creadas y asignadas a usuarios en Adobe Campaign Standard no se migrarán a Campaign V8.
