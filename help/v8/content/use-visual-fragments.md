---
audience: end-user
title: Añadir fragmentos visuales a los correos electrónicos
description: Aprenda a añadir fragmentos visuales a los correos electrónicos
badge: label="Disponibilidad limitada"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 20%

---

# Añadir fragmentos visuales a los correos electrónicos {#use-visual-fragments}

>[!AVAILABILITY]
>
>Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

Puede usar un fragmento visual en [envío de correo electrónico](../email/get-started-email-designer.md) o en [plantilla de contenido](../email/use-email-templates.md). Los pasos se detallan a continuación. [Aprenda a crear y administrar fragmentos de contenido](fragments.md).

![](assets/fragments.gif)

## Uso de un fragmento visual {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Opciones de fragmentos"
>abstract="Este panel proporciona opciones relacionadas con el fragmento seleccionado. Permite elegir en qué dispositivos desea que se muestre el fragmento y abrir el contenido de este fragmento. Use la pestaña **[!UICONTROL Estilos]** para personalizar aún más el fragmento. También puede romper la herencia con el fragmento visual original."

<!-- pas vu dans l'UI-->

Para insertar un fragmento visual en un contenido de correo electrónico, siga los pasos a continuación:

1. Abra cualquier contenido de correo electrónico o plantilla con [Email Designer](../email/get-started-email-designer.md).

1. Seleccione el icono **[!UICONTROL Fragmentos]** del carril izquierdo.

   ![](assets/fragments-in-designer.png)

1. Se muestra la lista de todos los fragmentos visuales creados en la zona protegida actual. Puede hacer lo siguiente:

   * Busque un fragmento específico escribiendo su etiqueta.
   * Ordene los fragmentos en orden ascendente o descendente.
   * Cambie la forma en que se muestran los fragmentos (tarjetas o vista de lista).

   >[!NOTE]
   >
   >Los fragmentos se ordenan por fecha de creación: los fragmentos añadidos recientemente se muestran primero en la lista.

   Si se han modificado o agregado fragmentos visuales mientras edita el contenido, haga clic en el icono **Actualizar** para actualizar la lista con los cambios más recientes.

1. Arrastre y suelte cualquier fragmento visual de la lista en el área en la que desea insertarlo. Al igual que cualquier otro componente, puede mover el fragmento por el contenido.

1. Seleccione el fragmento para mostrar sus opciones en el panel derecho.

   ![](assets/fragment-right-pane.png)

   En la ficha **[!UICONTROL Configuración]**, puede:

   * Elija los dispositivos en los que desea que se muestre el fragmento.
   * Haga clic en el botón **Editar contenido** para abrir el contenido de este fragmento. [Más información](../content/fragments.md#edit-fragments)

     Puede personalizar aún más el fragmento mediante la ficha **[!UICONTROL Estilos]**.

1. Si es necesario, puede romper la herencia con el fragmento visual original. [Más información](#break-inheritance)

   También puede eliminar el fragmento del contenido o duplicarlo. Estas acciones se pueden realizar directamente desde el menú contextual que se muestra sobre el fragmento.

1. Agregue tantos fragmentos visuales como desee y **[!UICONTROL guarde]** sus cambios.

## Romper herencia {#break-inheritance}

Al editar un fragmento visual, los cambios se sincronizan. Se propagan automáticamente a todas las entregas de correo electrónico y a las plantillas de contenido que contienen ese fragmento.

Cuando se añaden a un correo electrónico o a una plantilla de contenido, los fragmentos se sincronizan de forma predeterminada.

Sin embargo, puede romper la herencia del fragmento original. En ese caso, el contenido del fragmento se copia en el diseño actual y los cambios ya no se sincronizan.

Para interrumpir la herencia, siga los pasos a continuación:

1. Seleccione el fragmento visual.

1. Haga clic en el icono de desbloqueo de la barra de herramientas contextual.

   ![](assets/fragment-break-inheritance.png)

1. Ese fragmento se convierte en un elemento independiente que ya no está vinculado al fragmento original. Edítela como cualquier otro componente de contenido en el contenido. [Más información](../email/content-components.md)
