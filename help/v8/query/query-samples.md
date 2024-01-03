---
audience: end-user
title: Ejemplos de consultas
description: Aprenda a trabajar con el generador de reglas.
badge: label="Disponibilidad limitada"
source-git-commit: a53f33360f0dc7ca80b235bd5814fd3ccc0ff698
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 43%

---

# Ejemplos de consultas {#query-samples}

## Consultas sobre destinatarios {#querying-recipient-table}

* Recupere los nombres y correos electrónicos de los destinatarios cuyo dominio de correo electrónico es &quot;orange.co.uk&quot; y que no viven en Londres.

* destinatarios no contactados durante los últimos 7 días.

* dominios de correo electrónico que han sido objetivos más de 30 veces durante las entregas anteriores.

## Consultas sobre envíos {#number-of-clicks-for-a-specific-delivery}

* número de clics de una entrega específica.

* destinatarios que no hayan abierto un correo electrónico en los últimos 7 días.

* perfiles que han abierto un envío en las últimas 2 semanas:

* Realizar un seguimiento después de una entrega anterior.

  Se envía una “Oferta de deportes de verano”. Cuatro días después de la entrega, se realizan otras dos entregas. Uno de ellos es &quot;Oferta de deportes acuáticos&quot;, el otro es un seguimiento de la primera entrega &quot;Oferta de deportes de verano&quot;. La entrega “Oferta de deportes acuáticos” se realiza a los destinatarios que han hecho clic en el vínculo “Deportes acuáticos” en la primera entrega. Estos clics muestran que el destinatario está interesado en el tema. Esto tiene sentido para dirigirlos a ofertas similares. Sin embargo, los destinatarios que no hayan hecho clic en “Oferta de deportes de verano” reciben el mismo contenido nuevamente.
