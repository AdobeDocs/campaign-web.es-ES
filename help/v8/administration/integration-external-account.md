---
title: Administrar cuenta externa
description: Obtenga información sobre cómo configurar cuentas externas
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 50%

---

# Cuentas externas de Adobe Solution Integration {#integration-external-account}

Según el tipo de cuenta externa de integración de soluciones de Adobe que haya seleccionado, siga los pasos a continuación para configurar la conexión y la configuración de la cuenta para una integración perfecta con los servicios de Adobe.

## Adobe Experience Cloud

Para conectarse a la consola de Adobe Campaign mediante un Adobe ID, debe configurar la cuenta externa de Adobe Experience Cloud (MAC).

![Captura de pantalla que muestra los campos de configuración de cuenta externa de Adobe Experience Cloud MAC.](assets/external-MAC.png)

Para configurar la cuenta externa **[!UICONTROL Adobe Experience Cloud]**, rellene los campos siguientes:

* **[!UICONTROL Servidor IMS]**

  URL del servidor IMS. Asegúrese de que las instancias de ensayo y de producción indiquen el mismo punto final de producción IMS.

* **[!UICONTROL Ámbito de IMS]**

  Los ámbitos definidos aquí deben ser un subconjunto de los que proporciona IMS.

* **[!UICONTROL Identificador de cliente IMS]**

  ID de su cliente IMS.

* **[!UICONTROL Secreto de cliente IMS]**

  Credencial del secreto de su cliente IMS.

* **[!UICONTROL Callback server]**

  Acceso URL de su instancia de Adobe Campaign.

* **[!UICONTROL IMS organization ID]**

  ID de su organización. Para encontrar su ID de organización, consulte [esta página](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=es){target=_blank}.

* **[!UICONTROL Máscara de asociación]**

  Sintaxis que permitirá nombres de configuración en Enterprise Dashboard para sincronizar con los grupos en Adobe Campaign.

* **[!UICONTROL Servidor]**

  URL de su instancia de Adobe Experience Cloud.

* **[!UICONTROL Tenant]**

  Nombre su inquilino de Adobe Experience Cloud.
