---
audience: end-user
title: Añadir fragmentos visuales a los correos electrónicos
description: Aprenda a añadir fragmentos visuales a los correos electrónicos
badge: label="Disponibilidad limitada"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 13%

---

# Añadir fragmentos visuales a los correos electrónicos {#use-visual-fragments}

>[!AVAILABILITY]
>
>Esta capacidad requiere una actualización de Campaign v8.6.4. Obtenga más información en las [notas de la versión de la consola del cliente de Campaign v8](https://experienceleague.adobe.com/es/docs/campaign/campaign-v8/releases/release-notes).

En la interfaz web de Campaign, **los fragmentos visuales** son bloques visuales predefinidos que se pueden reutilizar en varios [envíos de correo electrónico](../email/get-started-email-designer.md) o en [plantillas de contenido](../email/use-email-templates.md). Aprenda a crear y administrar fragmentos de contenido en [esta sección](fragments.md).

![Representación visual de fragmentos visuales en uso](assets/do-not-localize/fragments.gif)

## Uso de un fragmento visual {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Opciones de fragmentos"
>abstract="Este panel proporciona opciones relacionadas con el fragmento seleccionado. Permite elegir en qué dispositivos desea que se muestre el fragmento y abrir el contenido de este fragmento. Use la pestaña **[!UICONTROL Estilos]** para personalizar aún más el fragmento. También puede romper la herencia con el fragmento visual original."

<!-- pas vu dans l'UI-->

Para insertar un fragmento visual en el contenido del correo electrónico, siga estos pasos:

1. Abra cualquier contenido de correo electrónico o plantilla con [Email Designer](../email/get-started-email-designer.md).

1. Seleccione el icono **[!UICONTROL Fragmentos]** del carril izquierdo.

   ![Captura de pantalla que muestra el icono Fragmentos en la interfaz de Designer de correo electrónico](assets/fragments-in-designer.png)

1. Se muestra la lista de todos los fragmentos visuales creados en la zona protegida actual. Puede hacer lo siguiente:

   * Busque un fragmento específico escribiendo su etiqueta.
   * Ordene los fragmentos en orden ascendente o descendente.
   * Cambie la forma en que se muestran los fragmentos (tarjetas o vista de lista).

   >[!NOTE]
   >
   >Los fragmentos se ordenan por fecha de creación. Los fragmentos agregados recientemente aparecen primero en la lista.

   Si se modifican o agregan fragmentos visuales mientras edita el contenido, haga clic en el icono **Actualizar** para actualizar la lista con los cambios más recientes.

1. Arrastre y suelte cualquier fragmento visual de la lista en el área en la que desea insertarlo. Al igual que cualquier otro componente, puede mover el fragmento por el contenido.

1. Seleccione el fragmento para mostrar sus opciones en el panel derecho.

   ![Captura de pantalla que muestra las opciones de fragmento en el panel derecho](assets/fragment-right-pane.png)

   En la ficha **[!UICONTROL Configuración]**, puede:

   * Elija los dispositivos en los que desea que se muestre el fragmento.
   * Haga clic en el botón **Editar contenido** para abrir el contenido de este fragmento. [Más información](../content/fragments.md#edit-fragments)

     Puede personalizar aún más el fragmento mediante la ficha **[!UICONTROL Estilos]**.

1. Si es necesario, interrumpa la herencia con el fragmento visual original. [Más información](#break-inheritance)

   También puede eliminar el fragmento del contenido o duplicarlo. Realice estas acciones directamente desde el menú contextual que se muestra en la parte superior del fragmento.

1. Agregue tantos fragmentos visuales como sea necesario y **[!UICONTROL guarde]** sus cambios.

### Fragmento visual en modo de solo lectura {#fragment-readonly}

Los derechos de acceso pueden aplicarse a los fragmentos visuales.

Si no se concede la edición de permisos para un fragmento visual concreto, la plantilla de contenido se muestra en **modo de solo lectura**. En este caso, el botón **[!UICONTROL Editar contenido]** se reemplaza con el botón **[!UICONTROL Ver contenido]**, lo que le permite ver el fragmento sin realizar cambios.

![Captura de pantalla que muestra un fragmento visual en modo de solo lectura](assets/fragment-readonly.png){zoomable="yes"}

Como se muestra a continuación, todos los iconos de funciones están desactivados, lo que limita la interacción únicamente a la visualización.

![Captura de pantalla que muestra iconos de funciones desactivadas en modo de solo lectura](assets/fragment-readonly-view.png){zoomable="yes"}

## Romper herencia {#break-inheritance}

Al editar un fragmento visual, los cambios se sincronizan y se propagan automáticamente a todas las entregas de correo electrónico y a las plantillas de contenido que contienen ese fragmento.

De forma predeterminada, los fragmentos se sincronizan cuando se añaden a un correo electrónico o a una plantilla de contenido.

Sin embargo, puede romper la herencia del fragmento original. En este caso, el contenido del fragmento se copia en el diseño actual y los cambios ya no se sincronizan.

Para interrumpir la herencia, siga estos pasos:

1. Seleccione el fragmento visual.

1. Haga clic en el icono de desbloqueo de la barra de herramientas contextual.

   ![Captura de pantalla que muestra el icono de desbloqueo para romper la herencia](assets/fragment-break-inheritance.png)

1. El fragmento se convierte en un elemento independiente que ya no está vinculado al fragmento original. Edítela como cualquier otro componente de contenido en el contenido. [Más información](../email/content-components.md)