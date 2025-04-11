---
audience: end-user
title: Usar un grupo de reventado
description: Aprenda a utilizar un grupo de reventado para su envío en la interfaz de usuario web de Campaign
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 4%

---

# Usar un grupo de reventado {#trap-group}

Se usa un **[!UICONTROL grupo de reventado]** (también conocido como **[!UICONTROL lista semilla]**) para incluir direcciones específicas en las entregas a fin de supervisar y verificar el proceso de distribución mediante perfiles de destino que no coinciden con los criterios de destino definidos. De este modo, los destinatarios que estén fuera del ámbito de la entrega pueden recibirlo, como cualquier otro destinatario objetivo.

Un **[!UICONTROL grupo de captura]** es un grupo de **[!UICONTROL direcciones semilla]**, denominadas **[!UICONTROL perfil de prueba]** en la interfaz de usuario web de Campaign.

## Razones para utilizar un grupo de captura {#why-trap-group}

Puede usar un **[!UICONTROL grupo de reventado]**:

1. **Como prueba**: Cada miembro del **[!UICONTROL grupo de captura]** recibe la entrega como si formara parte de la audiencia.

1. **Para proteger tu lista de correo**: Al recibir lo que la audiencia recibirá, cada **[!UICONTROL perfil de prueba]** del **[!UICONTROL grupo de trampas]** recibirá una notificación si la lista de correo la usa un tercero.

>[!NOTE]
>
>Además de [enviar pruebas durante la creación de la entrega](../email/create-email.md#preview-test) y desde [grupo de control](control-group.md), agregar un grupo de captura es una buena manera de probar la audiencia.

## Grupos de reventado {#about-trap-group}

Los perfiles de prueba se excluyen automáticamente de los informes en las siguientes estadísticas de envío: **Clics**, **Aperturas**, **Cancelaciones de suscripciones**. Los informes se centran únicamente en la audiencia real.

Para una entrega por correo electrónico, solo se requiere la dirección de correo electrónico para el **[!UICONTROL grupo de reventado]**. Campaign rellena aleatoriamente la personalización de otros campos.

## Adición de un grupo de captura en una entrega {#trap-group-in-delivery}

Para configurar un **[!UICONTROL grupo de reventado]**, ve a la configuración de **[!UICONTROL Audiencia]** de tu envío. Tendrá dos opciones:

* [Seleccionar perfiles de prueba](#select-test-profiles)
* [Crear condición](#create-condition)

[Captura de pantalla de la interfaz de configuración de grupos de reventado](assets/trap-group.png){zoomable="yes"}

### Seleccionar perfiles de prueba {#select-test-profiles}

Cuando elija **Seleccionar perfiles de prueba**, use el botón **Agregar perfiles de prueba** como se muestra a continuación:

[Agregar captura de pantalla del botón de perfil de prueba](assets/trap-no-test-profile.png){zoomable="yes"}

Al hacer clic en el botón, puede acceder a los perfiles de prueba para agregarlos a su **[!UICONTROL grupo de captura]**. Seleccione los que desee utilizar.

También puede crear nuevos perfiles de prueba. [Más información](#create-seed)

[Seleccionar la captura de pantalla de la interfaz de perfiles de prueba](assets/trap-select-test-profiles.png){zoomable="yes"}

Después de confirmar los perfiles de prueba, compruebe que aparece el número correcto en **[!UICONTROL Grupo de reventado]**.

[Captura de pantalla de confirmación de grupo de captura](assets/trap-check.png){zoomable="yes"}

### Crear condición {#create-condition}

Con la opción **[!UICONTROL Crear condición]**, cree una consulta para definir los perfiles de prueba que desee utilizar:

[Crear captura de pantalla de interfaz de condición](assets/trap-create-condition.png){zoomable="yes"}

Su consulta se muestra en **[!UICONTROL Grupo de reventado]**.

[Captura de pantalla de visualización de consulta de grupo de reventado](assets/trap-custom.png){zoomable="yes"}

## Creación de un nuevo perfil de prueba {#create-seed}

Puede crear un nuevo **[!UICONTROL perfil de prueba]** desde la carpeta **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]**.

[Crear captura de pantalla de navegación de perfil de prueba](assets/trap-create.png){zoomable="yes"}

Configure todas las opciones de su **[!UICONTROL perfil de prueba]** tal como lo haría para cualquier perfil:

[Captura de pantalla de configuración de perfil de prueba](assets/trap-create-contact.png){zoomable="yes"}