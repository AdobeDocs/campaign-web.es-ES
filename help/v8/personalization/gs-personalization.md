---
title: ¿Cómo hacer que su contenido sea dinámico?
description: Aprenda a hacer que su contenido sea dinámico mediante la personalización y el contenido condicional.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
exl-id: cce1da98-924b-415b-99d9-f4def4a4e874
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 47%

---

# ¿Cómo hacer que su contenido sea dinámico? {#gs-dynamic-content}

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="Personalización"
>abstract="El editor personalización le permite seleccionar, organizar, personalizar y validar todos los datos para crear un experiencia personalizado para su contenido. Puede personalizar los mensajes para cada destinatario aprovechando los datos de perfil y crear contenido condicional para adaptar el mensaje a cada destinatario y mostrar solo el contenido relevante."

Como experto en marketing, es crucial destino a los clientes que están realmente interesados en sus ofertas y atraerlos proporcionando contenido efectivos y relevantes. Dada la amplia gama de destinatarios que encuentra, crear varios fragmentos de contenido de marketing para atraer a diferentes personas puede consumir tiempo y ser un derroche. Aquí es donde contenido dinámico se vuelve esencial.

Adobe Campaign capacidades de contenido dinámico web le permiten personalizar su contenido en función de la información que ha recopilado sobre sus destinatarios. Al usar contenido dinámico, se asegura de que sus esfuerzos marketing sean más relevantes, evitando marketing productos o servicios no deseados o innecesarios. Este método hace que el contenido sea más atractivo y aumenta la probabilidad de que se lea. Además, le permite personalizar el contenido, lo que hace que los destinatarios sientan que están recibiendo información de una persona, en lugar de una máquina.

## ¿Cómo hacer que su contenido sea dinámico? {#make-content-dyn}

Puede hacer que su mensaje sea contenido dinámico insertando JavaScript construcciones en el editor de expresión Web Campaign. Al enviar el mensaje, Adobe Campaign interpreta esas expresiones para entregar la contenido correcta a cada uno de sus destinatarios:

* **Personalizar los mensajes** a cada destinatario específico aprovechando los datos de perfil como su nombre, intereses, dónde viven, qué compraron y mucho más. Puede seleccionar cualquier campo disponible en la base de datos desde el personalización editor relacionado con el destinatario, el mensaje o el envío. Estos atributos de personalización se pueden insertar en la línea de asunto o en el cuerpo de los mensajes. La sintaxis siguiente inserta la ciudad de la destinatario en el contenido: `<%= recipient.location.city %>`.

  [Descripción: Ejemplo de inserción de la ciudad del destinatario en la línea de asunto mediante atributos personalización.](assets/perso-subject-line.png){zoomable="yes"}{width="800" align="center"}

* **Creación de contenido condicional** para adaptar los envíos a cada destinatario y mostrar únicamente el contenido relevante para un cliente determinado en función de la información que tenga sobre él. Esto le permite mostrar bloques de texto o imágenes específicos basados en condiciones. Por ejemplo, adapte un banner de correo electrónico en función de la suscripción de los destinatarios a un servicio específico.

  [Descripción: ejemplo de contenido condicional en un banner de correo electrónico basado en la suscripción del destinatario.](assets/condition-sample.png){zoomable="yes"}{width="800" align="center"}

➡️ [Descubra esta funcionalidad en vídeo](#video)

## Acceso al editor de expresiones {#access}

Adobe Campaign Web proporciona un editor expresión donde puede seleccionar, organizar, personalizar y validar todos los datos para crear un experiencia personalizado para su contenido. El editor expresión está disponible para todos los canales, en todos los campos con el icono Abrir **[!UICONTROL personalización cuadro de diálogo]** , como el campo de línea de asunto, o correo electrónico vínculos y componentes de contenido de texto/botón.

A continuación se muestran algunos ejemplos de cómo acceder al editor de expresión en función de la contenido que desee dinamizar:

* *Acceso al editor de expresiones desde el campo Nombre del remitente*

  [Descripción: Ejemplo de acceso al editor de expresión desde el campo Nombre del remitente.](assets/expression-editor-access.png){zoomable="yes"}{width="800" align="center"}

* *Acceso al editor de expresiones desde un componente de texto de correo electrónico*

  [Descripción: ejemplo de acceso al editor de expresión desde un componente de texto correo electrónico.](assets/expression-editor-access-email.png){zoomable="yes"}{width="800" align="center"}

* *Acceso al editor de expresiones desde un vínculo en un correo electrónico*

  [Descripción: Ejemplo de acceso al editor de expresión desde una vincular de una correo electrónico.](assets/perso-link-insert-icon.png){zoomable="yes"}{width="800" align="center"}

>[!NOTE]
>
>Además del editor expresión, también puede utilizar un generador de contenido condicional específico al diseñar un correo electrónico. [Aprenda a crear contenido condicional en correos electrónicos](conditions.md)

## Vídeos explicativos {#video}

Aprenda a hacer que el contenido del mensaje sea dinámico mediante el editor de expresiones para personalizar el mensaje o añadir contenido condicional.

>[!VIDEO](https://video.tv.adobe.com/v/3425795?quality=12)