---
title: ¿Cómo hacer que su contenido sea dinámico?
description: Aprenda a hacer que su contenido sea dinámico mediante la personalización y el contenido condicional.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
old-role: Data Architect
role: Developer
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: ht
source-wordcount: '620'
ht-degree: 100%

---

# ¿Cómo hacer que su contenido sea dinámico? {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalización"
>abstract="El editor de personalización permite seleccionar, organizar, personalizar y validar todos los datos para crear una experiencia personalizada del contenido. Puede personalizar los mensajes para cada destinatario aprovechando los datos de perfil y crear contenido condicional para adaptar el mensaje a cada destinatario y mostrar solo el contenido relevante."

Como experto en marketing, es crucial dirigirse a los clientes que están genuinamente interesados en sus ofertas y comprometerse con ellas, proporcionando contenido efectivo y relevante. Dada la amplia gama de destinatarios que encuentra, crear varios fragmentos de contenido de marketing para atraer a diferentes personas puede consumir tiempo y ser un derroche. Aquí es donde el contenido dinámico se vuelve esencial.

Las funcionalidades de contenido dinámico de la web de Adobe Campaign le permiten personalizar el contenido en función de la información que haya recopilado sobre los destinatarios. Al utilizar contenido dinámico, se asegura de que sus esfuerzos de marketing sean más relevantes, lo que evita la comercialización de productos o servicios no deseados o innecesarios. Este método hace que el contenido sea más atractivo y aumenta la probabilidad de que se lea. Además, le permite personalizar el contenido, lo que hace que los destinatarios sientan que están recibiendo información de una persona, en lugar de una máquina.

## ¿Cómo hacer que su contenido sea dinámico? {#make-content-dyn}

Puede hacer que el contenido del mensaje sea dinámico insertando construcciones JavaScript en el editor de expresiones de la web de Campaign. Al enviar el mensaje, Adobe Campaign interpreta esas expresiones para entregar el contenido correcto a cada uno de sus destinatarios:

* **Personalizar los mensajes** a cada destinatario específico aprovechando los datos de perfil como su nombre, intereses, dónde viven, qué compraron y mucho más. Puede seleccionar cualquier campo disponible en la base de datos desde el editor de personalización relacionado con el destinatario, el mensaje o el envío. Estos atributos de personalización se pueden insertar en la línea de asunto o en el cuerpo de los mensajes. La siguiente sintaxis inserta la ciudad del destinatario en el contenido: `<%= recipient.location.city %>`.

  [Descripción: Ejemplo de inserción de la ciudad del destinatario en el asunto mediante atributos de personalización.](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **Creación de contenido condicional** para adaptar los envíos a cada destinatario y mostrar únicamente el contenido relevante para un cliente determinado en función de la información que tenga sobre él. Esto le permite mostrar bloques de texto o imágenes específicos basados en condiciones. Por ejemplo, adapte un banner de correo electrónico en función de la suscripción de los destinatarios a un servicio específico.

  [Descripción: Ejemplo de contenido condicional en un banner de correo electrónico basado en la suscripción del destinatario.](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [Descubra esta función en vídeo](#video)

## Acceso al editor de expresiones {#access}

La web de Adobe Campaign proporciona un editor de expresiones en el que puede seleccionar, organizar, personalizar y validar todos los datos para crear una experiencia personalizada para el contenido. El editor de expresiones está disponible para todos los canales en todos los campos con el **[!UICONTROL cuadro de diálogo Abrir personalización]**, como el campo de línea de asunto o los vínculos de correo electrónico y los componentes de contenido de texto/botón.

A continuación, se muestran algunos ejemplos sobre cómo acceder al editor de expresiones en función del contenido que desee hacer dinámico:

* *Acceso al editor de expresiones desde el campo Nombre del remitente*

  [Descripción: Ejemplo de acceso al editor de expresiones desde el campo Nombre del remitente.](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *Acceso al editor de expresiones desde un componente de texto de correo electrónico*

  [Descripción: Ejemplo de acceso al editor de expresiones desde un componente de texto de correo electrónico.](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *Acceso al editor de expresiones desde un vínculo en un correo electrónico*

  [Descripción: Ejemplo de acceso al editor de expresiones desde un enlace en un correo electrónico.](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>Además del editor de expresiones, también puede utilizar un generador de contenido condicional dedicado al diseñar un correo electrónico. [Aprenda a crear contenido condicional en correos electrónicos](conditions.md)

## Vídeos explicativos {#video}

Aprenda a hacer que el contenido del mensaje sea dinámico mediante el editor de expresiones para personalizar el mensaje o añadir contenido condicional.

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)