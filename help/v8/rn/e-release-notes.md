---
title: Notas de la versión preliminar de la interfaz de usuario web de Campaign v8
description: Descubra las nuevas funciones incluidas en la próxima versión de la interfaz de usuario web de Campaign
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: d4f9f3562f7dc2550bf9fea01f27456fdfdad43e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 46%

---

# Notas de la versión preliminar {#e-release}

La interfaz de usuario web de Adobe Campaign ofrece continuamente nuevas funciones, mejoras de las funciones existentes y correcciones de errores. Todos los cambios se consolidan al final de cada mes en las [notas de la versión](release-notes.md).

**Las notas de la versión preliminar que se indican a continuación están sujetas a cambios sin previo aviso hasta la fecha de disponibilidad final de la versión**. Los vínculos, las pantallas y la documentación actualizada se publican en las [notas de la versión](release-notes.md), en la fecha de lanzamiento.

## Notas de la versión de julio {#24-7-release}

**Fecha de la versión**: 30 y 31 de julio de 2024

Las siguientes funciones y mejoras están disponibles a partir de la versión de julio.

### Listas semilla {#24-7-2}

Una lista semilla, también conocida como. **Grupo de reventado**, es una lista de direcciones semilla. Se utiliza para incluir direcciones específicas en los envíos y, a continuación, concentrarse en los perfiles que no coinciden con los criterios objetivo definidos. De este modo, los destinatarios que estén fuera del público del envío pueden recibirlo como lo haría cualquier otro destinatario objetivo. Puede utilizar direcciones semilla al enviar pruebas o para proteger la lista de su campaña de correo.

### Plantillas de notificaciones push enriquecidas {#24-7.3}

Ahora puede enviar notificaciones push enriquecidas. Una notificación push enriquecida es una forma mejorada de notificación móvil que va más allá de los mensajes de texto simples mediante la incorporación de elementos multimedia como imágenes, botones interactivos u otro contenido multimedia enriquecido. Con esta versión, ya está disponible un conjunto de plantillas para notificaciones push enriquecidas para sus aplicaciones de iOS y Android.

>[!AVAILABILITY]
>
>Esta funcionalidad requiere una actualización de la versión 8.6.3 o 8.7.2 de Campaign. [Obtenga más información en las notas de la versión de la consola del cliente de Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes)


### Mejoras {#improvements-24-7}

**Administración de carpetas**: ahora puede administrar permisos y restricciones en las carpetas.

### Nuevas funciones en disponibilidad limitada {#acs-24-4}

>[!AVAILABILITY]
>
>Las siguientes capacidades están en disponibilidad limitada (LA). Están restringidos a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se pueden implementar en ningún otro entorno.
>
>Consulte las siguientes páginas de documentación: [Campaign Standard de la transición a Campaign v8](../rn/acs-migration.md) y [Funciones para usuarios de Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es).

#### Fragmentos de contenido {#LA-24-7}

Ahora puede crear y utilizar fragmentos de contenido. Un fragmento de contenido es un componente reutilizable al que se puede hacer referencia en uno o varios mensajes. Al modificar un fragmento, se actualiza todo el contenido que lo utiliza. Esta funcionalidad permite generar previamente varios bloques de contenido personalizados que los usuarios de marketing pueden utilizar para ensamblar rápidamente el contenido del mensaje en un proceso de diseño mejorado.

Hay dos tipos de fragmentos disponibles:

* **Los fragmentos de expresión** son expresiones predefinidas que están disponibles en una entrada dedicada en el editor de expresiones.
* **Los fragmentos visuales** son bloques visuales predefinidos que se pueden reutilizar en varios envíos de correo electrónico o en plantillas de contenido. [Más información](../email/fragments.md)

  >[!AVAILABILITY]
  >
  >**Los fragmentos visuales** están en disponibilidad limitada (LA). Esta capacidad está restringida a los clientes que migran **de Adobe Campaign Standard a Adobe Campaign v8** y no se puede implementar en ningún otro entorno.
