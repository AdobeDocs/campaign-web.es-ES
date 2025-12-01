---
title: Introducción a Adobe Campaign v8 después de la transición desde Campaign Standard
description: Conozca los pasos necesarios para empezar a utilizar la nueva aplicación de Campaign v8
role: User, Admin, Developer
level: Beginner
exl-id: 39d1f1b6-626b-48a2-92c3-9b593a377d66
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 29%

---

# De Campaign Standard a v8 {#ac-acs}

¡Bienvenido a Adobe Campaign v8!

Como usuario que está realizando la transición de Campaign Standard a Campaign v8, esta guía de referencia está diseñada para usted. Le ayuda a familiarizarse con su nuevo entorno de Campaign y a guiarle por los pasos necesarios para comenzar a utilizar su función.

1. Empiece por aprender [las novedades de la versión 8](#new) de Adobe Campaign.

1. A continuación, comprenda [las diferencias de experiencia entre Adobe Campaign Standard y Adobe Campaign v8 según su función](#experiences).

## Novedades {#new}

Eche un vistazo a las mejoras más recientes en la interfaz de usuario web de Adobe Campaign en esta página. Para obtener una lista completa de las funcionalidades clave y las características de las actualizaciones de la versión, consulte [esta sección](../../v8/rn/whats-new.md).

### Mejoras con Campaign v8 {#ac-enhancements}

A continuación, se enumeran las mejoras clave incluidas en Adobe Campaign v8.

* **Interfaz de usuario web**

  Adobe Campaign v8 ofrece una consola de cliente y una interfaz de usuario web, que satisfacen diferentes preferencias y necesidades de usuario. La consola del cliente proporciona una potente experiencia de aplicación de escritorio, mientras que la interfaz de usuario web está diseñada para ser intuitiva y accesible, lo que la convierte en una opción ideal para los especialistas en marketing familiarizados con Adobe Campaign Standard.

  La interfaz de usuario web comparte muchas similitudes con Adobe Campaign Standard, aunque algunas terminologías pueden diferir.

  Puede [obtener más información acerca de la interfaz de usuario web de Adobe Campaign aquí](../../v8/campaign-web-home.md).

  ![](assets/home.png){zoomable="yes"}

  Todas las nuevas funcionalidades y mejoras se enumeran en [Notas de la versión](../../v8/rn/release-notes.md). Las versiones de la interfaz de usuario web de Adobe Campaign funcionan con un modelo de envío continuo que permite un enfoque más escalable y gradual de la implementación de funcionalidades. Por lo tanto, estas notas de la versión se actualizan varias veces al mes. Compruébelas regularmente.


* **Rendimiento**

  Adobe Campaign v8 aprovecha las tecnologías avanzadas de bases de datos a escala de nube, lo que mejora significativamente el rendimiento y la eficacia. Esta arquitectura rediseñada ofrece varias ventajas clave:

   * *Escala*: El sistema ahora admite un aumento sustancial en las capacidades de procesamiento, con un rendimiento de procesamiento por lotes que alcanza hasta **20 millones de operaciones por hora**. Con esta nueva arquitectura, se pueden administrar perfiles aún más altos con un rendimiento predecible.
   * *Velocidad*: El sistema se ha mejorado para cualquier actividad de marketing: segmentación, preparación de envíos o rendimiento para mensajes transaccionales, que ahora es de **1 millón por hora**.

  Los servicios en la nube completamente administrados proporcionan al usuario lo siguiente:

   * Exploración de datos en tiempo real: Acceda y analice datos instantáneamente para obtener perspectivas rápidas y una toma de decisiones más informada.

   * Creación rápida de audiencias: Cree audiencias segmentadas fácilmente en cuestión de minutos para una segmentación de campaña más eficaz.

  En general, la sólida arquitectura de Adobe Campaign v8 proporciona una base sólida para administrar campañas de marketing extensas y complejas con una velocidad y eficiencia mejoradas.

### Nuevas funciones de la versión 8 de Adobe Campaign {#ac-new-features}

Como usuario de Campaign Standard que está realizando la transición a Adobe Campaign v8, ya tiene a su disposición las siguientes funciones:

* **Inserción enriquecida**

  Adobe Campaign v8 ofrece la capacidad de enviar notificaciones push enriquecidas, que pueden capturar la atención de los usuarios y animarlos a tomar medidas. Estas notificaciones pueden incluir una variedad de elementos como texto, imágenes, botones, temporizadores de cuenta atrás, sonidos, etc.

  ![](../../v8/push/assets/rich_push.png){zoomable="yes"}

  Para facilitar la creación de estas notificaciones rich, Adobe Campaign v8 proporciona varias plantillas que le permiten diseñar y personalizar el contenido de notificaciones complejas, como carruseles o temporizadores.

  Puede adaptar las notificaciones en función del sistema del cliente:

   * Para [Android](../../v8/push/rich-push.md) plantillas

   * Para [iOS](../../v8/push/rich-push.md) plantillas

  Las notificaciones push son una herramienta crucial para atraer a los usuarios de aplicaciones móviles, lo que le permite llegar a ellos incluso cuando no utilizan activamente la aplicación.

* **Adobe Experience Manager as a Cloud Service**

  Adobe Campaign v8 se integra perfectamente con Adobe Experience Manager as a Cloud Service, lo que mejora su capacidad para ofrecer experiencias personalizadas y enriquecidas en contenido a sus clientes. Esta integración nativa optimiza la administración de contenido y aprovecha las sólidas capacidades de Adobe Experience Manager para optimizar los esfuerzos de marketing.

  Estas son las funciones clave que habilita esta integración:

   * *Administración de recursos*: en Adobe Campaign v8, el diseñador de correo electrónico proporciona un selector para acceder y administrar recursos. Esta función simplifica la integración de elementos de Adobe Experience Manager en el envío, lo que hace que la administración de contenido sea más eficiente. [Más información acerca de la administración de recursos](../../v8/integrations/aem-assets.md)

     ![](../../v8/integrations/assets/assets_6.png){zoomable="yes"}

   * *Importación de plantillas de correo electrónico*: Adobe Campaign v8 permite examinar e importar plantillas de correo electrónico de Adobe Experience Manager directamente en Campaign. [Más información acerca de la importación de plantillas de correo electrónico](../../v8/integrations/aem-content.md)

     ![](../../v8/integrations/assets/aem_6.png){zoomable="yes"}

  Adobe Experience Manager as a Cloud Service ofrece agilidad nativa de la nube, lo que le permite acelerar su tiempo de respuesta al valor y adaptarse a las cambiantes necesidades empresariales. Esta integración no solo mejora las funciones de administración de contenido, sino que también le permite ofrecer experiencias más personalizadas y atractivas a sus clientes en todos los puntos de contacto.

* **Asistente de IA**

  El Asistente de IA de Campaign hace que la creación y ejecución de campañas de marketing en canales como correo electrónico, SMS y push sea intuitiva, sencilla y sin complicaciones, a la vez que ahorra tiempo, mejora la eficacia y obtiene mejores resultados.

  ![](../../v8/email/assets/full-email-1.png){zoomable="yes"}

  AI Assistant revoluciona la forma de crear contenido profesional y coherente con la marca en todos los canales. Con los modelos avanzados de GenAI y una comprensión profunda de las directrices de marca, AI Assistant genera automáticamente contenido personalizado, atractivo y eficaz en función del objetivo de marketing, con contenido optimizado para estilos, diseños, tonos y mucho más definidos por la marca.

  El asistente de IA hace que la creación y ejecución de campañas de marketing sea intuitiva, sencilla y sin complicaciones, a la vez que ahorra tiempo, mejora la eficiencia y obtiene mejores resultados.

  ![](../../v8/email/assets/full-email-2.png){zoomable="yes"}

  Proporciona una variante de plantillas de correo electrónico y genera y vuelve a generar imágenes. Obtenga más información acerca del Asistente de IA en [esta sección](../../v8/content/generative-full-content.md). Adobe Campaign v8 tiene un asistente de IA disponible para [correo electrónico](../../v8/content/generative-full-content.md), [SMS](../../v8/content/generative-text.md) y [push](../../v8/content/generative-full-content.md).

* **Infraestructura de SMS actualizada: SMS v2.0**

  La simplicidad y facilidad de uso de los SMS lo convierten en un canal de comunicación muy valioso además de su robustez y compatibilidad inigualable sobre miles de millones de terminales.

  Adobe Campaign v8 viene con una nueva infraestructura que mejora el envío de SMS. [Más información sobre la nueva configuración de SMS](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}.

* **Infraestructura push actualizada**

  La versión 8 de Adobe Campaign presenta nuestro último servicio de notificaciones push, con una estructura sólida basada en una tecnología moderna de vanguardia. Este servicio está diseñado para desbloquear nuevos niveles de escalabilidad, lo que garantiza que las notificaciones puedan llegar a una audiencia más grande con una eficiencia perfecta. Con nuestra infraestructura mejorada y los procesos optimizados, puede esperar una mayor escala y fiabilidad, lo que le permite interactuar y conectarse con los usuarios de sus aplicaciones móviles como nunca antes.

  [Más información sobre la infraestructura push actualizada](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.


## Managed Services {#ac-managed-services}

Adobe Campaign v8 está disponible como Managed Cloud Service y proporciona supervisión proactiva, alertas oportunas y control de servicios. Adobe Managed Cloud Service proporciona a los especialistas en marketing una solución de administración de campañas en canales múltiples más ágil, segura y escalable con un bajo coste total de propiedad. La nueva oferta combina servicios con supervisión proactiva y alertas oportunas.

## Funciones de Campaign Standard añadidas a la versión 8 de {#ac-v8-added}

Para que pueda realizar la transición sin problemas a Campaign v8, se han añadido funciones clave de Campaign Standard a Campaign v8. Se encuentran detalladas en [esta documentación](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=es){target="_blank"}.

* **Creación de informes dinámicos**: la creación de informes dinámicos proporciona informes totalmente personalizables y en tiempo real para medir el impacto de las actividades de marketing. Añade acceso a los datos de perfil, lo que permite el análisis demográfico por dimensiones de perfil como género, ciudad y edad, además de datos funcionales de campaña de correo electrónico como aperturas y clics. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=es){target="_blank"}.

* **Personalización de marca centralizada**: cada compañía tiene directrices técnicas y visuales de marca. Con Adobe Campaign, puede definir un conjunto de especificaciones para presentar una marca coherente a sus clientes, desde logotipos hasta aspectos técnicos, como el remitente de correos electrónicos, la dirección URL o los dominios. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=es)

* **API de REST**: como usuario migrado de Campaign Standard, puede utilizar las API de REST para crear integraciones para Adobe Campaign y construir su propio ecosistema al interconectar Adobe Campaign con el panel de tecnologías que utiliza. [Más información](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=es){target="_blank"}.

* **Páginas de destino**: se han introducido algunas mejoras en las páginas de destino de Campaign v8 para garantizar la paridad de las funciones con Campaign Standard. Obtenga más información en las [notas de la versión](../../v8/rn/release-notes.md#new-24-4) y la página de destino [documentación](../../v8/landing-pages/get-started-lp.md).

* **Fragmentos visuales**: los fragmentos visuales son componentes visuales reutilizables a los que se puede hacer referencia en uno o varios envíos de correo electrónico o en plantillas de contenido. Al modificar un fragmento, se actualiza todo el contenido que lo utiliza. Esta funcionalidad se utiliza para la construcción previa de múltiples bloques de contenido personalizado que pueden ser utilizados por los usuarios de marketing para combinar rápidamente los contenidos de los mensajes en un proceso de diseño mejorado. [Más información](../../v8//content/use-visual-fragments.md)

## Diferencias clave entre Campaign Standard y Campaign v8 {#experiences}

La mayoría de los conceptos son similares entre Adobe Campaign v8 y Adobe Campaign Standard. Sin embargo, existen algunas diferencias, como se describe a continuación.

A continuación, se muestran algunas diferencias terminológicas entre Campaign Standard y la versión 8 de Campaign.

* Los recursos personalizados son **Esquemas**
* Los mensajes se denominan **Envíos**
* Los usuarios de productos son **Operadores**.
* Las funciones se configuran con **Derechos asignados**
* Los grupos de seguridad son **Grupos de operadores**.
* Las entidades organizativas son **Permisos de la carpeta**

Además, como usuario de Campaign existente, tenga en cuenta que se ha cambiado el nombre de algunos conceptos para que se ajusten a los estándares terminológicos más recientes. Estos cambios solo se aplican a la interfaz de usuario web de Campaign y no se reflejan en la consola del cliente. Estos se encuentran detallados a continuación.

* Los destinatarios ahora son **Perfiles**. [Más información](../../v8/audience/gs-audiences-recipients.md).
* Las direcciones semilla ahora son **Perfiles de prueba**. [Más información](../../v8/preview-test/test-deliveries.md).
* El análisis del envío ahora es la **preparación del envío**. Cuando necesite iniciar la preparación del mensaje, haga clic en el botón **Preparar**. [Más información](../../v8/monitor/prepare-send.md).
* La vista previa del correo electrónico ya está disponible a través del botón **Simular contenido.** [Más información](../../v8/preview-test/preview-test.md)
* Las listas son ahora **Públicos**. [Más información](../../v8/audience/gs-audiences-recipients.md).


## Nueva experiencia del usuario

Acceda a la guía de referencia pertinente para su función con el fin de descubrir la nueva experiencia del usuario con Adobe Campaign v8.

<table>
<tr>
  <td>
    <a href="marketers.md">
      <img alt="Administrador de campañas"src="./assets/digital_marketing.jpeg"/>
    </a>
    <div>
  </td>
  <td>
  <a href="admin-developers.md">
    <img alt="Administrador o desarrollador" src="./assets/admin.jpeg"/>
    </a>
    <div>
  </td>
  </tr>
  <tr>
    <td>
    <a href="marketers.md">
    <strong>Experto en marketing</strong>
    </a>
    </td>
    <td>
      <a href="admin-developers.md">
      <strong>Administrador o Desarrollador</strong>
      </a>
    </td>
  </tr>
    <td>
    <em>Administrador de campañas, especialista en mercadotecnia de medios</em>
    </td>
    <td>
      <em> Administrador del sistema, especialista en mercadotecnia técnica</em>
    </td>
  <tr>
    <td>
    <b>Las tareas/responsabilidades clave incluyen:</b>
    </td>
      <td>
    <b>Las tareas/responsabilidades clave incluyen:</b>
    </td>
  </tr>
  <tr>
    <td>
      <li>Creación de campañas de marketing
      <li>Diseño de flujos de trabajo
      <li>Prueba y ejecución de campañas
      <li>Implementación de campañas multicanal
      <li>Optimización de campañas
      <li>Optimización de campañas automatizadas
    </td>
    <td>
        <li>Gestión de acceso
        <li>Configuración del sistema
        <li>Personalización del sistema
    </td>
</tr>
</table>
</div>

<!--
## Deprecated items

Adobe constantly evaluates product capabilities to identify older features that should be replaced with more modern alternatives to improve overall customer value, always under careful consideration of backward compatibility.

Please refer to [this documentation for information on deprecated items](https://experienceleague.adobe.com/es/docs/campaign-standard/using/release-notes/deprecated-features).-->
