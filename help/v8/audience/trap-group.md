---
audience: end-user
title: Usar un grupo de reventado
hide: true
hidefromtoc: true
description: Aprenda a utilizar un grupo de reventado para su envío en la interfaz de usuario web de Campaign
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# Usar un **[!UICONTROL grupo de reventado]** {#trap-group}

Se usa un **[!UICONTROL grupo de reventado]** (también conocido como **[!UICONTROL lista semilla]**) para incluir direcciones específicas en las entregas a fin de supervisar y verificar el proceso de distribución mediante perfiles de destino que no coinciden con los criterios de destino definidos. De este modo, los destinatarios que estén fuera del alcance de la entrega pueden recibirlo como lo haría cualquier otro destinatario.
Un **[!UICONTROL grupo de captura]** es un grupo de **[!UICONTROL direcciones semilla]**, denominadas **[!UICONTROL perfil de prueba]** en la interfaz de usuario web de CA.

## Por qué usar **[!UICONTROL Grupo de reventado]**

Puede usar **[!UICONTROL grupo de reventado]** :

1. **Como prueba** : cada miembro del **[!UICONTROL grupo de captura]** recibirá la entrega como si formara parte de la audiencia.


1. **Para proteger tu lista de correo** : al recibir lo que la audiencia recibirá, cada **[!UICONTROL perfil de prueba]** del **[!UICONTROL grupo de trampas]** recibirá una notificación si la lista de correo la usa un tercero.

>[!NOTE]
>
>El grupo de captura es diferente de [enviar pruebas durante la creación de la entrega](../email/create-email.md#preview-test) y de [grupo de control](control-group.md).


## Acerca de **[!UICONTROL Grupo de reventado]**

Los perfiles de prueba se excluyen automáticamente de los informes en las siguientes estadísticas de envío: **Clics**, **Aperturas**, **Cancelaciones de suscripciones**. Los informes solo tratan sobre la audiencia real.

Para una entrega por correo electrónico, solo se necesita la dirección de correo electrónico para el **[!UICONTROL grupo de reventado]**, la personalización de los demás campos se rellenará aleatoriamente mediante Campaign.

## Cómo configurar un **[!UICONTROL grupo de reventado]** en el envío

Para configurar un **[!UICONTROL grupo de reventado]**, ve a la configuración de **[!UICONTROL Audiencia]** de tu entrega. Dispone de dos opciones:
- [Seleccionar perfiles de prueba](#select-test-profile)
- [Crear condición](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Seleccionar perfiles de prueba {#select-test-profiles}

Al elegir &quot;Seleccionar perfiles de prueba&quot;, aparecerá la siguiente ventana donde se le invita a **[!UICONTROL Agregar perfil(es) de prueba]** :

![](assets/trap-no-test-profile.png){zoomable="yes"}

Al hacer clic en el botón, tendrá acceso a los perfiles de prueba a los que puede agregar su **[!UICONTROL grupo de captura]**. Seleccione los que desee utilizar.
Puede crear nuevos perfiles de prueba. [Más información](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Cuando confirme los perfiles de prueba, compruebe que dispone del número correcto en **[!UICONTROL Grupo de reventado]**.

![](assets/trap-check.png){zoomable="yes"}

### Crear condición {#create-condition}

Con la opción **[!UICONTROL Crear condición]** , obtendrá una nueva ventana donde podrá personalizar una consulta para definir los perfiles de prueba que desee utilizar

![](assets/trap-create-condition.png){zoomable="yes"}

Su consulta se mostrará en **[!UICONTROL Grupo de reventado]**.

![](assets/trap-custom.png){zoomable="yes"}

## Crear un nuevo **[!UICONTROL perfil de prueba]** {#create-seed}

Puede crear un nuevo **[!UICONTROL perfil de prueba]** en **[!UICONTROL Explorador]** > **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Miembros semilla]**

![](assets/trap-create.png){zoomable="yes"}

Puede completar todos los detalles sobre su **[!UICONTROL perfil de prueba]** como si fuera un perfil de audiencia:

![](assets/trap-create-contact.png){zoomable="yes"}