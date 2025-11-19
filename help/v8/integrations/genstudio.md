---
title: Trabajo con GenStudio for Performance Marketing en Adobe Campaign
description: Aprenda a trabajar con GenStudio for Performance Marketing en Adobe Campaign
feature: Email Design
topic: Content Management, Artificial Intelligence
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 61e6dcf13fc6a405f5e25328bf336e863701b2fe
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 8%

---

# Trabajo con GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="Uso de una plantilla creada con GenStudio"
>abstract="Gracias a la integración perfecta con Adobe GenStudio for Performance Marketing, puede importar fácilmente una plantilla de GenStudio mejorada con la tecnología de IA de Adobe."

## Introducción a GenStudio {#gs-genstudio}

[Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} es una aplicación generativa con prioridad de IA que permite a los equipos de marketing crear sus propios anuncios y correos electrónicos para impulsar campañas de marketing personalizadas e impactantes que se ajusten a los estándares de su marca y a las políticas de su empresa. Al aprovechar la tecnología de IA de Adobe, proporciona un conjunto completo de herramientas que simplifican las complejidades de la creación y administración de contenido para que los creativos puedan centrarse en la innovación.

>[!AVAILABILITY]
>
>Esta funcionalidad solo está disponible para el canal de correo electrónico.

Para mejorar la eficacia del marketing y mantener la coherencia de la marca, puedes integrar sin problemas las experiencias de [!DNL **GenStudio for Performance Marketing**] con [!DNL **Adobe Campaign**]. Esto le permite aprovechar la creación de contenido con potencia de IA de [!DNL GenStudio] junto con las capacidades de orquestación avanzadas de [!DNL Adobe Campaign].

>[!INFO]
>
>Para ir más lejos, mira esta [descripción general](https://business.adobe.com/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"} y una [demostración](https://business.adobe.com/products/genstudio-for-performance-marketing.html#demo){target="_blank"} de [!DNL Adobe GenStudio for Performance Marketing].

## Uso de las funcionalidades de GenStudio en Adobe Campaign {#use-genstudio}

La integración de [!DNL GenStudio for Performance Marketing] y [!DNL Adobe Campaign] le permite hacer que los especialistas en marketing de su compañía trabajen mejor juntos para optimizar los procesos.

Por ejemplo, un experto en marketing técnico, que usa [!DNL Adobe Campaign] para desarrollar y automatizar campañas por correo electrónico, puede colaborar con un especialista en marketing que crea contenido mediante [!DNL GenStudio].

Con esta integración, ambos pueden trabajar juntos para integrar fácilmente el contenido de marca de [!DNL GenStudio] en [!DNL Adobe Campaign], lo que proporciona correos electrónicos atractivos dirigidos a segmentos específicos de clientes e impulsa las ventas.

### Exportación de una plantilla de HTML de Adobe Campaign a GenStudio {#export-from-campaign-to-genstudio}

Primero, puede exportar una plantilla de HTML [!DNL Adobe Campaign] que incluya las directrices de su marca a [!DNL GenStudio for Performance Marketing]. Siga los pasos a continuación.

1. En [!DNL Adobe Campaign], acceda al contenido de su correo electrónico. [Descubra cómo](../email/create-email.md#create-content)

1. En Email Designer, seleccione **[!UICONTROL Exportar HTML]** del botón **[!UICONTROL Más]**.

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. Cargar esta plantilla exportada de HTML en [!DNL GenStudio for Performance Marketing]. <!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >Aprenda a cargar una plantilla de HTML en [!DNL GenStudio] en la sección [Guía del usuario de Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"} dedicada.<!--GenStudio doc to be updated with Campaign-->

1. En GenStudio, utilice esta plantilla para crear varias variaciones de correo electrónico con peticiones de datos de IA y guardarlas.

   >[!NOTE]
   >
   >Aprenda a crear experiencias de correo electrónico en la [sección](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"} de GenStudio.

### Aprovechamiento de las experiencias de GenStudio en Adobe Campaign {#leverage-genstudio-experiences}

Para aprovechar las [!DNL GenStudio] variaciones de correo electrónico que acaba de crear importándolas a [!DNL Adobe Campaign], siga los pasos a continuación.

1. En [!DNL Adobe Campaign], [cree un envío de correo electrónico](../email/create-email.md).

1. En el panel de envío de correo electrónico, haga clic en el botón **[!UICONTROL Editar contenido]**. [Más información](../email/create-email.md#create-content)

1. En la página de inicio de Designer de correo electrónico, seleccione **[!UICONTROL Importar HTML]** y haga clic en el botón **[!UICONTROL Adobe GenStudio for Performance Marketing]**.

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. Examine las experiencias de GenStudio para empezar a crear contenido. Puede filtrar las experiencias según varios criterios, como productos, personalidades, marcas o incluso colores.

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. Seleccione una experiencia y haga clic en **[!UICONTROL Usar]**.

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. Seleccione la carpeta donde desea importar la experiencia de GenStudio.

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. El contenido seleccionado se muestra en el Designer de correo electrónico.

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >Las experiencias de GenStudio [creadas a partir de una [!DNL Adobe Campaign] plantilla](#export-from-ajo-to-genstudio) se importan directamente en el Designer de correo electrónico. Las experiencias de GenStudio creadas sin una plantilla [!DNL Adobe Campaign] se importan en [modo de compatibilidad](../email/existing-content.md).

   Use las [herramientas de edición de contenido de correo electrónico](../email/create-email-content.md) y los [campos de personalización](../personalization/personalize.md) para editar su correo electrónico como desee. Guarde el contenido.

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456038/?quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->