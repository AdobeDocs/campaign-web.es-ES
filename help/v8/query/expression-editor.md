---
audience: end-user
title: Cree su primera consulta con el modelador de consultas
description: Aprenda a crear la primera consulta en el modelador de consultas web de Adobe Campaign.
exl-id: f9a365ac-c8be-423f-a99d-40ad5492223c
source-git-commit: df5883f8178bc5287145c587b06dd5664400ed90
workflow-type: tm+mt
source-wordcount: '2192'
ht-degree: 68%

---


# Editar expresiones {#expression}

La edición de una expresión implica la introducción manual de condiciones para formar una regla. Este modo permite utilizar funciones avanzadas, que permiten manipular los valores utilizados para llevar a cabo consultas específicas, como la manipulación de fechas, cadenas, campos numéricos y ordenación.

>[!NOTE]
>
>La sección siguiente proporciona información sobre cómo trabajar con el editor de expresiones para generar reglas. Tenga en cuenta que la sintaxis utilizada para generar reglas difiere de la utilizada para agregar personalización.

>[!IMPORTANT]
>
>Hay disponible una nueva interfaz para el modelador de consultas. Para cambiar a esta nueva experiencia del generador de reglas, presione el botón de alternancia en la esquina superior derecha. Puede volver al modelador de consultas clásico en cualquier momento simplemente pulsando la tecla de retroceso para desactivar la nueva interfaz. Puede aplicar los mismos principios que el modelador de consultas en esta nueva interfaz.
>![Imagen que muestra el conmutador para la nueva interfaz del generador de reglas](assets/query-modeler-toggle.png){zoomable="yes"}

## Trabajo con el editor de expresiones {#edit}

El editor de expresiones está disponible en el botón del modelador de consultas **[!UICONTROL Editar expresión]**, disponible para los campos **[!UICONTROL Atributo]** y **[!UICONTROL Valor]** al configurar una condición personalizada.

| Acceso desde el campo **Atributo** | Acceso desde el campo **Value** |
| --- | --- |
| ![Editor de expresiones para el campo de atributos](assets/expression-editor-attribute.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} | ![Editor de expresiones para el campo Valor](assets/edit-expression.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |

El editor de expresiones proporciona lo siguiente:

* Un **campo de entrada (1)** donde se define la expresión.
* Una lista de **campos (2)** disponibles que se pueden usar en la expresión y que corresponden a la dimensión de segmentación de la consulta.
* **Funciones de ayuda (3)**, ordenadas por categoría.

Edite la expresión introduciendo una expresión directamente en el campo de entrada. Para añadir un campo o una función de ayuda, coloque el cursor en la expresión donde desee añadirla y haga clic en el botón +.

![Interfaz del editor de expresiones](assets/expression-editor.png){zoomable="yes"}

Cuando la expresión esté lista, haga clic en el botón **[!UICONTROL Confirmar]**. La expresión se muestra en el campo seleccionado. Para editarlo, abra el editor de expresiones y realice los cambios deseados.

El ejemplo siguiente muestra una expresión configurada para el campo **[!UICONTROL Value]**. Para editarlo, abra el editor de expresiones con el botón **[!UICONTROL Editar expresión]**.

>[!BEGINTABS]

>[!TAB Modelador de consultas clásico]

![Ejemplo de expresión de edición para el campo Valor](assets/edit-expression-value.png){zoomable="yes"}

>[!TAB Nuevo generador de reglas]

![Ejemplo de expresión de edición para el campo Valor](assets/ruleb-12.png){zoomable="yes"}

>[!ENDTABS]

## Funciones de ayuda

La herramienta de edición de consultas le permite utilizar funciones avanzadas para realizar filtros complejos según los resultados deseados y los tipos de datos manipulados. Estas son las funciones disponibles:

### Agregado

Las funciones agregadas realizan cálculos en un conjunto de valores.

<table>
<tbody>
<tr>
<td><strong>Nombre</strong></td>
<td><strong>Descripción</strong></td>
<td><strong>Sintaxis</strong></td>
</tr>
<tr>
<td><strong>Avg</strong></td>
<td>Devuelve el promedio de una columna de tipo numérico</td>
<td>Avg(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>Recuento</strong></td>
<td>Cuenta los valores no nulos de una columna</td>
<td>Count(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>CountAll</strong></td>
<td>Cuenta los valores devueltos (todos los campos)</td>
<td>CountAll()</td>
</tr>
<tr>
<td><strong>Countdistinct</strong></td>
<td>Cuenta los distintos valores no nulos de una columna</td>
<td>Countdistinct(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>Max</strong></td>
<td>Devuelve el valor máximo de una columna numérica, cadena o tipo de fecha</td>
<td>Max(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>Min</strong></td>
<td>Devuelve el valor mínimo de una columna de número, cadena o tipo de fecha</td>
<td>Min(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>StdDev</strong></td>
<td>Devuelve la desviación estándar de una columna de número, cadena o fecha</td>
<td>StdDev(&lt;value&gt;)</td>
</tr>
<tr>
<td><strong>StringAgg</strong></td>
<td>Devuelve la concatenación de los valores de una columna de tipo de cadena, separados por el carácter del segundo argumento</td>
<td>StringAgg(&lt;Valor&gt;, &lt;Cadena&gt;)</td>
</tr>
<tr>
<td><strong>Sum</strong></td>
<td>Devuelve la suma de los valores de una columna de número, cadena o fecha.</td>
<td>Sum(&lt;value&gt;)</td>
</tr>
</tbody>
</table>

### Fecha

Las funciones de fecha manipulan los valores de fecha y hora.

<table>
<tbody>
<tr>
<td><strong>Nombre</strong></td>
<td><strong>Descripción</strong></td>
<td><strong>Sintaxis</strong></td>
</tr>
<tr>
<td><strong>AddDays</strong></td>
<td>Agrega un número de días a una fecha</td>
<td>AddDays(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddHours</strong></td>
<td>Agrega un número de horas a una fecha</td>
<td>AddHours(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddMinutes</strong></td>
<td>Añade un número de minutos a una fecha</td>
<td>AddMinutes(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddMonths</strong></td>
<td>Añade un número de meses a una fecha</td>
<td>AddMonths(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddSeconds</strong></td>
<td>Añade un número de segundos a una fecha</td>
<td>AddSeconds(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>AddYears</strong></td>
<td>Agrega un número de años a una fecha</td>
<td>AddYears(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>ConvertNTZ</strong></td>
<td>Convierte la marca de tiempo NTZ (marca de tiempo sin zona horaria) en TZ (marca de tiempo con zona horaria) aplicando la TZ de sesión definida</td>
<td>ConvertNTZ(&lt;fecha+hora&gt;)</td>
</tr>
<tr>
<td><strong>DateCmp</strong></td>
<td>Compara dos fechas</td>
<td>DateCmp(&lt;fecha&gt;, &lt;fecha&gt;)</td>
</tr>
<tr>
<td><strong>DateOnly</strong></td>
<td>Devuelve solo la fecha (con hora 00:00)</td>
<td>DateOnly(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>Día</strong></td>
<td>Devuelve el número que representa el día de la fecha.</td>
<td>Day(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>DayOfYear</strong></td>
<td>Devuelve el número de día del año de la fecha</td>
<td>DayOfYear(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>DaysAgo</strong></td>
<td>Devuelve la fecha correspondiente a la fecha actual menos “n” días</td>
<td>DaysAgo(&lt;number&gt;)</td>
</tr>
<tr>
<td><strong>DaysAgoInt</strong></td>
<td>Devuelve la fecha (entero aaaammdd) correspondiente a la fecha actual menos “n” días</td>
<td>DaysAgoInt(&lt;number&gt;)</td>
</tr>
<tr>
<td><strong>DaysDiff</strong></td>
<td>Devuelve el número de días entre dos fechas</td>
<td>DaysDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>DaysOld</strong></td>
<td>Devuelve la edad en días de una fecha</td>
<td>DaysOld(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>GetDate</strong></td>
<td>Devuelve la fecha del sistema actual del servidor</td>
<td>GetDate()</td>
</tr>
<tr>
<td><strong>Hora</strong></td>
<td>Devuelve la hora de la fecha</td>
<td>Hour(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>HoursDiff</strong></td>
<td>Devuelve el número de horas entre dos fechas</td>
<td>HoursDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>Minuto</strong></td>
<td>Devuelve los minutos de la fecha</td>
<td>Minute(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>MinutesDiff</strong></td>
<td>Devuelve el número de minutos entre dos fechas</td>
<td>MinutesDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>Mes</strong></td>
<td>Devuelve el número que representa el mes de la fecha</td>
<td>Month(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>MonthsAgo</strong></td>
<td>Devuelve la fecha correspondiente a la fecha actual menos n meses</td>
<td>MonthsAgo(&lt;number&gt;)</td>
</tr>
<tr>
<td><strong>MonthsDiff</strong></td>
<td>Devuelve el número de meses entre dos fechas</td>
<td>MonthsDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>MonthsOld</strong></td>
<td>Devuelve la edad en meses de una fecha</td>
<td>MonthsOld(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>Oldest</strong></td>
<td>Devuelve la fecha más antigua de un intervalo</td>
<td>Oldest(&lt;fecha, fecha&gt;)</td>
</tr>
<tr>
<td><strong>Second</strong></td>
<td>Devuelve los segundos de la fecha</td>
<td>Second(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>SecondsDiff</strong></td>
<td>Devuelve el número de segundos entre dos fechas</td>
<td>SecondsDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>SubDays</strong></td>
<td>Resta un número de días a partir de una fecha</td>
<td>SubDays(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubHours</strong></td>
<td>Resta un número de horas a partir de una fecha</td>
<td>SubHours(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubMinutos</strong></td>
<td>Resta un número de minutos desde una fecha</td>
<td>SubMinutes(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubMeses</strong></td>
<td>Resta un número de meses desde una fecha</td>
<td>SubMonths(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubSegundos</strong></td>
<td>Resta un número de segundos desde una fecha</td>
<td>SubSeconds(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>SubAños</strong></td>
<td>Resta un número de años a partir de una fecha</td>
<td>SubYears(&lt;date&gt;, &lt;number&gt;)</td>
</tr>
<tr>
<td><strong>ToDate</strong></td>
<td>Convierte una fecha y hora como fecha</td>
<td>ToDate(&lt;date + time&gt;)</td>
</tr>
<tr>
<td><strong>ToDateTime</strong></td>
<td>Convierte una cadena en una fecha + hora.</td>
<td>ToDateTime(&lt;string&gt;)</td>
</tr>
<tr>
<td><strong>ToTimestamp</strong></td>
<td>Convierte una cadena en una marca de tiempo</td>
<td>ToTimestamp(&lt;cadena&gt;)</td>
</tr>
<tr>
<td><strong>ToTimeZone</strong></td>
<td>Convierte una fecha y hora en una zona horaria</td>
<td>ToTimeZone(&lt;fecha&gt;, &lt;zona horaria&gt;)</td>
</tr>
<tr>
<td><strong>TruncDate</strong></td>
<td>Redondea una fecha y hora al segundo más cercano</td>
<td>TruncDate(@lastModified, &lt;number of seconds&gt;)</td>
</tr>
<tr>
<td><strong>TruncDateTZ</strong></td>
<td>Redondea una fecha y hora con una precisión determinada expresada en segundos</td>
<td>TruncDateTZ(&lt;date&gt;, &lt;number of seconds&gt;, &lt;time zone&gt;)</td>
</tr>
<tr>
<td><strong>TruncQuarter</strong></td>
<td>Redondea una fecha al trimestre</td>
<td>TruncQuarter(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>TruncTime</strong></td>
<td>Redondea la parte de tiempo hasta el segundo más cercano</td>
<td>TruncTime(&lt;date&gt;, &lt;number of seconds&gt;)</td>
</tr>
<tr>
<td><strong>TruncWeek</strong></td>
<td>Redondea una fecha a la semana</td>
<td>TruncWeek(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>TruncYear</strong></td>
<td>Redondea una fecha y hora al 1 de enero del año</td>
<td>TruncYear(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>WeekDay</strong></td>
<td>Devuelve un número que representa el día de la semana de la fecha (0=lunes, 6=domingo)</td>
<td>WeekDay(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>Año</strong></td>
<td>Devuelve el número que representa el año de la fecha</td>
<td>Year(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>AñoYMes</strong></td>
<td>Devuelve el número que representa el año y el mes de la fecha</td>
<td>YearAndMonth(&lt;date&gt;)</td>
</tr>
<tr>
<td><strong>YearsAgo</strong></td>
<td>Devuelve el número de años entre una fecha determinada y la fecha actual</td>
<td>YearsAgo(&lt;fecha&gt;)</td>
</tr>
<tr>
<td><strong>YearsDiff</strong></td>
<td>Devuelve el número de años entre dos fechas</td>
<td>YearsDiff(&lt;end date&gt;, &lt;start date&gt;)</td>
</tr>
<tr>
<td><strong>YearsOld</strong></td>
<td>Devuelve la edad en años de una fecha</td>
<td>YearsOld(&lt;date&gt;)</td>
</tr>
</tbody>
</table>

>[!NOTE]
>
>Tenga en cuenta que la función **DateOnly** tiene en cuenta la zona horaria del servidor, no la del operador.


### Geomarketing

Las funciones de geomarketing se utilizan para manipular los valores geográficos.

<table> 
 <tbody> 
  <tr> 
   <td> <strong>Nombre</strong><br /> </td> 
   <td> <strong>Descripción</strong><br /> </td> 
   <td> <strong>Syntax</strong><br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>Distance</strong><br /> </td> 
   <td> Devuelve la distancia entre dos puntos definidos por su longitud y latitud, expresada en grados<br /> </td> 
   <td> Distance(&lt;Longitude A&gt;, &lt;Latitude A&gt;, &lt;Longitude B&gt;, &lt;Latitude B&gt;)<br /> </td>  
  </tr> 
 </tbody> 
</table>

### Numérico

Las funciones numéricas se utilizan para convertir texto en números.

<table> 
 <tbody> 
  <tr> 
   <td> <strong>Nombre</strong><br /> </td> 
   <td> <strong>Descripción</strong><br /> </td> 
   <td> <strong>Syntax</strong><br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>Abs</strong><br /> </td> 
   <td> Devuelve el valor absoluto de un número<br /> </td> 
   <td> Abs(&lt;número&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Ceil</strong><br /> </td> 
   <td> Devuelve el menor entero que sea mayor o igual que un número<br /> </td> 
   <td> Ceil(&lt;número&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Floor</strong><br /> </td> 
   <td> Devuelve el mayor entero que sea mayor o igual que un número<br /> </td> 
   <td> Floor(&lt;number&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Greatest</strong><br /> </td> 
   <td> Devuelve el número mayor de dos números<br /> </td> 
   <td> Greatest(&lt;número 1&gt;, &lt;número 2&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Least</strong><br /> </td> 
   <td> Devuelve el número menor de dos números<br /> </td> 
   <td> Least(&lt;número 1&gt;, &lt;número 2&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Mod</strong><br /> </td> 
   <td> Devuelve el resto de la división del entero “n1” entre “n2”<br /> </td> 
   <td> Mod(&lt;number 1&gt;, &lt;number 2&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Percent</strong><br /> </td> 
   <td> Devuelve la proporción de dos números expresado como un porcentaje<br /> </td> 
   <td> Percent(&lt;número 1&gt;, &lt;número 2&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Aleatorio</strong><br /> </td> 
   <td> Devuelve un valor aleatorio<br /> </td> 
   <td> Aleatorio()<br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>Round</strong><br /> </td> 
   <td> Redondea un número a “n” decimales<br /> </td> 
   <td> Redondeo(&lt;número&gt;, &lt;número de decimales&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Sign</strong><br /> </td> 
   <td> Devuelve el signo del número<br /> </td> 
   <td> Sign(&lt;número&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>ToDouble</strong><br /> </td> 
   <td> Convierte un entero en flotante<br /> </td> 
   <td> ToDouble(&lt;número&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>ToInt64</strong><br /> </td> 
   <td> Convierte un flotante en un entero de 64 bits<br /> </td> 
   <td> ToInt64(&lt;número&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>ToInteger</strong><br /> </td> 
   <td> Convierte un flotante en un entero<br /> </td> 
   <td> ToInteger(&lt;número&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Trunc</strong><br /> </td> 
   <td> Trunca decimales de “n1” a “n2”<br /> </td> 
   <td> Trunc(&lt;n1&gt;, &lt;n2&gt;)<br /> </td>  
  </tr> 
 </tbody> 
</table>

### Otros

Esta tabla contiene las funciones restantes disponibles.

<table> 
 <tbody> 
  <tr> 
   <td> <strong>Nombre</strong><br /> </td> 
   <td> <strong>Descripción</strong><br /> </td> 
   <td> <strong>Syntax</strong><br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>AESEncrypt</strong><br /> </td> 
   <td> Cifrar la cadena proporcionada en el argumento <br /> </td> 
   <td> AESEncrypt(&lt;valor&gt;)<br /> </td> 
  </tr>
  <tr> 
   <td> <strong>Case</strong><br /> </td> 
   <td> Devuelve el valor 1 si la condición es verdadera. Si no es así, devuelve el valor 2.<br /> </td> 
   <td> Case(When(&lt;condition&gt;, &lt;value 1&gt;), Else(&lt;value 2&gt;))<br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>ClearBit</strong><br /> </td> 
   <td> Elimina el indicador del valor<br /> </td> 
   <td> ClearBit(&lt;identificador&gt;, &lt;indicador&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Coalesce</strong><br /> </td> 
   <td> Devuelve el valor 2 si el valor 1 es cero o nulo, de lo contrario devuelve el valor 1<br /> </td> 
   <td> Coalesce(&lt;valor 1&gt;, &lt;valor 2&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Decode</strong><br /> </td> 
   <td> Devuelve el valor 3 si el valor 1 = valor 2. Si no devuelve el valor 4.<br /> </td> 
   <td> Decode(&lt;value 1&gt;, &lt;value 2&gt;, &lt;value 3&gt;, &lt;value 4&gt;)<br /> </td>  
  </tr> 
  <!--<tr> 
   <td> <strong>DefaultFolder</strong><br /> </td> 
   <td> Returns value 3 if value 1 = value 2. If not returns value 4.<br /> </td> 
   <td> Decode(&lt;value 1&gt;, &lt;value 2&gt;, &lt;value 3&gt;, &lt;value 4&gt;)<br /> </td>  
  </tr> -->
  <tr> 
   <td> <strong>Else</strong><br /> </td> 
   <td> Devuelve el valor 1 (solo puede utilizarse como parámetro de la función case)<br /> </td> 
   <td> Else(&lt;value 1&gt;, &lt;value 2&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>GetEmailDomain</strong><br /> </td> 
   <td> Extrae el dominio de una dirección de correo electrónico<br /> </td> 
   <td> GetEmailDomain(&lt;valor&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>GetMirrorURL</strong><br /> </td> 
   <td> Recupera la URL del servidor de la página espejo<br /> </td> 
   <td> GetMirrorURL(&lt;valor&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Iif</strong><br /> </td> 
   <td> Devuelve el valor 1 si la expresión es verdadera. Si no es así, devuelve el valor 2<br /> </td> 
   <td> Iif(&lt;condition&gt;, &lt;value 1&gt;, &lt;value 2&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>IsBitSet</strong><br /> </td> 
   <td> Indica si el indicador se encuentra en el valor<br /> </td> 
   <td> IsBitSet(&lt;identificador&gt;, &lt;indicador&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>IsEmptyString</strong><br /> </td> 
   <td> Devuelve el valor 2 si la cadena 1 está vacía; en caso contrario, devuelve el valor 3<br /> </td> 
   <td> IsEmptyString(&lt;value 1&gt;, &lt;value 2&gt;, &lt;value 3&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>NuevoUUID</strong><br /> </td> 
   <td> Devuelve un identificador único <br /> </td> 
   <td> NewUUID()<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>NoNull</strong><br /> </td> 
   <td> Devuelve la cadena vacía si el argumento es NULL<br /> </td> 
   <td> NoNull(&lt;valor&gt;)<br /> </td>   
  </tr> 
  <tr> 
   <td> <strong>RowId</strong><br /> </td> 
   <td> Devuelve el número de línea<br /> </td> 
   <td> RowId<br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>SetBit</strong><br /> </td> 
   <td> Fuerza la marca en el valor<br /> </td> 
   <td> SetBit(&lt;identificador&gt;, &lt;indicador&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>ToBoolean</strong><br /> </td> 
   <td> Convierte un número en Boolean<br /> </td> 
   <td> ToBoolean(&lt;número&gt;)<br /> </td>   
  </tr> 
  <tr> 
   <td> <strong>When</strong><br /> </td> 
   <td> Devuelve el valor 1 si la expresión es verdadera. Si no es así, devuelve el valor 2 (solo puede utilizarse como parámetro de la función case)<br /> </td> 
   <td> When(&lt;condition&gt;, &lt;value 1&gt;)<br /> </td>  
  </tr> 
 </tbody> 
</table>

### Cadena

Las funciones de cadena se utilizan para manipular un conjunto de cadenas.

<table> 
 <tbody> 
  <tr> 
   <td> <strong>Nombre</strong><br /> </td> 
   <td> <strong>Descripción</strong><br /> </td> 
   <td> <strong>Syntax</strong><br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>AllNonNull2</strong><br /> </td> 
   <td> Indica si todos los parámetros no son nulos y no están vacíos.<br /> </td> 
   <td> AllNonNull2(&lt;string&gt;, &lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>AllNonNull3</strong><br /> </td> 
   <td> Indica si todos los parámetros no son nulos y no están vacíos.<br /> </td> 
   <td> AllNonNull3(&lt;string&gt;, &lt;string&gt;, &lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Ascii</strong><br /> </td> 
   <td> Devuelve el valor ASCII del primer carácter de la cadena.<br /> </td> 
   <td> Ascii(&lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Char</strong><br /> </td> 
   <td> Devuelve el carácter correspondiente al código ASCII “n”.<br /> </td> 
   <td> Char(&lt;number&gt;)<br /></td>  
  </tr> 
  <tr> 
   <td> <strong>Charindex</strong><br /> </td> 
   <td> Devuelve la posición de la cadena 2 en la cadena 1.<br /> </td> 
   <td> Charindex(&lt;string&gt;, &lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>dataLength</strong><br /> </td> 
   <td> Devuelve el tamaño en bytes de la cadena <br /> </td> 
   <td> dataLength(&lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>GetLine</strong><br /> </td> 
   <td> Muestra la línea nth (de 1 a n) de la cadena.<br /> </td> 
   <td> GetLine(&lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>IfEquals</strong><br /> </td> 
   <td> Devuelve el tercer parámetro si los dos primeros parámetros son iguales. Si no es así, devuelve el último parámetro<br /> </td> 
   <td> IfEquals(&lt;string&gt;, &lt;string&gt;, &lt;string&gt;, &lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>IsMemoNull</strong><br /> </td> 
   <td> Indica si la nota transferida como parámetro es nula<br /> </td> 
   <td> IsMemoNull(&lt;memo&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>JuxtWords</strong><br /> </td> 
   <td> Concatena las cadenas transferidas como parámetros. Añade espacios entre las cadenas si es necesario.<br /> </td> 
   <td> JuxtWords(&lt;string&gt;, &lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>JuxtWords3</strong><br /> </td> 
   <td> Concatena las cadenas transferidas como parámetros. Añade espacios entre las cadenas si es necesario<br /> </td> 
   <td> JuxtWords3(&lt;string&gt;, &lt;string&gt;, &lt;string&gt;)<br /></td>  
  </tr> 
  <tr> 
   <td> <strong>Left</strong><br /> </td> 
   <td> Devuelve los primeros “n” caracteres de la cadena<br /> </td> 
   <td> Left(&lt;string&gt;, &lt;number&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Length</strong><br /> </td> 
   <td> Devuelve la longitud de la cadena<br /> </td> 
   <td> Length(&lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Línea</strong><br /> </td> 
   <td> Extraer línea n de la cadena <br /> </td> 
   <td> Line(&lt;string&gt;,&lt;number&gt;)<br /></td> 
  </tr>
  <tr> 
   <td> <strong>Lower</strong><br /> </td> 
   <td> Devuelve la cadena en minúscula<br /> </td> 
   <td> Lower(&lt;cadena&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>LPad</strong><br /> </td> 
   <td> Devuelve la cadena completa a la izquierda<br /> </td> 
   <td> LPad (&lt;Cadena&gt;, &lt;Número&gt;, &lt;Carácter&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Ltrim</strong><br /> </td> 
   <td> Elimina los espacios a la izquierda de la cadena<br /> </td> 
   <td> Ltrim(&lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Md5Digest</strong><br /> </td> 
   <td> Devuelve una representación hexadecimal de la clave MD5 de una cadena<br /> </td> 
   <td> Md5Digest(&lt;string&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>MemoContains</strong><br /> </td> 
   <td> Especifica si la nota contiene la cadena transferida como parámetro<br /> </td> 
   <td> MemoContains(&lt;memo&gt;, &lt;cadena&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>ValorNodo</strong><br /> </td> 
   <td> Extrae el valor de un campo XML de su XPath y de los datos de campo <br /> </td> 
   <td> NodeValue (&lt;String&gt;, &lt;String&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Replace</strong><br /> </td> 
   <td> Reemplaza todas las apariciones de un valor de cadena especificado por otro valor de cadena.<br /> </td> 
   <td> Replace(&lt;cadena&gt;,&lt;cadena&gt;,&lt;cadena&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Right</strong><br /> </td> 
   <td> Devuelve los últimos “n” caracteres de la cadena<br /> </td> 
   <td> Right(&lt;cadena&gt;)<br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>RPad</strong><br /> </td> 
   <td> Devuelve la cadena completa a la derecha<br /> </td> 
   <td> RPad(&lt;cadena&gt;, &lt;número&gt;, &lt;carácter&gt;)<br /></td> 
  </tr> 
  <tr> 
   <td> <strong>Rtrim</strong><br /> </td> 
   <td> Elimina los espacios a la derecha de la cadena<br /> </td> 
   <td> Rtrim(&lt;cadena&gt;)<br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>Sha256Digest</strong><br /> </td> 
   <td> Representación hexadecimal de la clave SHA256 de una cadena.<br /> </td> 
   <td> Sha256Digest (&lt;cadena&gt;)<br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>Sha512Digest</strong><br /> </td> 
   <td> Representación hexadecimal de la clave SHA512 de una cadena.<br /> </td> 
   <td> Sha512Digest (&lt;cadena&gt;)<br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>Smart</strong><br /> </td> 
   <td> Devuelve la cadena con la primera letra de cada palabra en mayúscula<br /> </td> 
   <td> Smart(&lt;cadena&gt;)<br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>Substring</strong><br /> </td> 
   <td> Extrae la subcadena que comienza en el carácter “n1” de la cadena y de longitud “n2”<br /> </td> 
   <td> Substring(&lt;string&gt;, &lt;offset&gt;, &lt;length&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>ToString</strong><br /> </td> 
   <td> Convierte el número en una cadena<br /> </td> 
   <td> ToString(&lt;number&gt;, &lt;number&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Upper</strong><br /> </td> 
   <td> Devuelve la cadena en mayúsculas<br /> </td> 
   <td> Upper(&lt;cadena&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>VirtualLink</strong><br /> </td> 
   <td> Devuelve la clave externa de un vínculo transferido como parámetro si los otros dos parámetros son iguales<br /> </td> 
   <td> VirtualLink(&lt;número&gt;, &lt;número&gt;, &lt;número&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>VirtualLinkStr</strong><br /> </td> 
   <td> Devuelve la clave externa (texto) de un enlace transferido como parámetro si los otros dos parámetros son iguales<br /> </td> 
   <td> VirtualLinkStr(&lt;cadena&gt;, &lt;número&gt;, &lt;número&gt;)<br /> </td>  
  </tr> 
 </tbody> 
</table>

### Ventana

<table> 
 <tbody> 
  <tr> 
   <td> <strong>Nombre</strong><br /> </td> 
   <td> <strong>Descripción</strong><br /> </td> 
   <td> <strong>Syntax</strong><br /> </td> 
  </tr> 
  <tr> 
   <td> <strong>_Over__</strong><br /> </td> 
   <td> Ejecute la llamada a la función SQL introducida como primer parámetro, sobre Partición u Ordenar por los campos introducidos como segundo parámetro<br /> </td> 
   <td> _Over_ (&lt;Valor&gt;, &lt;Valor&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>Desc</strong><br /> </td> 
   <td> Aplica un orden descendente<br /> </td> 
   <td> Desc(&lt;valor 1&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>OrderBy</strong><br /> </td> 
   <td> Ordena el resultado dentro de la partición<br /> </td> 
   <td> OrderBy(&lt;valor 1&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>PartitionBy</strong><br /> </td> 
   <td> Particiona el resultado de una consulta en una tabla<br /> </td> 
   <td> PartitionBy(&lt;valor 1&gt;)<br /> </td>  
  </tr> 
  <tr> 
   <td> <strong>RowNum</strong><br /> </td> 
   <td> Genera un número de línea basado en la partición de tabla y en una secuencia de ordenación.<br /> </td> 
   <td> RowNum(PartitionBy(&lt;value 1&gt;), OrderBy(&lt;value 1&gt;))<br /> </td> 
  </tr> 
 </tbody> 
</table>