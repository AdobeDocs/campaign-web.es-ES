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
source-git-commit: 5a6b111d1aaa2a34ce165eaf6d1b1a997fd8bc85
workflow-type: tm+mt
source-wordcount: '1916'
ht-degree: 3%
---
# Diferencias entre Campaign Standard y Campaign v8 {#acs-v8-differences}

La mayoría de los conceptos son los mismos en Campaign Standard y Campaign v8. Esta página recopila las diferencias que le afectan después de la transición y establece vínculos a la página que explica cada una de ellas. Complementa las guías para [especialistas en marketing](marketers.md) y para [administradores y desarrolladores](admin-developers.md).

* Para ver los cambios terminológicos, consulte [Terminología](#terminology).
* Para que se ejecuten las comprobaciones y se notifiquen los problemas después de una transición, consulte [Comprobaciones y solución de problemas después de la transición](post-transition-checks.md).
* Para ver las funcionalidades que solo están disponibles en la consola del cliente, consulte [Consola de cliente de Campaign y web](../../v8/get-started/capability-matrix.md).

## Terminología {#terminology}

La mayoría de los conceptos son similares entre Adobe Campaign v8 y Adobe Campaign Standard. Sin embargo, existen algunas diferencias, empezando por la terminología.

| En Campaign Standard | En Campaign v8 |
|---|---|
| Recursos personalizados | **Esquemas** |
| Mensajes | **Entregas** |
| Usuarios de productos | **Operadores** |
| Funciones | Configurado con **derechos asignados** |
| Grupos de seguridad | **Grupos de operadores** |
| Unidades organizativas | Administrado mediante **permisos de carpeta** |

Además, como usuario de Campaign existente, tenga en cuenta que se ha cambiado el nombre de algunos conceptos para que se ajusten a los estándares terminológicos más recientes. Estos cambios solo se aplican a la interfaz de usuario de Campaign Web y no se reflejan en la consola del cliente.

| En Campaign Standard | En Campaign Web | Más información |
|---|---|---|
| Destinatarios | **Perfiles** | [Perfiles](../../v8/audience/gs-audiences-recipients.md) |
| Direcciones semilla | **Perfiles de prueba** | [Envíos de prueba](../../v8/preview-test/test-deliveries.md) |
| Análisis de envíos | **Preparación de envío**. Para iniciar la preparación del mensaje, haga clic en el botón **Preparar**. | [Preparar y enviar](../../v8/monitor/prepare-send.md) |
| Vista previa de correo electrónico | Disponible a través del botón **Simular contenido**. | [Vista previa y prueba](../../v8/preview-test/preview-test.md) |
| Listas | **Audiencias** | [Audiencias](../../v8/audience/gs-audiences-recipients.md) |

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
| Las audiencias creadas con la actividad Query en Campaign Standard se convierten en [filtros predefinidos](../../v8/query/build-query.md) en Campaign v8. Campaign v8 también admite la actividad Query. | [Administrar audiencias](marketers.md#acs-gs-marketers-audiences) |
| Una actividad Leer audiencia se convierte en una actividad de Consulta con un filtro predefinido. | [Administrar audiencias](marketers.md#acs-gs-marketers-audiences) |
| Un filtro predefinido solo toma el valor más reciente después de migrar la audiencia. | [Administrar audiencias](marketers.md#acs-gs-marketers-audiences) |
| Las audiencias de tipo de archivo se convierten en audiencias de tipo lista sin dimensiones. | [Administrar audiencias](marketers.md#acs-gs-marketers-audiences) |
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

## API e integraciones {#apis-and-integrations}

Estas diferencias afectan a las integraciones que llaman a Campaign a través de su API de REST y a las integraciones con otras soluciones y herramientas de Adobe.

| Qué cambios | Más información |
|---|---|
| Los valores de PKEY cambian tras la migración. Si almacena PKEY fuera de Campaign, siga las href devueltas por la API en su lugar. | [Uso de claves](#key-usage) |
| Algunos campos de perfil migrados, como la zona horaria y `ccpaOptOut`, solo los devuelve la API `profileAndServicesExt/profile`. | [Zona horaria del perfil y ccpaOptOut](#profile-timezone) |
| Adobe migra las configuraciones de Adobe Analytics y Audience Manager. Debe volver a configurar las integraciones de Déclencheur y Adobe Target. | [Administrar integraciones de Adobe Campaign](admin-developers.md#acs-gs-integrations) |

## Recomendaciones y limitaciones de la API de REST {#rest-api-limitations}

Las recomendaciones y limitaciones siguientes se aplican a las API de REST cuando realiza la transición de Campaign Standard a Campaign v8.

### Permisos y seguridad {#permissions}

#### Asignación de perfiles de producto {#rest-product-profiles}

En Campaign Standard, se le concedió acceso con funciones de administrador elevadas a las API independientemente del perfil de producto asignado. La versión 8 de Campaign presenta un conjunto diferente de perfiles de producto, que requieren la asignación de perfiles de producto de Campaign Standard a Campaign v8.

Con la migración, se añaden dos perfiles de producto a las cuentas técnicas existentes o creadas previamente: Administrador y Centro de mensajes (para acceder a las API transaccionales). Revise la asignación de perfiles de producto y asigne el perfil de producto necesario si no desea que el perfil de producto de administrador se asigne con su cuenta técnica.

#### ID de inquilino

Después de la migración, para cualquier integración futura, se recomienda usar su **ID de inquilino de Campaign v8** en las URL de REST, reemplazando su ID de inquilino de Campaign Standard anterior.

#### Uso de claves

La administración de los valores de clave principal difiere entre Campaign Standard y Campaign v8. Si almacenaba claves principales con Campaign Standard, asegúrese de que la implementación forme dinámicamente llamadas de API posteriores mediante claves principales o href obtenidas de llamadas de API anteriores.

### API disponibles {#available-apis}

Por ahora, las API de REST enumeradas a continuación están disponibles para su uso:

* **Perfiles**
* **Servicios y suscripciones**
* **Recursos personalizados**
* **Flujos de trabajo**
* **Mensajes transaccionales**

>[!AVAILABILITY]
>
>Las API de REST enumeradas a continuación están en desuso y no están disponibles para su uso:
>* Historial de marketing
>* Unidades organizativas
>* Administración de la privacidad

### Filtrado {#rest-filtering}

* Para utilizar los filtros en las cargas útiles de API REST, debe editarlos en Campaign v8 y proporcionar un nombre para utilizarlo en las cargas útiles. Para ello, obtenga acceso a los parámetros adicionales del filtro desde la ficha **[!UICONTROL Parámetros]** y proporcione el nombre que desee en el campo **[!UICONTROL Nombre del filtro en la API de REST]**.

  ![](assets/api-filtering.png)


* El prefijo &quot;by&quot; necesario para utilizar filtros personalizados ya no es necesario. El nombre del filtro debe usarse tal cual en sus solicitudes.

  Ejemplo:

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### Campos de base de datos descartados {#dropped-fields}

Algunos campos de la base de datos se pierden durante la migración. Al utilizar un campo colocado, las API de REST devolverán valores en blanco. En el futuro, todos los campos perdidos quedarán obsoletos y se eliminarán.

### PUBLICACIÓN con recursos vinculados {#post-linked}

Cuando se usa el siguiente formato de cuerpo de solicitud, con &quot;excipiente&quot; representando el enlace a &quot;nms:recipient&quot;:

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

Se ignora la información del vínculo. En consecuencia, se genera un nuevo registro en &quot;cusVehicle&quot; que contiene solo los valores de &quot;número de vehículo&quot; y &quot;nombre de vehículo&quot;. Sin embargo, el vínculo sigue siendo nulo, lo que hace que &quot;excipientePropietario&quot; se establezca en nulo.

En Campaign v8, cuando se utiliza la misma estructura de cuerpo de solicitud y el &quot;vehículo&quot; está vinculado a un perfil, se produce un error. Este error se produce porque la propiedad &quot;firstName&quot; no se reconoce como válida para &quot;cusVehicle&quot;. Sin embargo, un cuerpo de solicitud que incluye solo los atributos sin el vínculo funciona sin ningún problema.

### Operaciones de PATCH {#patch}

* La versión 8 de Campaign no admite PATCH con un cuerpo de solicitud vacío: devuelve el estado 204 Sin contenido.
* Aunque Campaign Standard admite PATCH en elementos/atributos dentro de un esquema, tenga en cuenta que las operaciones de PATCH en la ubicación no son compatibles con Campaign v8. Si se intenta un PATCH en una ubicación, se producirá un error de servidor interno 500 con un mensaje de error que indica que la propiedad &quot;zipCode&quot; no es válida para el recurso &quot;perfil&quot;.

### Respuestas REST {#rest-responses}

La sección siguiente enumera diferencias menores entre las respuestas de Campaign Standard y REST v8.

* Para registros GET únicos, la respuesta incluye el href en la respuesta.
* Cuando se consulta con el atributo, Campaign v8 proporciona Recuento y Paginación en la respuesta.
* Después de las operaciones POST, los valores de los recursos vinculados se devuelven en la respuesta.

### Códigos de error y mensajes {#rest-errors}

La sección siguiente enumera las diferencias entre los códigos de error y los mensajes de Campaign Standard y Campaign v8.

| Situación | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| Usar una clave principal no válida en el cuerpo de la solicitud | 500: atributo &#39;O5iRp40EGA&#39; desconocido (consulte la definición del esquema &#39;Profiles (nms:recipient)&#39;). XTK-170036 No se ha podido analizar la expresión &#39;@id = @O5iRp40EGA&#39;. | 404: No se puede descifrar la clave principal. (PKey=@jksad) |
| Usar una clave principal no válida en el URI | 500: atributo &#39;O5iRp40EGA&#39; desconocido (consulte la definición del esquema &#39;Profiles (nms:recipient)&#39;). XTK-170036 No se ha podido analizar la expresión &#39;@id = @O5iRp40EGA&#39;. | 404: No se puede descifrar la clave principal. (PKey=@jksad) Extremo no compatible. (extremo=rest/profileAndServices/profile/@jksad) |
| Uso de dos claves sin procesar diferentes en el URI y en el cuerpo de la solicitud | 500 - RST-360011 Se ha producido un error. Póngase en contacto con el administrador. RST-360012 Operación incoherente en el recurso &quot;servicio&quot;: no se puede actualizar la clave &quot;SVC3&quot; a &quot;SVC4&quot;. | 500 - Se ha producido un error - póngase en contacto con su administrador. |
| Uso de PKey en el URI y de una PKey sin procesar diferente en el cuerpo de la solicitud | 500: ya existe un &quot;servicio&quot; con la misma clave &quot;SVC4&quot;. PGS-220000 Error de PostgreSQL: ERROR: el valor de clave duplicado viola la restricción única &quot;nmsservice_name&quot; DETALLE: La clave (sname)=(SVC4) ya existe. | 500 - Se ha producido un error - póngase en contacto con su administrador. |
| Uso de raw-id no existente en el URI | 404 - RST-360011 Se ha producido un error. Póngase en contacto con el administrador. No se puede encontrar el documento con la ruta &#39;Servicio&#39; de la clave &#39;adobe_nl:0&#39; (documento con el esquema &#39;service&#39; y el nombre &#39;adobe_nl&#39;) | 404: No se puede encontrar el documento con la ruta &quot;Servicio&quot; de la clave &quot;adobe_nl&quot; (documento con el esquema &quot;service&quot; y el nombre &quot;adobe_nl&quot;) |
| Uso de raw-id no existente en el cuerpo de la solicitud | 404 - RST-360011 Se ha producido un error. Póngase en contacto con el administrador. No se pudo encontrar documento con ruta &#39;Servicio&#39; de la clave &#39;adobe_nl&#39; (documento con esquema &#39;service&#39; y nombre &#39;adobe_nl&#39;) | 404: No se puede encontrar el documento con la ruta &quot;Servicio&quot; de la clave &quot;adobe_nl&quot; (documento con el esquema &quot;service&quot; y el nombre &quot;adobe_nl&quot;) |
| - | 500 - RST-360011 Se ha producido un error. Póngase en contacto con el administrador. | 500 - Se ha producido un error - póngase en contacto con su administrador. |
| Inserte un perfil o servicio con un valor de enumeración de sexo no válido (o cualquier cosa) | 500 - RST-360011 Se ha producido un error. Póngase en contacto con el administrador. El valor &quot;invalid&quot; no es válido para la enumeración &quot;nms:recipient:gender&quot; del campo &quot;@gender&quot; | 500: Se ha producido un error. Póngase en contacto con el administrador. |

### Zona horaria del perfil y ccpaOptOut {#profile-timezone}

Con Campaign Standard, la zona horaria se muestra como parte de la respuesta JSON de **profileAndServices/profile** llamadas a la API de REST.

Con Campaign v8, la zona horaria solo se muestra al usuario como parte de las llamadas a la API REST **profileAndServicesExt/profile**. No forma parte de las llamadas a la API REST **profileAndServices/profile** porque se está agregando en un esquema extendido.

Lo mismo se aplica al campo `ccpaOptOut`: solo se muestra como parte de las llamadas a la API REST **profileAndServicesExt/profile**, no de las llamadas a **profileAndServices/profile**, ya que se agrega en un esquema extendido como parte de la migración de datos.

### Señales externas de flujo de trabajo {#workflow-signals}

La API de GET de flujo de trabajo de Campaign Standard devuelve nombres de parámetros como las variables de instancia de flujo de trabajo y sus tipos de datos (booleano, cadena, etc.). Se utiliza para crear un cuerpo de solicitud JSON con el formato adecuado al activar la señal a través de una llamada de API POST.

Campaign v8 no admite variables de instancia de flujo de trabajo de publicidad, pero espera que los desarrolladores sepan cuáles son. Como tal, después de la migración, la información de parámetros en el cuerpo de la solicitud POST deberá construirse sin la disponibilidad de la información de parámetros en la respuesta de la API de GET.
