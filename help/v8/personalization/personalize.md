---
title: Personalización del contenido en Campaign
description: Aprenda a personalizar el contenido en Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: f57e0f2de12780ff9f90c2c5f1933b0e9bffe493
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---


# Personalización de su contenido {#add-personalization}

El Personalization del contenido de la entrega es una función clave que le permite adaptar los mensajes a destinatarios individuales, lo que hace que la comunicación sea más relevante y atractiva.

En Adobe Campaign, al usar [datos de perfil](#data-personalization), como el nombre del perfil, la ubicación o las interacciones anteriores, y [variables específicas de tu envío](#variables-personalization), puedes personalizar dinámicamente elementos como texto, imágenes y ofertas en tu comunicación.

La personalización de la entrega no solo mejora la experiencia del usuario, sino que también mejora las tasas de participación, lo que conduce a una mayor conversión y satisfacción del cliente.

## Uso de datos de perfil para la personalización {#data-personalization}

Puede personalizar cualquier envío con datos de perfil mediante el editor de expresiones, al que se puede acceder en campos con el icono **[!UICONTROL Abrir cuadro de diálogo de personalización]**, como la línea de asunto, los vínculos de correo electrónico y los componentes de contenido de texto/botón. [Obtenga información sobre cómo acceder al editor de expresiones](gs-personalization.md/#access)

### Sintaxis de Personalization {#syntax}

Las etiquetas de Personalization siguen una sintaxis específica: `<%= table.field %>`. Por ejemplo, para insertar el apellido del destinatario de la tabla de destinatarios, utilice la sintaxis `<%= recipient.lastName %>`.

Durante el proceso de preparación de la entrega, Adobe Campaign interpreta automáticamente estas etiquetas y las sustituye por los valores de campo correspondientes para cada destinatario. Puede ver el reemplazo real simulando el contenido.

Al cargar contactos desde un archivo externo para una entrega de correo electrónico independiente, todos los campos del archivo de entrada están disponibles para la personalización. La sintaxis es: `<%= dataSource.field %>`.

### Añadir etiquetas de personalización {#add}

Para añadir etiquetas de personalización a un envío, siga estos pasos:

1. Abra el editor de expresiones mediante el icono **[!UICONTROL Abrir cuadro de diálogo de personalización]** al que se puede acceder desde campos de edición de tipo texto, como la línea de asunto o el cuerpo del SMS. [Obtenga información sobre cómo acceder al editor de expresiones](gs-personalization.md/#access)

   ![](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. Se abre el editor de expresiones. Los campos personalizados disponibles en la base de datos de Adobe Campaign están organizados en varios menús a la izquierda de la pantalla:

   ![](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menú | Descripción |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | El menú **[!UICONTROL Aplicación de suscriptores]** enumera campos relacionados con los suscriptores de una aplicación, como el terminal utilizado o el sistema operativo. *Este menú solo está disponible para notificaciones push* |
   | ![](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | El menú **[!UICONTROL Destinatario]** enumera los campos definidos en la tabla de destinatarios, como los nombres de los destinatarios, las edades o las direcciones. Cuando [se cargan contactos desde un archivo externo](../audience/file-audience.md) para una entrega de correo electrónico independiente, este menú enumera todos los campos disponibles en el archivo de entrada. |
   | ![](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | El menú **[!UICONTROL Mensaje]** enumera los campos relacionados con los registros de envío, incluidos todos los mensajes enviados a los destinatarios o dispositivos en todos los canales, como la fecha del último evento con un destinatario determinado |
   | ![](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | El menú **[!UICONTROL Envío]** enumera los campos relacionados con los parámetros necesarios para realizar envíos, como el canal o la etiqueta de envío. |

   >[!NOTE]
   >
   >De forma predeterminada, cada menú enumera todos los campos de la tabla seleccionada (Destinatarios, / Mensaje / Envío). Si desea incluir campos de tablas vinculadas a la tabla seleccionada, habilite la opción **[!UICONTROL Mostrar atributos avanzados]** ubicada debajo de la lista.

1. Para agregar un campo de personalización, coloque el cursor en la ubicación deseada dentro del contenido y haga clic en el botón `+` para insertarlo.

1. Una vez que el contenido esté listo, puede guardarlo y probar la renderización de la personalización simulando el contenido. El ejemplo siguiente muestra la personalización de un mensaje SMS con los nombres de los destinatarios.

   ![](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Uso de variables para la personalización {#variables-personalization}

También puede utilizar variables para personalizar el envío.
Más información sobre [agregar variables a un envío](../advanced-settings/delivery-settings.md#variables-delivery).

Por ejemplo, tenemos la variable `deliveryType` definida de la siguiente manera.

![](assets/variables-deliveryType.png){zoomable="yes"}

Esta variable se puede usar en el contenido del envío con el icono **[!UICONTROL Agregar Personalization]** y la expresión `<%= variables.deliveryType %>` para nuestro ejemplo.

![](assets/variables-perso.png){zoomable="yes"}

Puede comprobar el uso de la variable con el botón **[!UICONTROL Simular contenido]**.

![](assets/variables-simulate.png){zoomable="yes"}
