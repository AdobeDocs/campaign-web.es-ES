---
audience: end-user
title: Edición del contenido de correo electrónico
description: Obtenga información sobre cómo empezar a crear contenido con el Diseñador de correo electrónico en la interfaz de usuario web de Campaign
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 45%

---


# Introducción al Diseñador de correo electrónico {#get-started-email-designer}

Una vez creado un correo electrónico en Adobe Campaign, debe definir su contenido.

El Diseñador de correo electrónico le permite crear correos electrónicos personalizados y cautivadores con una interfaz intuitiva de arrastrar y soltar. Ya sea desde una pizarra en blanco, importando contenido existente o aprovechando las plantillas existentes, diseñe y perfeccione el contenido de cada correo electrónico, ya sea promocional o transaccional.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Uso las funciones de diseño de correo electrónico de [!DNL Campaign] para crear fácilmente correos electrónicos adaptables. [Más información](create-email-content.md)

* Mejore la experiencia de los clientes creando correos electrónicos personalizados basados en sus atributos de perfil. [Más información](../personalization/personalize.md)

* Configure campos de contenido condicionados para crear una personalización dinámica basada en el perfil del destinatario. [Más información](../personalization/conditions.md)

## Prácticas recomendadas de diseño de correo electrónico {#best-practices}

Al enviar correos electrónicos, tenga en cuenta que los destinatarios pueden reenviarlos, lo que a veces puede causar problemas con el procesamiento del correo electrónico. Esto es especialmente cierto cuando se utilizan clases CSS que puede que el proveedor de correo electrónico no admita para el reenvío. Por ejemplo, si utiliza la clase CSS &quot;is-desktop-hidden&quot; para ocultar una imagen en dispositivos móviles, es posible que no se represente correctamente.

Para minimizar estos problemas de procesamiento, mantenga la estructura de diseño del correo electrónico lo más sencilla posible. Utilice un único diseño que funcione bien tanto para dispositivos de escritorio como móviles, y evite utilizar clases CSS complejas u otros elementos de diseño que puedan no ser totalmente compatibles con todos los clientes de correo electrónico. Al seguir estas prácticas recomendadas, se garantiza que los correos electrónicos se representen de forma coherente, independientemente de cómo los destinatarios los vean o reenvíen.

## Comience a crear el contenido {#start-authoring}

En el panel de envío de correo electrónico, vaya a la pantalla [Editar contenido](edit-content.md) para abrir la página principal del Diseñador de correo electrónico. A partir de ahí, elija cómo desea diseñar el correo electrónico entre las siguientes opciones:

* **Diseñe su correo electrónico desde cero** mediante la interfaz del diseñador de correo electrónico. Aprenda a diseñar el contenido de su correo electrónico en [esta sección](create-email-content.md).

* **Codifique o pegue el HTML sin procesar** directamente en el diseñador de correo electrónico. Aprenda a codificar su propio contenido en [esta sección](code-content.md).

* **Importación de contenido de HTML existente** desde un archivo o una carpeta .zip. Aprenda a importar el contenido del correo electrónico en [esta sección](existing-content.md).

* **Seleccionar contenido existente** de una lista de plantillas integradas o personalizadas. Aprenda a trabajar con plantillas de correo electrónico en [esta sección](create-email-templates.md).

  ![Opciones disponibles en la interfaz de Designer de correo electrónico para crear contenido de correo electrónico](assets/email_designer_create_options.png){zoomable="yes"}
