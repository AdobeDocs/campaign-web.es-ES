---
title: Diferencias entre Campaign Standard y Campaign v8
description: Descubra qué cambios se producen al pasar de Campaign Standard a Campaign v8 y dónde encontrar los detalles
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 25814ce1c70a139c9727b3bfccccd3efe056b441
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 2%
---
# Diferencias entre Campaign Standard y Campaign v8 {#acs-v8-differences}

La mayoría de los conceptos son los mismos en Campaign Standard y Campaign v8. Esta página recopila las diferencias que le afectan después de la transición y establece vínculos a la página que explica cada una de ellas. Complementa las guías para [especialistas en marketing](marketers.md) y para [administradores y desarrolladores](admin-developers.md).

* Para ver los cambios terminológicos, consulte [Diferencias clave entre Campaign Standard y Campaign v8](overview.md#experiences).
* Para que se ejecuten las comprobaciones y se notifiquen los problemas después de una transición, consulte [Comprobaciones y solución de problemas después de la transición](post-transition-checks.md).
* Para ver las funcionalidades que solo están disponibles en la consola del cliente, consulte [Consola de cliente de Campaign y web](../../v8/get-started/capability-matrix.md).

## Canales y contenido {#channels}

Los pasos para crear y enviar mensajes son similares en ambos productos, tal como se describe en la [guía para especialistas en marketing](marketers.md). Las diferencias siguientes se refieren a la disponibilidad del canal, los envíos de prueba, las páginas de aterrizaje y los flujos de trabajo de correo directo.

| Qué cambios | Más información |
|---|---|
| El canal en la aplicación no está disponible en Campaign v8. | [Canal en la aplicación](marketers.md#acs-gs-marketers-in-app) |
| Para realizar la transición de flujos de trabajo push y envíos existentes, póngase en contacto con su administrador de transición de Adobe Campaign. | [Notificaciones push](marketers.md#acs-gs-marketers-push) |
| En Campaign Standard, un perfil de prueba podría marcarse como **trampa** para recibir el envío final. En la versión 8 de Campaign, agregue un **grupo de reventado** en la configuración Audiencia de la entrega. | [Grupo de reventado](../../v8/audience/trap-group.md) |
| Las páginas de destino creadas en la interfaz de usuario web de Campaign no admiten campos de entrada ocultos ni JavaScript personalizados. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
| En Campaign Standard, la transición saliente de una actividad de correo postal también llevaba el archivo generado. En Campaign v8, solo lleva la población de destino. Para enviar el archivo a un servidor, agregue una actividad **Extracción de datos** y luego una actividad **Transferencia de archivos**. | [Correo postal](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Audiencias, flujos de trabajo y envíos {#data-and-workflows}

Estas diferencias afectan a las audiencias y los flujos de trabajo migrados desde Campaign Standard, a algunas opciones de envíos recurrentes y de la actividad **Transferencia de archivos**, y al ámbito del sistema de informes dinámico.

| Qué cambios | Más información |
|---|---|
| Las audiencias se transforman durante la transición. Por ejemplo, las audiencias creadas con la actividad de consulta se convierten en filtros predefinidos y las audiencias de tipo de archivo se convierten en audiencias de tipo lista sin dimensiones. | [Administrar audiencias](marketers.md#acs-gs-marketers-audiences) |
| Los registros históricos de los flujos de trabajo ejecutados en Campaign Standard no se migran. | [Creación de un flujo de trabajo](marketers.md#acs-gs-marketers-wf) |
| En Campaign Standard, puede seleccionar el periodo de acumulación de un correo electrónico recurrente. Esta opción no está disponible para Campaign v8. | [Actividades de canal](../../v8/workflows/activities/channels.md) |
| Los informes dinámicos abarcan las entregas de correo electrónico, las campañas con entregas de correo electrónico y los mensajes transaccionales. | [Creación de informes](marketers.md#acs-gs-marketers-reporting) |

## Acceso y seguridad {#access}

Los grupos de seguridad, las funciones y las unidades organizativas de Campaign Standard se asignan a grupos de operadores, derechos asignados y permisos de carpetas durante la transición. Revise los puntos siguientes, en particular si algunos usuarios tienen derechos más amplios o más limitados que antes.

| Qué cambios | Más información |
|---|---|
| Los grupos de seguridad, las funciones y las unidades organizativas se asignan a grupos de operadores, derechos asignados y permisos de carpeta. Los roles personalizados no se migran. | [Administración de acceso de usuario](user-management-acs.md) |
| Los usuarios con el rol **Modelo de datos** pero no el rol **Administración** obtienen acceso a **Administración**. | [Administración de acceso de usuario](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| Los usuarios asignados a grupos de seguridad con unidades organizativas paralelas pueden tener un acceso más amplio en la versión 8 de Campaign. | [Asignación de unidad organizativa paralela](user-management-acs.md#parallel-assignments) |
| El acceso a las API transaccionales desde la instancia de ejecución requiere un nuevo perfil de producto. | [Asignación de perfiles de producto](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Las solicitudes de privacidad pueden llegar tanto a Campaign Standard como a Campaign v8 durante el periodo en el que el entorno de Campaign Standard permanece activo. | [Privacidad y consentimiento](admin-developers.md#privacy-and-consent) |

## Administración, seguimiento y páginas espejo {#admin-tracking}

Estas diferencias afectan a los envíos realizados desde Campaign Standard antes de la transición y a la información administrativa que no se transfiere a Campaign v8.

| Qué cambios | Más información |
|---|---|
| Las páginas espejo de los envíos realizados desde Campaign Standard antes de la transición no están disponibles. Las páginas espejo de los envíos enviados desde Campaign v8 funcionan como de costumbre. | [Páginas espejo](../../v8/email/mirror-page.md) |
| El seguimiento de datos de envíos transaccionales en tiempo real enviados desde Campaign Standard antes de la transición no se captura en Campaign v8. Los vínculos de estos mensajes se siguen redireccionando. | [Monitorizar mensajes transaccionales](../../v8/transactional-messaging/monitor-transactional.md) |
| Las unidades geográficas no están disponibles. Se pierde el control de acceso basado en unidades geográficas. | [Control de acceso](../../v8/get-started/connect-to-campaign.md#access-control) |

## API e integraciones {#apis-and-integrations}

Estas diferencias afectan a las integraciones que llaman a Campaign a través de su API de REST y a las integraciones con otras soluciones y herramientas de Adobe.

| Qué cambios | Más información |
|---|---|
| Los valores de PKEY cambian tras la migración. Si almacena PKEY fuera de Campaign, siga las href devueltas por la API en su lugar. | [API de REST](admin-developers.md#acs-gs-admin-apis) |
| Algunos campos de perfil migrados, como la zona horaria y `ccpaOptOut`, solo los devuelve la API `profileAndServicesExt/profile`. | [API de REST](admin-developers.md#acs-gs-admin-apis) |
| Las integraciones de Dreamweaver y Adobe Experience Platform Data Connector de Campaign Standard no están disponibles en la versión 8 de Campaign. | [Trabaje con Campaign y otras soluciones de Adobe](../../v8/integrations/integration.md) |
| Adobe migra las configuraciones de Adobe Analytics y Audience Manager. Debe volver a configurar las integraciones de Déclencheur y Adobe Target. | [Administrar integraciones de Adobe Campaign](admin-developers.md#acs-gs-integrations) |
