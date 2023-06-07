---
title: Cree contenido condicional
description: Obtenga información sobre cómo definir condiciones para personalizar su contenido en la IU de la web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 8%

---

# Creación de contenido condicional{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Cree contenido condicional"
>abstract="Cree contenido condicional para definir una personalización dinámica basada en el perfil del destinatario, sustituyendo automáticamente los bloques de texto y las imágenes cuando se cumplen determinadas condiciones. Esta función puede llevar las campañas a otro nivel y ofrecer experiencias personalizadas y enfocadas a la audiencia."

El contenido condicional es una práctica funcionalidad que permite crear una personalización dinámica basada en el perfil del destinatario y reemplazar automáticamente bloques de texto e imágenes cuando se cumplen determinadas condiciones. Esta función puede llevar las campañas a otro nivel y ofrecer experiencias personalizadas y enfocadas a la audiencia.

Al configurar los campos de contenido condicional, se puede crear una personalización dinámica avanzada basada en el perfil del destinatario, por ejemplo. Los bloques de texto, los vínculos, la línea de asunto o las imágenes se sustituyen en el contenido del mensaje cuando se cumple una condición concreta. Por ejemplo, puede mostrar &quot;Sr.&quot; o &quot;Sra.&quot; según el valor del campo Género en la base de datos de Adobe Campaign, o incluir un vínculo diferente basado en el idioma preferido del destinatario.

## Sintaxis de personalización{#perso-syntax}

## Trabajo con condiciones en el editor de personalización{#condition-perso-editor}

Para definir un contenido condicional para una entrega:

1. Abra una entrega y edite el contenido.
1. Haga clic en **[!UICONTROL Abrir diálogo de personalización]** , por ejemplo, para SMS, a la derecha del campo Mensaje.

   ![](assets/open-perso-editor-sms.png)

1. En el editor de personalización, busque **[!UICONTROL Funciones de ayuda]**.
1. Haga clic en el icono &quot;+&quot; junto al **If** función. Se añade la siguiente línea a la pantalla central:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Reemplazar `<FIELD>` mediante un campo de personalización. Por ejemplo, la empresa del destinatario: `recipient.company`.
1. Reemplazar `<VALUE>` por el valor que se va a satisfacer. Por ejemplo, `ADOBE`.

## Ejemplo: línea de asunto de SMS condicional{#condition-subject-line}

Para crear una línea de asunto condicional para un mensaje SMS, siga los pasos a continuación:

1. Abra una entrega y edite el contenido.
1. Haga clic en el icono del cuadro de diálogo Abrir personalización, a la derecha de la línea de asunto.
1. En el editor de personalización, busque


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
