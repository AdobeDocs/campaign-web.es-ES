---
title: Comprobación y solución de problemas después de la transición a Campaign v8
description: Obtenga información sobre qué comprobar y cómo solucionar problemas comunes después de la transición de Campaign Standard a Campaign v8
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 8b78a8494223fbcd3def29c955e6171cbb643fef
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%
---
# Comprobación y solución de problemas después de la transición {#post-transition-checks}

Después de realizar la transición de Campaign Standard a Campaign v8, algunas entregas, flujos de trabajo y páginas de aterrizaje pueden comportarse de forma diferente a lo esperado. La tabla siguiente enumera los síntomas notificados por los usuarios en transición, con la causa y qué hacer. Para ver la lista completa de diferencias, consulte [Diferencias entre Campaign Standard y Campaign v8](acs-v8-differences.md).

| Síntoma | Causa y qué hacer | Más información |
|---|---|---|
| Los vínculos de una entrega son direcciones URL directas y no se recopilan datos de clics. | El seguimiento está desactivado en la entrega o en la plantilla de entrega en la que se basa. Compruebe que **Activar seguimiento** esté habilitado, en particular en las plantillas de los envíos recurrentes. | [Configuración de seguimiento](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| Los destinatarios que cancelaron la suscripción a través del método List-Unsubscribe &quot;mailto&quot; no están en cuarentena. | Esto es esperable. Estos destinatarios no se envían a cuarentena. Se cancelan las suscripciones al servicio asociado con la entrega o se añaden a la lista de bloqueados de si la entrega no tiene servicio. Para realizar un seguimiento de estas bajas, comprueba las suscripciones del servicio o la sección **Ya no contactes** del perfil. | [Cuarentenas](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| Una página de aterrizaje no guarda un valor que se computa mediante una secuencia de comandos o que se almacena en un campo oculto. | Las páginas de destino creadas en la interfaz de usuario web de Campaign no admiten campos de entrada ocultos ni JavaScript personalizados. En su lugar, cree el formulario como aplicación web en la consola del cliente. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
| **Transferencia de archivos** no encuentra el archivo generado por una actividad de correo postal. | La transición saliente de una actividad de correo postal lleva la población objetivo, no el archivo de extracción. Agregue una actividad **Extracción de datos** y luego la actividad **Transferencia de archivos**. | [Correo postal](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| Varias olas de una entrega se envían juntas. | Las olas se programan desde la fecha de contacto de la entrega. Si la entrega se inicia después del tiempo planificado de algunas olas, esas olas se envían juntas en lugar de espaciarse. | [Enviar mediante olas](../../v8/advanced-settings/send-using-waves.md) |
| Una máscara de archivo con caracteres después del asterisco no encuentra ningún archivo en Azure Blob Storage. | Azure Blob Storage filtra los archivos por prefijo de nombre. Solo se admite un asterisco final. | [Transferir cuenta externa](../../v8/administration/transfer-external-account.md) |
| Una página de aterrizaje o bloque de contenido que utiliza JavaScript personalizado se comporta de forma diferente. | JavaScript personalizado se transforma durante la migración, pero se valida y ajusta, en particular si utiliza `queryDef`, las API de Campaign JavaScript, las escrituras de sesión, la administración de unidades organizativas o la generación de URL personalizada. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
| Una llamada a la API de REST devuelve un valor en blanco, un error o una respuesta inesperada. | Algunos campos de base de datos se pierden durante la migración y devuelven valores en blanco. Una PATCH vacía devuelve 204 y una PATCH en una ubicación devuelve 500. Una acción POST con un recurso vinculado ignora el vínculo o devuelve un error. Una PKEY no válida devuelve 404. | [Limitaciones de API de REST](acs-v8-differences.md#rest-api-limitations) |
| Una PKEY almacenada ya no funciona en las llamadas a la API. | Los valores de PKEY cambian tras la migración. No los almacene fuera de Campaign. De cada llamada desde las hrefs devueltas por la llamada anterior. | [Uso de claves](acs-v8-differences.md#key-usage) |
| Falta la zona horaria o `ccpaOptOut` en una respuesta de perfil. | Estos campos solo los devuelve `profileAndServicesExt/profile`, no `profileAndServices/profile`. Llame al extremo extendido. | [Zona horaria del perfil y ccpaOptOut](acs-v8-differences.md#profile-timezone) |
| Un filtro personalizado devuelve un error en una llamada a la API de REST. | En Campaign v8, asigne un nombre al filtro en el campo **Filter name in REST API** y utilice este nombre tal como está en la solicitud, sin el prefijo &quot;by&quot;. | [Filtrado](acs-v8-differences.md#rest-filtering) |
| Una llamada que pone en déclencheur una señal externa de flujo de trabajo no puede crear su cuerpo de solicitud. | La API GET de flujo de trabajo ya no devuelve las variables de flujo de trabajo. Cree los parámetros del cuerpo de la solicitud POST a partir de su propio conocimiento del flujo de trabajo. | [Señales externas de flujo de trabajo](acs-v8-differences.md#workflow-signals) |
| Se ha denegado el acceso a las API transaccionales. | El acceso a las API transaccionales desde la instancia de ejecución requiere un nuevo perfil de producto. Revise la asignación de perfil de producto de sus cuentas técnicas. | [Asignación de perfiles de producto](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| Una audiencia migrada solo muestra el valor más reciente, o una audiencia de archivo no tiene dimensiones. | Esto es esperable. Un filtro predefinido solo toma el valor más reciente después de la migración de audiencias y las audiencias de tipo de archivo se convierten en audiencias de tipo lista sin dimensiones. | [Administrar audiencias](marketers.md#acs-gs-marketers-audiences) |
| El historial de los flujos de trabajo ejecutados en Campaign Standard está vacío. | Los registros históricos de los flujos de trabajo ejecutados en Campaign Standard no se migran. Los flujos de trabajo ejecutados en Campaign v8 tienen su propio historial y registros. | [Creación de un flujo de trabajo](marketers.md#acs-gs-marketers-wf) |
| Algunos usuarios pueden ver o hacer más que antes. | Los usuarios con el rol **Modelo de datos** pero no el rol **Administración** obtienen acceso a **Administración**, y los grupos de seguridad con unidades organizativas paralelas pueden tener acceso más amplio. Revise los grupos de operadores, los derechos asignados y los permisos de carpeta. | [Administración de acceso de usuario](user-management-acs.md) |
| Un perfil de prueba marcado como **Trampa** no recibe el envío final. | En la versión 8 de Campaign, agregue un **grupo de reventado** en la configuración Audiencia de la entrega. | [Grupo de reventado](../../v8/audience/trap-group.md) |
| Un correo electrónico recurrente no tiene opción de periodo de acumulación. | Esta opción no está disponible para Campaign v8. | [Actividades de canal](../../v8/workflows/activities/channels.md) |
| El sistema de informes dinámico no muestra datos para una entrega. | Los informes dinámicos abarcan las entregas de correo electrónico, las campañas con entregas de correo electrónico y los mensajes transaccionales. | [Creación de informes](marketers.md#acs-gs-marketers-reporting) |
