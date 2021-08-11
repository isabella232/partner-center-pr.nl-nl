---
title: Uitbetalingsinstructies
description: Meer informatie over uitbetalingsverklaringen en samenvattingen, en hoe u uw betalingsgegevens kunt weergeven en exporteren vanuit Microsoft Partner Center
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: 8ad648d7ff7c5360ae61897ea98a633532ffd4c7de65ffa6b83984996ca24ac6
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115693375"
---
# <a name="payout-statements"></a>Uitbetalingsinstructies

**Juiste rollen:** Accountbeheerder | Globale beheerder

Het **uitbetalingsoverzicht** geeft een overzicht van uw uitbetalingen van aanbiedingen die via de commerciële marketplace worden verkocht. Het toont de transactionele geschiedenis van uw inkomsten, maakt een schatting van uw volgende betaling en toont betalingstrends. U kunt ook de transactiegeschiedenis en betalingsverklaringen downloaden. In dit artikel wordt uitgelegd hoe u toegang krijgt tot uw uitbetalingsoverzicht en de verschillende uitbetalingspagina's en downloads die voor u toegankelijk zijn in Partner Center.

>[!NOTE]
>U ziet alleen gegevens voor MPN-ID's en programma's die u hebt gekoppeld. Als u aanvullende gegevens wilt zien, moet u contact op nemen met de accountbeheerder voor machtigingen. 

## <a name="roles-and-permissions"></a>Rollen en machtigingen

Als u toegang wilt krijgen tot een uitbetalingsoverzicht, moet aan u de rol **Accounteigenaar of** Financieel **inzender zijn** toegewezen.

| Rapporten/pagina's | Accounteigenaar | Manager | Ontwikkelaar | Zakelijke inzender | Inzender voor financiën | Marketeer |
| --- | --- | --- | --- | --- | --- | --- |
| Overnamerapport (inclusief bijna realtime gegevens) | Kan weergeven | Kan weergeven | Geen toegang | Geen toegang | Kan weergeven | Geen toegang |
| Feedbackrapport/-antwoorden | Kan feedback weergeven en verzenden | Kan feedback weergeven en verzenden | Kan feedback weergeven en verzenden | Geen toegang | Geen toegang | Kan feedback weergeven en verzenden |
| Statusrapport (inclusief bijna realtime gegevens) | Kan weergeven | Kan weergeven | Kan weergeven | Kan weergeven | Geen toegang | Geen toegang |
| Gebruiksrapport | Kan weergeven | Kan weergeven | Kan weergeven | Kan weergeven | Geen toegang | Geen toegang |
| Uitbetalingsaccount | Kan worden bijgewerkt | Geen toegang | Geen toegang | Geen toegang | Kan worden bijgewerkt | Geen toegang |
| Belastingprofiel | Kan worden bijgewerkt | Geen toegang | Geen toegang | Geen toegang | Kan worden bijgewerkt | Geen toegang |
| Betalingsoverzicht | Kan weergeven | Geen toegang | Geen toegang | Geen toegang | Kan weergeven | Geen toegang |
|

## <a name="access-your-payout-statement"></a>Toegang tot uw uitbetalingsoverzicht

Meld u aan [Partner Center](https://partner.microsoft.com/dashboard/home) en selecteer het uitbetalingspictogram in de rechterbovenhoek van het scherm om toegang te krijgen tot deze verschillende samenvattingen:

- Transactiegeschiedenis
- Betalingen
- Gegevens exporteren

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Illustreert het uitbetalingspictogram in de rechterbovenhoek van Partner Center portal.":::

U kunt ook de Api voor [uitbetaling van partners gebruiken om](/rest/api/partner-center/partner-payouts) rechtstreeks verbinding te maken en uitbetalingstransactie- en betalingsgegevens te verkrijgen. Meer informatie in [Uitbetalingen beheren met behulp van de Uitbetalingsservice-API.](/partner-center/develop/manage-payouts)


## <a name="transaction-history"></a>Transactiegeschiedenis

Op **de pagina Transactiegeschiedenis** ziet u een overzicht van uw inkomsten, de geschatte volgende betaling en de trend in uw inkomsten en betalingen in de afgelopen 36 maanden. U kunt ook transactiedetails downloaden uit deze sectie.<br><br>Dit rapport bevat alle inkomsten die in aanmerking komen voor uitbetaling, inclusief betalingen die nog niet zijn verzonden. Inkomsten komen in aanmerking voor uitbetaling wanneer een ISV alle bank- en belastinggegevens in Partner Center heeft voltooid, >$ 50 heeft verdiend, het ISV-account actief is en de klant is gefactureerd (voor EA-transacties) of de betaling is ontvangen (voor niet-EA-transacties).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Transactieoverzicht.":::

- **Inkomsten die dit jaar worden verzonden:** totale inkomsten en uitsplitsing van de inkomsten die zijn betaald en die in de komende maand worden betaald.
- **Geschatte betalingsmaand:** de totale inkomsten worden in de komende maanden verwacht.
- **Inkomsten- en betalingstrend:** maandelijkse inkomsten en betalingsbedragen voor de afgelopen 36 maanden.
- **Downloaden:** transactiedetails downloaden in .csv of TSV-indeling.

Gebruik de selectie voor het datumbereik in de rechterbovenhoek van de pagina om de uitvoer van de pagina te filteren om de afgelopen 3, 6, 12 of 36 maanden weer te geven. U kunt ook een aangepast datumbereik van maximaal 36 maanden selecteren. Het standaarddatumbereik is 12 maanden. U kunt ook filteren op inschrijvings-id, programma, betalings-id, inkomstentype, lever en status. Gegevens zijn beschikbaar voor het huidige boekjaar (1 juli - 30 juni) en de vorige twee boekjaren.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Het zoekfilter rechtsboven op de pagina.":::

Als u meer informatie over een inkomsten wilt bekijken, selecteert u de pijl-omlaag aan de rechterkant van de pagina. Als u dit doet, worden de lever, de omzet, het product en de klant weergegeven. Als een van deze gegevens om de een of andere reden niet beschikbaar is, maar u er wel toegang tot nodig hebt, neem dan contact op met de ondersteuning. Als de inkomsten het resultaat zijn van een aanpassing en niet van een transactie, worden de velden Product en Customer niet weergegeven.

### <a name="transaction-history-summary"></a>Overzicht van transactiegeschiedenis

In deze weergave worden de inkomstendetails, waaronder de oorsprong van de inkomsten van het verkochte product, de inkomstendatum, de status en de geschatte betalingsmaand.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Transactiegeschiedenis.":::

- **Verdiend:** de aankoopdatum.
- **Inkomstentype:** het type inkomsten, zoals Verkopen, Huis of Co-op.
- **Totaal bedrag:** het netto-inkomstenbedrag. In de commerciële marketplace betekent dit dat de standaardkosten voor Marketplace in rekening zijn gebracht.
- **Status:** heeft drie opties:
    - **Aankomende** – inkomsten zijn in de verkoelingsperiode in behandeling.
    - **Verwerkt:** inkomsten worden voorbereid voor de volgende betaling.
    - **Verzonden:** inkomsten zijn betaald.
- **Geschatte betalingsmaand:** de maand dat de inkomsten naar verwachting worden betaald. Zie de [volgende sectie](#estimated-payment-month) voor meer informatie.

Inkomstentransacties worden weergegeven zodra de transactie voldoet aan de uitbetalingsvereisten. Zie Veelvoorkomende vragen over uitbetalingen op de commerciële marketplace om te begrijpen waarom er mogelijk inkomsten ontbreken [of onverwacht zijn.](payout-faq.yml#why-are-my-earnings-missing-)

#### <a name="estimated-payment-month"></a>Geschatte betalingsmaand

De pagina Transactiegeschiedenis bevat nu een tabel met de geschatte betalingsbedragen voor de komende maanden. U kunt deze informatie ook bekijken en downloaden in de export van het transactiegeschiedenis- en samenvattingsrapport. Deze informatie maakt afstemming en betalingsprognoses eenvoudiger.

De Geschatte betalingsmaand wordt berekend op basis van programmaconfiguratieregels en tijdlijnen en wordt verwerkt in de volgende/toekomstige betalingscyclus.

Geschatte betalingsmaand is momenteel beschikbaar voor alle inkomstentypen, met uitzondering van co-op, die wordt weergegeven **als Niet van toepassing.** Voor inkomsten vóór 1 juli 2020 wordt de Geschatte betalingsmaand weergegeven **als Niet beschikbaar.**

In de volgende tabel ziet u een voorbeeld van een geschatte betalingsmaand.

| Maand | Bedrag |
| ------ | :-----------: |
|  Sep-2020 |  $ 7.273,99   |
|  Okt-2020 | $ 8.692,30  |
|  November 2020 | $ 107,89  |

Het geschatte bedrag kan om verschillende redenen verschillen van het werkelijke bedrag:

- Herberekening van inkomsten: Als de inkomsten opnieuw worden berekend, is het werkelijke bedrag anders
- Aanpassingen: het werkelijke bedrag is afhankelijk van de aanpassingen die zijn opgetreden of zijn ingediend.
- Wijziging van regels: Een wijziging in regels kan een weerspiegeling zijn van herberekening in het werkelijke betaalde bedrag
- Crediteuren: Als er een betalingsfout optreedt, kan het werkelijke bedrag verschillen

Houd er rekening mee dat uw betaling alleen wordt vrijgegeven in de verwachte maand als aan de drempelwaarde van uw programma en aan de regels voor betalingsgemiddelden wordt voldaan. Deze regels omvatten, maar zijn niet beperkt tot de onderstaande lijst:

- Uw belastingprofiel moet up-to-date zijn
- Uw inkomsten moeten voldoen aan of de drempelwaarde voor minimale inkomsten overschrijden die is gedefinieerd in uw programmahandleiding.
- Uitbetaling in de wachtstand: als u de optie 'Mijn betaling in de wacht houden' selecteert op de profieltoewijzingspagina.
- Betaalmiddel niet beschikbaar: Het betalings- of belastingprofiel is niet voltooid.

### <a name="transaction-history-download"></a>Transactiegeschiedenis downloaden

Als u meer informatie wilt over inkomsten, selecteert **u Downloaden** bovenaan de pagina. In de volgende tabel wordt elke kolom in het rapport uitgelegd.

>[!NOTE]
>De downloadexport transactiegeschiedenis heeft vanaf augustus 2020 twee nieuwe velden:
>
>- **lastPaymentCurrency**  De valuta waarin de meest recente betaling is ontvangen, voor alle MPN's waarvoor de partner die momenteel is aangemeld, toegang heeft. Als er geen betaling wordt ontvangen, is de laatste betalingsvaluta Amerikaanse dollars.
>- **earningAmountInLastPaymentCurrency**  Het inkomstenbedrag in de laatste betalingsvaluta.

| Kolomnaam | Beschrijving | Toepasbaarheid voor incentive-programma's/marketplaces |
| --- | --- | --- |
| agreementEndDate | Einddatum overeenkomst | Incentives: alleen voor sommige programma's |
| agreementNumber | Overeenkomstnummer | Incentives: alleen voor sommige programma's |
| agreementStartDate | Begindatum overeenkomst | Incentives: alleen voor sommige programma's |
| calculationDate | Datum waarop de inkomsten zijn berekend in het systeem | Alles |
| claimId | Unieke id voor claim | Incentives: alleen voor sommige programma's |
| customerCountry | Land/regio van de klant | Markten |
| customerEmail |  |  |
| customerName | Mag leeg zijn | Alleen Incentive-programma's (uitzondering: OEM) en marketplaces. Voor CSP-transacties geven marketplaces de naam van de CSP weer |
| customerTenantId |  |  |
| distributorId | Distributor-id | Incentives: alleen voor sommige programma's |
| distributorName | Naam van distributeur | Incentives: alleen voor sommige programma's |
| earningAmount | Inkomstenbedrag in de oorspronkelijke transactievaluta | Alles |
| earningAmountInLastPaymentCurrency | Inkomstenbedrag in de laatste betalingsvaluta (veld is leeg als er geen eerdere betalingen zijn betaald) |  |
| earningAmountUSD | Inkomstenbedrag in USD | Alles |
| earningDate | Datum van de inkomsten | Alles |
| earningExchangeRate | Exchange die wordt gebruikt om het bijbehorende bedrag in USD weer te geven | Alles |
| earningId | Unieke id voor elke inkomstendering | Alles |
| earningRate | Incentives-tarief toegepast op transactiebedrag om inkomsten te genereren | Alles |
| earningType | Geeft aan of het gaat om kosten, voertuigen, samenwerking, verkoop, en meer | Alles |
| exchangeRateDate | Exchange voor het berekenen van het inkomstenbedrag USD | Alles |
| externalReferenceId | Unieke id voor het programma | Direct Pay-programma's (incentives en marketplaces) |
| externalReferenceIdLabel | Uniek id-label | Direct Pay-programma's (incentives en marketplaces) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Factuurnummer (alleen van toepassing voor ondernemingen) | Incentives en marketplaces: alleen voor sommige programma's |
| lastPaymentCurrency | Laatste betalingsvaluta (veld is leeg als er geen eerdere betaling is betaald) |  |
| hendel | Hiermee wordt de bedrijfsregel voor de inkomsten aangegeven | Alles |
| LicensingProgramName | Naam van het licentieprogramma |  |
| LineItemId | Afzonderlijke regel in de factuur van een klant |  |
| localProviderSeller | Lokale provider/verkoper van record |  |
| Vervaldatummaand | De geschatte betalingsmaand | Alles |
| OrderId | Is gerelateerd aan de factuur van een klant  | Markten |
| parentProductId | Unieke bovenliggende product-id. Als er geen bovenliggend product voor de transactie is, wordt bovenliggend product-id = product-id. | Markten |
| parentProductName | Naam van het bovenliggende product. Als er geen bovenliggend product voor de transactie is, gebruikt u Bovenliggende productnaam = Productnaam. | Markten |
| participantId | De primaire identiteit van de partner die in het programma verdient | Alles |
| participantIdType | Voornamelijk programma-id voor incentive-programma's en Verkoper-IF voor marketplaces | Alles |
| participantName | Naam van de inkomstenpartner | Alles |
| partnerCountryCode | Locatie/land/regio van de inkomstenpartner | Alles |
| partNumber | Is altijd leeg | Sommige incentive-programma's en marketplaces |
| paymentId | Unieke id om alle transacties in het transactierapport te correleren met een specifieke betaling in het betalingsrapport | Alles |
| paymentStatus | Betalingsstatus | Alles |
| paymentStatusDescription | Beschrijvende beschrijving van de betalingsstatus | Alles |
| productId | Unieke product-id | Markten |
| Productnaam | Productnaam die is gekoppeld aan de transactie | Alles |
| productType | Type product, zoals App, Invoeg-on of Game | Markten |
| Programmacode | Tekenreeks die moet worden weergegeven met de programmanaam |  |
| programName | Naam incentive-/winkelprogramma | Alles |
| purchaseOrderCoverageEndDate | Is altijd leeg | Incentive-programma - CRI |
| purchaseOrderCoverageStartDate | Is altijd leeg | Incentive-programma - CRI |
| purchaseOrderType | Is altijd leeg | Incentive-programma - CRI |
| purchaseTypeCode | Is altijd leeg | Incentive-programma - CRI |
| quantity | Varieert op basis van het programma. Geeft de gefactureerde hoeveelheid voor transactionele programma's aan | Alles |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Reseller-id | Incentives: alleen sommige programma's |
| resellerName | Reseller name |  |
| SkuId | SKU-id zoals gedefinieerd tijdens het publiceren. Een aanbieding kan veel SKU's hebben, maar een SKU kan slechts aan één aanbieding worden gekoppeld. Incentives: alleen sommige programma's |  |
| storeFee | Het bedrag dat door Microsoft wordt bewaard als kosten voor het beschikbaar maken van de app of invoeg-app in de Store | Markten |
| subscriptionEndDate | Einddatum van abonnement | Incentives: alleen sommige programma's |
| subscriptionId | Abonnements-id die is gekoppeld aan de klant | Incentives: alleen sommige programma's |
| subscriptionStartDate | Begindatum van abonnement | Incentives: alleen sommige programma's |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Partij die verantwoordelijk is voor het betalen van belastingen (verkoop, gebruik of btw-/GST-belastingen) | Markten |
| taxRemitted | Bedrag van de belasting die wordt terugverkend (verkoop, gebruik of btw-/GST-belastingen) | Markten |
| taxState | Status van de klant |  |
| taxZipCode | Postcode van klant |  |
| tpan | Geeft het ad-netwerk van derden aan | marketplaces Ads |
| transactionAmount | Transactiebedrag in de oorspronkelijke transactievaluta op basis waarvan inkomsten worden gegenereerd | Alles |
| transactionAmountUSD | Transactiebedrag in USD | Alles |
| transactionCountryCode | Land-/regiocode waarin de transactie is gebeurd |  |
| transactionCurrency | Valuta waarin de oorspronkelijke klanttransactie heeft plaatsgevonden (dit is geen partnerlocatievaluta) | Alles |
| transactionDate | De datum van de transactie. Handig voor programma's waarbij veel transacties bijdragen aan één inkomsten | Alles |
| transactionExchangeRate | Exchange die wordt gebruikt om het bijbehorende transactiebedrag in USD weer te geven | Alles |
| transactionId | Unieke id voor de transactie | Alles |
| transactionPaymentMethod | Betaalmiddel van de klant dat wordt gebruikt voor de transactie, zoals creditcard, facturering van mobiele provider of PayPal | Markten |
| transactionType | Type transactie, zoals aankoop, restitutie, betaling of terugboeking | Markten |
| workload | Workload | Incentives: alleen sommige programma's |
|

### <a name="transaction-adjustment-codes"></a>Transactiecorrectiecodes

De volgende tabel bevat de redencodes voor aanpassingen en de bijbehorende beschrijvingen.

|**Redencode**   |**Beschrijving**   |
|------------------|:-------------------------------------|
| AR-naleving | Aanpassing die de inkomsten verlaagt wanneer Microsoft-facturen niet op tijd worden betaald door de partner. |
| Co-op rollover | Aanpassing die co-op-inkomsten overboekt naar een andere periode, of co-op-inkomsten converteert naar inkomsten. |
| Aanpassing van ops | Aanpassing die fouten in microsoft-systeemberekeningen corrigeert. |
| Ops-aanpassing Microsoft onjuiste berekening | Aanpassing die onjuiste berekening corrigeert. |
| Ops Adjustment Microsoft incorrect enrollment | Aanpassing voor onjuiste enrollment-gerelateerde berekeningen. |
| Partnertoewijzing (abonnement) MCI/CSP | Aanpassing die onjuiste uitlijning van abonnement corrigeert. |
| Beleids uitzondering | Aanpassing die een programmaregel overschrijven.  |
| Inkomsten uit de vorige periode | Aanpassing voor inkomsten buiten de huidige inkomstenperiode. |

## <a name="payments"></a>Betalingen

Op **de** pagina Betalingen vindt u informatie over het geld dat u hebt verdiend met Microsoft. U ziet ook wanneer en hoeveel u moet betalen.

>[!Note]
> Als u in aanmerking wilt komen voor uitbetaling, moet uw omzet de [betalingsdrempel](payment-thresholds-methods-timeframes.md) van $ 50 bereiken. Zie de Microsoft Publisher [overeenkomst voor meer informatie.](/legal/marketplace/msft-publisher-agreement)

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Scherm Overzicht van betalingen.":::

- **Totaal betaald dit jaar:** het gecombineerde totaal dat u dit jaar hebt betaald, in Amerikaanse dollars, voor al uw programma's.
- **Volgende geschatte betaling:** de eerstvolgende betaling (zelfs als er binnenkort andere zijn), in Amerikaanse dollars.
- **Laatste betaling:** het bedrag (in Amerikaanse dollars), de programmanaam en het programma van uw meest recente betaling.
- **Betaling per bron:** het bedrag aan betalingen (in Amerikaanse dollars) per programma in de afgelopen 12 maanden.

### <a name="payments-list"></a>Lijst met betalingen

In **de tabel Lijst met betalingen** worden betaalde en in behandeling zijnde betalingen weergegeven. U kunt belastinggegevens voor servicekosten downloaden in PDF-indeling en de inkomstengegevens voor een bepaalde betaling bekijken.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Transactiegeschiedenis exporteren.":::

- **Betaald:** alle betalingen zijn verzonden. Kies het jaar in de vervolgkeuzelijst om te filteren op de betalingen die in dat jaar zijn uitgebracht.
- **In behandeling:** toekomstige betalingen.
- **Servicekostenbelasting (PDF-formulier)** : beschikbaar voor de betalingen die zijn onderworpen aan servicekostenbelasting. Servicekostenbelastingen worden weergegeven in **Andere belastingen.**
- **Weergave:** wordt omgeleid naar de transactiegeschiedenis met een lijst met inkomsten die zijn opgenomen in de betaling.

Zie Veelvoorkomende vragen over uitbetalingen op de commerciële marketplace om te begrijpen waarom er mogelijk inkomsten ontbreken of onverwacht [zijn.](payout-faq.yml#why-are-my-earnings-missing-)

### <a name="payment-status"></a>Betalingsstatus

In de volgende tabel worden de verschillende inkomstenstatussen uitgelegd.

| Inkomstenstatus | Reden | Actie van partner vereist? |
| --- | --- | --- |
| Onverwerkte | De inkomsten komen in aanmerking voor betaling. Deze blijft in deze status voor een koelperiode zoals gedefinieerd in de programmahandleiding voor de Incentives-programma. | No |
| Aankomend | Gegenereerde betalingsorder in behandeling interne beoordelingen voordat de betaling wordt verwerkt. | No |
| Belastingfactuur in behandeling | Uw btw-factuur is onvolledig of ongeldig. | U moet uw btw-factuur bijwerken voordat u kunt worden betaald |
| Geweigerd tijdens beoordeling | De betaling is geweigerd tijdens de beoordeling. | Neem contact op met Microsoft Ondersteuning voor meer informatie |
| Mislukt | De betaling is mislukt vanwege een systeemfout van Microsoft. | Neem contact op met Microsoft Ondersteuning voor meer informatie |
| Actief | De betaling wordt uitgevoerd. | No |
| Onjuiste betaling | De betaling wordt terugverdiend. | No |
| Verzonden | De betaling is verzonden naar uw bank. | No |
| Opwerking | Bij de betaling is een systeemfout van Microsoft opgetreden en deze wordt opnieuw verwerkt. | No |
| Reversed | De betaling is teruggedraaid door uw bank en wordt opnieuw verzonden in de volgende betalingscyclus. | No |
| Btw-factuur afgewezen | Uw btw-factuur is geweigerd tijdens de beoordeling. Alle in behandeling zijnde betalingen worden in de wacht gezet totdat de controle van de btw-factuur is voltooid. | Neem contact op met Microsoft Ondersteuning voor meer informatie |
| Belastingfactuur wordt beoordeeld | Uw btw-factuur wordt gecontroleerd. Uw betaling wordt vrijgegeven zodra de btw-factuur is goedgekeurd. | No |
| Afgewezen | De betaling is afgewezen door uw bank. | Neem contact op met uw bank voor meer informatie. |
|

### <a name="payments-download"></a>Betalingen downloaden

 In de volgende tabel wordt elke kolom in het rapport uitgelegd. Als u meer informatie over uw betalingen wilt zien, selecteert u **Downloaden** bovenaan de pagina Betalingen.

| Kolomnaam | Beschrijving |
| --- | --- |
| participantID | De primaire identiteit van de partner die in het programma verdient |
| participantIDType | Meestal programma-id voor Incentives-programma's en Verkoper-id voor Store-programma's |
| participantName | Naam van de inkomstenpartner |
| programName | Incentives/store-programmanaam |
| Verdiend | Het bedrag dat is verdiend in de valuta Betalen naar voor dat programma/de deelnemer-id |
| earnedUSD | Bedrag dat is verdiend voor het programma-/deelnemer-id, in USD |
| withheldTax | Bedrag van de belasting ingehouden in de valuta betalen naar voor het programma/participantID |
| salesTax | Totale btw-bedrag in de valuta Betalen naar voor het programma/de participantID (alleen van toepassing op incentives-programma's) |
| serviceFeeTax | Totale hoeveelheid serviceFeeTax in de valuta Betalen naar voor het programma/de participantID (alleen van toepassing op store-programma'Azure Marketplace) |
| totalPayment | Totale betaling in lokale valuta, met uitzondering van de bronbelasting en inclusief de omzetbelasting (indien van toepassing) voor het programma/de deelnemer-id |
| currencyCode | Betalen naar valutacode |
| paymentMethod | De methode die wordt gebruikt om de partner te betalen, bijvoorbeeld elektronische bankoverdracht, kredietnota |
| paymentID | Unieke id voor de betaling. Dit nummer is meestal zichtbaar in uw bankoverzicht (alleen van toepassing op SAP-betalingen). |
| paymentStatus | Betalingsstatus |
| paymentStatusDescription | Beschrijvende beschrijving van de betalingsstatus |
| paymentDate | De datum waarop de betaling is verzonden door Microsoft |
|

## <a name="export-data"></a>Gegevens exporteren

De **pagina Gegevens** exporteren wordt niet zelf vernieuwd. Mogelijk moet u de pagina handmatig vernieuwen om de meest recente gegevens weer te geven. Selecteer een van de drie tabbladen om **transactiegeschiedenis,** **betalingen,** **transactieoverzicht** of historische **instructie te exporteren.**

Uw filter kan resulteren in de **fout Geen gegevens** beschikbaar. Dit kan gebeuren als u de standaardperiode van drie maanden hebt ingeschakeld en vervolgens een betalings-id hebt geselecteerd op basis van een inkomsten die buiten die periode is. Als dit het geval is, vouwt u de periode uit en probeert u het opnieuw.

Hier is een voorbeeldexport van betalingen:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Rapport betalingen exporteren.":::

### <a name="historical-statements"></a>Historische instructies

De **samenvatting Gegevens exporteren** biedt ook toegang tot historische instructies.

> [!NOTE]
> Een historische instructie is een momentopname en wordt niet vernieuwd. Neem contact op [met de](https://partner.microsoft.com/support/v2/?stage=1) ondersteuning en vraag zo nodig de meest recente gegevens aan.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Historische instructies exporteren.":::

- De transactiegeschiedenis van vóór 1 juli 2019 wordt afzonderlijk verwerkt en maakt gebruik van verschillende velden uit latere geschiedenisrapporten.
- Verouderde transactiegeschiedenis heeft een kolom met de naam 'Gereserveerd' die overeenkomt met de kolom 'Inkomsten' in de moderne geschiedenis, behalve dat alle inkomsten met een status die gelijk is aan 'Verzonden betaling' worden uitgesloten.
- Filters zoals 3M, 6M of 12M zijn niet van toepassing op de sectie Historische instructies.

### <a name="historical-statement-downloads"></a>Downloads van historische instructie

In de volgende tabel wordt elke kolom in een historische instructie uitgelegd.

| Veldnaam | Beschrijving |
| --- | --- |
| Bron van omzet | De bron van uw omzet op basis van waar de transactie heeft plaatsgevonden, zoals Microsoft Store, Windows Phone Store, Windows Store 8 of reclame |
| Order-id | Unieke order-id. Met deze id kunt u aankooptransacties identificeren met hun respectieve niet-aankooptransacties, zoals restituties of terugboekingen. Beide hebben dezelfde order-id. Als er splitsingskosten zijn waarbij meerdere betalingswijzen zijn gebruikt voor één aankoop, kunt u de aankooptransacties koppelen. |
| Transactie-id | Unieke transactie-id. |
| Transactiedatum en -tijd | De datum en tijd waarop de transactie is opgetreden (UTC). |
| Bovenliggende product-id | Unieke bovenliggende product-id. Als er geen bovenliggend product voor de transactie is, wordt bovenliggend product-id = product-id. |
| Product-id | Unieke product-id. |
| Bovenliggende productnaam | Naam van het bovenliggende product. Als er geen bovenliggend product voor de transactie is, dan is Bovenliggend productnaam = Productnaam. |
| Productnaam | Naam van het product |
| Producttype | Type product, zoals App, Invoeg-app of Game |
| Aantal | Wanneer de Omzetbron is Microsoft Store voor Bedrijven, vertegenwoordigt De Hoeveelheid het aantal aangeschafte licenties. Voor alle andere omzetbronnen is de Hoeveelheid altijd 1. Zelfs wanneer één transactie wordt gesplitst in twee regelitems omdat er twee verschillende betalingswijzen zijn gebruikt, wordt voor elk regelitem een Hoeveelheid van 1 weer geven. |
| Transactietype | Type transactie, zoals aankoop, restitutie, betaling of terugboeking |
| Betalingsmethode | Betaalmiddel van de klant dat wordt gebruikt voor de transactie, zoals creditcard, facturering van mobiele provider of PayPal |
| Land/regio | Land/regio waar de transactie heeft plaatsgevonden |
| Lokale provider/verkoper | Lokale provider/verkoper van record |
| Transactievaluta | Valuta van de transactie |
| Transactiebedrag | Bedrag van de transactie |
| Btw-belasting is teruggestuurd | Bedrag van de belasting die is teruggestuurd (verkoop, gebruik of BTW/GST-belastingen) |
| Netto-omzet | Transactiebedrag minder belasting overgemaakt |
| Winkelkosten | Het percentage netto-omzet dat door Microsoft wordt bewaard als een vergoeding voor het beschikbaar maken van de app of invoeg-app in de Store |
| App gaat verder | Netto-omzet minus de winkelkosten |
| Belastingen ingetrokken | Ingehouden hoeveelheid inbelasting (ot  opgenomen in het csv-bestand met gereserveerde gegevens) |
| Betaling | De app gaat verder met minder toepasselijke in holding (bedrag dat wordt weergegeven in transactievaluta). Niet opgenomen in **gereserveerd** CSV-bestand. |
| FX-snelheid | Wisselkoers die wordt gebruikt om transactievaluta om te zetten in betalingsvaluta |
| Betalingsvaluta | Valuta waarin uw betaling wordt gedaan |
| Geconverteerde betaling | Betalingsbedrag geconverteerd naar betalingsvaluta met behulp van het FX-tarief |
| Belastingafgiftemodel | Partij die verantwoordelijk is voor het aftrekken van belastingen (verkoop, gebruik of btw/GST-belastingen) |
| Datum/tijd van geschiktheid | De datum en tijd waarop de transactie doorgaat, komen in aanmerking voor uitbetaling (UTC). Wanneer een uitbetaling wordt gemaakt, wordt de transactie verwerkt met een datum/tijd voor geschiktheid vóór de aanmaakdatum van de uitbetaling (alleen opgenomen **in** het csv-bestand met gereserveerde gegevens). |
| Kosten | Geeft een uitsplitsing weer van alle kostendetails die zijn geaggregeerd in de kolom Transactiebedrag (alleen opgenomen voor Azure Marketplace; niet opgenomen in het **gereserveerde** CSV-bestand). |
|||

## <a name="next-steps"></a>Volgende stappen

- [API voor uitbetaling van partners](https://apidocs.microsoft.com/services/partnerpayouts)
- [Details van betaalbeleid](payout-policy-details.md)
- Neem voor factureringsondersteuning contact op met de uitgeversondersteuning [van de commerciële marketplace.](https://partner.microsoft.com/support/v2/?stage=1)
