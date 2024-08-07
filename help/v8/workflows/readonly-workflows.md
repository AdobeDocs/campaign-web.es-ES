---
audience: end-user
title: Acerca de los flujos de trabajo solo de lectura
description: Descubra por qué los flujos de trabajo están en modo de solo lectura
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 89633454bb3de1ac05d37d767df45d9d143c80b5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 13%

---

# Acerca de los flujos de trabajo solo de lectura {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Este flujo de trabajo es de solo lectura"
>abstract="No puede editar este flujo de trabajo debido a sus derechos o al tipo de flujo de trabajo."

Algunos flujos de trabajo pueden estar en modo de solo lectura. Se puede ver con :

- La mención **[!UICONTROL ** Solo lectura **]** cerca del botón **[!UICONTROL Configuración]**
- Los botones de acción no están accesibles

![](assets/readonly-workflow.png){zoomable="yes"}

No puede editar nada en un flujo de trabajo de solo lectura. No tiene permiso para cambiar la configuración de las actividades.


![](assets/scheduler-readonly.png){zoomable="yes"}


Tampoco tiene derechos para eliminar el flujo de trabajo.

![](assets/readonly-rights.png){zoomable="yes"}

## Por qué flujos de trabajo de solo lectura

El modo de solo lectura es para usuarios que no tienen permiso y derechos de acceso para editar esos flujos de trabajo. [Obtenga más información aquí](../get-started/permissions.md)

Un usuario de una campaña puede tener restricciones en los datos a los que puede acceder en Adobe Campaign. El administrador puede darle la posibilidad de ver algunas funciones, pero no trabajar en ellas.

## Tipos de flujos de trabajo de solo lectura

Según el tipo de flujo de trabajo, el modo de solo lectura puede ser diferente.

### Flujos de trabajo de la campaña

En el caso de un flujo de trabajo de campaña de solo lectura, el usuario no puede acceder al botón de monitorización.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Flujos de trabajo técnicos

Los flujos de trabajo técnicos están en modo de solo lectura para los usuarios de Campaign.
Los flujos de trabajo técnicos integrados están en modo de solo lectura para todos, incluso para los usuarios administradores. Pero el usuario puede **pausar** o **detener** si es necesario. Esas son las únicas acciones permitidas. [Obtenga más información aquí](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}
