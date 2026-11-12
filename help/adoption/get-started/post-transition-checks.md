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
source-git-commit: 071900a6c0b717161ae123097aeae8bf9e97898c
workflow-type: tm+mt
source-wordcount: '433'
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
