---
title: Administración de husos horarios
description: Descubra cómo la interfaz de usuario web de Adobe Campaign muestra valores de fecha y hora en función del explorador, el operador, el flujo de trabajo y las zonas horarias del servidor.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 4%

---

# Administración de husos horarios {#timezone-management}

La interfaz de usuario web de Adobe Campaign muestra todos los valores de fecha y hora según la **zona horaria local del explorador web del usuario**. Este comportamiento puede provocar diferencias al comparar marcas de tiempo entre la interfaz de usuario web y la consola de cliente.

En esta sección se explican las diferencias esperadas entre las zonas horarias **Interfaz de usuario web**, **Consola de cliente** y **Ejecución de flujo de trabajo**.

>[!NOTE]
>
>No se modifica ningún dato almacenado en el servidor. Solo cambia su visualización en la interfaz.

## Conceptos clave

* **Zona horaria del servidor**: la zona horaria del servidor corresponde a la configurada en el sistema operativo del servidor. Todas las marcas de tiempo se almacenan internamente en UTC en el servidor.

* **Comportamiento de la consola del cliente**: la consola del cliente muestra marcas de tiempo utilizando la zona horaria del operador **definida en la configuración del operador.** De manera predeterminada, corresponde a la zona horaria del **servidor**.

* **Comportamiento de la interfaz de usuario web**: la interfaz de usuario web muestra marcas de tiempo usando la **zona horaria local del explorador**. Cuando un usuario cambia la zona horaria del sistema o del explorador, los valores de fecha y hora mostrados se actualizan automáticamente.

* **Comportamiento del flujo de trabajo**: los flujos de trabajo interpretan las marcas de tiempo locales en función de la **zona horaria configurada del flujo de trabajo**. Si no se especifica, se usa la zona horaria **del servidor** de forma predeterminada.

## Ejemplo

| Interfaz | Zona horaria utilizada | Visualización de ejemplo |
|------------|----------------|-----------------|
| Consola del cliente | Operador (predeterminado = servidor) | `2025-10-20 14:00:00` |
| IU web | Zona horaria local del explorador | `2025-10-20 21:00:00` (para explorador en UTC +7) |

En este ejemplo, ambas interfaces hacen referencia a la misma marca de tiempo UTC subyacente, pero cada una la procesa con una zona horaria diferente.

## Impacto

Las diferencias en los tiempos mostrados pueden aparecer en:

* Campos de datos o perfil que contienen `datetime` valores
* Registros de envío o fechas de contacto
* Ejecución del flujo de trabajo e importación de marcas de tiempo

Los datos subyacentes siguen siendo idénticos. La diferencia solo está en **renderización**.

>[!NOTE]
>
>Si los usuarios de varias regiones colaboran en la misma instancia, pueden producirse discrepancias aparentes entre las marcas de tiempo de la interfaz de usuario web y de la consola.

## Recomendaciones

Para alinear los valores de visualización entre interfaces, puede:

* Cambie la **zona horaria del explorador** para que coincida con la **zona horaria del operador o del servidor**.
* Al exportar datos (las exportaciones utilizan UTC), asegúrese de que haya una conversión coherente en las herramientas de creación de informes.
* Al diseñar flujos de trabajo, establezca explícitamente la **zona horaria del flujo de trabajo** en las propiedades de la actividad para una programación y un comportamiento de importación predecibles.
* Comunique a los usuarios empresariales que las diferencias de marca de tiempo entre la interfaz de usuario web y las vistas de la consola de cliente son **normales y esperadas**.
