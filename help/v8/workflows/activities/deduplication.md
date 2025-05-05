---
audience: end-user
title: Usar el actividad de flujo de trabajo de deduplicación
description: Aprenda a utilizar la flujo de trabajo de deduplicación actividad
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 19%

---

# Deduplicación {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campos para identificar los duplicados"
>abstract="En la **sección Campos para identificar duplicados, haga clic en el** botón atributo **de añadir para especificar los campos para los que se pueden identificar valores idénticos a duplicados**, como correo electrónico dirección, nombre y apellidos. El orden de los campos especifica aquellos que se deben procesar primero."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Actividad de deduplicación"
>abstract="La **actividad de deduplicación** elimina los duplicados en los resultados de las actividades entrantes. Se utiliza principalmente después de direccionamiento actividades y antes de actividades que utilizan datos segmentados."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Generación de un complemento"
>abstract="Puede generar una transición saliente adicional con la población restante excluida como duplicados. Para ello, active la opción **Generar complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configuración de la deduplicación"
>abstract="Para eliminar duplicados en los datos entrantes, defina el método de deduplicación en los campos siguientes. De forma predeterminada, solo se guarda un registro. Seleccione el modo deduplicación en función de una expresión o un atributo. De forma predeterminada, el registro que se va a excluir de los duplicados se selecciona de forma aleatoria."

La **actividad de deduplicación** es un **actividad de objetivo** . Este actividad elimina los duplicados en los resultados de las actividades entrantes, como perfiles duplicados en el lista de destinatario. La **actividad de deduplicación generalmente se usa después de direccionamiento actividades y antes de** actividades que usan datos segmentados.

## Configuración del actividad de deduplicación {#deduplication-configuration}

Siga estos pasos para configurar el **actividad de deduplicación** :

![Flujo de trabajo deduplicación proceso de configuración](../assets/workflow-deduplication.png)

1. añadir un actividad de **deduplicación** a su flujo de trabajo.

1. En la **sección Campos para identificar duplicados, haga clic en el** botón atributo **de añadir para especificar los campos para los que se pueden identificar valores idénticos a duplicados**, como correo electrónico dirección, nombre y apellidos. El orden de los campos especifica aquellos que se deben procesar primero. [Aprenda a seleccionar atributos y agregarlos a favoritos](../../get-started/attributes.md).

1. En la **sección Configuración** de deduplicación, seleccione el número de duplicados únicos **que desea conservar**. El valor predeterminado de este campo es 1. El valor 0 mantiene todos los duplicados.

   Por ejemplo, si los registros A y B se consideran duplicados del registro Y y el registro C se considera un duplicado del registro Z:

   * Si el valor del campo es 1: solo se guardan los registros Y y Z.
   * Si el valor del campo es 0: se guardan todos los registros.
   * Si el valor del campo es 2: los registros C y Z se mantienen, y dos registros de A, B e Y se mantienen, ya sea por casualidad o dependiendo del método deduplicación seleccionado.

1. Seleccione el método **de** deduplicación que desea utilizar:

   * **Selección** aleatoria: selecciona aleatoriamente el registro que desea evitar los duplicados.
   * **Uso de un expresión**: Mantiene los registros en los que el valor del expresión ingresado es el más pequeño o el más grande.
   * **Valores no vacíos**: mantiene los registros para los que el expresión no está vacío.
   * **A continuación de un lista de valores**: Define la prioridad de valores para uno o varios campos. Para definir los valores, haga clic en **Atributo** para seleccionar un campo o crear una expresión y, a continuación, agregue los valores a la tabla adecuada. Para definir un nuevo campo, haga clic en el botón **Add** situado sobre la lista de valores.

1. Marque la **opción Generar complemento** para explotar la población restante. El complemento está formado por todos los duplicados. A continuación, se añade un transición adicional al actividad.

## Ejemplo {#deduplication-example}

En el ejemplo siguiente, utilice un actividad de deduplicación para excluir duplicados del destino antes de enviar un envío. Los perfiles duplicados identificados se añaden a un audiencia específico que se puede reutilizar si es necesario. Elija la dirección de **correo electrónico** para identificar los duplicados. Mantenga 1 entrada y seleccione el método de **&#x200B;**&#x200B;deduplicación aleatorio.

![Ejemplo de actividad deduplicación en una flujo de trabajo](../assets/workflow-deduplication-example.png)