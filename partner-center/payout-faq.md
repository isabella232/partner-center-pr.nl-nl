---
title: Veelgestelde vragen over uitbetaling voor micro soft Commercial Marketplace
description: Krijg antwoorden op veelgestelde vragen over uitbetalingen in de commerciële Marketplace. Bevat antwoorden over waarom uw inkomsten anders zijn dan verwacht.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/11/2020
ms.openlocfilehash: 5775eb497940870344e0d3da85def7c3e717c65f
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532018"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Veelgestelde vragen over uitbetalingen door commerciële Marketplace

In dit artikel vindt u antwoorden op veelgestelde vragen over uitbetalingen in de commerciële Marketplace.

## <a name="earnings-incorrect-or-missing"></a>Winst is onjuist of ontbreekt

#### <a name="why-are-my-earnings-missing"></a>Waarom ontbreken mijn inkomsten?

- De klantorder komt mogelijk nog niet in aanmerking voor uitbetaling. Voor niet-zakelijke klanten moet Microsoft de betaling van de klant hebben ontvangen voordat de uitgever in aanmerking komt voor uitbetaling. Voor zakelijke klantorders zijn uw inkomsten 1-2 dagen na de datum van de aankoop beschikbaar. Controleer de status van de bestelling in [Orderrapporten](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Inkomsten van transacties vóór juli 2019 mogen niet worden weergegeven in het transactieoverzichtrapport. Controleer historische instructies in [Uitbetalingen downloaden](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Controleer het [tijds bestek van de afbetalings cyclus](payment-thresholds-methods-timeframes.md) en begrijp wanneer uw winst moet worden weer gegeven in de uitbetalings verklaring.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>Waarom is mijn loon bedrag anders dan verwacht?

- Als de bestelling deels door uw klant is betaald, wordt uw verdienen bedrag gebaseerd op het gedeeltelijk betaalde bedrag na aftrek van de kosten en de juiste belasting.
- De verantwoordelijkheid voor het BTW-tarief controleren per land. In het geval van landen/regio's waar btw de verantwoordelijkheid van Microsoft is, int Microsoft de btw en trekt deze van de inkomsten van de uitgever af. Het transactiebedrag dat op het overzicht wordt weergegeven, is het bedrag na btw-aftrek. Zie [Belastinginformatie](tax-details-marketplace.md).
- SaaS-en IaaS-aanbiedingen hebben een gereduceerd tarief voor de organisatie tegen 10% in plaats van de standaard 20%, waardoor er een inkomsten tarief van 90% wordt gelaten. Deze aanbieding is geldig tot en met 30 juni 2021.

**Meer Lees** : [commerciële Marketplace Publisher-overeenkomst](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details](payout-policy-details.md)van uitbetalings beleid, [betalings drempel, methode en tijds bestek](payment-thresholds-methods-timeframes.md), [betaald in de commerciële Marketplace](marketplace-get-paid.md), [belasting gegevens](tax-details-marketplace.md), uitzonderings [instructies](payout-statement.md), [dash board orders in commerciële Marketplace-analyse](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>Inkomstenafstemming
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>Hoe kan ik uitbetalingsoverzichten afstemmen op order- of gebruiksrapporten in analyses?
Gebruik AssetID, orderID en regel item-ID die wordt weer gegeven in het rapport uitbetalings transactie geschiedenis met analytische orders en gebruiks rapporten. Deze toewijzing gebruiken:

- Uitbetalingstransactie History.AssetID = order.OrderID
- Uitbetalingstransactie History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>Hoe weet ik wanneer ik betalingen voor mijn klantorders kan verwachten?
- Controleer eerst met behulp van uw assetID de orders van klanten in de [rapporten orders](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Controleer het klant kanaal voor uw klant abonnement in het [rapport klanten](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- Voor zakelijke klanten worden de Publisher-inkomsten weer gegeven in de verklaring 1-2 dagen na de datum van de aankoop order.
- Voor niet-zakelijke klanten worden de Publisher-inkomsten weer gegeven in de verklaring 1-2 dagen nadat de betaling van de klant is ontvangen.

**Meer Lees** : [uitbetalings instructies](payout-statement.md), [dash board orders in commerciële Marketplace-analyse](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Beleid voor uitbetaling

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>Hoe kan ik de huidige bemiddelingskosten en het uitbetalingspercentage vinden?

- Bekijk de overeenkomst voor uitgevers van de commerciële marketplace. De standaardbemiddelingskosten zijn 20%. SaaS Co-Sell in aanmerking komende trans acties hebben een korting van 10% op kosten. Controleer of er aanbiedingen zijn voor korting op bemiddelingskosten.
- In uw uitbetalings verklaring geeft u het rente bedrag op voor een bepaalde trans actie.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Wanneer kan ik een betaling van Microsoft verwachten wanneer de inkomsten op mijn overzicht worden weergegeven?
- Als uw inkomsten de status Niet-verwerkt hebben, kunt u de vervaldatum controleren voor de maand waarin uw inkomsten worden verwerkt voor betaling. Zodra uw betaling is voor bereid, wordt de status van uw loon gewijzigd in ' verwerkt '.  Microsoft verstrekt betalingen op de 15e van de maand van de vervaldatum.
- Voor bestellingen die met een credit card zijn betaald, houdt micro soft betalingen 30 dagen tot het verdienen is vervallen.

 **Verdere Lees** : [commerciële Marketplace Uitgever overeenkomst](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details van uitbetalings beleid](payout-policy-details.md), [belasting gegevens](tax-details-marketplace.md), [betalings drempel, methode en tijds bestek](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>Betalingen en aanpassingen

#### <a name="why-is-my-payment-missing"></a>Waarom ontbreekt mijn betaling?

- Zorg ervoor dat de status van de uitbetaling en het BTW-profiel *geldig* zijn op de [pagina overzicht](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Mogelijk hebt u niet voldaan aan de minimumdrempel voor een betaling. De inkomsten moeten ten minste $ 50 USD zijn om een betaling te ontvangen.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Mijn account Hoe kan ik instellen dat er geen betaling wordt ontvangen?
U kunt betalingen in het [profiel voor uitbetaling](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)bewaren. Controleer gewoon de **wacht stand**. Micro soft houdt de betaling over aan u totdat u de blok kering uitbrengt.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>Waarom ontvang ik mijn betaling in een andere valuta dan de aankoopvaluta?

De valuta voor uitbetaling is gebaseerd op de valuta die u hebt geselecteerd in het uitbetalingsprofiel. De aankoopvaluta is gebaseerd op de valuta waarin de klant heeft betaald.

#### <a name="how-do-i-reconcile-adjustments"></a>Hoe kan ik correcties afstemmen?

Betalingscorrecties zijn correcties voor compensatiecorrecties zoals systeemproblemen. In het uitbetalingsoverzicht geeft ReasonCode de reden voor de correctie aan. Deze zijn niet bedoeld om rechtstreeks afzonderlijke transacties af te stemmen.

**Verdere Lees** : [commerciële Marketplace Uitgever overeenkomst](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details van uitbetalings beleid](payout-policy-details.md), [belasting gegevens](tax-details-marketplace.md), [betalings drempel, methode en tijds bestek](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>Belastingen

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>Hoe kan ik op het uitbetalingsoverzicht zien of Microsoft of de uitgever verantwoordelijk is voor de btw-afdracht?

Zoek in de download van het transactieoverzicht de kolom Btw-model op. Hierin wordt aangegeven of dit door Microsoft of de aanbieder wordt beheerd. Zie landspecifieke belastingregels en gevolgen voor uitbetalingen in [Belastinginformatie](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hoe kan ik belastingformulieren voor servicekosten downloaden?

Ga naar de pagina **Betaling uitbetaling** en vervolgens naar het gedeelte **Lijst met betalingen**. Er wordt een link naar het belastingformulier voor servicekosten weergegeven voor een betaling met servicekostenbelasting.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Hoe kan ik een bronbelastingformulier als PDF downloaden?

Ga naar de pagina *Betaling uitbetaling* en vervolgens naar het gedeelte **Lijst met betalingen**. Er wordt een koppeling naar een bronbelastingformulier weergegeven naast een betaling.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Waar vind ik de belastingformulieren voor het eind van het jaar?

Ga naar de [Profielpagina](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) om uw belastingformulieren voor het eind van het jaar weer te geven.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>Hoe kan ik de bronbelasting voor een transactie vinden?
Bronbelasting is van toepassing op Amerikaanse uitgevers die een W-9-formulier hebben ingediend. Bronbelasting wordt berekend over een maandelijkse betaling.

**Meer Lees** : [commerciële Marketplace Uitgever overeenkomst](https://go.microsoft.com/fwlink/p/?LinkID=699560), [Details van uitbetalings beleid](payout-policy-details.md)

## <a name="payout-statement-access"></a>Toegang tot uitbetalings instructies

#### <a name="how-do-i-access-a-payout-statement"></a>Hoe kan ik toegang krijgen tot een uitbetalingsoverzicht?

1. Controleer uw rollen. U moet de rol *financiële bijdrager* of *accounteigenaar* hebben om toegang te krijgen tot het uitbetalingsoverzicht.
2. Selecteer in de rechter bovenhoek het **uitbetalings** pictogram om uw uitbetalings verklaring weer te geven. U kunt kiezen tussen **transactie geschiedenis** , **betaling** en **downloaden**.

**Meer Lees** : [uitbetalings rollen en machtigingen](payout-statement.md#roles-and-permissions), [uitbetalings instructies](payout-statement.md) 

## <a name="payout-statement-report"></a>Rapport uitbetalings overzicht

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>Wat betekent elk veld in de download van de transactie?

Zie [uitbetalings instructies](payout-statement.md) voor een gedetailleerde lijst met kenmerken en hun betekenis.

#### <a name="what-is-earning-status"></a>Wat is de inkomstenstatus?

Hiermee wordt uw winst weer gegeven als een niet-verwerkt, verwerkt of verzonden.

- Niet- **verwerkte** : de winst wordt in een borg periode tot de verval datum.
- **Verwerkt** : de winst is gerijpd en wordt voor bereid op een maandelijkse betaling. De betalingen worden door 15e van elke maand vrijgegeven.
- **Verzonden** : betaling is op basis van uw uitzonderings profiel aan uw bank uitgegeven.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>Hoe kan ik belastingformulieren voor servicekosten downloaden?

Ga naar de pagina **Betaling uitbetaling** en vervolgens naar het gedeelte **Lijst met betalingen**. Er wordt een link naar het belastingformulier voor servicekosten weergegeven voor een betaling met servicekostenbelasting.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Hoe kan ik een bronbelasting formulier in PDF downloaden?

Ga naar de pagina **Betaling uitbetaling** en vervolgens naar het gedeelte **Lijst met betalingen**. Er wordt een koppeling naar een bronbelastingformulier weergegeven naast een betaling.

#### <a name="where-do-i-find-year-end-tax-forms"></a>Waar vind ik de belastingformulieren voor het eind van het jaar?

Ga naar de [Profielpagina](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) om uw belastingformulieren voor het eind van het jaar weer te geven.

**Meer Lees** : [uitbetalings instructies](payout-statement.md), [downloaden van transactie geschiedenis](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Historische instructies

#### <a name="how-do-i-view-historical-information"></a>Hoe kan ik historische gegevens weer geven?

In het historische overzicht wordt een momentopname weergegeven van de uitbetalingsgegevens van oktober 2019. Helaas worden de informatie over de uitbetaling niet vernieuwd. Als u de meest recente informatie wilt ontvangen, dient u een ondersteunings ticket in voor de meest recente gegevens.

**Meer Lees** : [uitbetalings instructies](payout-statement.md), [downloaden van transactie geschiedenis](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API voor betaling exporteren

#### <a name="how-do-i-download-payout-data"></a>Hoe kan ik uitbetalingsgegevens downloaden?

Gebruik de [partner-uitbetalings-API](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Volgende stappen

- [Betaald krijgen in de commerciële marketplace](marketplace-get-paid.md)
