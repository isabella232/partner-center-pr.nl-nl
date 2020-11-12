---
title: Uitbetalings schema's en beleids Details-Azure Marketplace
description: Meer informatie over de details van het uitzonderings beleid voor commerciële Marketplace, met inbegrip van planningen en rekoppeling.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/06/2020
ms.openlocfilehash: 9c03878ec69b9df06795054464ef7f76e038e780
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/12/2020
ms.locfileid: "94531984"
---
# <a name="payout-schedules-and-policy-details"></a>Uitbetalings schema's en beleids Details

In dit artikel wordt het uitzonderings schema van micro soft beschreven, waar u de status van een uitbetaling en het proces voor niet-betaling van de klant kunt vinden.

## <a name="payment-schedules"></a>Betalings schema's

In de volgende secties wordt het proces voor uitbetalingen voor **Enterprise Agreement** en **Credit Card-en factuur** transacties beschreven.

### <a name="enterprise-agreement-transactions"></a>Enterprise Agreement trans acties

Wanneer een klant een product koopt van Microsoft AppSource of Azure Marketplace met behulp van hun bestaande micro soft-Enterprise Agreement voor trans acties, zullen we uitbetalingen doen in de volgende uitbetalings cyclus 30 dagen na de klant factuur. Trans acties waarbij een klant gebruikmaakt van een credit card, hebben een periode van 30 dagen vóór de betaling.

Een uitbetaling vindt vaak plaats voordat micro soft de betaling van de klant verzamelt. Zie het [proces voor klant niet-betaling](#process-for-customer-non-payment) hieronder voor de acties die we ondernemen als de klant micro soft niet kan betalen, maar er al een uitbetaling is verleend.

| Gebeurtenis | Beschrijving | Zicht baarheid van rapporten | Time |
| --- | --- | --- | --- |
| Gebruik of maand van trans actie | Klant gebruikt of koopt een service. | [Gebruik](/azure/marketplace/partner-center-portal/usage-dashboard) of [volg orde](/azure/marketplace/partner-center-portal/orders-dashboard) van een dash board | **Maand 1** |
| Inkoop order is gemaakt | Het totale gebruik, het totaal aantal trans acties bepalen | [Gebruik](/azure/marketplace/partner-center-portal/usage-dashboard) of [volg orde](/azure/marketplace/partner-center-portal/orders-dashboard) van een dash board | **Maand 2** |
| Het verdienen van ISV-uitbetaling is gemaakt | De kosten van het Agency en de inkomsten van de betaling bepalen | Gemarkeerd als niet-verwerkt in de transactie geschiedenis van de uitbetalings verklaring | **Maand 3 (1e week)** |
| Uitbetaling voorbereiden | De inkomsten worden voor bereid voor de maandelijkse betaling | Gemarkeerd als gepland in de transactie geschiedenis van de uitbetalings verklaring | **Maand 3 (1e week)** |
| **Uitbetalings datum** | **De betaling wordt verzonden naar Publisher** | **Gemarkeerd als verzonden in de transactie geschiedenis en in de sectie betalingen van de uitbetalings verklaring** | **Maand 3 (niet later dan de 15e)** |
| Factuur betaald door klant | Micro soft verzamelt de betaling van de klant | Geen wijziging | **Maand 4 tot en met 12** |
|

\* De uitbetalings datum is in Pacific (standaard tijd) (PST).

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>Klanten die betalen met een credit card of factuur

Voor alle aankopen met een credit card of een maandelijkse factuur geldt een periode van 30 dagen om ervoor te zorgen dat de klant geld wordt verzameld.

| Gebeurtenis | Beschrijving | Zicht baarheid van rapporten | Time |
| --- | --- | --- | --- |
| Gebruik of maand van trans actie | Klant gebruikt of koopt een service. | [Gebruik](/azure/marketplace/partner-center-portal/usage-dashboard) of [volg orde](/azure/marketplace/partner-center-portal/orders-dashboard) van een dash board | **Maand 1** |
| Factuur betaald door klant | Het totale gebruik, de totale transactie waarde en de factuur van de klant bepalen | [Gebruik](/azure/marketplace/partner-center-portal/usage-dashboard) of [volg orde](/azure/marketplace/partner-center-portal/orders-dashboard) van een dash board | **Maand 2** |
| Het verdienen van ISV-uitbetaling is gemaakt | De kosten van het Agency en de inkomsten van de betaling bepalen | Gemarkeerd als niet-verwerkt in de transactie geschiedenis van de uitbetalings verklaring | **Maand 2** |
| Periode van 30 dagen voor het bedrijf | Zorgen voor verzameling van middelen, mogelijke terugstortingen en restitutie aanvragen | Gemarkeerd als niet-verwerkt in de transactie geschiedenis van de uitbetalings verklaring | **Maand 3** |
| Uitbetaling voorbereiden | De inkomsten worden voor bereid voor de maandelijkse betaling | Gemarkeerd als gepland in de transactie geschiedenis van de uitbetalings verklaring | **Eerste week van maand 4** |
| **Uitbetalings datum** | **De betaling wordt verzonden naar Publisher** | **Gemarkeerd als verzonden in de transactie geschiedenis en in de sectie betalingen van de uitbetalings verklaring** | **Maand 4 (niet later dan de 15e)** |
|

\* De uitbetalings datum is in Pacific (standaard tijd) (PST).

## <a name="process-for-customer-non-payment"></a>Proces voor niet-betaling van klant

In zeldzame gevallen kan micro soft geen betalingen van klanten verzamelen voor hun aankopen op de Commercial Marketplace. Wanneer een klant micro soft niet kan betalen volgens hun facturerings schema, beginnen we met het incasso proces. Dit proces duurt ongeveer vier maanden en houdt permanente communicatie van micro soft met zich mee. Als de betaling niet aan het einde van dit proces wordt ontvangen, schrijft micro soft de fondsen als niet-geïncasseerd.

Op basis van het uitbetalings proces dat hier is gegeleeerd, heeft micro soft mogelijk al fondsen betaald aan uitgevers (u) die uiteindelijk niet worden geïncasseerd. Daarom hebben we een proces voor het afstemmen van deze bedragen. Om ervoor te zorgen dat uw (al ontvangen) betaling kan worden afgestemd, ontvangt u een melding wanneer een klant zich in het incasso proces bevindt en worden de aankopen waarschijnlijk afgeschreven.

Micro soft brengt alle uitbetalingen die u aan u hebt betaald, aan met een van de volgende methoden: (1) micro soft kan de onbetaalde bedragen van toekomstige uitbetalingen aftrekken; Als bijvoorbeeld $1.000 in uitbetalingen als niet-verzamelend wordt beschouwd en wordt afgeschreven, worden uw toekomstige uitbetalingen Inge houden tot de $1.000 wordt hersteld, of (2) micro soft kan een restitutie of factuur uitgevers aanvragen voor alle niet-geïnde bedragen.

Hier volgt een voorbeeld schema:

| Gebeurtenis | Geschatte datum * | Zicht baarheid partner |
| --- | --- | --- |
| Voor beeld van uitbetalings datum | 10/15/2020 | Gemarkeerd als **verzonden** in de sectie transactie geschiedenis en in betalingen in het uitbetalings dashboard |
| <font color="red">Als de klant micro soft niet betaalt</font> | 12/2/2020 – 12/5/2020 | Geen wijziging, hetzelfde als hierboven |
| Klant ontvangt eerste e-mail adres voor betaling | 12/6/2020 | Geen |
| De klant ontvangt regel matige e-mails met een oplopende urgentie | 12/7/2020 – 1/31/2021 | Geen |
| Publisher wordt op de hoogte gesteld van uitschrijving waarschijnlijk | 1/7/2021 | Er is een e-mail melding verzonden naar de uitgever dat de klant nog geen betaling heeft verzonden. De trans actie-ID en het dollar bedrag zijn opgenomen. |
| Opzeg ging van klant ontvangt | 2/1/2021 | Geen |
| Beëindiging van het verzamelings proces/fondsen zijn afgeschreven | 2/15/2021 | Er is een e-mail melding verzonden naar de uitgever die de fondsen afschrijven. De trans actie-ID en het dollar bedrag zijn opgenomen. |
| Uitbetaling wordt in mindering gebracht | 01-03-2021 | Er wordt een negatieve trans actie weer geven in de uitbetalings verklaring van partner Center |
| Uitbetaling wordt Inge houden | 3/15/2021 | Toekomstige uitbetalingen worden weer gegeven in de uitbetalings verklaring van partner Center. De betaling wordt pas ontvangen als het saldo niet langer negatief is.  |
|||

\* De uitbetalings datum is in Pacific (standaard tijd) (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Aantal dagen dat betalingen een uitbetalings account bereiken

Normaal gesp roken verstuurt de betaling in een bepaalde maand op de vijftiende dag van die maand, maar neemt het extra tijd in beslag om uw account te bereiken. Het aantal dagen is afhankelijk van de betalings wijze die we voor uw account gebruiken, zoals hieronder wordt beschreven.

> [!NOTE]
> De dagen die hieronder worden weer gegeven, zijn ongeveer gelijk aan. elke betaling kan een langere of korter tijd duren om uw account te bereiken.

| Betalingswijze     | Aantal dagen voor het bereiken van het uitbetalings account     |
|--------------------|--------------------------------------------|
| PayPal             | 1 werkdag                             |
| ACH/SEPA           | 2-3 werk dagen                          |
| Overschrijving      | 7-10 werk dagen                         |
|

## <a name="next-steps"></a>Volgende stappen

Meer informatie over [belasting gegevens](tax-details-marketplace.md).
