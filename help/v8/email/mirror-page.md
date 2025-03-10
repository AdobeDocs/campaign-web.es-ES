---
audience: end-user
title: Añadir un vínculo a la página espejo
description: Aprenda a añadir y administrar el vínculo a la página espejo
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 00a612513bcb649d23b2c5b4d5ed05b06a6a80ef
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 73%

---

# Página espejo {#mirror-page}

La página espejo es una versión en línea del correo electrónico. Añadir un vínculo a la página espejo es una práctica recomendada de marketing por correo electrónico. Los usuarios pueden navegar a la página espejo de un correo electrónico, por ejemplo, si están experimentando problemas de renderización o imágenes rotas al intentar verlo en su bandeja de entrada. También se recomienda proporcionar una versión en línea por motivos de accesibilidad o para fomentar el uso compartido en redes sociales.

La página espejo generada por Adobe Campaign contiene todos los datos de personalización.

![ejemplo de vínculo espejo](assets/mirror-page-link.png){width="600" align="left"}

## Añadir un vínculo a la página espejo{#link-to-mirror-page}

En Adobe Campaign, puede insertar un vínculo a la página espejo en el contenido del correo electrónico mediante el **bloque de personalización** específico. El bloque de personalización integrado **Vínculo a página espejo** inserta el siguiente código en el contenido del correo electrónico: `<%@ include view='MirrorPage' %>`.

Para añadir un vínculo a una página espejo en el correo electrónico, siga estos pasos:

1. Seleccione un elemento (texto o imagen) y haga clic en **[!UICONTROL Insertar vínculo]** en la barra de herramientas contextual.

   ![](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Seleccione el icono **[!UICONTROL Añadir personalización]** para acceder al menú de personalización.

   ![](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. En el menú **[!UICONTROL Fragmentos]**, seleccione **[!UICONTROL URL de página espejo]** y haga clic en **[!UICONTROL Agregar]**. [Aprenda a utilizar fragmentos de expresiones](../content/use-expression-fragments.md)

   ![](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

La página espejo se crea automáticamente.

Una vez enviado el correo electrónico, cuando los destinatarios hacen clic en el vínculo de la página espejo, el contenido del correo electrónico se muestra en su navegador web predeterminado.

De manera predeterminada, el período de retención de una página espejo es de **60 días**. Después de ese retraso, la página espejo ya no está disponible.

>[!CAUTION]
>
>* Los vínculos de páginas espejo se generan automáticamente y no se pueden editar. Contienen todos los datos personalizados cifrados necesarios para procesar el correo electrónico original. Como resultado, el uso de atributos personalizados con valores grandes puede generar direcciones URL de páginas espejo largas, lo que puede impedir que el vínculo funcione en exploradores web que tengan una longitud máxima de direcciones URL.
>
>* En la prueba enviada a los perfiles de prueba, el vínculo a la página espejo no está activo. Solo está activo en los mensajes finales.


## Generación de páginas espejo {#mirror-page-generation}

De forma predeterminada, Adobe Campaign genera automáticamente la página espejo si el contenido del correo electrónico no está vacío y si contiene un vínculo a la página espejo (también conocido como vínculo espejo).

Puede controlar el modo de generación de la página espejo del correo electrónico. Las opciones están disponibles en las propiedades del envío. [Más información](../advanced-settings/delivery-settings.md#mirror)
