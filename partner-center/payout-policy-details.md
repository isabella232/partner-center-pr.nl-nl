---
title: Uitbetalingsschema's en-processen
description: Meer informatie over uitbetalingen en transacties, zoals betalingsschema's en recoupmentprocessen voor Azure Marketplace en andere transacties.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: bcecd4c31d80a4130331c652491e7951af180c67
ms.sourcegitcommit: f1255fb65eac6ee2e0ff0cb95cc16a02dc57fc1a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/27/2021
ms.locfileid: "110582414"
---
# <a name="payout-schedules-and-processes"></a>Uitbetalingsschema's en-processen

**Juiste rollen:** Accountbeheerder | Globale beheerder

In dit artikel wordt het betalingsschema van Microsoft beschreven, waar u de status van een uitbetaling kunt vinden en het proces voor het niet-betalen van klanten.

## <a name="payment-schedules"></a>Betalingsschema's

In de volgende secties wordt het uitbetalingsproces voor **Enterprise Agreement** en **Microsoft-klantovereenkomst CSP-transacties** beschreven.

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>Transacties wanneer de klant een Enterprise Agreement

Wanneer een klant een product aanschaft bij Microsoft AppSource of Azure Marketplace met behulp van hun bestaande Microsoft Enterprise Agreement voor transacties, zullen we uitbetalingen uitgeven in de volgende uitbetalingscyclus, 30 dagen na klantfactuur. Transacties waarbij een klant een creditcard gebruikt, hebben een periode van 30 dagen vóór uitbetaling.

Er wordt vaak een uitbetaling uitgevoerd voordat Microsoft de betaling van de klant int. Zie [Proces voor niet-betaling door](#process-for-customer-non-payment) klant hieronder voor de acties die we uitvoeren als de klant Microsoft niet kan betalen, maar we al een uitbetaling hebben uitgegeven.

| Gebeurtenis | Beschrijving | Zichtbaarheid van rapportage | Timing* |
| --- | --- | --- | --- |
| Gebruik of transactiemaand | De klant gebruikt of koopt een service. | [Gebruiks-](/azure/marketplace/partner-center-portal/usage-dashboard) [of orderdashboard](/azure/marketplace/partner-center-portal/orders-dashboard) | **Maand 1** |
| Microsoft berekent het factureringsbedrag | Het totale gebruik en het totale aantal transacties bepalen | [Gebruiks-](/azure/marketplace/partner-center-portal/usage-dashboard) [of orderdashboard](/azure/marketplace/partner-center-portal/orders-dashboard) | **Maand 2** |
| Geplaatste uitbetaling | Instantiekosten en uitbetalingsverdiensten bepalen | Gemarkeerd als Niet-verwerkt in transactiegeschiedenis op het [uitbetalingsoverzicht](payout-statement.md) | **Maand 3 (eerste week)** |
| Uitbetaling voorbereiden | Inkomsten worden voorbereid voor maandelijkse betaling | Gemarkeerd als aanstaande in transactiegeschiedenis in het [uitbetalingsoverzicht](payout-statement.md) | **Maand 3 (eerste week)** |
| **Uitbetaling verzonden** | **Betaling wordt verzonden naar uitgever** | **Gemarkeerd als Verzonden in transactiegeschiedenis en in de sectie Betalingen van het [uitbetalingsoverzicht](payout-statement.md)** | **Maand 3 (niet later dan de 15e)** |
| Factuur betaald door klant | Microsoft verzamelt betaling van klant | Geen wijziging | **Maand 4 tot en met 12** |
|

\* De uitbetalingsdatum is in Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Tijdlijn van betalingen voor Enterprise Agreement-klanten.":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>Transacties wanneer de klant een Microsoft-klantovereenkomst of CSP heeft

Alle aankopen met een creditcard of maandelijkse factuur hebben een periode van 30 dagen om ervoor te zorgen dat er geld wordt verzameld bij de klant.

| Gebeurtenis | Beschrijving | Zichtbaarheid van rapportage | Timing* |
| --- | --- | --- | --- |
| Gebruik of transactiemaand | De klant gebruikt of koopt een service. | [Gebruiks-](/azure/marketplace/partner-center-portal/usage-dashboard) [of orderdashboard](/azure/marketplace/partner-center-portal/orders-dashboard) | **Maand 1** |
| Factuur betaald door klant | Het totale gebruik, de totale transactiewaarde en de factuur van de klant bepalen | [Gebruiks-](/azure/marketplace/partner-center-portal/usage-dashboard) [of orderdashboard](/azure/marketplace/partner-center-portal/orders-dashboard) | **Maand 2** |
| Uitbetaling gepost | Instantiekosten en uitbetalingsverdiensten bepalen | Gemarkeerd als Niet-verwerkt in transactiegeschiedenis op het [uitbetalingsoverzicht](payout-statement.md) | **Maand 2** |
| Periode van 30 dagen | Zorg voor het verzamelen van tegoeden, mogelijke terugboekingen en restitutieaanvragen | Gemarkeerd als Niet-verwerkt in transactiegeschiedenis op het [uitbetalingsoverzicht](payout-statement.md) | **Maand 3** |
| Uitbetaling voorbereiden | Inkomsten worden voorbereid voor maandelijkse betaling | Gemarkeerd als Aanstaande in transactiegeschiedenis in het [uitbetalingsoverzicht](payout-statement.md) | **Maand 4 (eerste week)** |
| **Uitbetaling verzonden** | **Betaling wordt verzonden naar uitgever** | **Gemarkeerd als Verzonden in transactiegeschiedenis en in de sectie Betalingen van het [uitbetalingsoverzicht](payout-statement.md)** | **Maand 4 (niet later dan de 15e)** |
|

\* De uitbetalingsdatum is in Pacific Standard Time (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Tijdlijn van betalingen voor creditcard- en factuurklanten.":::

## <a name="process-for-customer-non-payment"></a>Proces voor niet-betaling door klant

In zeldzame gevallen kan Microsoft geen betalingen van klanten innen voor hun aankopen op de commerciële marketplace. Wanneer een klant microsoft niet kan betalen volgens het factureringsschema, beginnen we met het verzamelingsproces. Dit proces duurt ongeveer vier maanden en omvat permanente communicatie van Microsoft. Als er aan het einde van dit proces geen betaling is ontvangen, schrijft Microsoft het bedrag af als niet-in te zamelijk.

Volgens het uitbetalingsproces dat hier wordt verwoord, heeft Microsoft mogelijk al geld betaald aan uitgevers (u) die uiteindelijk niet kunnen worden opgehaald. Daarom hebben we een proces voor het afstemmen van deze bedragen.

Microsoft maakt alle uitbetalingen die al aan u zijn betaald, terug met behulp van een van de volgende methoden: (1) Microsoft kan de onbetaalde bedragen aftrekken van toekomstige uitbetalingen; Als bijvoorbeeld $ 1.000 aan uitbetalingen als oninbaar en afgeschreven wordt beschouwd, worden uw toekomstige uitbetalingen ingetrokken tot de $ 1000 is hersteld, of (2) Microsoft kan een restitutie of factuuruitgevers aanvragen voor alle niet-opgehaalde bedragen.

De volgende planning is een voorbeeld:

| Gebeurtenis | Geschatte datum* | Zichtbaarheid van partners |
| --- | --- | --- |
| Voorbeeld van uitbetalingsdatum | 10/15/2020 | Gemarkeerd als **verzonden** in transactiegeschiedenis en in de sectie Betalingen in uitbetalingsdashboard |
| <font color="red">Als de klant microsoft niet betaalt</font> | 12/2/2020 – 12/5/2020 | Geen wijziging, hetzelfde als hierboven |
| Klant ontvangt eerste e-mail met te late betaling | 12/6/2020 | Geen |
| De klant ontvangt regelmatig e-mailberichten met een toenemende urgentie | 12/7/2020 – 1/31/2021 | Geen |
| Uitgever krijgt een melding dat afschrijven waarschijnlijk is | 1/7/2021 | - |
| Klant ontvangt bericht over beëindiging | 2/1/2021 | Geen |
| Einde van het verzamelingsproces/ geld wordt afgeschreven | 2/15/2021 | E-mailmelding verzonden naar uitgever dat het bedrag is afgeschreven. |
| Uitbetaling wordt in mindering gebracht | 01-03-2021 | De uitgever ziet een negatieve transactie in Partner Center uitbetalingsoverzicht |
| Uitbetaling is ingehouden | 3/15/2021 | Toekomstige uitbetalingen worden weergegeven in Partner Center uitbetalingsoverzicht. De uitgever ontvangt geen betaling totdat het saldo niet langer negatief is.  |
|||

\* De uitbetalingsdatum is in Pacific Standard Time (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Aantal dagen dat betalingen een uitbetalingsaccount bereiken

Normaal gesproken verzenden we elke betaling die in een bepaalde maand op de 15e dag van die maand moet worden betaald, maar het duurt een andere keer om de betaling te bereiken. Het aantal dagen is afhankelijk van de betalingswijze die we voor uw account gebruiken, zoals hieronder wordt beschreven.

> [!NOTE]
> De onderstaande dagen zijn bij benadering; Het kan meer of minder tijd duren voor elke betaling uw account heeft bereikt.

| Betalingswijze     | Aantal dagen dat de uitbetalingsrekening moet worden bereikt     |
|--------------------|--------------------------------------------|
| PayPal             | 1 werkdag                             |
| BES/SEPA           | 2-3 werkdagen                          |
| Overschrijving      | 7-10 werkdagen                         |
|

## <a name="next-steps"></a>Volgende stappen

- [Belastinginformatie](tax-details-marketplace.md)
