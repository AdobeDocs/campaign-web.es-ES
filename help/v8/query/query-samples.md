---
audience: end-user
title: Ejemplos de consultas
description: Aprenda a trabajar con el modelador de consultas.
hide: true
hidefromtoc: true
exl-id: 6f8154ea-5d64-4950-9da3-427070ec7bf0
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 42%

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
