---
audience: end-user
title: Usar un grupo de reventado
hide: true
hidefromtoc: true
description: Aprenda a utilizar un grupo de reventado para su envío en la interfaz de usuario web de Campaign
source-git-commit: 15d8ea478a234136dc654683798957d6c7026327
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 3%

---

# Usar un **[!UICONTROL grupo de reventado]** {#trap-group}

Se usa un **[!UICONTROL grupo de reventado]** para dirigirse a los destinatarios que no coinciden con los criterios de destino definidos. De este modo, los destinatarios que estén fuera del alcance de la entrega pueden recibirlo como lo haría cualquier otro destinatario.
Un **[!UICONTROL grupo de captura]** es un grupo de **[!UICONTROL direcciones semilla]**.

## Por qué usar **[!UICONTROL grupo de reventado]**

Puede usar **[!UICONTROL grupo de reventado]** :

1. **Como prueba** : cada miembro del **[!UICONTROL grupo de captura]** recibirá la entrega como si formara parte de la audiencia.


1. **Para proteger tu lista de correo** : al recibir lo que la audiencia recibirá, cada **[!UICONTROL dirección semilla]** del **[!UICONTROL grupo de trampas]** recibirá una notificación si la lista de correo la usa un tercero.

## Acerca de **[!UICONTROL Grupo de reventado]**

Las direcciones semilla se excluyen automáticamente de los informes en las siguientes estadísticas de envío: **Clics**, **Aperturas**, **Cancelaciones de suscripciones**. Los informes solo tratan sobre la audiencia real.

Para una entrega por correo electrónico, solo se necesita la dirección de correo electrónico para el **[!UICONTROL grupo de reventado]**, la personalización de los demás campos se rellenará aleatoriamente mediante Campaign.

## Cómo configurar un **[!UICONTROL grupo de reventado]** en el envío

Para configurar un **[!UICONTROL grupo de reventado]**, ve a la configuración de **[!UICONTROL Audiencia]** de tu entrega. Dispone de dos opciones:
- [Seleccionar perfiles de prueba](#select-test-profile)
- [Crear condición](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Seleccionar perfiles de prueba {#select-test-profiles}

Al elegir &quot;Seleccionar perfiles de prueba&quot;, aparecerá la siguiente ventana donde se le invita a **[!UICONTROL Agregar perfil(es) de prueba]** :

![](assets/trap-no-test-profile.png){zoomable="yes"}

Al hacer clic en el botón, tendrá acceso a las direcciones semilla a las que puede agregar su **[!UICONTROL grupo de captura]**. Seleccione los que desee utilizar.
Se pueden crear nuevas direcciones semilla. [Más información](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Cuando confirme las direcciones de captura, compruebe que tiene el número correcto en **[!UICONTROL Grupo de captura]**.

![](assets/trap-check.png){zoomable="yes"}

### Crear condición {#create-condition}

Con la opción **[!UICONTROL Crear condición]** , obtendrá una nueva ventana donde podrá personalizar una consulta para definir las direcciones semilla que desee utilizar

![](assets/trap-create-condition.png){zoomable="yes"}

Su consulta se mostrará en **[!UICONTROL Grupo de reventado]**.

![](assets/trap-custom.png){zoomable="yes"}

## Cómo crear una nueva **[!UICONTROL dirección semilla]** {#create-seed}

Puede crear una nueva **[!UICONTROL dirección semilla]** en **[!UICONTROL Explorador]** > **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Miembros semilla]**

![](assets/trap-create.png){zoomable="yes"}

Puede completar todos los detalles sobre el miembro semilla como si fuera un perfil de audiencia

![](assets/trap-create-contact.png){zoomable="yes"}