---
title: Migración de usuarios técnicos a la consola de Adobe Developer
description: Obtenga información sobre cómo migrar la administración de acceso de usuarios de Campaign Standard a Campaign v8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: 9354c07f173f67c23ce64e591f869bdd374c3334
workflow-type: tm+mt
source-wordcount: '1403'
ht-degree: 2%

---

# Administración de acceso de usuario de Campaign Standard a Campaign v8 {#user-management-acs}

Tanto Adobe Campaign Standard como Adobe Campaign v8 permiten a los usuarios definir y administrar permisos para distintos usuarios/operadores. Estos permisos constan de derechos específicos que conceden a los usuarios acceso a varias funciones del producto. Sin embargo, los dos productos utilizan enfoques e implementaciones diferentes para administrar el acceso de los usuarios.

En Adobe Campaign Standard y Campaign v8 se utilizan los siguientes conceptos para lograr la administración del acceso de los usuarios:

| Campaign Standard | Campaign v8 |
|---------|----------|
| Usuario | Operador |
| Función | Derecho con nombre |
| Grupo de seguridad | Grupo de operadores |
| Entidades organizativas | Permiso de carpeta |

## Enfoque de migración del grupo de seguridad al grupo de operadores

>[!IMPORTANT]
>
>Las capacidades de estas funciones/derechos asignados pueden variar en la implementación, lo que podría causar problemas de autorización (por ejemplo, elevación de privilegios o interrupciones en la funcionalidad). Recomendamos a los usuarios que revisen estas asignaciones después de la transición para garantizar un control de acceso adecuado. [Más información sobre los permisos](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

En la tabla siguiente se describe el método de migración para grupos de funciones de usuario al realizar la transición de Adobe Campaign Standard a Campaign v8. En Campaign Standard, se usa un **grupo de seguridad**, denominado **grupo de operadores** en Campaign v8, para asignar un conjunto de funciones a un usuario. Aunque algunos grupos de operadores/grupos de seguridad están disponibles de forma predeterminada, los usuarios pueden crear grupos nuevos o modificar los existentes si es necesario.

| | **Campaign Standard** | **Versión 8 de Campaign** |
|---------|----------|---------|
| **Terminología**  | Grupo de seguridad | Grupo de operadores |

Tanto en Adobe Campaign Standard como en Campaign v8, **los grupos de seguridad** y **los grupos de operadores** están asignados a perfiles de producto en Admin Console. Si desea asignar un **grupo de seguridad** o **grupo de operadores** a un usuario, puede vincular el **perfil de producto** correspondiente en Admin Console. Esta asociación se sincroniza cuando el usuario inicia sesión. [Más información sobre el perfil del producto](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Grupo de seguridad de Campaign Standard** | **Grupo de operadores de Campaign v8** |
|----------|---------|
| Administradores | Administradores |
| Supervisores de envío | Administradores |
| Supervisores de flujo de trabajo | Supervisores de flujo de trabajo  |

## Enfoque de migración de funciones de usuario a derechos asignados

>[!IMPORTANT]
>
>Durante la migración de Adobe Campaign Standard a Campaign v8, los usuarios con la función **Modelo de datos** pero no la función **Administración** obtendrán automáticamente acceso a **Administración**, ya que la creación de esquemas en Campaign v8 requiere derechos de administración. Para evitarlo, quite la función **Modelo de datos** antes de la migración.

En Adobe Campaign Standard, el término **función de usuario** se denomina **derecho asignado** en Campaign v8. La tabla siguiente describe la terminología utilizada para **Derechos asignados** en Campaign v8 correspondientes a **Funciones de usuario** en Campaign Standard.

| **Función de usuario de Campaign Standard** | **Campaña v8 con nombre correcto** | **Descripción**  |
|----------|---------|---------|
| Administración | Administración | El usuario con derecho de administración tiene acceso completo a la instancia. |
| Modelo de datos  | Administración | El derecho para ejecutar publicaciones y crear recursos personalizados. Funcionalidad relacionada con la creación de esquemas disponible para el administrador en Campaign v8.  |
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

>[!IMPORTANT]
>
>Las unidades organizativas en Adobe Campaign Standard sin **All (all)** como elemento principal directo o indirecto no se migrarán a Campaign v8.
></br>
>A los usuarios de varios grupos de seguridad se les asigna la unidad organizativa del grupo de seguridad de mayor clasificación. Si varios grupos tienen unidades de nivel superior paralelas, el sistema selecciona la unidad organizativa del usuario en Campaign Standard y el usuario solo tendría acceso a la unidad organizativa seleccionada por el sistema y a sus elementos secundarios. En Campaign v8 después de la migración, el usuario tendría acceso a **todas las unidades organizativas asignadas y a sus elementos secundarios**, lo que podría escalar privilegios. Para evitarlo, evite asignar usuarios a grupos de seguridad con unidades organizativas paralelas. Más información sobre la [asignación paralela de unidades organizativas](#parallel-assignments).


En Adobe Campaign Standard, la **unidad organizativa** está asignada al modelo de jerarquía **Folder** existente en Campaign v8 para mantener un control de acceso similar. [Más información acerca de la administración de carpetas](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Versión 8 de Campaign** |
|---------|----------|---------|
| **Terminología**  | Entidades organizativas | Carpeta |


### Acerca de la asignación de unidades organizativas paralelas {#parallel-assignments}

Una asignación de unidad organizativa paralela se produce cuando un usuario tiene acceso a varias unidades (asignadas a través de grupos de seguridad) que existen en ramas independientes de la jerarquía sin tener acceso a una unidad organizativa principal común. Esto crea un riesgo de seguridad durante la migración.

Por ejemplo, considere la siguiente jerarquía de unidades organizativas:

![Diagrama de muestra de asignación de unidades organizativas paralelas](assets/do-not-localize/parallel-org-units-sample.png){width="50%" zoomable="yes"}

Una asignación sin unidades organizativas paralelas tendría el siguiente aspecto:

![Sin diagrama de muestra de unidad organizativa paralela](assets/do-not-localize/without-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

En este caso, el usuario tiene acceso a las unidades organizativas A, A1 y A2-1, todas conectadas bajo la unidad organizativa principal A. El usuario puede acceder a todo en A.

La siguiente asignación contiene unidades organizativas paralelas:

![Con diagrama de muestra de unidad organizativa paralela](assets/do-not-localize/with-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

El usuario tiene acceso a A1-1, A2 y A2-1, que existen en ramas independientes sin elemento principal asignado en común.


**Implicaciones de seguridad**

* En Campaign Standard, el sistema selecciona una unidad organizativa de nivel superior (A1-1 o A2) para el usuario, limitando el acceso únicamente a esa unidad y a sus elementos secundarios.
* Después de la migración a Campaign V8, el usuario obtiene acceso a los recursos de todas las unidades organizativas asignadas y a sus elementos secundarios.

**Resolución**

La asignación de unidades organizativas paralelas se puede resolver asegurándose de que todas las unidades organizativas asignadas a un usuario se encuentren dentro de una única unidad principal común que también se asigne al usuario.

A continuación se mencionan algunas formas de lograrlo:

1. Eliminar el acceso a varias ramas: revoque el acceso a varias ramas paralelas y asegúrese de que todo el acceso se encuentre en una sola rama principal.
1. Asignar un elemento principal común: Conceda acceso a una unidad organizativa principal común adecuada que incluya todos los puntos de acceso necesarios.
1. Reestructurar la jerarquía: modifique la estructura de la unidad organizativa para colocar todos los accesos necesarios debajo de una sola rama.

En el ejemplo anterior, en el que un usuario tiene acceso a A1-1, A2 y A2-1, los pasos específicos de resolución son:

1. Eliminar el acceso a varias ramas:

   1. Revocar acceso a A1-1, dejando solo acceso a A2 (que incluye A2-1), o
   1. Revocar acceso a A2 y A2-1, dejando solo acceso a A1-1

1. Asignar un elemento principal común:

   1. Conceda acceso a la unidad organizativa A, que es la matriz común de A1-1 y A2, o
   1. Conceder acceso a Todo, que cubre toda la jerarquía

1. Reestructurar la jerarquía:

   1. Mueva A1-1 bajo A2 o
   1. Mueva A2 y A2-1 bajo A1-1


## Enfoque de migración del programa

En Campaign v8, **Los programas** se representan como **carpetas**. Campaign v8 permite la creación de carpetas y restringir el acceso a ellas.

Mediante **Grupos** y **Derechos asignados**, se puede otorgar acceso a **Operadores** a **Carpetas** específicas dentro de la jerarquía de navegación, con la capacidad de asignar permisos de lectura, escritura y eliminación. [Más información acerca de la administración de carpetas](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Dado que un **programa** se trata como una **carpeta** en Campaign v8, su acceso se puede administrar de la misma manera que cualquier otra carpeta. Después de la migración, los administradores de Campaign Standard pueden seguir estos pasos:

1. Desde el explorador, haga clic con el botón derecho en cualquier carpeta y seleccione **[!UICONTROL Propiedades...]**.

1. Vaya a la ficha **[!UICONTROL Seguridad]**.

1. Modifique los permisos del grupo de operadores según el modelo de acceso deseado. 

## Asignación de perfil de producto para acceder a las API de REST 

Para acceder a las API transaccionales desde la instancia de ejecución en Campaign v8, se requiere un nuevo **perfil de producto**, además de los perfiles de producto **Administrador** y **Centro de mensajes**. Este nuevo **perfil de producto** se agregará a las cuentas técnicas existentes o creadas previamente en Campaign Standard.

Después de la migración, los usuarios de Campaign Standard deben revisar sus **asignaciones de perfiles de producto** y asignar el **perfil de producto** correspondiente si no desean vincular sus **cuentas técnicas** al perfil de producto **Administrador**. Para integraciones futuras, recomendamos usar la versión 8 de Campaign **ID de inquilino** en la **URL de REST** en lugar de la versión anterior de Campaign Standard **ID de inquilino**.

## Migración del acceso a los recursos integrados de Campaign para los operadores de Campaign Standard

Los operadores migrados de Campaign Standard tendrán acceso de lectura a recursos integrados específicos en Campaign v8.

## Grupos y funciones de seguridad no migrados {#non-migrated-groups-roles}

A continuación se muestra una lista de funciones de Campaign Standard que no se han transferido:

* Cuenta de retransmisión predeterminada 

* Push del centro de mensajes 

A continuación se muestra una lista de asignaciones de grupos de seguridad de Campaign Standard que no se han transferido.

* Agentes del centro de mensajes

* Agentes push del centro de mensajes

* Administradores de aplicaciones de Adobe Experience Manager

* Cuenta de retransmisión

>[!NOTE]
>
>Las funciones personalizadas creadas y asignadas a usuarios en Adobe Campaign Standard no se migrarán a Adobe Campaign v8.
