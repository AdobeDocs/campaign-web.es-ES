---
audience: end-user
title: Configuración de un envío multilingüe
description: Obtenga información sobre cómo configurar un envío multilingüe
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '1514'
ht-degree: 4%

---

# Configuración de un envío multilingüe {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Envíos multilingües"
>abstract="Ahora puede enviar mensajes en varios idiomas en la interfaz de usuario web de Campaign. Para las notificaciones push, rellene todas las variantes de idioma cargando un archivo CSV."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=es" text="Consulte las notas de la versión"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Añadir idiomas"
>abstract="En esta pestaña, encontrará una lista de idiomas en los que se va a realizar el envío. Para añadir más idiomas, haga clic en el botón Añadir idioma o duplique otro idioma desde esta pestaña."

>[!CONTEXTUALHELP]
>id="acw_multilingual_file_upload"
>title="Importar variantes de idioma"
>abstract="Utilice este cuadro de diálogo para añadir una variante de idioma mediante la importación de un archivo CSV. El archivo rellena automáticamente todos los campos disponibles para el idioma seleccionado. Puede arrastrar y soltar el archivo o elegirlo en el equipo antes de confirmarlo."

En la interfaz de usuario web de Campaign, puede configurar las entregas como multilingües, lo que le permite enviar mensajes en función del idioma preferido de un perfil. Cuando no se define ninguna preferencia, el mensaje se envía en el idioma predeterminado.

En un envío multilingüe, la administración de idiomas se basa en variantes. Cada variante representa un idioma. Durante la creación de la entrega, puede añadir varias variantes de idioma para que coincidan con el número de idiomas necesarios en el mensaje. También puede cambiar el idioma predeterminado en cualquier momento después de agregar estas variantes.

Actualmente, la capacidad multilingüe está disponible para correos electrónicos, notificaciones push, mensajes transaccionales y SMS.

Para configurar envíos multilingües, siga estos pasos principales:

1. Agregar una variante de idioma [leer más](#add-variant)
1. Defina el contenido para cada variante [leer más](#define-content)
1. Administrar variantes de idioma, [leer más](#manage-variant)

## Añadir una variante de idioma{#add-variant}

Para crear variantes de idioma, siga estos pasos:

1. En el panel de entregas, haga clic en el icono de lápiz para acceder a la pantalla de edición de contenido de entrega y, a continuación, haga clic en **[!UICONTROL Añadir idioma]**.

   >[!IMPORTANT]
   >
   >El botón **[!UICONTROL Agregar idioma]** solo está disponible si la dimensión de destino contiene el esquema **Idioma**. Para obtener más información sobre esquemas y dimensiones de destino, consulte la [documentación detallada](../audience/targeting-dimensions.md).

   ![](assets/edit-content_2.png){zoomable="yes"}

1. En el menú desplegable **Agregar idioma**, seleccione el idioma que desee agregar y confirme la acción. Para las notificaciones push, también puede [cargar un archivo CSV](#csv-upload) para importar todas las variantes de idioma a la vez.

   El primer idioma que agregue se establecerá automáticamente como predeterminado y el contenido existente se convertirá en la versión predeterminada. Cuando se añaden idiomas adicionales, su contenido se copia inicialmente del idioma predeterminado.

   ![](assets/edit-content_3.png){zoomable="yes"}

   >[!NOTE]
   >
   >Los idiomas disponibles en esta lista dependen de los valores definidos por el atributo **Language** (valores como: system, user, dbenum, etc.). Obtenga más información acerca de la administración de la enumeración en esta [sección](../administration/enumerations.md).

1. Repita esta operación para agregar otros idiomas. El panel **[!UICONTROL Idiomas]**, a la izquierda, muestra la lista de idiomas que ha elegido, el número de idiomas y el idioma predeterminado.

   Por ejemplo, si ha elegido inglés, francés y sueco, puede ver estos 3 idiomas como se muestra a continuación:

   ![](assets/edit-content_9.png){zoomable="yes"}

   Para aprender a administrar las variantes de idioma, consulte esta [sección](#manage-variant).

## Definir el contenido para cada variante{#define-content}

Una vez configurados los idiomas, defina el contenido del envío para cada idioma.

1. En la pantalla de edición de contenido de entrega, seleccione un idioma en el panel **[!UICONTROL Idiomas]** que hay a la izquierda.

   ![](assets/edit-content_11.png){zoomable="yes"}

1. Defina el contenido del mensaje para este idioma. Obtenga más información en esta [sección](../msg/create-deliveries.md).

1. Repita esta operación para cada idioma.

<!--
>[!BEGINTABS]

>[!TAB Email delivery]

1. From the delivery content edition screen, choose a language and click the **[!UICONTROL Edit email body]** button. You can also hover over the email preview and select **[!UICONTROL Open email designer]**.

    ![](assets/edit-content_11.png){zoomable="yes"}

1. Define the content of your email for this language. [Read more](../email/get-started-email-designer.md#start-authoring)

1. Repeat this operation for each language.

>[!TAB SMS delivery]

1. From the delivery content edition screen, choose a language.

1. Edit the content of the SMS message for this language. [Read more](../sms/create-sms.md)

    ![](assets/edit-content_11-sms.png){zoomable="yes"}

1. Repeat this operation for each language.

>[!ENDTABS]

-->

Para obtener una vista previa del envío, haga clic en el botón **[!UICONTROL Simular contenido]** y seleccione perfiles. Asegúrese de que se muestra el contenido correcto para cada perfil.

![](assets/edit-content_5.png){zoomable="yes"}

## Administrar variantes de idioma{#manage-variant}

En el panel izquierdo, se muestra toda la información de la variante de idioma. Para eliminar todos los idiomas, haga clic en el botón Expandir y, a continuación, haga clic en **[!UICONTROL Eliminar todas las variantes]**.

![](assets/edit-content_13.png){zoomable="yes"}

En la lista de variantes de idioma, puede realizar las siguientes acciones:

* **Editar**: cambia el idioma mientras se mantiene el contenido asociado.
* **Establecer como predeterminado**: establezca el idioma como predeterminado. Cuando un perfil no tiene definido ningún idioma, el mensaje se envía en el idioma predeterminado.
* **Duplicate**: duplica el contenido definido para este idioma y elige una variante diferente.
* **Eliminar**: elimine la variante y su contenido asociado.

![](assets/edit-content_13-sms.png){zoomable="yes"}

## Importar variantes de idioma desde CSV (notificaciones push) {#csv-upload}

Para las notificaciones push, puede rellenar rápidamente todas las variantes de idioma cargando un archivo CSV que contenga su contenido multilingüe. Esta función optimiza la creación de campañas multilingües, ya que le permite preparar contenido sin conexión e importarlo por lotes.

* **Eficiencia**: agregue varios idiomas y su contenido en una sola operación
* **Coherencia**: garantice mensajes uniformes en todas las variantes de idioma
* **Collaboration**: permita que los equipos de contenido preparen traducciones en herramientas de hoja de cálculo conocidas
* **Administración masiva**: administre y actualice fácilmente un gran número de variantes de idioma

### Requisitos previos {#csv-best-practices}

Siga estas prácticas recomendadas para garantizar una importación correcta de CSV:

* **Use la estructura de columnas exacta**: las 14 columnas deben estar presentes en el archivo CSV, aunque deje algunas en blanco. Si faltan columnas, se produce un error de importación. Puede utilizar un orden diferente, pero todas las columnas deben estar presentes.
* **Igualar nombres de columna exactamente**: Los nombres de columna distinguen entre mayúsculas y minúsculas. Usar `title` no `Title`, `badge` no `Bbadge`, `locale` no `Locale`.
* **Use códigos de configuración regional en minúsculas**: dé formato a los códigos de configuración regional como `en_us`, `fr_fr`, `de_de` (en minúsculas con guion bajo), no como `en_US` ni `en-us`.
* **Rellenar columnas obligatorias**: Las columnas `locale` y `language` deben contener valores para cada fila. Si los valores están vacíos, se producirá un error de importación.
* **Mantener configuraciones regionales únicas**: Cada código de configuración regional debe aparecer solo una vez en el archivo CSV. Se rechazarán las configuraciones regionales duplicadas.
* **Guardar como UTF-8**: Guarde siempre el archivo CSV con la codificación UTF-8 para admitir correctamente los caracteres internacionales.
* **Contenido que contiene comas**: Si el título o el cuerpo del mensaje contiene comas, escriba todo el campo entre comillas dobles: `"Hello, welcome!"`.
* **Use valores numéricos correctamente**: Para las columnas de indicador (isContentAvailable, isMutableContent, quietPush), use `1` para true, `0` para false o déjelo en blanco para default.
* **Validar formato JSON**: Si utiliza la columna customFields, asegúrese de que el JSON tenga el formato correcto: `{"key":"value"}` con comillas y corchetes correctos.
* **Primero realice la prueba con datos mínimos**: empiece con un CSV sencillo en 2-3 idiomas para comprobar el formato antes de crear archivos grandes.

>[!NOTE]
>
>La estructura de columnas se detalla en esta [sección](#csv-columns).

### Importar el archivo CSV {#csv-steps}

Para importar variantes de idioma desde un archivo CSV, siga estos pasos:

1. En el editor de contenido de la entrega, haga clic en **[!UICONTROL Agregar idioma]**.

   ![Captura de pantalla que muestra el botón Agregar idioma en el editor de contenido de notificaciones push](assets/multilingual-csv.png){zoomable="yes"}

1. Seleccione el archivo CSV arrastrándolo y soltándolo en el área de carga, o haga clic en para examinar el equipo.

   El sistema valida el formato y el contenido del archivo. Si la validación falla, los mensajes de error indican qué columnas o datos son incorrectos. Solucione los problemas en el archivo CSV y vuelva a cargar. Consulte esta [sección](#csv-troubleshooting).

   ![Captura de pantalla que muestra una validación correcta de CSV con todos los idiomas importados](assets//multilingual-csv2.png){zoomable="yes"}

1. Revise el contenido importado en el panel Variantes de idioma para confirmar que todas las traducciones se han cargado correctamente.

   ![Captura de pantalla que muestra la vista previa de variantes de contenido multilingüe importado](assets/multilingual-csv3.png){zoomable="yes"}

### Estructura de columna {#csv-columns}

Esta es la estructura de columnas correcta que se debe utilizar:

>[!NOTE]
>
>Puede utilizar un orden diferente, pero todas las columnas deben estar presentes. Para obtener más prácticas recomendadas, consulte esta [sección](#csv-best-practices).

1. **title**: título de notificación (obligatorio)
1. **messageBody**: cuerpo del mensaje de notificación (obligatorio)
1. **sound**: nombre del archivo de sonido (por ejemplo: `default`, `custom_sound.mp3`) - dejar en blanco de forma predeterminada
1. **distintivo**: número de distintivo que se mostrará en el icono de la aplicación (iOS) - usar solo números
1. **deeplinkURI**: URL de vínculo profundo que se abrirá al pulsar la notificación (déjelo en blanco si no se usa)
1. **category**: Identificador de categoría de notificación para acciones personalizadas (iOS): déjelo en blanco si no se usa.
1. **iosMediaAttachmentURL**: URL del archivo adjunto de medios para las notificaciones de iOS; déjelo en blanco si no se utiliza.
1. **androidMediaAttachmentURL**: URL de archivo adjunto multimedia para notificaciones de Android. Déjelo en blanco si no se utiliza.
1. **isContentAvailable**: indicador de contenido disponible (iOS): use `1` para true, `0` para false y déjelo en blanco para default (0)
1. **isMutableContent**: indicador de contenido mutable (iOS): use `1` para true, `0` para false y déjelo en blanco para default (0)
1. **customFields**: datos personalizados en formato JSON (por ejemplo, `{"key1":"value1","key2":"value2"}`): déjelo en blanco si no se usa.
1. **configuración regional**: el código de idioma (obligatorio) (por ejemplo, `en_us`, `fr_fr`, `de_de` - **obligatorio) debe ser único por fila**
1. **idioma**: nombre del idioma (obligatorio); por ejemplo, `English-United States`, `French-France` - **obligatorio**
1. **quietPush**: indicador de inserción silenciosa: use `1` para la inserción silenciosa, `0` para la normal, déjelo en blanco para la predeterminada (0)

### Ejemplo de archivo CSV {#csv-examples}

Este es un ejemplo básico con los campos obligatorios:

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
Welcome!,Thank you for joining us,,,,,,,,,, en_us,English-United States,0
Bienvenue !,Merci de nous avoir rejoint,,,,,,,,,,fr_fr,French-France,0
Willkommen!,Vielen Dank für Ihre Anmeldung,,,,,,,,,, de_de,German-Germany,0
¡Bienvenido!,Gracias por unirte a nosotros,,,,,,,,,, es_es,Spanish-Spain,0
```

Este es un ejemplo con campos opcionales:

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
Welcome!,Thank you for joining us,default,1,,,https://example.com/welcome-en.jpg,https://example.com/welcome-en.jpg,,,, en_us,English-United States,0
Bienvenue !,Merci de nous avoir rejoint,default,1,,,https://example.com/welcome-fr.jpg,https://example.com/welcome-fr.jpg,,,, fr_fr,French-France,0
Willkommen!,Vielen Dank für Ihre Anmeldung,default,1,,,https://example.com/welcome-de.jpg,https://example.com/welcome-de.jpg,,,, de_de,German-Germany,0
¡Bienvenido!,Gracias por unirte a nosotros,default,1,,,https://example.com/welcome-es.jpg,https://example.com/welcome-es.jpg,,,, es_es,Spanish-Spain,0
```

Este es un ejemplo con campos personalizados

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
New Collection,Discover our latest products,default,1,,,,,,,"{"campaign":"summer2025","segment":"premium"}",en_us,English-United States,0
Nouvelle Collection,Découvrez nos derniers produits,default,1,,,,,,,"{"campaign":"summer2025","segment":"premium"}",fr_fr,French-France,0
```

>[!NOTE]
>
>Para las notificaciones push enriquecidas con carruseles o botones de acción, Campaign utiliza un método de configuración diferente al de la importación de CSV. Configure el contenido push enriquecido directamente en el editor de envíos después de importar contenido multilingüe básico.

### Personalization en archivos CSV {#csv-personalization}

Para utilizar campos de personalización en el contenido CSV, debe utilizar etiquetas `<span>`:

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
"Hello <span class=""nl-dce-field nl-dce-done"" data-nl-expr=""recipient.firstName"">recipient.firstName</span>","Your order has shipped!",,,,,,,,,,en_us,English-United States,0
"Bonjour <span class=""nl-dce-field nl-dce-done"" data-nl-expr=""recipient.firstName"">recipient.firstName</span>","Votre commande a été expédiée !",,,,,,,,,,fr_fr,French-France,0
```

Durante la entrega, Campaign reemplaza estos marcadores de posición con los datos de destinatario reales.

### Solución de problemas {#csv-troubleshooting}

| Error | Causa | Solución |
|-------|-------|----------|
| Faltan columnas necesarias | El archivo CSV no contiene las 14 columnas | Asegúrese de que el CSV tenga las 14 columnas en el orden exacto mostrado anteriormente. Utilice valores vacíos para las columnas que no se utilicen. |
| Valores de configuración regional/idioma no válidos | las columnas configuración regional o de idioma están vacías | Las columnas de configuración regional y de idioma deben tener valores para cada fila |
| Duplicar configuraciones regionales | El mismo código de configuración regional aparece varias veces | Cada valor de configuración regional debe ser único: elimine las filas duplicadas |
| Problemas de codificación de archivos | El archivo CSV utiliza una codificación incompatible | Guarde el archivo CSV con codificación UTF-8 |
| Discordancia de columnas | Las filas tienen un número de columnas diferente al encabezado | Asegúrese de que todas las filas tengan exactamente 14 columnas que coincidan con el encabezado |
| Valores numéricos no válidos | badge, isContentAvailable, isMutableContent o quietPush contienen valores no numéricos | Utilice solo números: 0 o 1 para los indicadores o déjelo en blanco para los predeterminados |
| JSON mal formado | La columna customFields contiene un archivo JSON no válido | Asegúrese de que la sintaxis de JSON sea correcta: `{"key":"value"}` o déjelo en blanco |
| No coinciden las mayúsculas y minúsculas de columna | Los nombres de columna no coinciden exactamente | Los nombres de columna distinguen entre mayúsculas y minúsculas. Use nombres exactos como los que se muestran arriba (p. ej., `badge`, no `Badge` ni `BADGE`) |

>Las prácticas recomendadas se enumeran en esta [sección](#csv-best-practices). La estructura de columnas se detalla en esta [sección](#csv-columns).

