---
audience: end-user
title: Edición del contenido de correo electrónico
description: Obtenga información sobre cómo empezar a crear contenido con el Diseñador de correo electrónico en la interfaz de usuario web de Campaign
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: d7fc756b2e1d94b43c76ced748e1bf7c7ae5da0d
workflow-type: ht
source-wordcount: '409'
ht-degree: 100%

---


# Introducción al Diseñador de correo electrónico {#get-started-email-designer}

Una vez creado un correo electrónico en Adobe Campaign, debe definir su contenido.

El Diseñador de correo electrónico le permite crear correos electrónicos personalizados y cautivadores con una interfaz intuitiva para arrastrar y soltar. Ya sea desde una pizarra en blanco, importando contenido existente o aprovechando las plantillas existentes, diseñe y perfeccione el contenido de cada correo electrónico, ya sea promocional o transaccional.

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* Uso las funciones de diseño de correo electrónico de [!DNL Campaign] para crear fácilmente correos electrónicos adaptables. [Más información](create-email-content.md)

* Mejore la experiencia de los clientes creando funciones personalizadas basadas en sus atributos de perfil. [Más información](../personalization/personalize.md)

* Configure campos de contenido condicionados para crear una personalización dinámica basada en el perfil del destinatario. [Más información](../personalization/conditions.md)

## Prácticas recomendadas de diseño de correo electrónico {#best-practices}

Al enviar correos electrónicos, hay que tener en cuenta que los destinatarios pueden reenviarlos, lo que a veces puede causar problemas con el renderizado del correo electrónico. Esto es especialmente cierto cuando se utilizan clases CSS que pueden no ser compatibles con el proveedor de correo electrónico utilizado para el reenvío. Por ejemplo, si utiliza la clase CSS &quot;is-desktop-hidden&quot; para ocultar una imagen en dispositivos móviles, es posible que no se procese correctamente.

Para minimizar estos problemas de procesamiento, recomendamos mantener la estructura de diseño del correo electrónico tan simple como sea posible. Intente utilizar un solo diseño que funcione bien tanto para dispositivos de escritorio como móviles, y evite utilizar clases CSS complejas u otros elementos de diseño que puedan no ser totalmente compatibles con todos los clientes de correo electrónico. Cuando utilice imágenes en los correos electrónicos, evite las imágenes que tengan más de 2 MB o utilice vínculos de imagen codificados.

Al seguir estas prácticas recomendadas, puede ayudar a garantizar que los correos electrónicos se representen correctamente de forma coherente, independientemente de cómo los destinatarios los vean o reenvíen.

## Comience a crear el contenido {#start-authoring}

En el panel de envío de correo electrónico, vaya a la pantalla [Editar contenido](edit-content.md) para abrir la página principal del Diseñador de correo electrónico. A partir de ahí, elija cómo desea diseñar el correo electrónico entre las siguientes opciones:

* **Diseñe su correo electrónico desde cero** mediante la interfaz del diseñador de correo electrónico. Aprenda a diseñar el contenido de su correo electrónico en [esta sección](create-email-content.md).

* **Codifique o pegue el HTML sin procesar** directamente en el diseñador de correo electrónico. Aprenda a codificar su propio contenido en [esta sección](code-content.md).

* **Importación de contenido de HTML existente** desde un archivo o una carpeta .zip. Obtenga información sobre cómo importar contenido de correo electrónico en [esta sección](existing-content.md).

* **Seleccionar contenido existente** de una lista de plantillas integradas o personalizadas. Aprenda a trabajar con plantillas de correo electrónico en [esta sección](create-email-templates.md).

  ![Opciones disponibles en la interfaz del Diseñador de correo electrónico para crear correo electrónico contenido](assets/email_designer_create_options.png){zoomable="yes"}
