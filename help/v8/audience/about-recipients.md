---
title: Trabajar con destinatarios y públicos
description: Aprenda a trabajar con destinatarios en Campaign Web
badge: label="Beta"
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 25%

---

# Trabajar con destinatarios y públicos {#about-recipients}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Vista 360 de sus destinatarios"
>abstract="Cree nuevos destinatarios y monitorícelos mediante potentes informes y herramientas. Acceda a los atributos, interacciones y registros de su destinatario. Utilice las opciones de filtrado para examinar la lista de destinatarios, editar y actualizar su perfil."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Consulte las notas de la versión"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfiles"
>abstract="Un perfil es una persona que está destinada a recibir mensajes enviados por Adobe Campaign. En Adobe Campaign, los destinatarios son los perfiles predeterminados a los que se dirigen los envíos (correos electrónicos, SMS). En esta lista, puede ver el perfil del destinatario en función de sus permisos. Utilice las opciones de filtrado para examinar esta lista. Puede editar y actualizar un pequeño conjunto de atributos del destinatario."

Un destinatario es un perfil que está destinado a recibir mensajes enviados por Adobe Campaign. En Adobe Campaign, los destinatarios son los perfiles predeterminados a los que se dirigen los envíos (correos electrónicos, SMS, etc.). Los datos de destinatario almacenados en la base de datos permiten crear audiencias que reciban cualquier entrega dada y añadir datos de personalización en el contenido de la entrega. En la base de datos se almacenan otros tipos de perfiles. Están diseñados para diferentes usos: por ejemplo, se crean perfiles semilla para probar los envíos antes de enviarlos a la audiencia final.

Los destinatarios solo se pueden agregar desde la consola del cliente de Campaign. Sin embargo, se pueden ver en la web de Campaign, en la **Destinatarios** entrada del carril de navegación izquierdo. También puede editar los atributos del destinatario desde esa pantalla.

Para editar los datos del destinatario, haga clic en los tres puntos junto a su nombre y seleccione **Editar...**.

![Edición de un perfil de destinatario](assets/recipient-edit.png)

Puede actualizar un conjunto limitado de atributos, que son: nombre, apellidos, correo electrónico y número de teléfono.

![Actualización de un perfil de destinatario](assets/recipient-update.png)

>[!NOTE]
>
>Este formulario limitado de edición de perfiles solo se proporciona para pruebas de programas beta. Se mejorará en la versión futura. Permite al usuario añadir rápidamente una dirección de correo electrónico y un número de teléfono a cualquier perfil para que pueda probar los canales de correo electrónico y SMS y recibir los mensajes enviados.

Puede filtrar los destinatarios utilizando el campo de búsqueda, desde el **Mostrar filtros** botón.

También puede acceder a los destinatarios desde el **Explorer** vea, examine y cree carpetas y subcarpetas, y compruebe los permisos asociados.

![Lista de destinatarios de la vista del explorador](assets/recipients-from-explorer.png)

>[!NOTE]
>
>Según los permisos, es posible que no tenga acceso a la lista completa de destinatarios almacenados en la base de datos. Puede obtener más información sobre permisos en [esta sección](../get-started/permissions.md).

Además, puede administrar las suscripciones y bajas de sus destinatarios a servicios como los boletines informativos. Aprenda a trabajar con servicios de suscripción en [esta página](manage-services.md)

Puede crear flujos de trabajo para deduplicar, enriquecer, combinar perfiles y crear audiencias. Obtenga más información en [esta sección](../workflows/gs-workflows.md).
