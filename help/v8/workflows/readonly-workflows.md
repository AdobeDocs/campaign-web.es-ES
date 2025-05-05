---
audience: end-user
title: Acerca de los flujos de trabajo solo de lectura
description: Descubra por qué flujos de trabajo están en modo de solo lectura
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 11%

---

# Acerca de los flujos de trabajo solo de lectura {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Este flujo de trabajo es de solo lectura"
>abstract="No puede editar este flujo de trabajo debido a sus derechos o al tipo de flujo de trabajo."

Algunos flujos de trabajo son de solo lectura. Los flujos de trabajo técnicos integrados son siempre de solo lectura, pero esta restricción también se puede aplicar a otros tipos de flujos de trabajo.

Campaign usuarios pueden tener acceso restringido a Adobe Campaign datos. Un administrador de Campaign puede concederles el derecho para vista ciertas funciones, pero no para editarlas ni modificarlas. Los permisos de usuario sobre los datos son esenciales para garantizar la seguridad de los datos y los procesos. Obtenga más información sobre la administración de permisos en Campaign en [esta sección](../get-started/permissions.md).

Cuando una flujo de trabajo está en modo de solo lectura:

* La mención **[!UICONTROL Sólo lectura]** aparece cerca del **[!UICONTROL botón Configuración]** .
* No se puede acceder a los botones de acción.

![Interfaz de flujo de trabajo de solo lectura que muestra la configuración botón y los botones de acción desactivados.](assets/readonly-workflow.png){zoomable="yes"}

Los usuarios no pueden editar nada en un flujo de trabajo de solo lectura. No se les permite cambiar la configuración de las actividades.

![Interfaz del programador en modo de solo lectura, que muestra las opciones de configuración deshabilitadas.](assets/scheduler-readonly.png){zoomable="yes"}

Los usuarios no pueden eliminar el flujo de trabajo.

![Interfaz que muestra derechos restringidos para eliminar flujos de trabajo.](assets/readonly-rights.png){zoomable="yes"}

## Tipos de flujos de trabajo de solo lectura {#readonly-workflow-types}

Según el tipo de flujo de trabajo, el modo de solo lectura puede variar.

### Flujos de trabajo de la campaña {#readonly-campaign-wf}

En un flujo de trabajo de campaña de solo lectura, el usuario no puede acceder al botón de supervisión.

![Campaign flujo de trabajo interfaz en modo de solo lectura, mostrando las opciones de supervisión deshabilitadas.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Flujos de trabajo técnicos {#readonly-tech-wf}

Los flujos de trabajo técnicos integrados son de solo lectura para todos los usuarios Campaign, incluidos los administradores. Sin embargo, los usuarios pueden **ponerlas en pausa** o **detenerlas** si es necesario. Estas son las únicas acciones permitidas.

![Interfaz de flujo de trabajo técnica en modo de solo lectura, con opciones para pausar o detener flujos de trabajo.](assets/readonly-technical-workflow.png){zoomable="yes"}

Obtenga más información sobre flujos de trabajo técnicos en [esta sección](https://experienceleague.adobe.com/es/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).