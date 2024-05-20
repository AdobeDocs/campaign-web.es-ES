---
audience: end-user
title: Crear fragmentos de contenido
description: Aprenda a crear con fragmentos de contenido
hidefromtoc: true
hide: true
exl-id: d155d102-a5bc-4b9b-b29c-24fde4d95ceb
source-git-commit: f96c807c2ee094ad4775b6bf56f5f02822da8d28
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 22%

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
* Utilícelos tantas veces como sea necesario en el contenido mediante el Diseñador de correo electrónico. Consulte [Añadir fragmentos visuales a los correos electrónicos](../email/use-visual-fragments.md).

## Creación de un fragmento visual {#create-fragments}

Existen dos formas de crear fragmentos:

* Cree un fragmento desde cero utilizando **[!UICONTROL Fragmentos]** menú específico. [Descubra cómo](#create-from-scratch)

* Al diseñar contenido, guarde una parte del contenido como fragmento. [Descubra cómo](#save-as-fragment)

Una vez guardado, el fragmento estará disponible para usar en un correo electrónico o en una plantilla de correo electrónico. Tanto si se crea desde cero como a partir de contenido existente, ahora puede utilizar este fragmento al crear cualquier contenido dentro de Campaign. Consulte [Añadir fragmentos visuales](../email/use-visual-fragments.md).

### Crear un fragmento desde cero {#create-from-scratch}

Para crear un fragmento desde cero, siga los pasos a continuación.

1. [Acceso a la lista de fragmentos](#access-manage-fragments) a través de **[!UICONTROL Gestión de contenido]** > **[!UICONTROL Fragmentos]** menú izquierdo.

   ![](assets/fragments-list.png)

1. Seleccionar **[!UICONTROL Crear fragmento]**.

1. Introduzca la etiqueta del fragmento.

   ![](assets/fragment-create.png)

1. Si es necesario, puede definir opciones adicionales, como el nombre interno del fragmento, su carpeta y una descripción.

   >[!NOTE]
   >
   >Por ahora, solo puede crear fragmentos visuales.

1. Haga clic en **Crear** para configurar el contenido del fragmento.

1. El [Diseñador de correo electrónico](../email/get-started-email-designer.md) muestra. Edite el contenido según sea necesario, del mismo modo que lo haría para cualquier correo electrónico dentro de una campaña. Puede añadir imágenes, vínculos, campos de personalización y contenido dinámico.

   ![](assets/fragment-designer.png)

1. Cuando el fragmento esté listo, haga clic en **[!UICONTROL Guardar y cerrar]**. Se añade a [lista de fragmentos](#access-manage-fragments).

Este fragmento ya está listo para utilizarse al crear cualquier [email](../email/get-started-email-designer.md) o [plantilla de contenido](use-email-templates.md) en Campaign. [Descubra cómo](../email/use-visual-fragments.md)


### Guardar contenido como fragmento {#save-as-fragment}

Cualquier contenido del correo electrónico se puede guardar como fragmento para su reutilización futura. Al diseñar una [plantilla de contenido](use-email-templates.md) o un [email](../email/get-started-email-designer.md) de envío, puede guardar una parte del contenido como fragmento visual. Para realizar esto, siga los pasos a continuación:

1. En el [Diseñador de correo electrónico](../email/get-started-email-designer.md), haga clic en **Más** en la parte superior derecha de la pantalla.

1. Seleccionar **[!UICONTROL Guardar como fragmento]** en el menú desplegable.

   ![](assets/fragment-save-as.png)

1. El **[!UICONTROL Guardar como fragmento]** se muestra. Seleccione los elementos que desee incluir en el fragmento, incluidos los campos de personalización y el contenido dinámico.

   >[!CAUTION]
   >
   >Sólo se pueden seleccionar secciones adyacentes entre sí. No puede seleccionar una estructura vacía u otro fragmento.

   ![](assets/fragment-save-as-screen.png)

1. Haga clic en **[!UICONTROL Crear]**. Rellene el nombre del fragmento y guárdelo.

   ![](assets/fragment-save-confirm.png)

   Este contenido es ahora un fragmento independiente , añadido al [lista de fragmentos](#manage-fragments)y accesibles desde el menú específico. Ahora puede utilizar este fragmento al crear cualquier [email](../email/get-started-email-designer.md) o [plantilla de contenido](use-email-templates.md) en Campaign. [Descubra cómo](../email/use-visual-fragments.md)

>[!NOTE]
>
>Cualquier cambio en ese nuevo fragmento no se propaga al correo electrónico o a la plantilla de los que proviene. Del mismo modo, cuando el contenido original se edita dentro de ese correo electrónico o plantilla, el nuevo fragmento no se modifica.

## Administrar los fragmentos {#manage-fragments}

Puede editar, actualizar, duplicar o eliminar un fragmento de la lista de fragmentos.

### Edición y actualización de un fragmento {#edit-fragments}

Para editar un fragmento, siga los pasos a continuación.

1. Haga clic en el nombre del fragmento para editarlo desde el **[!UICONTROL Fragmentos]** lista.
1. Haga clic en **Editar contenido** para abrir el contenido de este fragmento.

   ![](assets/fragment-edit-content.png)

1. Realice los cambios necesarios y guarde las modificaciones.

>[!CAUTION]
>
>Cualquier cambio en un fragmento se propaga a los envíos de correo electrónico o a las plantillas que lo utilizan.


### Eliminación de un fragmento {#delete-fragments}

Para eliminar un fragmento, siga estos pasos:

1. Vaya a la lista de fragmentos y haga clic en **[!UICONTROL Más acciones]** junto al fragmento que se va a eliminar.
1. Clic **Eliminar** y confirme.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Al eliminar un fragmento de contenido, se actualizan las entregas de correo electrónico y las plantillas que lo utilizan: el fragmento se elimina del contenido del correo electrónico, pero se sigue haciendo referencia a él. Para mantener el contenido del fragmento en esas entregas y plantillas, debe interrumpir la herencia antes de eliminar el fragmento, [como se detalla en esta sección](use-visual-fragments.md#break-inheritance).
>

### Duplicación de un fragmento {#duplicate-fragments}

Puede duplicar fácilmente un fragmento para crear uno nuevo. Para duplicar un fragmento existente, siga estos pasos:

1. Vaya a la lista de fragmentos y haga clic en **[!UICONTROL Más acciones]** junto al fragmento que se va a eliminar.
1. Clic **Duplicar** y confirme.
1. Introduzca la etiqueta del nuevo fragmento y guarde los cambios.

   El fragmento se agregará a la lista de fragmentos. Puede editarlo y configurarlo según sea necesario.
