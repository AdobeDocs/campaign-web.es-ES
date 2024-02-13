---
audience: end-user
title: Cree su primera consulta con el modelador de consultas
description: Aprenda a crear la primera consulta en el modelador de consultas web de Adobe Campaign.
exl-id: efd762b5-a7ae-49b4-ab74-5b43da1e574d
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '1960'
ht-degree: 15%

---

# Genere su primera consulta {#build-query}

Para empezar a crear una consulta, acceda al modelador de consultas desde la ubicación que elija, según la acción que desee realizar. El modelador de consultas se abre con un lienzo en blanco. Haga clic en **+** para configurar el primer nodo de la consulta.

Se pueden añadir dos tipos de elementos:

* **Filtrado de componentes** (Condición personalizada, Seleccionar audiencia, Filtro predefinido) le permite crear sus propias reglas, seleccionar una audiencia o un filtro predefinido para restringir la consulta. [Aprenda a trabajar con los componentes de filtrado](#filtering)

  *Destinatarios que se han suscrito al boletín &quot;Deportes&quot;*. *Destinatarios que viven en Nueva York*, *Destinatarios que viven en San Francisco*

* **Operadores de grupo** (AND, OR, EXCEPT) permiten agrupar los componentes de filtrado en el diagrama para adaptarlos a sus necesidades. [Aprenda a trabajar con operadores](#filtering)

  *Destinatarios que se suscribieron al boletín &quot;Deportes&quot;**Y**que viven en Nueva York **O**San Francisco*.

![](assets/query-add-component.png){zoomable=&quot;yes&quot;}

## Adición de componentes de filtrado {#filtering}

Los componentes de filtrado le permiten refinar la consulta utilizando:

* **[Condiciones personalizadas](#custom-condition)**: filtre la consulta creando su propia condición con atributos de la base de datos y expresiones avanzadas.
* **[Audiencias](#audiences)**: filtre la consulta utilizando una audiencia existente.
* **[Filtro predefinido](#predefined-filters)**: filtre la consulta utilizando filtros predefinidos existentes.

### Configuración de una condición personalizada {#custom-condition}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condición personalizada"
>abstract="Condición personalizada"

Para filtrar la consulta mediante una condición personalizada, siga estos pasos:

1. Haga clic en **+** en el nodo deseado y seleccione **[!UICONTROL Condición personalizada]**. El panel de propiedades de condición personalizada se abre en el lado derecho.

1. En el **Atributo** , seleccione el atributo de la base de datos que desee aprovechar para crear la condición. La lista de atributos incluye todos los atributos de la base de datos de Campaign, incluidos los atributos de las tablas vinculadas.

   ![](assets/query-custom-condition-fields.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >El botón Edit expression permite aprovechar el editor de expresiones web de Campaign para definir manualmente una expresión mediante campos de la base de datos y funciones de ayuda. [Obtenga información sobre cómo editar expresiones](expression-editor.md)

1. Seleccione el operador que desee aplicar en la lista desplegable. Hay varios operadores disponibles. Tenga en cuenta que los operadores disponibles en la lista desplegable dependen del tipo de datos del atributo.

   +++Lista de operadores disponibles

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

1. En el **Valor** , defina el valor esperado. También puede aprovechar el editor de expresiones web de Campaign para definir manualmente una expresión utilizando los campos de la base de datos y las funciones de ayuda. Para ello, haga clic en el **Editar expresión** botón. [Obtenga información sobre cómo editar expresiones](expression-editor.md)

   *Ejemplo de consulta que devuelve todos los perfiles de 21 años o más:*

   ![](assets/query-custom-condition.png){zoomable=&quot;yes&quot;}

#### Condiciones personalizadas en las tablas vinculadas (vínculos 1-1 y 1-N){#links}

Las condiciones personalizadas permiten consultar tablas vinculadas a la tabla que utiliza actualmente la regla. Esto incluye tablas con un vínculo de cardinalidad 1-1 o tablas de recopilación (vínculo 1-N).

Para un **Vínculo 1-1**, vaya a la tabla vinculada, seleccione el atributo deseado y defina el valor esperado.

También puede seleccionar directamente un vínculo de tabla en la **Valor** selector y confirmar. En ese caso, los valores disponibles para la tabla seleccionada deben seleccionarse mediante un selector dedicado, como se muestra en el ejemplo siguiente.

+++Ejemplo de consulta

En este caso, la consulta está dirigida a marcas cuya etiqueta está &quot;en ejecución&quot;.

1. Navegue dentro de **Marca** y seleccione la **Etiqueta** atributo.

   ![](assets/1-1-attribute.png){zoomable=&quot;yes&quot;}{width="85%" align="center"}

1. Defina el valor esperado para el atributo.

   ![](assets/1-1-table.png){zoomable=&quot;yes&quot;}{width="85%" align="center"}

Este es un ejemplo de consulta en el que se ha seleccionado directamente un vínculo de tabla. Los valores disponibles para esta tabla deben seleccionarse de un selector específico.

![](assets/1-1-table-direct.png){zoomable=&quot;yes&quot;}{width="85%" align="center"}

+++

Para un **Vínculo 1-N**, puede definir subcondiciones para restringir la consulta, como se muestra en el ejemplo siguiente.

+++Ejemplo de consulta

En este caso, la consulta está dirigida a destinatarios que han realizado compras relacionadas con el producto BrewMaster, por un importe total de al menos 100 $.

1. Seleccione el **Compras** y confirme.

   ![](assets/1-N-collection.png){zoomable=&quot;yes&quot;}{width="50%" align="center"}

1. Se añade una transición saliente, que le permite crear subcondiciones.

   ![](assets/1-n-subcondition.png){zoomable=&quot;yes&quot;}{width="85%" align="center"}

1. Seleccione el **Precio** compras de atributo y destino de 1000 $ o más

   ![](assets/1-n-price.png){zoomable=&quot;yes&quot;}{width="85%" align="center"}

1. Añada subcondiciones para adaptarlas a sus necesidades. Aquí hemos agregado una condición a los perfiles de destino que compraron un producto BrewMaster.

   ![](assets/custom-condition-1-N.png){zoomable=&quot;yes&quot;}{width="85%" align="center"}

+++

#### Trabajo con datos agregados {#aggregate}

Las condiciones personalizadas le permiten realizar operaciones acumuladas. Para ello, debe seleccionar directamente un atributo de una tabla de recopilación:

1. Desplácese dentro de la tabla de recopilación deseada y seleccione el atributo en el que desea realizar una operación de acumulado.

   ![](assets/aggregate-attribute.png){zoomable=&quot;yes&quot;}{width="85%" align="center"}

1. En el panel de propiedades, active la opción **Datos agregados** y seleccione la función de acumulado que desee.

   ![](assets/aggregate.png){zoomable=&quot;yes&quot;}{width="85%" align="center"}

### Selección de un público {#audiences}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Seleccionar la audiencia"
>abstract="Seleccionar la audiencia"

Para filtrar la consulta utilizando una audiencia existente, siga estos pasos:

1. Haga clic en **+** en el nodo deseado y elija **[!UICONTROL Seleccionar audiencia]**.

1. El **Seleccionar audiencia** el panel de propiedades se abre en el lado derecho. Elija la audiencia que desee utilizar para filtrar la consulta.

   *Ejemplo de consulta que devuelve todos los perfiles pertenecientes a la audiencia &quot;Asistentes al festival&quot;:*

   ![](assets/query-audience.png){zoomable=&quot;yes&quot;}

### Uso de un filtro predefinido {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtro predefinido"
>abstract="Filtro predefinido"

Para filtrar la consulta utilizando un filtro predefinido, siga estos pasos:

1. Haga clic en **+** en el nodo deseado y seleccione **[!UICONTROL Filtro predefinido]**.

1. El **Filtro predefinido** el panel de propiedades se abre en el lado derecho. Seleccione un filtro predefinido de la lista de filtros personalizados o de favoritos.

   *Ejemplo de consulta que devuelve todos los perfiles correspondientes al filtro predefinido &quot;Clientes inactivos&quot;:*

   ![](assets/query-predefined-filter.png){zoomable=&quot;yes&quot;}

### Copiar y pegar componentes {#copy}

El modelador de consultas permite copiar uno o varios componentes de filtrado y pegarlos al final de una transición. Esta operación se puede ejecutar dentro del lienzo de consulta actual o en cualquier lienzo de la instancia.

>[!NOTE]
>
>La selección copiada se conserva mientras esté trabajando en la instancia. Si cierra la sesión y vuelve a iniciarla, la selección ya no estará disponible para pegar.

Para copiar y pegar componentes de filtrado, siga estos pasos:

1. Seleccione el componente de filtrado que desea copiar haciendo clic en él en el lienzo de la consulta. Para seleccionar varios componentes, utilice la herramienta de selección múltiple disponible en la barra de herramientas situada en la esquina superior derecha del lienzo.

1. Haga clic en **[!UICONTROL Copiar]** en el panel de propiedades del componente o en la cinta azul de la parte inferior de la pantalla si ha seleccionado varios componentes.

   | Copiar un solo componente | Copiar varios componentes |
   |  ---  |  ---  |
   | ![](assets/copy-single-component.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} | ![](assets/copy-multiple-components.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |

1. Para pegar los componentes, haga clic en el botón + al final de la transición deseada y seleccione **Pegar elementos n**.

   ![](assets/copy-paste.png){zoomable=&quot;yes&quot;}

## Combinación de componentes de filtrado con operadores {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Grupo"
>abstract="Grupo"

Cada vez que se añade un nuevo componente de filtrado a la consulta, se vincula automáticamente al otro componente mediante una variable **Y** operador. Esto significa que los resultados de los dos componentes de filtrado se combinan.

En este ejemplo, se han añadido nuevos componentes de filtrado de tipo audiencia en la segunda transición. El componente está vinculado a la condición de tipo de filtro predefinido con un **Y** operador, lo que significa que los resultados de la consulta incluyen destinatarios dirigidos por el filtro predefinido &quot;Madridians&quot; Y que pertenecen a la audiencia &quot;Cazadores de descuento&quot;.

![](assets/query-operator.png){zoomable=&quot;yes&quot;}

Para cambiar el operador utilizado para vincular las condiciones de filtrado, haga clic en él y seleccione el operador deseado en la **Grupo** panel que se abre en el lado derecho.

Los operadores disponibles son:

* **Y (intersección)**: combina los resultados que coinciden con todos los componentes de filtrado en las transiciones salientes.
* **O (Unión)**: incluye resultados que coinciden con al menos uno de los componentes de filtrado en las transiciones salientes.
* **EXCEPT (Exclusión)**: excluye los resultados que coinciden con todos los componentes de filtrado de la transición saliente.

![](assets/query-operator-change.png){zoomable=&quot;yes&quot;}

Además, puede crear grupos intermedios de componentes haciendo clic en el **+** en una transición. Esto le permite agregar un operador en esta ubicación específica para agrupar varios componentes y refinar la consulta.

VIP VIP En el ejemplo siguiente, hemos creado un grupo intermedio para incluir los resultados de las audiencias &quot;recompensar con un&quot; o &quot;&quot;.

![](assets/query-intermediate-group.png){zoomable=&quot;yes&quot;}

## Compruebe y valide la consulta

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Propiedades de las reglas"
>abstract="Propiedades de las reglas"

Una vez que haya creado la consulta en el lienzo, puede comprobarla con el **Propiedades de regla** situado en el lado derecho. Las operaciones disponibles son:

* **Ver resultados:** Muestra los datos resultantes de la consulta.
* **Vista de código**: Muestra una versión basada en código de la consulta en SQL.
* **Calcular**: actualiza y muestra el número de registros dirigidos por la consulta.
* **Seleccionar o guardar filtro**: elija un filtro predefinido existente para utilizarlo en el lienzo o guarde la consulta como un filtro predefinido para su reutilización futura. [Aprenda a trabajar con filtros predefinidos](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Seleccione un filtro predefinido en el panel de propiedades de la regla para reemplazar la consulta que se ha creado en el lienzo por el filtro seleccionado.

Cuando la consulta esté lista, haga clic en **[!UICONTROL Confirmar]** en la esquina superior derecha para guardarlo.

Puede modificar la consulta en cualquier momento abriéndola. Tenga en cuenta que al abrir una consulta existente, se muestra en una vista simplificada sin la visibilidad de  **+** botones. Para añadir nuevos elementos a la consulta, seleccione un componente u operador en el lienzo para mostrar el **+** botones.

![](assets/edit-audience.png){zoomable=&quot;yes&quot;}
