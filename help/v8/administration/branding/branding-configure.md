---
title: Promoción de la marca
description: Descubra cómo configurar su marca
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 8b93ddd9c655c9ca461f28392c70872e4005b44f
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 29%

---

# Configurar marcas {#branding-configure}

>[!IMPORTANT]
>
>Los usuarios finales no pueden crear ni modificar marcas: estas operaciones deben ser realizadas por el administrador técnico de Adobe Campaign. Para cualquier pregunta, póngase en contacto con el servicio de atención al cliente de Adobe.

En Adobe Campaign V8, las marcas se encuentran en el menú **[!UICONTROL Administración > Plataforma > Marca]**.

Una **[!UICONTROL marca]** se define con las siguientes características:

* Una **[!UICONTROL identidad]**, que define y personaliza su marca. Esta sección contiene los campos siguientes:

   * **[!UICONTROL Etiqueta]** visible en la interfaz.
   * **[!UICONTROL ID]**
   * **[!UICONTROL Nombre de la marca]**.
   * **[!UICONTROL Dirección URL]** y **[!UICONTROL etiqueta del sitio web]** de la marca.
   * **[!UICONTROL Logotipo de marca]**.

  ![](assets/branding_1.png)

* **[!UICONTROL Parámetros de encabezado de correos electrónicos enviados]** que personalizan lo que verán los destinatarios de sus campañas. Esta sección contiene los campos siguientes:

   * **[!UICONTROL Remitente (dirección de correo electrónico)]** con la dirección de correo electrónico de la marca.
   * **[!UICONTROL Remitente (nombre)]** con el nombre de la marca.
   * **[!UICONTROL Responder a (dirección de correo electrónico)]** con la dirección de correo electrónico a la que el cliente puede responder.
   * **[!UICONTROL Responder a (nombre)]** con el nombre de la marca.
   * **[!UICONTROL Error (dirección de correo electrónico)]** con la dirección de correo electrónico que se utiliza en caso de error.

  >[!IMPORTANT]
  >
  >Después de haber actualizado los parámetros de encabezado de los correos electrónicos, si el nombre y la dirección de correo electrónico del remitente no han cambiado en el correo electrónico creado a partir de la plantilla, compruebe la configuración avanzada de esta.

  ![](assets/branding_2.png)

* **[!UICONTROL Configuraciones de marca]** define los servidores que se usan para realizar el seguimiento también para el acceso a la página de aterrizaje. Esta sección contiene los campos siguientes:

   * **[!UICONTROL Subdominio de marca]** hace referencia a la dirección URL de subdominio designada específica de esta marca, solicitada para delegación desde Adobe.

  Tenga en cuenta que la configuración de los servidores de seguimiento, réplica y aplicaciones se almacena en cuentas externas independientes asociadas con el enrutamiento. Esta configuración se aplica durante el aprovisionamiento y no debe modificarse. Para mostrar las direcciones URL, acceda a la pestaña **[!UICONTROL Prefijos de marca]** desde su cuenta externa.

  ![](assets/branding_3.png)

* El menú **[!UICONTROL Configuraciones de URL de seguimiento]** le permite mejorar el seguimiento de URL mediante la definición de parámetros adicionales para la integración con herramientas de Web Analytics como Adobe Analytics y Google Analytics.

  Utilice el menú **[!UICONTROL Parámetros de URL adicionales]** para crear parámetros adicionales como pares clave-valor junto con sus condiciones de aplicabilidad. Cada nombre de parámetro debe ser único y no vacío, y cada valor de parámetro no debe estar vacío. La condición de aplicabilidad puede estar vacía, pero ninguno de estos valores puede incluir etiquetas JST.

  Estos parámetros se aplicarán a las direcciones URL rastreadas que coincidan con cualquier nombre de dominio especificado en la **[!UICONTROL Lista de nombres de dominio]**, que puede incluir expresiones regulares.

  **Ejemplo:** Una dirección URL rastreada como `https://www.example.com` pasará a ser `https://www.example.com/?age=21&deliveryName=DM101` cuando los parámetros adicionales `age=21` y `deliveryName=DM101` estén configurados para ese dominio.

## Configuración de la marca para la mensajería transaccional {#branding-transactional-config}

>[!IMPORTANT]
>
>Esta sección se aplica solo a los mensajes transaccionales (Centro de mensajes).
>
>Aunque las funcionalidades transaccionales están disponibles en la interfaz de usuario web de Campaign, los pasos siguientes deben realizarse en la consola del cliente de Campaign v8 (instancia de control).

Si utiliza mensajes transaccionales (centro de mensajes) con marca, se requiere una configuración adicional.

### Seguimiento de fórmulas para instancias en tiempo real

Cuando la promoción de la marca se activa en una instancia de control en tiempo real (RT), se utilizan opciones de seguimiento específicas para administrar las fórmulas de seguimiento. Estas fórmulas se configuran de forma centralizada en la instancia de control de RT en lugar de individualmente en cada instancia de ejecución de RT.

Las siguientes opciones definen las fórmulas de seguimiento utilizadas por los envíos RT:

* **`NmsTracking_RT_ClickFormula`**: especifica la fórmula utilizada para el rastreo de clics en instancias RT

* **`NmsTracking_RT_OpenFormula`**: especifica la fórmula utilizada para el seguimiento de aperturas en instancias RT

Si su implementación requiere fórmulas de seguimiento personalizadas para la mensajería transaccional, utilice la siguiente opción:

* **`Branding_RT_ListXtkOptions_toPublish`**: enumere aquí los nombres de las opciones XTK para las fórmulas personalizadas (separados por comas). Esto garantiza que los envíos de RT puedan aplicar las fórmulas de seguimiento personalizadas.