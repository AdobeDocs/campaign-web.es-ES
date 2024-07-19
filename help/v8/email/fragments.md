---
audience: end-user
title: Crear fragmentos de contenido
description: Aprenda a crear con fragmentos de contenido
exl-id: d155d102-a5bc-4b9b-b29c-24fde4d95ceb
source-git-commit: 2d6b885642fbb6e1545f899219db05c156b069c4
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 24%

---

# Crear fragmentos de contenido {#fragments}

>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Defina sus propios fragmentos"
>abstract="Un fragmento es un componente reutilizable al que se puede hacer referencia en uno o varios correos electrónicos de distintas campañas. Esta capacidad se utiliza para la construcción previa de múltiples bloques de contenido personalizado que pueden ser utilizados por los usuarios de marketing para montar rápidamente los contenidos de correo electrónico en un proceso de diseño mejorado."

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Guardar fragmentos"
>abstract="Guardar fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Defina sus propios fragmentos"
>abstract="Un fragmento es un componente reutilizable al que se puede hacer referencia en uno o varios correos electrónicos de distintas campañas."

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Propiedades de fragmentos"
>abstract="Propiedades de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Tipo de fragmento"
>abstract="Seleccione el tipo de fragmento. Por ahora, solo están disponibles los fragmentos visuales para correos electrónicos."

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Defina sus propios fragmentos"
>abstract="Un fragmento es un componente reutilizable al que se puede hacer referencia en uno o varios correos electrónicos de distintas campañas. También puede utilizar fragmentos en las plantillas de correo electrónico. Por ahora, solo están disponibles los fragmentos visuales."

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Detalles de fragmentos"
>abstract="Detalles de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_create_fragment"
>title="Defina sus propios fragmentos"
>abstract="Un fragmento es un componente reutilizable al que se puede hacer referencia en uno o varios correos electrónicos de distintas campañas."

Un fragmento es un componente reutilizable al que se puede hacer referencia en uno o varios correos electrónicos de distintas campañas. Al modificar un fragmento, se actualiza todo el contenido que lo utiliza.

Esta funcionalidad permite crear previamente varios bloques de contenido personalizados que los usuarios de marketing pueden utilizar para ensamblar rápidamente el contenido del correo electrónico en un proceso de diseño mejorado.

![](assets/fragments.gif)

Para aprovechar al máximo los fragmentos:

* Cree sus propios fragmentos visuales, como se detalla a continuación.
* Utilícelos tantas veces como sea necesario en el contenido, a través del correo electrónico Designer. Ver [Agregar fragmentos visuales a los correos electrónicos](../email/use-visual-fragments.md).

>[!AVAILABILITY]
>
>Esta capacidad se encuentra en disponibilidad limitada (LA). Está restringido a los clientes que migran **de Adobe Campaign Standard a la versión 8 de Adobe Campaign** y no se puede implementar en ningún otro entorno.

## Creación de un fragmento visual {#create-fragments}

Existen dos formas de crear fragmentos:

* Cree un fragmento desde cero mediante el menú específico **[!UICONTROL Fragmentos]**. [Descubra cómo](#create-from-scratch)

* Al diseñar contenido, guarde una parte del contenido como fragmento. [Descubra cómo](#save-as-fragment)

Una vez guardado, el fragmento estará disponible para usar en un correo electrónico o en una plantilla de correo electrónico. Tanto si se crea desde cero como a partir de contenido existente, ahora puede utilizar este fragmento al crear cualquier contenido dentro de Campaign. Consulte [Agregar fragmentos visuales](../email/use-visual-fragments.md).

### Crear un fragmento desde cero {#create-from-scratch}

Para crear un fragmento desde cero, siga los pasos a continuación.

1. [Acceda a la lista de fragmentos](#access-manage-fragments) a través del menú que queda de **[!UICONTROL Administración de contenido]** > **[!UICONTROL Fragmentos]**.

   ![](assets/fragments-list.png)

1. Seleccione **[!UICONTROL Crear fragmento]**.

1. Introduzca la etiqueta del fragmento.

   ![](assets/fragment-create.png)

1. Si es necesario, puede definir opciones adicionales, como el nombre interno del fragmento, su carpeta y una descripción.

   >[!NOTE]
   >
   >Por ahora, solo puede crear fragmentos visuales.

1. Haga clic en el botón **Crear** para configurar el contenido del fragmento.

1. Se muestra [Email Designer](../email/get-started-email-designer.md). Edite el contenido según sea necesario, del mismo modo que lo haría para cualquier correo electrónico dentro de una campaña. Puede añadir imágenes, vínculos, campos de personalización y contenido dinámico.

   ![](assets/fragment-designer.png)

1. Una vez que el fragmento esté listo, haz clic en **[!UICONTROL Guardar y cerrar]**. Se agrega a la [lista de fragmentos](#access-manage-fragments).

Este fragmento ya está listo para usarse al generar [correo electrónico](../email/get-started-email-designer.md) o [plantilla de contenido](use-email-templates.md) en Campaign. [Descubra cómo](../email/use-visual-fragments.md)


### Guardar contenido como fragmento {#save-as-fragment}

Cualquier contenido del correo electrónico se puede guardar como fragmento para su reutilización futura. Al diseñar una [plantilla de contenido](use-email-templates.md) o un envío de [correo electrónico](../email/get-started-email-designer.md), puede guardar una parte del contenido como fragmento visual. Para realizar esto, siga los pasos a continuación:

1. En [Email Designer](../email/get-started-email-designer.md), haga clic en el botón **Más** en la parte superior derecha de la pantalla.

1. Seleccione **[!UICONTROL Guardar como fragmento]** en el menú desplegable.

   ![](assets/fragment-save-as.png)

1. Se muestra la pantalla **[!UICONTROL Guardar como fragmento]**. Seleccione los elementos que desee incluir en el fragmento, incluidos los campos de personalización y el contenido dinámico.

   >[!CAUTION]
   >
   >Sólo se pueden seleccionar secciones adyacentes entre sí. No puede seleccionar una estructura vacía u otro fragmento.

   ![](assets/fragment-save-as-screen.png)

1. Haga clic en **[!UICONTROL Crear]**. Rellene el nombre del fragmento y guárdelo.

   ![](assets/fragment-save-confirm.png)

   Este contenido es ahora un fragmento independiente , agregado a la [lista de fragmentos](#manage-fragments) y accesible desde el menú dedicado. Ahora puede usar este fragmento al crear cualquier [correo electrónico](../email/get-started-email-designer.md) o [plantilla de contenido](use-email-templates.md) en Campaign. [Descubra cómo](../email/use-visual-fragments.md)

>[!NOTE]
>
>Cualquier cambio en ese nuevo fragmento no se propaga al correo electrónico o a la plantilla de los que proviene. Del mismo modo, cuando el contenido original se edita dentro de ese correo electrónico o plantilla, el nuevo fragmento no se modifica.

## Administrar los fragmentos {#manage-fragments}

Puede editar, actualizar, duplicar o eliminar un fragmento de la lista de fragmentos.

### Edición y actualización de un fragmento {#edit-fragments}

Para editar un fragmento, siga los pasos a continuación.

1. Haga clic en el nombre del fragmento para editarlo desde la lista **[!UICONTROL Fragmentos]**.
1. Haga clic en el botón **Editar contenido** para abrir el contenido de este fragmento.

   ![](assets/fragment-edit-content.png)

1. Realice los cambios necesarios y guarde las modificaciones.

>[!CAUTION]
>
>Cualquier cambio en un fragmento se propaga a los envíos de correo electrónico o a las plantillas que lo utilizan.


### Eliminación de un fragmento {#delete-fragments}

Para eliminar un fragmento, siga estos pasos:

1. Vaya a la lista de fragmentos y haga clic en el botón **[!UICONTROL Más acciones]** que está junto al fragmento que desea eliminar.
1. Haga clic en **Eliminar** y confirme.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Al eliminar un fragmento de contenido, se actualizan las entregas de correo electrónico y las plantillas que lo utilizan: el fragmento se elimina del contenido del correo electrónico, pero se sigue haciendo referencia a él. Para mantener el contenido del fragmento en esas entregas y plantillas, debe interrumpir la herencia antes de eliminar el fragmento [, tal como se detalla en esta sección ](use-visual-fragments.md#break-inheritance).
>

### Duplicación de un fragmento {#duplicate-fragments}

Puede duplicar fácilmente un fragmento para crear uno nuevo. Para duplicar un fragmento existente, siga estos pasos:

1. Vaya a la lista de fragmentos y haga clic en el botón **[!UICONTROL Más acciones]** que está junto al fragmento que desea eliminar.
1. Haga clic en **Duplicar** y confirme.
1. Introduzca la etiqueta del nuevo fragmento y guarde los cambios.

   El fragmento se agregará a la lista de fragmentos. Puede editarlo y configurarlo según sea necesario.
