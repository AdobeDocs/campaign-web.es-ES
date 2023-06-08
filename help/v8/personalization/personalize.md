---
title: Personalización del contenido en Campaign
description: Obtenga información sobre cómo personalizar su contenido en la IU de la web de Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: d12c3019fb47164864259ecc40225fcb04de0e6c
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 8%

---


# Personalización de su contenido{#add-personalization}

La personalización se puede añadir a cualquier entrega mediante el editor de expresiones.

Una etiqueta de personalización siempre utiliza la siguiente sintaxis: `<%=table.field%>`Por ejemplo, para insertar el nombre del destinatario, almacenado en la tabla de destinatarios, la etiqueta de personalización utiliza la sintaxis &lt;%= recipient.lastName %>.

Cuando se prepara una entrega, Adobe Campaign interpreta automáticamente estas etiquetas y las sustituye el valor del campo para un destinatario determinado. El reemplazo físico se puede ver al simular el contenido.

Para añadir etiquetas de personalización a un envío, haga clic en el icono del cuadro de diálogo Open personalization al que se puede acceder desde campos de edición de tipo texto, como la línea de asunto o el cuerpo del SMS.

![](assets/perso-access.png)

Se muestra el editor de expresiones. Los campos personalizados se organizan en tres menús, situados a la izquierda de la pantalla. Estos menús proporcionan acceso a todos los campos disponibles en la base de datos de Adobe Campaign.

| Menú | Descripción |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | El **[!UICONTROL Destinatario]** El menú enumera todos los campos definidos en la tabla de destinatarios, como el nombre, la edad o la dirección de los destinatarios. |
| ![](assets/do-not-localize/perso-message-menu.png) | El **[!UICONTROL Mensaje]** El menú enumera todos los campos relacionados con los &quot;logs&quot; de entrega, es decir, todos los mensajes enviados a los destinatarios o dispositivos en todos los canales, como la fecha del último evento con un destinatario determinado |
| ![](assets/do-not-localize/perso-delivery-menu.png) | El **[!UICONTROL Envío]** El menú enumera todos los campos relacionados con los parámetros necesarios para realizar entregas, como el canal de entrega, la etiqueta, etc. |

>[!NOTE]
>
>De forma predeterminada, la lista muestra todos los campos de la tabla seleccionada (Destinatarios, / Mensaje / Envío). Si desea incluir campos de tablas vinculadas a la tabla seleccionada, habilite la opción **[!UICONTROL Mostrar atributos avanzados]** opción situada debajo de la lista.

Para añadir un campo de personalización, coloque el cursor en la ubicación deseada dentro del contenido y haga clic en el botón + para insertarlo.

![](assets/perso-insert-field.png)
