---
title: Uitbetalings verklaring voor de commerciële Marketplace in het partner centrum
description: Meer informatie over uitbetalings overzichten en samen vattingen en het weer geven en exporteren van uw betalings gegevens voor de commerciële Marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.date: 09/23/2020
ms.openlocfilehash: 460a7b1992d7db40e0f45d3aeb7e2236e9495e07
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/25/2020
ms.locfileid: "92528624"
---
# <a name="payout-statements"></a>Uitbetalingsinstructies

De **uitbetalings verklaring** geeft een overzicht van uw uitbetalingen uit aanbiedingen die via de commerciële Marketplace worden verkocht. Hierin worden de transactie geschiedenis van uw inkomsten weer gegeven, wordt uw volgende betaling geschat en worden de betalings trends weer gegeven. U kunt ook transactie geschiedenis en betalings overzichten downloaden. In dit artikel wordt uitgelegd hoe u toegang krijgt tot uw uitbetalings verklaring en de verschillende uitbetalings pagina's en down loads die voor u toegankelijk zijn in het partner centrum.

## <a name="roles-and-permissions"></a>Rollen en machtigingen

Als u toegang wilt krijgen tot een uitbetalings verklaring, moet u de rol **account eigenaar** of **financiële bijdrager** toewijzen.

| Rapporten/pagina's | Accounteigenaar | Manager | Ontwikkelaar | Zakelijke Inzender | Bijdrage financier | Verkoper |
| --- | --- | --- | --- | --- | --- | --- |
| Verwervings rapport (inclusief bijna realtime gegevens) | Kan weer geven | Kan weer geven | Geen toegang | Geen toegang | Kan weer geven | Geen toegang |
| Feedback rapport/reacties | Kan feedback weer geven en verzenden | Kan feedback weer geven en verzenden | Kan feedback weer geven en verzenden | Geen toegang | Geen toegang | Kan feedback weer geven en verzenden |
| Status rapport (inclusief bijna realtime gegevens) | Kan weer geven | Kan weer geven | Kan weer geven | Kan weer geven | Geen toegang | Geen toegang |
| Gebruiks rapport | Kan weer geven | Kan weer geven | Kan weer geven | Kan weer geven | Geen toegang | Geen toegang |
| Uitbetalings account | Kan bijwerken | Geen toegang | Geen toegang | Geen toegang | Kan bijwerken | Geen toegang |
| BTW-profiel | Kan bijwerken | Geen toegang | Geen toegang | Geen toegang | Kan bijwerken | Geen toegang |
| Betalingsoverzicht | Kan weer geven | Geen toegang | Geen toegang | Geen toegang | Kan weer geven | Geen toegang |
|

## <a name="access-your-payout-statement"></a>Toegang tot uw uitbetalings verklaring

Meld u aan bij [partner centrum](https://partner.microsoft.com/dashboard/home) en selecteer het uitbetalings pictogram in de rechter bovenhoek van het scherm om deze verschillende samen vattingen te openen:

- Transactie geschiedenis
- Betalingen
- Gegevens exporteren

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Illustreert het uitbetalings pictogram in de rechter bovenhoek van de Partner Center-Portal":::

U kunt ook de [partner-uitbetalings-API](https://apidocs.microsoft.com/services/partnerpayouts) gebruiken om direct verbinding te maken en trans actie-en betalings gegevens te verkrijgen.


## <a name="transaction-history"></a>Transactie geschiedenis

Op de pagina **transactie geschiedenis** ziet u het overzicht van uw inkomsten, de geschatte volgende betaling en uw inkomsten-en betalings trends in de afgelopen 36 maanden. U kunt ook transactie gegevens uit deze sectie downloaden.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Illustreert het uitbetalings pictogram in de rechter bovenhoek van de Partner Center-Portal":::

- De **inkomsten die dit jaar zijn verzonden** , zijn het totale inkomen en de uitsplitsing van de inkomsten die zijn betaald en worden betaald in de komende maand.
- **Geschatte betalings maand** : de totale inkomsten die in de komende maanden worden verwacht.
- **Trend van inkomsten en betalingen** : maandelijks betaalde en betalings bedragen voor de afgelopen 36 maanden.
- **Downloaden** : transactie gegevens downloaden in CSV-of. TSV-indeling.

Gebruik de selectie in het datum bereik in de rechter bovenhoek van de pagina om de uitvoer van de pagina te filteren zodat de afgelopen 3, 6, 12 of 36 maanden worden weer gegeven. Of selecteer een aangepast datum bereik van Maxi maal 36 maanden. Het standaard datum bereik is 12 maanden.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Illustreert het uitbetalings pictogram in de rechter bovenhoek van de Partner Center-Portal":::

### <a name="transaction-history-summary"></a>Overzicht transactie geschiedenis

Dit toont details over het verdienen, waaronder de oorsprong van het verdienen van het product, de status en de geschatte betalings maand.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Illustreert het uitbetalings pictogram in de rechter bovenhoek van de Partner Center-Portal":::

- **Huidige datum** : de datum van aankoop.
- **Type verdienen** : het type van verdienen, zoals verkoop, korting of co-op.
- **Totaal bedrag** : het bedrag van het nettobedrag. In de commerciële Marketplace houdt dit in dat de kosten voor de standaard Marketplace worden afgetrokken.
- **Status** : heeft drie opties:
    - **Gepland** : de inkomsten zijn in afwachting van wachtende koel periode.
    - **Verwerkt** : de inkomsten worden voor bereid voor de volgende betaling.
    - **Verzonden** : de winst is betaald.
- **Geschatte betalings maand** : de maand dat de inkomsten zullen worden betaald.

Er worden verdienen trans acties weer gegeven zodra de trans actie voldoet aan de toekennings kwalificatie. Zie [Veelgestelde vragen over uitbetalingen door commerciële Marketplace](payout-faq.md#why-are-my-earnings-missing)als u wilt weten waarom er sprake is van ontbrekende of onverwachte inkomsten.

### <a name="transaction-history-download"></a>Transactie geschiedenis downloaden

Klik boven aan de pagina op **downloaden** om meer informatie over een verdienen te bekijken. In de volgende tabel wordt elke kolom in het rapport uitgelegd.

| Kolomnaam | Description | Toepasselijkheid voor prikkel Programma's/markt plaatsen |
| --- | --- | --- |
| agreementEndDate | Eind datum van overeenkomst | Prikkel-sommige Program ma's alleen |
| agreementNumber | Overeenkomst nummer | Prikkel-sommige Program ma's alleen |
| agreementStartDate | Begin datum overeenkomst | Prikkel-sommige Program ma's alleen |
| calculationDate | De datum waarop het verdienen is berekend in het systeem | Alles |
| claimId | Unieke id voor claim | Prikkel-sommige Program ma's alleen |
| customerCountry | Land/regio van klant | markt plaatsen |
| customerEmail |  |  |
| customerName | Is altijd leeg | Alleen prikkel programma's (uitzonde ring: OEM) en marketplaces |
| customerTenantId |  |  |
| distributorId | Id van distributie server | Prikkel-sommige Program ma's alleen |
| Distributor | Naam van Distributor | Prikkel-sommige Program ma's alleen |
| earningAmount | Het verdienen van het bedrag in de oorspronkelijke transactie valuta | Alles |
| earningAmountInLastPaymentCurrency | Het verdienen van het bedrag in de laatste betalings valuta (veld is leeg als er geen eerdere betaling is betaald) |  |
| earningAmountUSD | Verdienen bedrag in USD | Alles |
| earningDate | Datum van het verdienen | Alles |
| earningExchangeRate | De wissel koers die wordt gebruikt om het overeenkomstige USD-bedrag weer te geven | Alles |
| earningId | Unieke id voor elk verdienen | Alles |
| earningRate | Prijs stimulans toegepast op transactie bedrag om een verdienen te genereren | Alles |
| earningType | Hiermee wordt aangegeven of het om kosten, korting, mede op, verkopen, enzovoort gaat | Alles |
| exchangeRateDate | Wisselkoers datum die wordt gebruikt voor het berekenen van EarningAmount USD | Alles |
| externalReferenceId | De unieke id voor het programma | Program ma's voor direct betalen (prikkels en markt plaatsen) |
| externalReferenceIdLabel | Label voor unieke id | Program ma's voor direct betalen (prikkels en markt plaatsen) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Factuur nummer (alleen van toepassing voor bedrijven) | Prikkels en marketplaces-sommige Program ma's |
| lastPaymentCurrency | De laatste betalings valuta (veld is leeg als er geen eerdere betaling is betaald) |  |
| kern | Geeft bedrijfs regel voor het verdienen aan | Alles |
| LicensingProgramName | Naam van het licentie programma |  |
| LineItemId | Afzonderlijke regel in de factuur van een klant |  |
| localProviderSeller | Lokale provider/verkoper van record |  |
| Maand van verval datum | De geschatte betalings maand | Alles |
| OrderId | Is gekoppeld aan de factuur van een klant  | markt plaatsen |
| parentProductId | Unieke id van het bovenliggende product. Als er geen bovenliggend product voor de trans actie is, dan is de product-id van de bovenliggende product-id. | markt plaatsen |
| parentProductName | De naam van het bovenliggende product. Als er geen bovenliggend product voor de trans actie is, dan is de naam van het bovenliggende product = product naam. | markt plaatsen |
| participantId | De primaire identiteit van de partner die onder het programma is aangegaan | Alles |
| participantIdType | Voornamelijk programma-ID voor prikkel Programma's en verkopers als voor marketplaces | Alles |
| deel nemer | Naam van de verdienen partner | Alles |
| partnerCountryCode | Locatie/land/regio van de verdienen partner | Alles |
| partNumber | Is altijd leeg | Sommige stimulerings Programma's en markt plaatsen |
| paymentId | De unieke id voor de betaling. Dit nummer is doorgaans zichtbaar in uw bank afschrift | Alleen SAP-betalingen |
| paymentStatus | Betalingsstatus | Alles |
| paymentStatusDescription | Beschrijvende beschrijving van de betalings status | Alles |
| productId | Unieke product-id | markt plaatsen |
| Product | Product naam die aan de trans actie is gekoppeld | Alles |
| productType | Type product, zoals app, invoeg toepassing of spel | markt plaatsen |
| Programma code | Teken reeks die moet worden toegewezen aan de programma naam |  |
| programName | Naam van het prestatie/archief programma | Alles |
| purchaseOrderCoverageEndDate | Is altijd leeg | Prestatie programma-CRI |
| purchaseOrderCoverageStartDate | Is altijd leeg | Prestatie programma-CRI |
| purchaseOrderType | Is altijd leeg | Prestatie programma-CRI |
| purchaseTypeCode | Is altijd leeg | Prestatie programma-CRI |
| quantity | Is afhankelijk van het programma. Hiermee wordt de gefactureerde hoeveelheid voor transactionele Program ma's aangegeven | Alles |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Wederverkoper-id | Prikkel-sommige Program ma's alleen |
| Verkoperstatus | Reseller name |  |
| SkuId | SKU-ID zoals gedefinieerd tijdens het publiceren. Een aanbieding kan veel Sku's hebben, maar een SKU kan slechts worden gekoppeld aan één aanbieding. Prikkel-sommige Program ma's alleen |  |
| storeFee | Het bedrag dat door micro soft wordt bewaard als een vergoeding voor het maken van de app of invoeg toepassing die beschikbaar is in de Store | markt plaatsen |
| subscriptionEndDate | Eind datum van abonnement | Prikkel-sommige Program ma's alleen |
| subscriptionId | De abonnements-id die is gekoppeld aan de klant | Prikkel-sommige Program ma's alleen |
| Subscription | Begin datum van het abonnement | Prikkel-sommige Program ma's alleen |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Partij verantwoordelijk voor het remitteren van belastingen (verkoop, gebruik of btw/GST-belastingen) | markt plaatsen |
| taxRemitted | Bedrag van overgeschreven BTW (verkoop, gebruik of btw/GST-belastingen) | markt plaatsen |
| taxState | Provincie van de klant |  |
| taxZipCode | Post code van de klant |  |
| tpan | Hiermee wordt het AD-netwerk van derden aangegeven | alleen advertenties voor Marketplace |
| transactionAmount | Transactie bedrag in de oorspronkelijke transactie valuta op basis waarvan het verdienen is gegenereerd | Alles |
| transactionAmountUSD | Transactie bedrag in USD | Alles |
| transactionCountryCode | Land-/regiocode waarin de trans actie plaatsvond |  |
| transactionCurrency | Valuta waarin de oorspronkelijke klant transactie heeft plaatsgevonden (dit is geen valuta voor de partner locatie) | Alles |
| transactionDate | De datum van de trans actie. Handig voor Program ma's waarbij veel trans acties bijdragen aan één verdienen | Alles |
| transactionExchangeRate | De wisselkoers datum die wordt gebruikt voor het weer geven van het corresponderende bedrag van de transactie belasting | Alles |
| transactionId | De unieke id voor de trans actie | Alles |
| transactionPaymentMethod | Het betalings instrument van de klant dat wordt gebruikt voor de trans actie, zoals kaart, facturering van mobiele provider of PayPal | markt plaatsen |
| transactionType | Type trans actie, zoals aankoop, terugbetaling, omkering of terugstorting | markt plaatsen |
| workload | Workload | Prikkel-sommige Program ma's alleen |
|

## <a name="payments"></a>Betalingen

De pagina **betalingen** bevat informatie over het geld dat u bij micro soft hebt behaald. Ook wordt weer gegeven wanneer en hoeveel u gaat uitbetalen.

>[!Note]
> Om in aanmerking te komen voor toekenning, moet uw opbrengst de [betalings drempelwaarde](payment-thresholds-methods-timeframes.md) van $50 bereiken. Zie de [micro soft Publisher-overeenkomst](https://go.microsoft.com/fwlink/?LinkID=699560)voor meer informatie.

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Illustreert het uitbetalings pictogram in de rechter bovenhoek van de Partner Center-Portal":::

- **Totaal betaald dit jaar** : het gecombineerde totaal bedrag dat aan u dit jaar is betaald, in Amerikaanse dollars, voor al uw Program ma's.
- **Volgende geraamde betaling** : de enkele volgende betaling die aan u wordt toegeleverd (zelfs als er binnenkort nog andere betalingen beschikbaar zijn), in Amerikaanse dollars.
- **Laatste betaling** : het bedrag (in Amerikaanse dollars), de programma naam en het programma van uw meest recente betaling.
- **Betaling per bron** : bedrag van de betalingen (in Amerikaanse dollars), per programma, in de afgelopen 12 maanden.

### <a name="payments-list"></a>Lijst met betalingen

In de **lijst met betalingen** worden betaalde en openstaande betalingen weer gegeven. U kunt BTW-gegevens voor service kosten downloaden in PDF-indeling en de details van het verdienen van een bepaalde betaling bekijken.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Illustreert het uitbetalings pictogram in de rechter bovenhoek van de Partner Center-Portal":::

- **Betaald** : alle betalingen zijn verzonden. Kies het jaar in de vervolg keuzelijst om te filteren op de betalingen die in dat jaar zijn uitgebracht.
- **In behandeling** : toekomstige betalingen.
- **Belasting service kosten (PDF-formulier)** : beschikbaar voor de betalingen die zijn onderhevig aan belasting van service kosten. Belastingen voor service kosten worden in **andere belastingen** weer gegeven.
- **Weer geven** : omleiden naar de transactie geschiedenis met een lijst van de inkomsten die in de betaling zijn opgenomen.

Zie [Veelgestelde vragen over uitbetalingen door commerciële Marketplace](payout-faq.md#why-are-my-earnings-missing)als u wilt weten waarom er sprake is van ontbrekende of onverwachte inkomsten.

### <a name="payment-status"></a>Betalingsstatus

In de volgende tabel worden de verschillende statussen voor het verdienen beschreven.

| Status verdienen | Reden | Partner actie vereist? |
| --- | --- | --- |
| Verwerkte | Het verdienen komt in aanmerking voor betaling. Deze status blijft van toepassing op een koel periode zoals gedefinieerd in de programma gids voor het programma prikkel. | Nee |
| Verschijnen | De betalings order is gegenereerd interne beoordelingen voordat de betaling wordt verwerkt. | Nee |
| Factuur met openstaande BTW | Uw belasting factuur is onvolledig of ongeldig. | U moet uw BTW-factuur bijwerken voordat u kunt betalen |
| Afgewezen tijdens beoordeling | De betaling is tijdens de controle afgewezen. | Neem contact op met micro soft ondersteuning voor meer informatie |
| Mislukt | De betaling is mislukt vanwege een micro soft-systeem fout. | Neem contact op met micro soft ondersteuning voor meer informatie |
| Actief | De betaling wordt uitgevoerd. | Nee |
| Onjuiste betaling | Het terugkoppelings bedrag wordt uitgevoerd. | Nee |
| Verzonden | De betaling is naar uw bank verzonden. | Nee |
| Verwerkt | De betaling heeft een micro soft-systeem fout aangetroffen en wordt opnieuw verwerkt. | Nee |
| Reversed | De betaling is teruggestort door uw bank en wordt opnieuw verzonden in de volgende betalings cyclus. | Nee |
| Geweigerde BTW-factuur | Uw belasting factuur is afgewezen tijdens de controle. Alle openstaande betalingen worden in de wacht stand gezet totdat de beoordeling van de belasting factuur is voltooid. | Neem contact op met micro soft ondersteuning voor meer informatie |
| Factuur belasting onder beoordeling | Uw belasting factuur wordt gecontroleerd. Uw betaling wordt vrijgegeven zodra de belasting factuur is goedgekeurd. | Nee |
| Afgewezen | De betaling is door uw bank afgewezen. | Neem contact op met uw bank voor meer informatie. |
|

### <a name="payments-download"></a>Betalingen downloaden

Klik boven aan de pagina op **downloaden** om meer informatie over uw betalingen weer te geven. In de volgende tabel wordt elke kolom in het rapport uitgelegd.

| Kolomnaam | Description |
| --- | --- |
| participantID | De primaire identiteit van de partner die onder het programma is aangegaan |
| participantIDType | Doorgaans programma-ID voor prikkel Programma's en verkoper-ID voor Store-Program ma's |
| deel nemer | Naam van de verdienen partner |
| programName | Naam stimulans/archief programma |
| ontvangt | Het bedrag dat is verdiend in de factuur voor dat programma-participantID |
| earnedUSD | De hoeveelheid die is behaald voor de programma/deel nemer-ID, in EUR |
| withheldTax | De hoeveelheid belasting die is inge houden in de factuur voor het programma-participantID |
| Omzet | Totale omzet belasting in de valuta voor het programma-participantID (alleen van toepassing op prikkelings Programma's) |
| serviceFeeTax | Totale hoeveelheid serviceFeeTax in betalen aan valuta voor het programma/participantID (alleen van toepassing op Store-Program ma's en Azure Marketplace) |
| totalPayment | Totale betaling in lokale valuta met uitzonde ring van de bron belasting en inclusief de BTW (indien van toepassing) voor het programma-participantID |
| currencyCode | Betalen naar valuta code |
| paymentMethod | De methode die wordt gebruikt om de partner te betalen, bijvoorbeeld elektronische bank overschrijving, credit nota |
| paymentID | De unieke id voor de betaling. Dit nummer is doorgaans zichtbaar in uw bank overzicht (alleen van toepassing op SAP-betalingen). |
| paymentStatus | Betalingsstatus |
| paymentStatusDescription | Beschrijvende beschrijving van de betalings status |
| paymentDate | De datum waarop de betaling is verzonden van micro soft |
|

## <a name="export-data"></a>Gegevens exporteren

De pagina **gegevens exporteren** wordt niet automatisch vernieuwd. Mogelijk moet u de pagina hand matig vernieuwen om de meest recente gegevens te zien. Selecteer op de drie tabbladen een **transactie geschiedenis** , **betalingen** , **transactie overzicht** of **historische instructie** exporteren.

Het filter kan ertoe leiden dat er **geen gegevens beschikbaar zijn** . Dit kan gebeuren als u de standaard periode van drie maanden hebt geselecteerd en vervolgens een betalings-ID hebt geselecteerd van een verdienen dat buiten die periode valt. Als dit het geval is, vouwt u uw tijds periode uit en probeert u het opnieuw.

Hier volgt een voor beeld van een export van een betaling:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Illustreert het uitbetalings pictogram in de rechter bovenhoek van de Partner Center-Portal":::

### <a name="historical-statements"></a>Historische instructies

De samen vatting **export gegevens** biedt ook toegang tot historische instructies.

> [!NOTE]
> Een historische instructie is een moment opname en wordt niet vernieuwd. Neem contact op met de [ondersteuning](https://partner.microsoft.com/support/v2/?stage=1) en vraag zo nodig de meest recente gegevens aan.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Illustreert het uitbetalings pictogram in de rechter bovenhoek van de Partner Center-Portal":::

- De transactie geschiedenis van vóór 1 juli 2019 wordt afzonderlijk verwerkt en maakt gebruik van verschillende velden uit latere geschiedenis rapporten.
- De verouderde transactie geschiedenis bevat een kolom met de naam ' gereserveerd ' die overeenkomt met de kolom ' winst ' in de moderne geschiedenis, behalve dat alle inkomsten met een status gelijk aan ' betaling verzonden ' worden uitgesloten.
- Filters zoals 3 ter, 6 min. of 12M zijn niet van toepassing op de sectie historische instructies.

### <a name="historical-statement-downloads"></a>Historische instructie downloads

In de volgende tabel wordt elke kolom in een historische instructie uitgelegd.

| Veldnaam | Beschrijving |
| --- | --- |
| Opbrengst bron | De bron van uw omzet op basis van waar de trans actie plaatsvond, zoals Microsoft Store, Windows Phone Store, Windows Store 8 of Advertising |
| Order-id | Unieke order-id. Met deze ID kunt u aankoop transacties identificeren met hun respectieve niet-aankoop transacties, zoals terugstortingen of terugstortingen. Beide hebben dezelfde order-ID. Als er sprake is van een splits kosten waarbij meerdere betalings wijzen voor één aankoop zijn gebruikt, kunt u hiermee de inkoop transacties koppelen. |
| Transactie-id | Unieke trans actie-id. |
| Datum en tijd van trans actie | De datum en tijd waarop de trans actie is opgetreden (UTC). |
| ID van bovenliggend product | Unieke id van het bovenliggende product. Als er geen bovenliggend product voor de trans actie is, dan is de product-id van de bovenliggende product-id. |
| Product-id | Unieke product-id. |
| Naam van bovenliggend product | De naam van het bovenliggende product. Als er geen bovenliggend product voor de trans actie is, dan is de naam van het bovenliggende product = product naam. |
| Productnaam | Naam van het product |
| Producttype | Type product, zoals app, invoeg toepassing of spel |
| Aantal | Wanneer de opbrengst bron Microsoft Store voor bedrijven, vertegenwoordigt de hoeveelheid het aantal aangeschafte licenties. Voor alle andere opbrengst bronnen is de hoeveelheid altijd 1. Zelfs wanneer één trans actie wordt gesplitst in twee regel items omdat er twee verschillende betalings methoden zijn gebruikt, wordt voor elk regel item een hoeveelheid van 1 weer gegeven. |
| Transactietype | Type trans actie, zoals aankoop, terugbetaling, omkering of terugstorting |
| Betalings wijze | Het betalings instrument van de klant dat wordt gebruikt voor de trans actie, zoals kaart, facturering van mobiele provider of PayPal |
| Land/regio | Het land of de regio waar de trans actie plaatsvond |
| Lokale provider/verkoper | Lokale provider/verkoper van record |
| Transactie valuta | Valuta van de trans actie |
| Transactie bedrag | Bedrag van de trans actie |
| Geremitteerde BTW | Bedrag van overgeschreven BTW (verkoop, gebruik of btw/GST-belastingen) |
| Netto-ontvangst bewijzen | Transactie bedrag verminderd met teruggeschreven BTW |
| Winkel kosten | Het percentage netto-ontvangst bewijzen dat door micro soft wordt bewaard als een vergoeding voor het maken van de app of invoeg toepassing die beschikbaar is in de Store |
| App-opbrengsten | Netto-ontvangsten min de winkel kosten |
| Inge houden belastingen | Inge houden inkomsten belasting (gerekend in **gereserveerde** CSV-bestand) |
| Betaling | De app verloopt over minder toepasselijke inhoudingen voor inkomsten belasting (bedrag weer gegeven in transactie valuta). Niet opgenomen in het **gereserveerde** CSV-bestand. |
| FX-tarieven | Wissel koers die wordt gebruikt om transactie valuta om te zetten in de betalings valuta |
| Betalingsvaluta | De valuta waarin uw betaling is gedaan |
| Omgezette betaling | Bedrag van betaling dat is omgezet in de betalings valuta met het FX-percentage |
| Model voor belasting remise | Partij verantwoordelijk voor het remitteren van belastingen (verkoop, gebruik of btw/GST-belastingen) |
| Datum en tijd van geschiktheid | De datum en tijd waarop trans actie-opbrengsten in aanmerking komen voor uitbetaling (UTC). Wanneer er een uitbetaling wordt gemaakt, omvat deze trans actie-opbrengst met een datum/tijd van de geschiktheid vóór de aanmaak datum van de betaling (alleen opgenomen in het **gereserveerde** CSV-bestand). |
| Kosten | Toont een uitsplitsing van alle kosten details die zijn samengevoegd in de kolom transactie bedrag (alleen opgenomen voor Azure Marketplace, niet opgenomen in het **gereserveerde** CSV-bestand). |
|||

## <a name="next-steps"></a>Volgende stappen

- [API voor uitbetaling van partners](https://apidocs.microsoft.com/services/partnerpayouts)
- [Details van betaalbeleid](payout-policy-details.md)
- Neem contact op met de ondersteuning voor commerciële Marketplace- [Uitgever](https://partner.microsoft.com/support/v2/?stage=1)voor ondersteuning bij facturering.