---
title: Samenvatting van omzet in Partner Center dashboard
description: U kunt de samenvatting Revenue gebruiken om te begrijpen hoe de omzet die wordt gegenereerd door het klantverbruik van Azure-services bijdraagt aan uw inkomsten en waarom bepaalde omzet mogelijk niet in aanmerking komt voor inkomsten.
author: satinder37
ms.author: sabaja
ms.service: partner-dashboard
ms.topic: conceptual
ms.date: 10/04/2021
ms.custom: template-concept
customer intent: As an incentive user or incentive admin, I want to be able to read and export revenue data from Partner Center so I can see our earnings and learn why any transactions were reported ineligible.
ms.openlocfilehash: 11e58324adf38e92fc892ec5dd62933e6372f2cb
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593341"
---
# <a name="revenue-summary"></a>Opbrengstoverzicht

U kunt de samenvatting Revenue gebruiken om te begrijpen hoe de omzet die wordt gegenereerd door het klantverbruik van Azure-services bijdraagt aan uw inkomsten en waarom bepaalde omzet mogelijk niet in aanmerking komt voor inkomsten.

:::image type="content" source="images/revenue-summary/revenue-reporting-diagram.png" alt-text="Diagram van hoe de omzet wordt geëvalueerd en gerapporteerd op Partner Center":::

De samenvatting Omzet wordt pas bijgewerkt nadat de transacties zijn geëvalueerd, zodat het Azure-verbruik dat plaatsvindt in oktober pas wordt weergegeven in de samenvatting Omzet tot bijvoorbeeld november.

De samenvatting Omzet staat in de werkruimte Uitbetalingen, samen met de [pagina Transactiegeschiedenis](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) [en Betalingen.](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments)

## <a name="using-the-revenue-summary"></a>De samenvatting Revenue gebruiken

Met behulp van de samenvatting Revenue kunt u het volgende doen:

- Zoek in aanmerking komende omzet en de resulterende inkomsten op per klant of abonnement.
- Aanvulling op wat u leert uit de [transactiegeschiedenis met](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory)  inzichten over onderliggende omzetbedragen.
- Zoek eventuele in aanmerking komende omzet op en ontdek waarom die omzet niet in aanmerking komt.
- Gegevens exporteren over ineligible transacties, met inbegrip van de redenen voor [ineligibility](#ineligibility-reasons) en [kenmerken,](#exported-data-attributes)waarmee u beter begrijpt waarom deze transacties geen incentives hebben verdiend.

## <a name="access-roles-and-permissions"></a>Toegang tot rollen en machtigingen

Incentive-gebruikers en incentive-beheerders hebben toegang tot de samenvatting Revenue.
De informatie die beschikbaar is in de samenvatting is afhankelijk van de combinatie van programma en Microsoft Partner Network (MPN) die gebruikers en beheerders toegang hebben (net als bij de pagina's Transactiegeschiedenis en Betalingen). (Zie [Rollen en machtigingen toewijzen voor](permissions-overview.md) meer informatie over het instellen van gebruikers met rollen en wachtwoorden.)

## <a name="when-data-is-available"></a>Wanneer gegevens beschikbaar zijn

Azure-verbruiksgegevens worden doorgaans enkele weken na de maand waarin transacties plaatsvinden geëvalueerd. Informatie over de samenvatting van de omzet wordt alleen bijgewerkt wanneer deze evaluatie is voltooid. Dit resulteert in een vertraging tussen het moment waarop transacties plaatsvinden en wanneer ze worden gerapporteerd, zodat u het verbruik voor de huidige maand niet kunt zien in de samenvatting Omzet. Gegevens voor maart worden bijvoorbeeld doorgaans geëvalueerd in ongeveer de derde week van april en de samenvattingsinformatie over de omzet wordt doorgaans kort daarna bijgewerkt.

## <a name="customer-summary-view"></a>Klantoverzichtsweergave

In de samenvattingsweergave Klant ziet u de geaggregeerde omzet per klantnaam en programma/betrokkenheid.

Inzichten in klantsamenvatting zijn onder andere:

- **Top 10 op in aanmerking komende omzet** toont de top 10 van klanten die bijdragen aan de maximaal in aanmerking komende omzet.
- **Top 10 op ineligible omzet** toont de top 10 van klanten die bijdragen aan de maximale omzet die niet in aanmerking komt.
- **Top 10 op inkomsten toont** de top 10 van klanten die bijdragen aan de maximale inkomsten.

U kunt zoeken naar informatie over elke klant in het klantoverzicht, niet alleen de top 10.

## <a name="eligible-transactions"></a>In aanmerking komende transacties

*In aanmerking komende transacties* zijn transacties die omzet opleveren die in aanmerking komen voor inkomstenbetalingen.

U kunt zoeken naar informatie over in aanmerking komende transacties op klant-id of abonnements-id. U kunt echter geen gegevens exporteren over in aanmerking komende transacties.

## <a name="ineligible-transactions"></a>Niet-in aanmerking komende transacties

*Ineligible transacties zijn* transacties die niet in aanmerking komen voor inkomstenbetalingen.

- De redenen waarom transacties als niet-in aanmerking komend voor inkomsten worden vermeld in de sectie Redenen voor [ineligibility](#ineligibility-reasons) van dit artikel.
- U kunt gegevens over  [niet-in](#exporting-data) aanmerking komende transacties zoeken en exporteren om erachter te komen waarom u mogelijk geen MCI-incentives hebt verdiend.
- In de samenvatting Omzet wordt altijd de meest recente omzetclassificatie weergegeven (zodat u niet kunt zien hoe een transactie een maand eerder is geclassificeerd). Een transactie die één maand als niet-in aanmerking komend is gemarkeerd, kan de volgende maand als in aanmerking komend worden gemarkeerd.

Niet-in aanmerking komende transacties die worden vermeld in de samenvatting Omzet hebben kenmerken die het volgende omvatten:

- product
- niet-in aanmerking komende omzet
- [reden van ineligibility](#ineligibility-reasons)
- subscription ID
- naam van de klant (meestal beschikbaar nadat een abonnement voor de eerste keer is gefactureerd)

U kunt in aanmerking komende transacties doorzoeken op klantnaam en abonnements-id. (Het aantal weergegeven records is beperkt tot 10.) Als de informatie die u vindt geen antwoord biedt op uw vragen, neemt u contact op met de ondersteuning voor hulp.

## <a name="ineligibility-reasons"></a>Redenen voor ineligibility

*Ineligibility reasons* in the tables that follow indicate why revenue was classified ineligible for earnings. Elke rij in de tabellen bevat ook een uitleg over of en hoe een partner met ineligible verdiensten weer in aanmerking kan komen voor inkomsten.

Sommige ineligibility redenen in deze tabellen zijn mogelijk niet van toepassing op een bepaalde betrokkenheid.

Er zijn drie categorieën van ineligibility:

- [Niet-in aanmerking komende klant](#ineligible-customer)
- [Ineligible partner](#ineligible-partner)
- [Niet-in aanmerking komende transactie](#ineligible-transaction)

### <a name="ineligible-customer"></a>Niet-in aanmerking komende klant

|Reden van ineligibility|Actie van partner vereist?|Opnieuw in aanmerking komen|
|---------|---------|---------|
|Klant is een openbare sector|Ja, als de klant zich in Verenigde Staten, Bijeen of India|Als u hebt gereageerd op een PO-aanvraag (Proof of Execution) en deze is afgewezen, kunt u niet opnieuw in aanmerking komen. (Wanneer een POE wordt afgewezen, wordt er een e-mail verzonden waarin wordt uitgelegd waarom.)<br><br>U kunt binnen 90 dagen na de transactie/inkomstendatum een andere POE aanvragen. (Zorg ervoor dat u de ontvangst van de E-MAIL-e-mail bevestigt wanneer deze binnenkomt.) U kunt ineligibility ook binnen 90 dagen betwisten door contact op te nemen met ondersteuning met de reden van ineligibility, abonnement en klantgegevens en de reden voor betwisting.|
|De omzet van China mag niet eigendom zijn van een niet-China-partner|No|Partner kan niet opnieuw in aanmerking komen door beleid.|

### <a name="ineligible-partner"></a>Ineligible partner

|Reden van ineligibility|Partneractie vereist|Opnieuw in aanmerking komen|
|---------|---------|---------|
|Er is niet voldaan aan een geavanceerde specialisatievereiste|Yes|[Meer informatie over geavanceerde specialisaties](advanced-specializations.md)|
|Competentiestatus niet bereikt of verlopen|Yes|Bekijk uw competentiestatus op [Competenties](https://partner.microsoft.com/pcv/partnership/competencies). Bekijk de vereiste competenties voor uw betrokkenheid bij [Incentives Engagements](https://partner.microsoft.com/dashboard/incentives/engagements/ux)|
|MPA-overeenkomst is verlopen of niet ondertekend|Yes|Verifieer en onderteken de MPA-overeenkomst aan de hand van [de richtlijnen Microsoft Partner-overeenkomst voor CSP-programmapartners](microsoft-partner-agreement.md)|
|Geschiktheid voor co-verkoop is verlopen of niet vastgesteld|Yes|Zie Co-sell with Microsoft sales teams and partners overview (Overzicht [van co-verkoop met Microsoft-verkoopteams en -partners)](/azure/marketplace/co-sell-overview)|
|Partnerlocatie komt niet in aanmerking voor incentives|No|Partner kan niet opnieuw in aanmerking komen door beleid|
|MPN-id komt niet in aanmerking voor deelname aan betrokkenheid|No|Partner kan niet opnieuw in aanmerking komen door beleid|

### <a name="ineligible-transaction"></a>Niet-in aanmerking komende transactie

|Reden van ineligibility|Actie van partner vereist?|Opnieuw in aanmerking komen|
|---------|---------|---------|
|Bewijs van uitvoering is niet goedgekeurd|Ja, als u niet hebt gereageerd op een E-mail van Microsoft over het bewijs van uitvoering van een digitale partner of record (DPOR)|Het bewijs van uitvoering van de aanvraag is alleen van toepassing op de openbare sector of DPOR. Met ingang van 1 oktober 2021 wordt DPOR niet langer gecentraliseerd voor Azure, waardoor ERE-aanvragen niet meer worden verzonden.<br><br>Als u op een e-mail hebt gereageerd met het onderwerp 'Bewijs van uitvoering vereist' en uw antwoord is afgewezen, kunt u niet opnieuw in aanmerking komen.|

## <a name="exporting-data"></a>Gegevens exporteren

U kunt informatie over niet-in aanmerking komende transacties (maar niet in aanmerking komende transacties) downloaden in het overzicht van de omzet.

:::image type="content" source="images/revenue-summary/export-data-page.png" alt-text="Schermopname van de pagina Gegevens exporteren Partner Center":::

### <a name="exported-data-attributes"></a>Geëxporteerde gegevenskenmerken

Kenmerken van niet-in aanmerking komende transacties zijn:

|Kenmerknaam  |Description  |
|---------|---------|
|agreementNumber|Overeenkomstnummer (alleen beschikbaar indien van toepassing)|
|customerId|De identiteit van de klant die is gekoppeld aan een abonnement/resource. (Voor Azure-verbruik is deze informatie niet beschikbaar voor de eerste 30 tot 45 dagen van een nieuw abonnement, tenzij de eerste factuur is gemaakt.)|
|customerIdType|TPID- of MCAPI-id|
|customerName|Naam van de klant|
|invoiceNumber|Factuurnummer (alleen beschikbaar voor partner-led, field-led en customer-led)|
|partnerCountryCode|Geregistreerde MPN-locatie|
|partnerId|MPN-id van de geregistreerde partner|
|partnerName|Naam van de partner|
|productId|Commerce-productnaam|
|productFamily|Productfamilie|
|reason|Reden voor ineligibility|
|subscriptionId|Abonnements-id|
|transactionAmountUSD|Verbruiksbedrag in Amerikaanse dollars|
|transactionDate|Datum van verbruik of facturering
|unearnedId|Unieke id die u kan helpen bij het maken van een ondersteuningsvraag|
|workload|Servicenaam of workloadnaam|

## <a name="next-steps"></a>Volgende stappen

Bekijk de volgende artikelen voor meer informatie over transacties, omzet, inkomsten en betalingen.

- Bekijk de [pagina Transactiegeschiedenis](https://partner.microsoft.com/dashboard/payouts/reports/transactionhistory) om inkomsten en bijbehorende transactiegegevens weer te geven voor al uw programma's met de bijbehorende betalingsstatus.
- Bekijk de [pagina Betalingen om](https://partner.microsoft.com/dashboard/payouts/reports/incentivepayments) voltooide en in behandeling zijnde betalingen voor al uw programma's weer te geven.
- Bekijk de [pagina Uitbetalingsoverzichten](payout-statement.md) voor een overzicht van uw uitbetalingen van aanbiedingen die via de commerciële marketplace worden verkocht.
