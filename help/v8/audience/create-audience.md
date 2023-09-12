---
audience: end-user
title: Creación de audiencias
description: Obtenga información sobre cómo crear audiencias en Adobe Campaign Web
badge: label="Beta"
source-git-commit: ba449ee0b5a4b41db8efbbabeb37ce7cd7cc3720
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 4%

---


# Creación de audiencias {#create-audiences}

menú audiencias

puede crearlos y segmentarlos en envíos o campañas independientes

## Cree su primera audiencia {#create}

1. Audiencia > menú
1. Crear público
1. Propiedades : etiqueta y opciones adicionales
1. Lienzo de flujo de trabajo con una actividad de audiencia de compilación
1. Editar actividad, editar flujo de trabajo según sus necesidades
1. inicie el flujo de trabajo (¿puede añadir actividades de direccionamiento solamente?) ¿No hay actividades de canal?) = Crea la audiencia y el flujo de trabajo

## Monitorización y administración de audiencias {#monitor}

En la audiencia creada, el panel tiene dos pestañas:
* información general: propiedades + estado del flujo de trabajo y número de destinatarios de esta audiencia mediante cling calculate + puede acceder y editar el flujo de trabajo desde aquí
* datos: vea los perfiles de datos como parte de la audiencia. Puede agregar nuevas columnas si es necesario. Consulte datos enriquecidos

lista de audiencias: duplicar, eliminar

**preguntas:**

El flujo de trabajo en &quot;modo audiencia&quot; => enviando actividades de canal no está disponible

* en la instancia de fase: podemos eliminar la última actividad de qsave y añadir una actividad de canal en su lugar
* ¿cómo reconocemos un flujo de trabajo en el modo &quot;audiencia&quot;?
