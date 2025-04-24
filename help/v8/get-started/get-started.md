---
audience: end-user
title: Introducción a Adobe Campaign Web
description: Introducción a Adobe Campaign Web
exl-id: 885d7851-4e5d-4b03-ba6f-71f90ede83e8
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Introducción a Adobe Campaign Web {#get-started}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_learnmore"
>title="Introducción"
>abstract="La nueva interfaz de Adobe Campaign Web ofrece una experiencia del usuario integrada, intuitiva y coherente."

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_learnmore"
>title="Introducción"
>abstract="La nueva interfaz de Adobe Campaign Web ofrece una experiencia del usuario integrada, intuitiva y coherente."

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="Introducción"
>abstract="La nueva interfaz de Adobe Campaign Web ofrece una experiencia del usuario integrada, intuitiva y coherente."

Adobe Campaign ofrece una plataforma para diseñar experiencias de canales múltiples para clientes, y proporciona un entorno para la orquestación de campañas visual, la administración de interacciones en tiempo real y la ejecución multicanal.

La versin 8 de Adobe Campaign es la herramienta de campañas de última generación creada para diversos canales de marketing como el correo electrónico, las notificaciones push, los SMS y el correo directo. Proporciona sólidas capacidades de ETL y de administración de datos para diseñar y depurar la campaña perfecta. Su motor de orquestación permite programas de marketing multitáctil enriquecidos con un enfoque central en los recorridos impulsados por lotes. También incluye un servidor de mensajería en tiempo real escalable que permite a los equipos de marketing enviar mensajes predefinidos basados en una carga útil inclusiva desde cualquier sistema de TI para comunicaciones como restablecimiento de contraseñas, confirmación de pedidos, recibos electrónicos y mucho más.

Utilice Campaign para lo siguiente:

* **Impulso** de la personalización y la participación mediante una única vista accesible del cliente.
* **Integración** de canales de correo electrónico, móviles, en línea y sin conexión en el recorrido del cliente.
* **Automatización** del envío de mensajes y ofertas significativos y oportunos.

## Descubra la interfaz de usuario web de Campaign {#web}

Inicialmente, solo estaba disponible a través de la [consola del cliente](#ac-client). Aunque ahora, Campaign ofrece una nueva interfaz web de usuario (IU) mejorada: con mejores en la facilidad de uso, en la accesibilidad, y un nuevo diseño para mejorar significativamente la experiencia del usuario. Esta interfaz de usuario moderna simplifica el diseño y el envío de las campañas de marketing, y aporta coherencia junto con otras soluciones de Adobe, como Adobe Experience Platform.

![Captura de pantalla de la pantalla de inicio de la interfaz de usuario web de Adobe Campaign](assets/home.png){zoomable="yes"}

Esta nueva interfaz de usuario web cubre principalmente las necesidades de los **profesionales empresariales**. Las tareas de administración habituales no están disponibles en esta versión inicial, pero se abordarán en versiones posteriores. Tenga en cuenta que no todas las funcionalidades u opciones disponibles en la consola del cliente están disponibles en la nueva interfaz de usuario. En futuras versiones se introducirán nuevos casos de uso, opciones y funciones.

Como administrador o usuario experto, si necesita acceder a las funciones de la versión 8 de Campaign que no están disponibles en la interfaz de usuario web de Campaign, conéctese a la [consola del cliente](#ac-client).

Obtenga información sobre cómo conectarse a la web de Adobe Campaign en [esta página](connect-to-campaign.md).

➡️ [Descubra la web de Campaign en vídeo](#video)

## Acerca de la consola del cliente de Campaign {#ac-client}

La consola de cliente está diseñada para que los administradores y los usuarios avanzados realicen sus tareas. La consola del cliente de Campaign es una aplicación basada en el explorador que se instala en el sistema. Utiliza la API de servicios web para conectarse al servidor de aplicaciones de Campaign.

Los datos de campaña se almacenan en el servidor de aplicaciones. Los datos son accesibles tanto en la consola del cliente como en la interfaz de usuario web de Campaign. Por ejemplo, si crea una plantilla de envíos mediante la consola del cliente, también estará disponible en la interfaz de usuario web de Campaign. De manera similar, si crea un envío de correo electrónico en la interfaz de usuario web de Campaign, puede acceder a este envío desde la consola del cliente.

Algunos objetos solo se pueden crear y administrar en la consola del cliente. Estos objetos pueden ser visibles y utilizarse en la interfaz de usuario web de Campaign, pero no se pueden crear ni modificar desde este entorno. Todos los objetos y componentes de Campaign son accesibles en la vista de Explorer, en el menú de navegación de la izquierda.

Para obtener más información sobre el uso de la versión 8 de Campaign con su consola de cliente, consulte la [documentación de la versión 8 de Campaign (consola de cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=es){target="_blank"}.

<!--
## How-to video {#video}

Learn how to access and navigate the Campaign Web user interface and how to customize the inventory lists. Discover the AI-powered Knowledge Assistant.

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12)
-->

<!--
## Get started for marketers and administrators

>[!BEGINTABS]

>[!TAB Get started for Marketers]

**Discover the interface**

The new Adobe Campaign Web interface offers a modern and intuitive user experience to simplify marketing campaign design and delivery. Learn more in this section. [Learn more](user-interface.md)

**Use plans, programs, campaigns**

Adobe Campaign allows you to easily orchestrate your targeted marketing initiatives, using the built-in campaign management capability. With the ability to define a schedule, you can plan the duration and timing of your campaigns to align with strategic objectives and maximize audience engagement. [Learn more](../campaigns/gs-campaigns.md)

**Create and manage profiles and audiences**

A profile is a record stored in the database, serving as a key component to create audiences for deliveries and add personalization data to your content. Learn how to access, manage, and explore profiles using the Campaign Web User Interface in [this page](../audience/gs-audiences-recipients.md).

Audiences are sets of profiles who share similar behaviors and/or characteristics. This collection of people can either be generated, selected, or loaded. Once created, audiences can be leveraged as the target population of your deliveries. Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups. Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups in [this section](../audience/delivery-recipients.md).

**Configure workflows**

With workflows, you can orchestrate the full range of processes and tasks, improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery. Plus, you can get your channels in sync with a single, easy-to-use interface for campaign orchestration.

Understand how workflows work and how to create a targeting workflow in this how-to video:

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)

Adobe Campaign Web user interface features a query modeler that simplifies the process of filtering the database based on various criteria. Learn how to use it in [this section](../query/query-modeler-overview.md)

**Work with deliveries**

You can create standalone deliveries from the **Deliveries** left menu, or create deliveries in the context of a workflow, included or not in a campaign. Learn how to create a delivery in [this page](../msg/gs-deliveries.md).

For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns. [Learn more](../msg/delivery-template.md)

Delivery settings are technical delivery parameters that are defined in the delivery template. They can be overloaded for each delivery. These settings are available from the **Settings** button available when editing a delivery or a delivery template.

Adobe Campaign Web dynamic content capabilities allow you to customize your content based on the information you have gathered about your recipients. By utilizing dynamic content, you ensure that your marketing efforts are more relevant, avoiding marketing unwanted or unnecessary products or services. Learn more about dynamic content in [this section](../content/fragments.md).

Once your delivery content has been defined, you can use profiles and test profiles to preview and test it before sending the message. This is a crucial step to ensure that it is accurate but also free of errors both in content and personalization settings.

* **Send email** - Learn how to create an email delivery from scratch, define the audience, design the content, simulate preview, and send a proof.
    Learn how to create your first targeted email. In this use case, you schedule the sending of an email to Silver and Gold loyalty members on a specific date.

    The Email Designer enables you to create captivating, individually tailored emails through an intuitive drag-and-drop interface.

    Learn how to preview email message content and personalization, send test deliveries (proofs) to specific recipients or subscribers for testing and validation, and check the email rendering in popular desktop, mobile, and web-based clients.

* **Send SMS** - SMS deliveries provide a practical and efficient way to send text messages to your customers' mobile devices. With this feature, you can create, personalize, and preview text-based messages for effective communication.

* **Send push notifications** - Push notifications are essential for reaching out to your mobile app users, even when they're not actively using your app. They serve various purposes like providing updates, driving specific actions, and notifying about deals.

    Adobe Campaign v8 can send rich push notifications. Parameters and settings depend on the mobile operating system:
    * Android Rich push documentation
    * iOS Rich push documentation

* **Send direct mail** - Direct mail is an offline channel that allows you to produce files to mass deliver personalized letters to your customers such as postcards, flyers, or catalogs. When creating a direct mail delivery, Adobe Campaign automatically generates an extraction file containing all the targeted profiles and selected data, such as postal addresses and profile attributes.<br/>

* **Create landing pages** - Adobe Campaign allows you to create, design, and share landing pages. Landing pages enable you to direct your users to online forms where they can update their data, opt-in/out from receiving your communications, or subscribe to a specific service such as a newsletter.

* **Use reporting** -  Adobe Campaign suite of reporting tools provides valuable insights into the effectiveness of your marketing efforts, allowing you to optimize your campaigns for maximum impact.

    Dynamic Reporting provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city, and age in addition to functional email campaign data like opens and clicks.

>[!TAB Get started for Admins]

**Work with the client console** 

* **Install client console** - Learn how to download and install the Adobe Campaign Client Console, create and manage your connections to multiple environments, and verify access to the Adobe Campaign Client console with this tutorial video.

    Learn how to download, install, and manage the Adobe Campaign Client Console with this documentation.

* **Discover console client interface** - Learn about the Adobe Campaign v8 user interface and how to navigate the main features with this tutorial video.

    You can access Adobe Campaign via its client console or its Web user interface. You can also use APIs to manage data and perform tasks in your Campaign platform.

**Understand Campaign general architecture**

Learn about the typical Adobe Campaign solution deployment.

Adobe Campaign is a cross-channel marketing solution that automates email, mobile, social, and offline campaigns. Adobe Campaign provides a central place to access your customer data and profiles. Use Adobe Campaign to orchestrate consistent experiences for your customers, design, execute, and personalize your marketing across channels, while improving customer experiences on every device and touchpoint.

**Administrate environment**

* **Connect to your environment(s)** - Once the client console is installed, follow the steps in this documentation to create the connection to the application server.

* **Define permissions** - Adobe Campaign lets you define and manage the rights assigned to users. These permissions are defined by combining operator group permissions, named rights, and permissions on folders.

* **Use Campaign control panel** - The Adobe Campaign Control Panel allows Adobe Campaign administrators to monitor key assets and perform administrative tasks, such as managing the SFTP storage by instance, managing GPG keys, or subdomains and certificates.

    Control Panel allows you to set up new connections to your instances by adding IP address ranges to the allow list.
    Subdomain configuration allows you to configure a sub-section of your domain (technically a "DNS zone") for use with Adobe Campaign.
    In the Control Panel, you can interact with all SFTP servers that are connected to Campaign instances that you have access to.

* **Use the audit trail** - In Adobe Campaign Web User Interface, the Audit trail feature provides users with full visibility into all modifications made to important entities within your instance, typically those that significantly impact a smooth operation of the instance.

**Set up user interface**

* **Customize campaign UI** - Guidelines for managing user interface settings like lists, units, or data display.

* **Add custom fields** - Custom fields are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. These custom fields are displayed in various screens, for example, the details of a profile or a test profile.

**Set up the branding**

Every company has brand guidelines that define both visual elements and technical details. Adobe Campaign helps you manage these guidelines centrally, so you can present a consistent brand image to your customers in everything you do, from logos in emails to the URLs and domains used in your campaigns.

**Understand data model creation**

Adobe Campaign comes with a pre-defined data model. This section gives some details on the built-in tables of the Adobe Campaign data model and their interaction. Adobe Campaign relies on a Cloud database containing tables that are linked together.

A schema is an XML document associated with a database table. It defines data structure and describes the SQL definition of the table.
When you create or extend a schema, you need to create or modify the associated input forms to make those changes visible to end-users.
An input form lets you edit an instance associated with a data schema from the Adobe Campaign client console. The form is identified by its name and namespace.

**Understand data management**

Use Adobe Campaign workflows to improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery.

Campaign helps you add contacts to the Cloud database. You can load a file, schedule and automate multiple contact updates, collect data on the Web, or enter profile information directly into the recipient table.

You can easily export your different reports to PDF or CSV format, which enables you to share, manipulate, or print them.
Quarantine is the way to manage the invalid addresses in deliveries.

**About delivery management**

Campaign Optimization is the Adobe Campaign module which lets you control, filter, and monitor the sending of deliveries. To avoid conflicts between campaigns, Adobe Campaign can test various combinations by applying specific constraint rules. This guarantees that the messages sent meet the needs and expectations of customers and company communication policies.

All marketing campaigns are based on a template, which stores main characteristics and capabilities. Campaign comes with a built-in template to create campaigns. This template has all functionalities enabled: Documents, Seed addresses, Approvals, Delivery outlines, etc.

Learn how to set up and manage subscriptions and target subscribers.

**Work with templates**

* **Campaigns** - Campaign templates contain pre-configured settings which can be reused for creating new campaigns. A set of built-in templates is available to help you get started.

* **Delivery** - For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns.

* **Workflows** - Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows. Using a workflow template is a best practice if you need to regularly import files with the same structure.

* **Content blocks** - Learn how to create dynamic content blocks and how to use them to personalize the content of your email delivery.

* **Landing pages** - Once you design your landing page content, you can save it for future reuse.

* **Content fragments** - A content fragment is a reusable component that can be referenced in one or more messages. When modifying a fragment, every content using it is updated.

* **Triggers** - Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message.

**Use subscription services**

Use Adobe Campaign Web to manage and create your services such as newsletters, and to check the subscriptions or unsubscriptions to these services.

**Configure delivery sending**

External accounts are used by technical processes such as technical workflows or campaign workflows. For example, when setting up a file transfer in a workflow or a data exchange with any other application (Adobe Target, Experience Manager, or other tools), you need to select an external account.

**Manage Adobe Campaign integrations**

You can connect your Campaign environment with Adobe Experience Cloud solutions and apps to combine capabilities.<br/>
Adobe Campaign comes with several connectors that allow you to communicate with external applications, connect to database engines, and share and synchronize data. These connections are configured by Adobe.

Here are the possible integrations:

**Use transactional messages**

Transactional messaging (Message Center) is a Campaign module designed for managing trigger messages. These notifications are generated from events triggered from information systems, and can include: invoices, order confirmations, shipping confirmations, password changes, product unavailability notifications, account statements, website account creations, and more.

**Use reporting**

Adobe Campaign provides a set of reporting tools.

>[!ENDTABS]

-->