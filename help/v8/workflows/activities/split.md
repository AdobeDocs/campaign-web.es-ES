---
audience: end-user
title: Uso de la actividad de flujo de trabajo Split
description: Descubra más información sobre cómo utilizar la actividad del flujo de trabajo División
badge: label="Alfa"
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 2%

---


# División {#split}

El **Split** la actividad es una **Segmentación** actividad que permite segmentar las poblaciones entrantes en varios subconjuntos en función de diferentes criterios de selección, como reglas de filtrado o tamaño de población.

## Configuración {#general}

Siga estos pasos para configurar el **Split** actividad:

1. Añadir un **Split** a su flujo de trabajo.

1. El panel de configuración de actividad se abre con un subconjunto predeterminado. Haga clic en **Añadir segmento** para añadir tantos subconjuntos como desee para segmentar la población entrante.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Cuando se ejecuta la actividad Split, la población se segmenta en los diferentes subconjuntos en el orden en que se añaden a la actividad. Por ejemplo, si el primer subconjunto recupera el 70 % de la población inicial, el siguiente subconjunto añadido aplicará sus criterios de selección solo al 30 % restante, y así sucesivamente.
   >
   > Antes de configurar los subconjuntos, asegúrese de haberlos añadido en el orden correcto, ya que su posición no se puede cambiar.

1. Una vez añadidos los subconjuntos, la actividad muestra tantas transiciones de salida como subconjuntos. Se recomienda encarecidamente cambiar la etiqueta de cada subconjunto para identificarlo fácilmente en el lienzo del flujo de trabajo.

1. Configure cómo debe filtrar cada subconjunto la población entrante. Para ello, siga estos pasos:

   1. Abra el subconjunto para mostrar sus propiedades.

   1. Para aplicar una condición de filtrado al subconjunto, haga clic en **[!UICONTROL Crear filtro]** y configure la regla de filtrado que desee. Por ejemplo, incluya perfiles de la población entrante cuya dirección de correo electrónico existe en la base de datos.

   1. Para limitar el número de perfiles seleccionados por el subconjunto, active la opción **[!UICONTROL Habilitar límite]** y especifique el número o los porcentajes de la población que desea incluir.

      >[!NOTE]
      >
      >Al establecer un límite de población para un subconjunto, puede clasificar los perfiles seleccionados en función de un atributo de perfil específico, en orden ascendente o descendente. Para ello, active la opción **[!UICONTROL Habilitar ordenación]** opción. Por ejemplo, puede restringir un subconjunto para incluir solo los 50 perfiles con la cantidad de compra más alta.

   ![](../assets/workflow-split-subset.png)

1. Una vez configurados todos los subconjuntos, puede seleccionar la población restante que no coincide con ninguno de los subconjuntos e incluirlos en una transición saliente adicional. Para ello, active la opción **[!UICONTROL Generar complemento]** opción.

   ![](../assets/workflow-split-complement.png)

La actividad está configurada. En la ejecución del flujo de trabajo, la población se segmenta en los diferentes subconjuntos, en el orden en que se hayan añadido a la actividad.

## Ejemplo

En el ejemplo siguiente, la variable **[!UICONTROL Split]** la actividad se utiliza para segmentar una audiencia en distintos subconjuntos basados en el canal de comunicación que queremos utilizar:

* **Subconjunto 1 &quot;push&quot;**: Este subconjunto incluye todos los perfiles que han instalado nuestra aplicación móvil.
* **Subconjunto 2 &quot;sms&quot;**: Usuarios de teléfonos móviles: Para la población restante que no pertenecía al subconjunto 1, el subconjunto 2 aplica una regla de filtrado para seleccionar perfiles con teléfonos móviles en la base de datos.
* **Transición de complemento**: Esta transición captura todos los perfiles restantes que no coinciden con el subconjunto 1 o el subconjunto 2. Específicamente, incluye perfiles que no han instalado la aplicación móvil ni tienen teléfono móvil, como usuarios que no han instalado la aplicación móvil o que carecen de un número de móvil registrado.

![](../assets/workflow-split-example.png)