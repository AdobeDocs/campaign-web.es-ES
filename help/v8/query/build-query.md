---
audience: end-user
title: Cree su primera consulta con el modelador de consultas
description: Aprenda a crear la primera consulta en el modelador de consultas web de Adobe Campaign.
source-git-commit: a974221fa5b46ea9463c98724b1f49a7edb0adb7
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 20%

---

# Cree su primera consulta {#build-query}

Para empezar a crear una consulta, acceda al modelador de consultas desde la ubicación que elija, según la acción que desee realizar. El modelador de consultas se abre con un lienzo en blanco. Haga clic en el botón + para añadir el primer nodo de la consulta.

![](assets/query-add-component.png)

Se pueden añadir dos tipos de elementos:

* Los componentes de filtrado (condición personalizada, seleccionar audiencia, filtro predefinido) le permiten crear sus propias reglas, seleccionar una audiencia o un filtro predefinido para restringir la consulta.

  Ejemplo *Destinatarios que se han suscrito al boletín &quot;Deportes&quot;*. *Destinatarios que viven en Nueva York*, *Destinatarios que viven en San Francisco*

* Los operadores de grupo (AND, OR, EXCEPT) permiten agrupar los componentes de filtrado en el diagrama para adaptarlos a sus necesidades.

  Ejemplo: *Destinatarios que se suscribieron al boletín &quot;Deportes&quot;**Y**que viven en Nueva York **O**San Francisco*.

A continuación, se encuentran disponibles los pasos detallados para añadir y combinar componentes de filtrado y operadores de grupo.

## Adición de componentes de filtrado

Los componentes de filtrado le permiten refinar la consulta utilizando:

* **Condiciones personalizadas**: filtre la consulta creando su propia condición con atributos de la base de datos y expresiones avanzadas.
* **Audiencias**: filtre la consulta utilizando una audiencia existente.
* **Filtro predefinido**: filtre la consulta utilizando filtros predefinidos existentes.

### Configuración de una condición personalizada

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condición personalizada"
>abstract="Condición personalizada"

Para filtrar la consulta mediante una condición personalizada, siga estos pasos:

1. Haga clic en el botón + del nodo deseado y seleccione **[!UICONTROL Condición personalizada]**.
1. El panel de propiedades de condición personalizada se abre en el lado derecho. En el campo Attribute, seleccione el atributo de la base de datos que desea aprovechar para crear la condición.

   Los atributos disponibles representan todos los campos de la base de datos de Campaign, incluidos los campos de las tablas vinculadas a la tabla Recipients.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >El botón Edit expression permite aprovechar el editor de expresiones web de Campaign para definir manualmente una expresión mediante campos de la base de datos y funciones de ayuda.

1. Seleccione el operador que desee aplicar en la lista desplegable.

   +++Lista de operadores disponibles

   >[!NOTE]
   >
   >Los operadores disponibles en la lista desplegable dependen del tipo de datos del atributo seleccionado.

   | Operador | Objetivo | Ejemplo |
   |  ---  |  ---  |  ---  |
   | Igual a | Devuelve un resultado idéntico a los datos introducidos en la segunda columna Valor. | Apellido (@lastName) igual a &quot;Jones&quot;, solo devuelve como resultado los destinatarios cuyo apellido sea Jones. |
   | No igual a | El resultado son todos los valores que no son idénticos al valor ingresado. | Idioma (@language) igual a &quot;inglés&quot; |
   | Mayor que | El resultado es un valor mayor que el valor introducido. | Edad (@age) mayor de 50 años</strong>, devolverá todos los valores mayores que &quot;50&quot;, es decir, &quot;51&quot;, &quot;52&quot;, etc. |
   | Menor que | El resultado es un valor menor que el valor introducido. | Fecha de creación (@created) antes de &quot;DaysAgo(100)&quot;</strong>, devuelve todos los destinatarios creados hace menos de 100 días. |
   | Mayor o igual que | El resultado son todos los valores iguales o mayores que el valor introducido. | Edad (@age) mayor o igual que &quot;30&quot;</strong>, devuelve como resultado todos los destinatarios de 30 años o más. |
   | Menor o igual que | El resultado son todos los valores iguales o inferiores al valor introducido. | Edad (@age) inferior o igual a &quot;60&quot;</strong>, devuelve como resultado todos los destinatarios de 60 años o menos. |
   | Incluido en | Devuelve los resultados incluidos entre los valores indicados. Estos valores deben separarse con una coma. | Fecha de nacimiento (@birthDate) incluida en &quot;12/10/1979,12/10/1984&quot;, devuelve como resultado los destinatarios que nacieran entre esas fechas. |
   | No en | Funciona como el operador Is included in. Aquí queremos excluir los destinatarios según los valores ingresados. | Fecha de nacimiento (@birthDate) no incluida en &quot;12/10/1979,12/10/1984&quot;. A diferencia del ejemplo anterior, no se recuperan los destinatarios nacidos entre esas fechas. |
   | Is empty | En este caso, el resultado que estamos buscando coincide con un valor vacío en la segunda columna Valor. | Móvil (@mobilePhone) está vacío devuelve todos los destinatarios que no tienen número de móvil. |
   | Is not empty | Funciona de forma inversa al operador Is empty. No es necesario introducir datos en la segunda columna Valor. | Correo electrónico (@email) no está vacío. |
   | Comienza con | Devuelve los resultados que comienzan con el valor ingresado. | N.º cuenta (@account) comienza con “32010”. |
   | No empieza con | Devuelve los resultados que no empiezan con el valor introducido. | N.º cuenta (@account) no comienza con &quot;20&quot; |
   | Contiene | Devuelve los resultados que contienen al menos el valor ingresado. | Email domain (@domain) contains &#39;mail&#39;</strong>, devolverá todos los nombres de dominio que contengan &quot;mail&quot;. Por lo tanto, también devuelve el dominio “gmail.com”. |
   | Does not contain | Devuelve los resultados que no contienen el valor introducido. | Dominio de correo electrónico (@domain) no contiene &quot;vo&quot;</strong>. En este caso, no devuelve como resultado los nombres de dominio que contengan “vo”. El nombre de dominio “voila.fr” no aparece en los resultados. |
   | Como | Like es muy similar al operador Contains. Permite insertar % wild card character in the value. | Apellido (@lastName) como &quot;Jon%s&quot;. En este caso, el carácter comodín se utiliza para encontrar el nombre “Jones”, en el caso de que el operador haya olvidado la letra que falta entre la “n” y la “s”. |
   | Not like | Like es muy similar al operador Contains. Permite insertar % wild card character in the value. | Apellido (@lastName) como &quot;Smi%h&quot;. En este caso, no devuelve los destinatarios cuyo apellido sea “Smi%h”. |

+++

1. En el campo Value, seleccione el valor esperado.

   También puede aprovechar el editor de expresiones web de Campaign para definir manualmente una expresión utilizando los campos de la base de datos y las funciones de ayuda. Para ello, haga clic en el botón Edit expression.

   *Ejemplo: Consulta que devuelve todos los perfiles de 21 años o más*

   ![](assets/query-custom-condition.png)

<!--
querying linked tables
collect additional information on the targeted population, e.g. contract numbers, subscriptions to newsletters or origin.
Select the type of data you want to add. This can be data belonging to the filtering dimension or data stored in linked tables. Select the table which contains the information you want to collect and click Next.

aggregates: Define a calculation mode for the field to be added, such as an aggregate for example.-->

### Selección de un público

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Seleccionar público"
>abstract="Seleccionar público"

Para filtrar la consulta utilizando una audiencia existente, siga estos pasos:

1. Haga clic en el botón + del nodo deseado y seleccione **[!UICONTROL Seleccionar audiencia]**.

1. El panel Seleccionar propiedades de audiencia se abre en el lado derecho. Seleccione la audiencia que desee aprovechar para filtrar la consulta.

   *Ejemplo: Consulta que devuelve todos los perfiles pertenecientes a la &quot;Audiencia de asistentes al festival&quot;*

   ![](assets/query-audience.png)

### Uso de un filtro predefinido

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtro predefinido"
>abstract="Filtro predefinido"

Para filtrar la consulta utilizando un filtro predefinido, siga estos pasos:

1. Haga clic en el botón + del nodo deseado y seleccione **[!UICONTROL Filtro predefinido]**.

1. El panel Seleccionar propiedades de audiencia se abre en el lado derecho. Seleccione un filtro predefinido de la lista de filtros personalizados o de favoritos.

   *Ejemplo: consulta que devuelve todos los perfiles correspondientes al filtro predefinido &quot;Clientes inactivos&quot;.*

   ![](assets/query-predefined-filter.png)

## Combinación de componentes de filtrado con operadores

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Grupo"
>abstract="Grupo"

Al agregar un componente de filtrado a la consulta, se crea automáticamente una nueva transición en el lienzo de la consulta y el nuevo componente de filtrado se vincula al primero mediante un operador AND. Esto significa que los resultados de ambos componentes de filtrado se combinan en los resultados de la consulta.

En este ejemplo, se añade un nuevo componente de filtrado de tipo de audiencia al lienzo. Se añade automáticamente en una nueva transición y se vincula a la condición de tipo de filtro predefinido con un operador AND. En este caso, los resultados de la consulta incluyen destinatarios dirigidos por el filtro predefinido &quot;Madridians&quot; Y pertenecientes a la audiencia &quot;Discount hunters&quot;.

![](assets/query-operator.png)

Para cambiar el operador utilizado para vincular las condiciones de filtrado, haga clic en él y seleccione el operador deseado en el menú You can change the operator by click on it and selection the wished operator from the Group pane that opens on the right side.

![](assets/query-operator-change.png)

Los operadores disponibles son:

* AND (Intersection): combina los resultados de todos los componentes de filtrado en las transiciones salientes.
* OR (Unión): incluye los resultados de al menos uno de los componentes de filtrado en las transiciones salientes.
* EXCEPT (Exclusion): excluye los resultados de todos los componentes de filtrado de la transición saliente.

## Comprobación y validación de la consulta

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Propiedades de regla"
>abstract="Propiedades de regla"

Una vez que haya creado la consulta en el lienzo, puede comprobarla mediante el panel de propiedades de regla situado a la derecha. Las operaciones disponibles son las siguientes:

* **Ver resultados:** muestra los datos resultantes de la consulta.
* **Vista de código**: muestra una versión basada en código de la consulta en SQL.
* **Calcular**: actualiza y muestra el número de registros dirigidos por la consulta.
* **Seleccionar o guardar filtro**: elija un filtro predefinido existente para utilizarlo en el lienzo o guarde la consulta como un filtro predefinido para su reutilización futura. [Aprenda a trabajar con filtros predefinidos](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Seleccione un filtro predefinido en el panel de propiedades de la regla para reemplazar la consulta que se ha creado en el lienzo por el filtro seleccionado.
