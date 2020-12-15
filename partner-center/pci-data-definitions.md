---
title: Insights-gegevens definities
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Het document bevat de lijst met verschillende rapporten en de gegevens definities van elk rapport, dat kan worden gedownload via de pagina Insights-Download rapport.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2020
ms.locfileid: "97502127"
---
# <a name="export--data-definitions"></a>Exporteren – gegevens definities 

 **Juiste rollen** 

- Rapport viewer 
- Rapport Viewer Executive 

## <a name="introduction"></a>Inleiding 

Met de hub voor het downloaden van rapporten in het Insights-dash board kunt u de onbewerkte gegevens sets exporteren.  

De verschillende rapporten, die samen met de definitie van de gegevens kunnen worden gedownload, zijn als volgt: 

**Partner profiel**: de gegevens definities van de verschillende velden van het profiel rapport zijn: 


| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|MPNId|Microsoft Partner Network-ID|
|PartnerName|De naam van de partner |
|PGA_MPNId|MPN-ID van partner Global-account|
|PGA_PartnerName|Globale account naam partner|
|Plaats|Locatie van de vestiging van de partner |
|Land/regio|Land locatie van partner |
|HierarchyLevel|Hiermee wordt aangegeven of het een globale MPN-ID of locatie MPN-ID is|

**Klant Details**: de gegevens definities van de verschillende velden van het rapport klant Details zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|CustomerName|Naam van de klant |
|CustomerTenantId|Tenant-id van de klant |
|CustomerTpid|Bovenliggende id van de klant |
|CustomerSegment|Klant segment |
|CustomerMarket|Geografische markt van de klant  |
|CustomerStatus|Klant status (actieve/inactive) |
|Product|Het product dat door de MPN aan de klant wordt verkocht. Dit is een van O365, D365, Enter prise Mobility, Power BI, Microsoft Azure.|
|SKU|   Product-SKU|
|Maand| Maand waarvoor het gebruik en de opbrengst worden gerapporteerd|
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   De naam van de partner|
|Databasenames|   Geografische locatie van de partner|
|PartnerAttributionType|    Type partner toewijzing|
|SalesChannel|  Verkoop kanaal|
|AvailableSeats|    Beschik bare stoelen| 
|RevenueUSD|    Omzet in USD|

**Prestaties wederverkoper**: de gegevens definities van de verschillende velden van de reseller Performance rapporten zijn:

> [!Note]
> Opbrengst-en ACR-gegevens zijn alleen beschikbaar voor gebruikers die een management rapport hebben.

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|ResellerMpnid|ID Microsoft Partner Network wederverkoper| 
|ResellerName|Naam wederverkoper|
|ResellerMarket|Land van wederverkoper van de markt| 
|IndirectProviderMPNId|Id van de indirecte provider Microsoft Partner Network|
|IndirectProviderName|Naam van de indirecte provider|
|Maand|Maand waarvoor het gebruik en de opbrengst worden gerapporteerd|
|Product|Productnaam|
|Abonnements|Abonnement-id|
|AvailableSeats|Aantal beschik bare seats|
|AssignedSeats|Aantal toegewezen stoelen|
|BilledRevenueUSD|Gefactureerde omzet (in $)|
|CustomerName|Naam van de klant| 
|CustomerTPid|Bovenliggende id van de klant| 
|CustomerSegment|Klant segment |
|CustomerMarket|Geografische markt van de klant |
|ResellerStatus|Reseller-status| 

**Details van abonnementen**: de gegevens definities van de verschillende velden van het rapport abonnements Details zijn:

>[!Note]
>Opbrengst-en ACR-gegevens zijn alleen beschikbaar voor gebruikers die een leidinggevende rapport kijkers hebben

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|SubscriptionId|    GUID van het abonnement|
|Subscription| Begin datum van het abonnement|
|SubscriptionEndDate|   Eind datum van het abonnement|
|Subscription State| De status van het abonnement (actief of verloop)|
|Maand| Maand waarvoor het gebruik en de opbrengst worden gerapporteerd|
|IsAutoRenew|   Hiermee wordt aangegeven of het abonnement automatisch wordt verlengd of niet (j/N)|
|CustomerName|  Naam van klant| 
|CustomerTenantId|  Klant-GUID|
|CustomerTpid|  Bovenliggende id van de klant| 
|CustomerSegment|   Markt segment van de klant| 
|CustomerMarket|    Geografische markt van de klant|
|Product|   Product dat door de partner aan de klant wordt verkocht| 
|SKU|   SKU van het product |
|MPNId| Microsoft Partner Network-ID van de partner |
|PartnerName|   De naam van de partner |
|Databasenames|   Geografische locatie van de partner |
|PartnerAttributionType|    Type toewijzing voor het abonnement|
|SalesChannel|  Kanaal van de verkoop (direct/CSP, enz.) |
|AvailableSeats|    Huidige beschik bare seat|
|RevenueUSD|    Omzet in USD|
|Inschrijvings-ID| Inschrijvings-ID van het abonnement|

**Azure-gebruik**: de gegevens definities van de verschillende velden van het Azure-gebruiks rapport zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|SubscriptionId|    GUID van het abonnement|
|Subscription| De begin datum van het abonnement.|
|SubscriptionEndDate|   De datum waarop het abonnement eindigt.|
|Subscription State| Huidige status van het abonnement (open/gesloten/actief/respijt periode)|
|Maand| Datum samengevoegd per maand |
|ServiceName|   De naam van de Azure-service|
|MeterCategory| Naam van de meter categorie|
|UsageUnits|    Het aantal eenheden dat wordt gebruikt tijdens de facturerings cyclus |
|CustomerName|  Naam van de klant |
|CustomerTenantId|  Tenant-ID van klant |
|CustomerTpid|  Bovenliggende ID van de klant |
|CustomerSegment|   Segment van de klant |
|CustomerMarket|    Geografische markt van de klant |
|MPNId  |Microsoft Partner Network ID van de klant |
|PartnerName|   De naam van de partner |
|Databasenames    |Locatie van het geografische land van de partner |
|PartnerAttributionType |Type partner toewijzing|
|SalesChannel|  Kanaal van de verkoop (direct/CSP indirect/CSP direct enzovoort) |
|ACR_USD|   Door Azure verbruikte omzet in USD|
|Inschrijvings-ID| Inschrijvings-ID van het Azure-abonnement|

**Office 365-licentie gebruik**: de gegevens definities van de verschillende velden van het gebruiks rapport van het Office 365-licentie zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|CustomerTenantId|  Tenant-ID van klant| 
|CustomerTpid|  Bovenliggende ID van de klant |
|Workload|  SFB, teams, EXO |
|Maand| Maand waarvoor het gebruik wordt gerapporteerd|
|PaidAvailableUnits|    Aantal betaalde beschik bare eenheden|
|MonthlyActiveUsers|    Aantal maandelijkse actieve gebruikers|
|CustomerName|  Naam van de klant|
|CustomerMarket|    Locatie van het geografische land van de markt van de klant |
|CustomerSegment|   Klant segment |
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   De naam van de partner|
|Databasenames|   Geografische locatie van de partner|
|PartnerAttributionType|    Type partner toewijzing|

**Enter prise Mobility – licentie gebruik**: de gegevens definitie van de verschillende velden in het gebruiks rapport van EMS-licentie zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|CustomerTenantId|  Tenant-ID van klant| 
|CustomerTpid|  Bovenliggende ID van de klant |
|Workload|  Naam van de EMS-workload |
|Maand| Maand waarvoor het gebruik wordt gerapporteerd|
|PaidAvailableUnits|    Aantal betaalde beschik bare eenheden|
|MonthlyActiveUsers|    Aantal maandelijkse actieve gebruikers|
|CustomerName|  Naam van de klant|
|CustomerMarket|Locatie van het geografische land van de markt van de klant |
|CustomerSegment|   Klant segment |
|MPNId| Microsoft Partner Network-ID|
|PartnerName|   De naam van de partner|
|Databasenames|   Geografische locatie van de partner|
|PartnerAttributionType|    Type partner toewijzing|

**Dynamics 365 – licentie gebruik**: de gegevens definitie van de verschillende velden van het Dynamics 365 – gebruiks rapport voor licenties zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|SubscriptionId|GUID van het abonnement|
|Subscription| Begin datum van het abonnement|
|SubscriptionEndDate|   Eind datum van het abonnement|
|SubscriptionStatus|    Status van het abonnement |
|Maand| Maand waarvoor het gebruik wordt gerapporteerd|
|RevSumDivisionName|    Naam van de verdeling van de Rev-som|
|RevSumCategoryName|    Naam van de categorie voor de opbrengst som|
|SKU|   SKU van het product |
|SKUId| SKU-ID van het product |
|FreeVsPaidSKU| Hiermee wordt aangegeven of het een gratis of betaalde SKU is |
|SalesModel|    Verkoop kanaal dat wordt gebruikt voor het verkopen van het abonnement|
|DetailedSalesModel|    Gedetailleerd verkoop model voor het abonnement|
|CustomerName|  Naam van klant |
|CustomerTenantId|  Tenant-GUID van klant |
|CustomerTpid|  Bovenliggende id van de klant |
|CustomerSegment|   Markt segment van de klant |
|CustomerMarket|    Geografische markt van de klant |
|MPNId| Netwerk-ID van micro soft-partner |
|PartnerName|   De naam van de partner |
|Databasenames|   Locatie van het geografische land van de partner |
|PartnerAttachType| Type toewijzing voor het abonnement|
|AvailableSeats|    Huidige beschik bare seat|
|AssignedSeats| Huidige toegewezen seat |
|ActiveSeats|   Huidige actieve stoelen |
|DeploymentOpportunity| Huidige implementatie opportuniteit|
|ActiveUsagePercent|    Huidig actief gebruiks percentage|
 
**Power bi licentie gebruik**: de gegevens definitie van de verschillende velden van het gebruiks rapport van de Power bi-licentie zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|SubscriptionId|    GUID van het abonnement|
|Subscription| Begin datum van het abonnement|
|SubscriptionEndDate|   Eind datum van het abonnement|
|SubscriptionStatus|    Status van het abonnement (actief of In-Active of in de respijt periode)|
|Maand| Datum samengevoegd per maand |
|SKU|   SKU van het product |
|SKUId| SKU-ID van het product |
|FreeVsPaidSKU| Gratis of betaalde SKU onderscheid |
|SalesModel|    Verkoop model dat wordt gebruikt om het abonnement te verkopen|
|DetailedSalesModel|    Gedetailleerd verkoop model voor het abonnement|
|CustomerName|  Naam van klant |
|CustomerTenantId|  Tenant-GUID van klant |
|CustomerTpid|  Bovenliggende id van de klant| 
|CustomerSegment|   Markt segment van de klant |
|CustomerMarket|    Geografische markt van de klant |
|MPNId| Microsoft Partner Network-ID |
|PartnerName|   De naam van de partner |
|Databasenames|   Locatie van het geografische land van de partner |
|PartnerAttachType| Type toewijzing voor het abonnement|
|AvailableSeats|    Huidige beschik bare stoelen|
|AssignedSeats| Huidig toegewezen stoelen|
|ActiveSeats|   Huidige actieve stoelen|
|DeploymentOpportunity| Huidige implementatie opportuniteit|
|ActiveUsagePercent|    Huidig actief gebruiks percentage|

**Gebruik van teams – vergaderingen en aanroepen**: de gegevens definities van de verschillende velden zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|CustomerTenantId|  Tenant-ID van klant |
|CustomerTpid|  Bovenliggende ID van de klant |
|Maand| Maand waarvoor het gebruik wordt gerapporteerd|
|Subbelasting|   Subworkload waarvoor het gebruik wordt gerapporteerd (vergaderingen, aanroepen, telefoon systemen)|
|Aantal vergaderingen| Aantal vergaderingen|
|Duur van vergadering|  Totale duur van de vergadering in uren|

**Teams-maandelijks gebruiks gegevens**: de gegevens definities van de verschillende velden zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|CustomerTenantId|  Tenant-ID van klant |
|CustomerTpid|  Bovenliggende ID van de klant |
|Maand| Maand waarvoor het gebruik wordt gerapporteerd|
|Subbelasting|   Subworkload waarvoor het gebruik wordt gerapporteerd (vergaderingen, aanroepen, telefoon systemen)|
|Bureaublad gebruikers| Aantal gebruikers die teams op het bureau blad gebruiken|
|Mobiele gebruikers|  Aantal gebruikers die teams gebruiken op mobiele apparaten|
|Webgebruikers| Aantal gebruikers die teams op Internet gebruiken|
|AllUpParticipants| Aantal afzonderlijke gebruikers van teams voor de maand|

**Gebruik van teams – 3P apps**: de gegevens definities van de verschillende velden zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|CustomerTenantId|  Tenant-ID van klant| 
|CustomerTpid|  Bovenliggende ID van de klant |
|Maand| Maand waarvoor het gebruik wordt gerapporteerd|
|Naam van de 3P-app|   De naam van de teams-app|
|Aantal gebruikers|    Aantal gebruikers voor de app|


**Cursus Details**: de gegevens definities van de verschillende velden van het rapport met trainings Details zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|TrainingActivityId|    Id van de training |
|TrainingTitle| Titel van de training |
|TrainingType|  Type training (certificering/examen)|
|IndividualFirstName|   Voor naam van de klant| 
|IndividualLastName|    Achternaam van de klant| 
|E-mail| Persoonlijke e-mail-ID van de klant|
|CorpEmail| Office-e-mail-ID van klant|
|TrainingCompletionDate|    Voltooiings datum van de training |
|Maand| Maand waarvoor de gegevens worden gerapporteerd|
|IcMCP| Hiermee wordt aangegeven of de gebruiker een micro soft Certified Professional is|
|MCPID| MCP-ID van de gebruiker|
|MPNId| Microsoft Partner Network-ID |
|PartnerName|   De naam van de partner |
|PartnerCityLocation|   Locatie van de geografische plaats van de partner |
|PartnerCountryLocation|    Locatie van het geografische land van de partner |

**Microsoft Learn**: de gegevens definities van de verschillende velden van het Microsoft Learn rapport zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|UserName|De naam van de gebruiker| 
|UserId|Gebruikers-GUID |
|Opleidingsnaam|De naam van de training |
|TrainingType|Type training (module/Learning pad)|
|Producten|Product waarvoor de leer module van toepassing is|
|Rollen|Toepasselijke rollen van de training |
|CompletionDate|Datum waarop de training is voltooid |
|MPNId|Microsoft Partner Network-ID |
|PartnerName|De naam van de partner |
|Land/regio|Locatie van het geografische land van de partner |

**Competentie overzicht en geschiedenis**: de gegevens definitie van de verschillende velden van het rapport competentie samen vatting en geschiedenis is:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|CompetencyName|Naam van de competentie |
|CompetencyLevel|Niveau van competentie (goud/Silver)|
|CompetencyStatus|Huidige status van competentie (actief/inactief/in respijt periode)|
|CompetencyStartDate|Begin datum van de gegeven competentie| 
|CompetencyEndDate|Eind datum van gegeven competentie |

**Competentie-prestaties**: de gegevens definities van de verschillende velden van het competentie-prestatie rapport zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|CompetencyName|    Naam van de competentie |
|CompetencyAttainmentOptionName|    Naam van de optie competentie-verhoudingen|
|Maand| De maand waarvoor de metrische gegevens worden gerapporteerd|
|MetricName|    De naam van de metrische gegevens die relevant zijn voor de competentie|
|MetricMonthlyContribution| Maandelijkse bijdrage van de metriek|
|TTMAggregate|  Cumulatieve metrische gegevens voor de periode van 12 maanden|
|AnniversaryYearAggregate|  Cumulatieve metrische gegevens voor het huidige jubileum jaar|
|GoldThreshold| Prestatie vereiste om te voldoen aan de Gold-competentie|
|SilverThreshold|   Prestatie vereiste om te voldoen aan de Silver-competentie|

**M365 neiging** in de Cloud: de gegevens definities van de verschillende velden van het M365 neiging-rapport in de Cloud zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|MPN-id|    Microsoft Partner Network-ID|
|Partner naam|  De naam van de partner|
|Klant-ID|   Klant-id-nummer |
|DUNS-nummer|   Het Bradstreet-nummer van de inbel netwerk-& van de klant die wordt beoordeeld op neiging|
|Accountnaam|  Naam van het account |
|Domain|    Domein van het account|
|Grootte van org|  Grootte van organisatie|
|Branche|  Branche  |
|Verticaal|  De verticale van de klant met een score voor neiging, zoals wordt bepaald door micro soft en andere industrie normen (D&B)|
|Gebied|  Geografisch gebied van de locatie|
|Dochteronderneming|    De dochter onderneming van de klant die wordt beoordeeld op neiging|
|Verkoopterritorium|   Het verkoop gebied van de klant met de score voor neiging|
|Plaats|  Locatie van geografische plaats |
|Staat| Locatie van geografische status|
|Postcode|   Postcode|
|Land/regio|   Locatie van geografisch land |
|Segment|   Markt segment |
|Subsegment|   Subsegment op de markt |
|Overzicht van SMC-typen|  SMC-type |
|Top niet-beheerd-Compute base|  Top unmanaged Customers – compute|
|Boven onbeheerd: gebruikers basis| Belangrijkste onbeheerde klanten – gebruiker|
|IsNonProfit|   Of niet-winst of voor winst (Ja/Nee)|
|Externe werk doelen inschakelen voor Exchange Online|   Klanten die een actief Exchange Online-abonnement hebben, verkopen aan M365|
|On-premises aanschaf op afstand inschakelen (huidige versie) met CLAS neiging-+ 10 licenties|Klant die actuele on-premises Office of Win-client heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft 10 of meer licenties. Klant die een neiging score heeft. Partners moeten gericht zijn op conversie naar M365.|
|On-premises aanschaf op afstand inschakelen (huidige versie) met CLAS neiging-<10 licenties|Klant die actuele on-premises Office of Win-client heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft minder dan 10 licenties. Klant die een neiging score heeft. Partners moeten gericht zijn op conversie naar M365.|
|On-premises aanschaf op afstand inschakelen (huidige versie) zonder CLAS neiging-+ 10 licenties| Klant die actuele on-premises Office of Win-client heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft 10 of meer licenties. Klant heeft geen neiging score. Partners moeten gericht zijn op conversie naar M365.|
|On-premises aanschaf op afstand inschakelen (huidige versie) zonder CLAS neiging-<10 licenties| Klant die actuele on-premises Office of Win-client heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft minder dan 10 licenties. Klant heeft geen neiging score. Partners moeten gericht zijn op conversie naar M365.|
|On-premises aanschaf op afstand (EOS) met CLAS neiging-+ 10 licenties inschakelen|Klant die een EOS-on-premises Office-of Win-client heeft (dat wil zeggen, versies die ouder zijn dan en die van de EOS-producten zijn inbegrepen. De klant heeft 10 of meer licenties. De klant heeft een neiging score. Partners moeten gericht zijn op conversie naar M365.|
|On-premises aanschaf op afstand (EOS) inschakelen met CLAS neiging-<10 licenties|Klant die een EOS-on-premises Office-of Win-client heeft (dat wil zeggen, versies die ouder zijn dan en die van de EOS-producten zijn inbegrepen. De klant heeft minder dan 10 licenties. De klant heeft een neiging score. Partners moeten gericht zijn op conversie naar M365.|
|On-premises aanschaf op afstand (EOS) inschakelen zonder CLAS neiging-+ 10-licenties| Klant die actuele on-premises Office of Win-client heeft (dat wil zeggen, versies die ouder zijn dan en met de EOS-producten). De klant heeft 10 of meer licenties. Klant heeft geen neiging score. Partners moeten gericht zijn op conversie naar M365.|
|On-premises aanschaf op afstand (EOS) inschakelen zonder CLAS neiging-<10 licenties| Klant die actuele on-premises Office of Win-client heeft (dat wil zeggen, versies die ouder zijn dan en met de EOS-producten). De klant heeft minder dan 10 licenties. Klant heeft geen neiging score. Partners moeten gericht zijn op conversie naar M365.|
|Extern werk inschakelen-neiging prospect voor M365 (nu handelen/evalueren)| Prospect klant met hoge neiging voor M365.|
|Extern werk inschakelen-concurrentie beding (inzoomen) met M365| Klanten met zoom-en M365, doel voor conversie naar teams|
|Extern werk inschakelen-concurrentie beding (zoom) zonder M365|  Klanten met Inzoomen, doel voor conversie naar teams|
|Kosten verlagen en beheren M365 E3 gericht op M365 E5| Bestaande klant met M365 E3, Target voor M365 E5|
|Kosten verlagen en beheer M365 BB en BS-klanten die gericht zijn op M365 BP|    Bestaande M365 BB en BS-klanten, gericht op M365 BP|
|De productiviteit van de organisatie neiging|    De klant toont neiging voor het Opper vlak.|
|M365Cluster|Identificeert de neiging van de klant voor het aanschaffen van M365.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|M365Fit|   Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een model op basis van onze beste SMB om klanten te vergelijken en te controleren of ze geschikt zijn voor Microsoft Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt.|
|M365Intent|    Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De bewaarde score voor het maken van de clusters is van groot belang. Beoordeling van de intentie is maandelijks bijgewerkt.|
|SurfaceCluster|    Hiermee wordt de neiging van de klant geïdentificeerd om het Opper vlak aan te schaffen door de aanpassings-en intentie aanbevelingen in een cluster te consolideren.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|SurfaceFit|    Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een model op basis van onze beste SMB om klanten te vergelijken en te controleren of ze geschikt zijn voor Microsoft Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt.|
|SurfaceIntent| Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De bewaarde score voor het maken van de clusters is van groot belang. Beoordeling van de intentie is maandelijks bijgewerkt.|
|O365Cluster|   Hiermee wordt de neiging van de klant geïdentificeerd om O365 aan te schaffen.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|O365Fit|   Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een model op basis van onze beste SMB om klanten te vergelijken en te controleren of ze geschikt zijn voor Microsoft Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt.|
|O365Intent|    Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De bewaarde score voor het maken van de clusters is van groot belang. Beoordeling van de intentie is maandelijks bijgewerkt.|
|M365UpsellCustomer|    Hiermee wordt aangegeven of de klant verkoop neiging voor M365 weergeeft|
|Heeft Google|    Met deze markering wordt aangegeven of een klant concurrerende signalen voor de eigenaar van Google-producten wordt weer gegeven|
|Heeft AWS|   Met deze markering wordt aangegeven of een klant concurrerende signalen voor de eigenaar van AWS-producten wordt weer gegeven|
|Bevat EA|    Hiermee wordt aangegeven of een vernieuwing een Enter prise Agreement (EA) of een EA-abonnement is|
|Heeft open|  Hiermee wordt aangegeven of een verlenging een open-of Open Value-overeenkomst is|

**D365 neiging** in de Cloud: de gegevens definities van de verschillende velden van het D365 neiging-rapport in de Cloud zijn:

| **Kolom naam** | **Gegevens beschrijving** |
|---------|:---------|
|MPN-id|    Microsoft Partner Network-ID|
|Partner naam|  De naam van de partner|
|Klant-ID|   Klant-id-nummer |
|DUNS-nummer|   Het Bradstreet-nummer van de inbel netwerk-& van de klant die wordt beoordeeld op neiging|
|Accountnaam|  Naam van het account |
|Domain|    Domein van het account|
|Grootte van org|  Grootte van organisatie|
|Branche|  Branche  |
|Verticaal|  De verticale van de klant met een score voor neiging, zoals wordt bepaald door micro soft en andere industrie normen (D&B)
|Gebied|  Geografisch gebied van de locatie|
|Dochteronderneming|    De dochter onderneming van de klant die wordt beoordeeld op neiging|
|Verkoopterritorium|   Verkoopterritorium|
|Plaats|  Locatie van geografische plaats |
|Staat| Locatie van geografische status|
|Postcode|   Postcode|
|Land/regio|   Locatie van geografisch land |
|Segment|   Markt segment |
|Subsegment|   Subsegment op de markt |
|Overzicht van SMC-typen|  De categorisatie van een klant: de belangrijkste onbeheerde gebruikers bases zijn klanten met 300 + werk nemers, de belangrijkste onbeheerde Compute Base is klanten met $10.000 in azure 3 jaar potentieel, middel grote bedrijven zijn klanten met minder dan 25 werk nemers|
|Top niet-beheerd-Compute base   |Top unmanaged Customers – compute|
|Boven onbeheerd: gebruikers basis| Belangrijkste onbeheerde klanten – gebruikers|
|IsNonProfit|   Of niet-winst of voor winst (Ja/Nee)|
|Activering van digitale verkoop-M365-Seat-grootte >= 25 stoelen (SalesPro neiging model)|   Klant zonder D365. Grootte van Seat: 25 +. Partners moeten gericht zijn op het cross-sell van D365 Salespro|
|Digital selling activeren-D365 SalesPro neiging (Act Now/evaluate) |High-neiging-klanten zonder D365.  Partners moeten gericht zijn op D365 SalesPro.|
|Financieel risico beheren & fraude-Dynamics on-premises installatie base-Navision (BC neiging model)|Bestaande klant met premises Navision.  Partner moet gericht zijn op D365 BC|
|Financieel risico beheren & fraude-Dynamics on-premises install base-AX (F&O neiging model)    |Bestaande klant met premises AX.  Partner moet gericht zijn op D365 F&O|
|Financieel risico beheren & fraude-Dynamics on-premises install base-Great Plains (BC neiging model)|  Bestaande klant met premises Great Plains.  Partner moet gericht zijn op D365 BC|
|Financieel risico beheren & fraude-Dynamics on-premises install base-Solomon (BC neiging model)|Bestaande klant met premises Solomon.  Partner moet gericht zijn op D365 BC|
|Financieel risico beheren & fraude-Dynamics on-premises installatie base-overige (BC neiging model) |Bestaande klant met andere premises-oplossingen die niet hierboven worden vermeld.  Partner moet gericht zijn op D365 BC|
|Flexibele bedrijfs processen bouwen-Dynamics on-premises installatie base-AX/GP/SL/NAV/Overig (D365 neiging model)|   Flexibele bedrijfs processen bouwen-Dynamics on-premises installatie base-AX/GP/SL/NAV/Overig (D365 neiging model)|
|Flexibele bedrijfs processen bouwen-Dynamics-concurrentie Mendix/Outsystems/Sales Force (D365 neiging model)| Flexibele bedrijfs processen bouwen-Dynamics-concurrentie Mendix/Outsystems/Sales Force (D365 neiging model)|
|Flexibele bedrijfs processen bouwen-D365 F&O install base |Bestaande D365 F&O-klanten.  Partner om Power-apps te richten.|
|Flexibele bedrijfs processen bouwen-basis installatie van D365 BC| Bestaande D365 BC-klanten. Partner om Power-apps te richten.|
|Flexibele bedrijfs processen bouwen-basis van D365 CE-installatie| Bestaande D365 CE-klanten. Partner om Power-apps te richten.|
|Bouw een robuuste toeleverings keten-Win en activeer de eerste D365-werk belasting als D365 toeleverings keten met niet-Oracle/SAP ERP-klanten|  Doel klanten voor een D365-toeleverings keten.|
|Bouw een robuuste toeleverings keten-cross-sell D365-toeleverings keten en/of retail/commerce aan bestaande D365 CE-klanten |Bestaande D365 CE-klanten om te richten op D365 toeleverings keten voor cross-selling|
|Bouw een robuuste toeleverings keten om D365 sup te verkopen. Keten en/of retail/commerce to D365 CE en (Oracle of SAP)| Bestaande D365 CE-klanten met Oracle of SAP om te richten op de D365-toeleverings keten|
|D365BCCluster| Hiermee wordt de neiging van de klant geïdentificeerd om D365 Business Central te kopen.  Klanten die neiging voor BC worden weer gegeven, zijn de categorieën middel grote en kleine.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|D365BCFit| Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een model op basis van onze beste SMB om klanten te vergelijken en te controleren of ze geschikt zijn voor Microsoft Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt.|
|D365BCIntent|  Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De bewaarde score voor het maken van de clusters is van groot belang. Beoordeling van de intentie is maandelijks bijgewerkt.|
|D365FOCluster| Hiermee wordt de neiging van de klant geïdentificeerd om D365 Finance and Operations te kopen.  Klanten die neiging voor F&O tonen, staan in de hoofd categorieën zonder begeleiding. Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|D365FOFit| Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een model op basis van onze beste SMB om klanten te vergelijken en te controleren of ze geschikt zijn voor Microsoft Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt.|
|D365FOIntent|  Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De bewaarde score voor het maken van de clusters is van groot belang. Beoordeling van de intentie is maandelijks bijgewerkt.|
|D365CECluster| Hiermee wordt de neiging van de klant geïdentificeerd om de klant betrokkenheid van D365 aan te schaffen.  Klanten die neiging voor CE weer geven, zijn de categorieën middel grote en kleine.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|D365CEFit| Passend voor D365 CE|
|D365CEIntent|  Intentie voor D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Hiermee wordt aangegeven of een klant een openstaande verlenging voor Dynamics on-premises AX of CRM heeft.|
|M365UpsellCustomer|    Hiermee wordt aangegeven of de klant verkoop neiging voor M365 weergeeft|
|Heeft Google|    Met deze markering wordt aangegeven of een klant concurrerende signalen voor de eigenaar van Google-producten wordt weer gegeven|
|Heeft AWS|   Met deze markering wordt aangegeven of een klant concurrerende signalen voor de eigenaar van AWS-producten wordt weer gegeven|
|Bevat EA |Hiermee wordt aangegeven of een vernieuwing een Enter prise Agreement (EA) of een EA-abonnement is|
|Heeft open|  Hiermee wordt aangegeven of een verlenging een open-of Open Value-overeenkomst is|

**Cloud Ascent-Azure neiging**: de gegevens definities van de verschillende velden van het Ascent-Azure neiging-rapport in de Cloud zijn:

|**Kolom naam** |**Gegevens beschrijving** |
|---------|:---------|
|MPN-id|    Microsoft Partner Network-ID|
|Partner naam|  De naam van de partner|
|Klant-ID|   Klant-id-nummer |
|DUNS-nummer|   Het Bradstreet-nummer van de inbel netwerk-& van de klant die wordt beoordeeld op neiging|
|Accountnaam|  Naam van het account |
|Domain|    Domein van het account|
|Grootte van org|  Grootte van organisatie|
|Branche|  Branche  |
|Verticaal|  De verticale van de klant met een score voor neiging, zoals wordt bepaald door micro soft en andere industrie normen (D&B)|
|Gebied|  Geografisch gebied van de locatie|
|Dochteronderneming|    De dochter onderneming van de klant die wordt beoordeeld op neiging|
|Verkoopterritorium|   Verkoopterritorium|
|Plaats|  Locatie van geografische plaats |
|Staat| Locatie van geografische status|
|Postcode|   Postcode|
|Land/regio|   Locatie van geografisch land |
|Segment|   Markt segment |
|Subsegment|   Subsegment op de markt |
|Overzicht van SMC-typen|  SMC-type |
|Top niet-beheerd-Compute base|  Top unmanaged Customers – compute|
|Boven onbeheerd: gebruikers basis| Belangrijkste onbeheerde klanten – gebruikers|
|IsNonProfit|   Of niet-winst of voor winst (Ja/Nee)|
|Migrate-EOS win server-EOS Windows Server IB met CLAS neiging-5 + licenties|   Klanten die een on-premises win server van EOS hebben (dat wil zeggen, versies die ouder zijn dan en met EOS-producten). De klant heeft 5 of meer licenties. Klant die een neiging score heeft.  Partners moeten deze klanten richten op de migratie naar Azure.|
|Migrate-EOS win server-EOS Windows Server IB met CLAS neiging-<5-licenties|   Klant die over EOS (End of service) beschikt over een on-premises win-server (dat wil zeggen, versies die ouder zijn dan en met EOS-producten). De klant heeft minder dan 5 licenties. Klant die een neiging score heeft.  Partners moeten deze klanten richten op de migratie naar Azure.|
|Migrate-EOS win server-EOS Windows Server IB zonder CLAS neiging-5 + licenties |Klanten die een on-premises win server van EOS hebben (dat wil zeggen, versies die ouder zijn dan en met EOS-producten). De klant heeft meer dan vijf licenties. Klant heeft geen neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migrate-EOS win server-EOS Windows Server IB zonder CLAS neiging-<5-licenties|    Klanten die een on-premises win server van EOS hebben (dat wil zeggen, versies die ouder zijn dan en met EOS-producten). Heeft minder dan 5 licenties. Klant heeft geen neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreer-EOS SQL-EOS SQL Server IB met CLAS neiging-5 + licenties|  Klant die een EOS-on-premises SQL Server heeft (dat wil zeggen, versies die ouder zijn dan en met EOS-producten). De klant heeft 5 licenties. De klant heeft een neiging score.  Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreer-EOS SQL-EOS SQL Server IB met CLAS neiging-<5-licenties|  Klant die een EOS-on-premises SQL Server heeft (dat wil zeggen, versies die ouder zijn dan en met EOS-producten). Heeft minder dan 5 licenties. Klant die een neiging score heeft. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreer-EOS SQL-EOS SQL Server IB zonder CLAS neiging-5 + licenties|   Klant die een EOS-on-premises SQL Server heeft (dat wil zeggen, versies die ouder zijn dan en met EOS-producten). De klant heeft 5 of meer licenties. Klant heeft geen neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreer-EOS SQL-EOS SQL Server IB zonder CLAS neiging-<5-licenties|   Klant die een EOS-on-premises SQL Server heeft (dat wil zeggen, versies die ouder zijn dan en met EOS-producten). De klant heeft minder dan 5 licenties. Klant heeft geen neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren: on-premises win server migreren-huidige Windows Server IB met CLAS neiging-5 + licenties|   Klant die de huidige on-premises win server heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft 5 licenties. De klant heeft een neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren: on-premises win server migreren-huidige Windows Server IB met CLAS neiging-<5-licenties|   Klant die de huidige on-premises win server heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft minder dan 5 licenties. De klant heeft een neiging-score voor Azure. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren: on-premises win server migreren-huidige Windows Server IB zonder CLAS neiging-5 + licenties|    Klant die de huidige on-premises win server heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft 5 licenties. Klant heeft geen neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migratie migreren: on-premises win server-huidige Windows Server IB zonder CLAS neiging-<5-licenties |Klant die de huidige on-premises win server heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft minder dan 5 licenties. Klant heeft geen neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren: migreren naar Azure SQL of SQL-Vm's-huidige SQL Server IB met CLAS neiging-5 + licenties|  Klant die actuele on-premises SQL Server heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft 5 licenties. De klant heeft een neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren: migreren naar Azure SQL of SQL-Vm's-huidige SQL Server IB met CLAS neiging-<5-licenties|  Klant die actuele on-premises SQL Server heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft minder dan 5 licenties. De klant heeft een neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren: migreren naar Azure SQL of SQL-Vm's-huidige SQL Server IB zonder CLAS neiging-5 + licenties|   Klant die actuele on-premises SQL Server heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft 5 licenties. Klant heeft geen neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren: migreren naar Azure SQL of SQL-Vm's-huidige SQL Server IB zonder CLAS neiging-<5-licenties|   Klant die actuele on-premises SQL Server heeft (dat wil zeggen, versies die na EOS-producten vallen). De klant heeft minder dan 5 licenties. Klant heeft geen neiging score. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren-OSS-migreren naar OSS DB| Bestaande klant met een van de volgende concurrentie producten: PostgreSQL, MySQL, MariaDB. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migrate-OSS-Linux op Azure |Bestaande klant met het product: Linux. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migrate-SAP-SAP on Azure|  Bestaande klant met het product: SAP. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migrate-WVD-RDS IB |Identificeert klanten met actieve Windows Extern bureaublad-services. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migrate-WVD-moderne werk door verkopen aan Azure/WVD|   Identificeert klanten met M365 en heeft geen Azure. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migreren-VMware IB|   Bestaande klant met het product: VMware. Partners moeten deze klanten richten op de migratie naar Azure.|
|Migrate-Citrix IB|   Bestaande klant met het product: Citrix Systems. Partners moeten deze klanten richten op de migratie naar Azure.|
|Innoveren-Analytics-Power BI IB met hoge Azure neiging|   Klanten met en actief Power BI abonnement met inbegrip van: Power BI-zelfstandige Pro, Power BI-Azure-suites, Power BI Office-suites, Power BI suites-M365|
|Enable-DevOps met GitHub-Visual Studio/MSDN IB|    Geïdentificeerde klanten met actieve visuele Studios|
|Standaard versie van Windows Server|   Hier wordt de versie van Windows Server Standard-aankopen door de klant weer gegeven|
|Standard-licentie voor Windows Server|   Hier wordt het licentie type van Windows Server Standard-aankopen door de klant weer gegeven|
|Win Server Data Center-versie|    Hier wordt de versie van Windows Data Center-aankopen door de klant weer gegeven|
|Win Server Data Center-licentie| Hier wordt het licentie type van Windows Data Center-aankopen door de klant weer gegeven|
|AzureFit|  Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een model op basis van onze beste SMB om klanten te vergelijken en te controleren of ze geschikt zijn voor Microsoft Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt.|
|AzureIntent|   Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De bewaarde score voor het maken van de clusters is van groot belang. Beoordeling van de intentie is maandelijks bijgewerkt.|
|AzureCluster|  Hiermee wordt de neiging van de klant geïdentificeerd voor het kopen van Azure door het samen voegen van de aanpassings-en intentie aanbevelingen in een cluster.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|WindowsServerDataCenter_HasOpenRenewal|    Hiermee wordt aangegeven of een klant een open vernieuwing heeft voor een Windows Server-Data Center|
|WindowsServerStandard_HasOpenRenewal|  Hiermee wordt aangegeven of een klant een openstaande vernieuwing heeft voor een Windows Server-Standard|
|AzureUpsellCustomer|   Hiermee wordt aangegeven of de klant verkoop neiging voor Azure weergeeft|
|Heeft Google|    Met deze markering wordt aangegeven of een klant concurrerende signalen voor de eigenaar van Google-producten wordt weer gegeven|
|Heeft AWS|   Met deze markering wordt aangegeven of een klant concurrerende signalen voor de eigenaar van AWS-producten wordt weer gegeven|
|Bevat EA |Hiermee wordt aangegeven of een vernieuwing een Enter prise Agreement (EA) of een EA-abonnement is|
|Heeft open|  Hiermee wordt aangegeven of een verlenging een open-of Open Value-overeenkomst is|

**Cloud Ascent-Agreement vernieuwt neiging**: de gegevens definities van de verschillende velden van het rapport vernieuwingen in de Cloud met een aflopende neiging zijn:

|**Kolom naam** |**Gegevens beschrijving** |
|---------|:---------|
|MPN-id|    Microsoft Partner Network-ID|
|Partner naam|  De naam van de partner|
|Klant-ID|   Klant-id-nummer |
|DUNS-nummer|   Het Bradstreet-nummer van de inbel netwerk-& van de klant die wordt beoordeeld op neiging|
|Accountnaam|  Naam van het account |
|Domain|    Domein van het account|
|Grootte van org|  Grootte van organisatie|
|Branche|  Branche  |
|Verticaal|  De verticale van de klant met een score voor neiging, zoals wordt bepaald door micro soft en andere industrie normen (D&B)|
|Gebied|  Geografisch gebied van de locatie|
|Dochteronderneming|    De dochter onderneming van de klant die wordt beoordeeld op neiging|
|Verkoopterritorium|   Verkoopterritorium|
|Plaats|  Locatie van geografische plaats |
|Staat| Locatie van geografische status|
|Postcode|   Postcode|
|Land/regio|   Locatie van geografisch land |
|Segment|   Markt segment |
|Subsegment|   Subsegment op de markt |
|Overzicht van SMC-typen|  SMC-type |
|Top niet-beheerd-Compute base|  Top unmanaged Customers – compute|
|Boven onbeheerd: gebruikers basis| Belangrijkste onbeheerde klanten – gebruikers|
|IsNonProfit|Of niet-winst of voor winst (Ja/Nee)|
|Heeft Google|Met deze markering wordt aangegeven of een klant concurrerende signalen voor de eigenaar van AWS-producten wordt weer gegeven|
|Heeft AWS|Met deze markering wordt aangegeven of een klant concurrerende signalen voor de eigenaar van AWS-producten wordt weer gegeven|
|Azure-cluster|Hiermee wordt de neiging van de klant geïdentificeerd om Azure aan te schaffen.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|D365 F&O-cluster|  Hiermee wordt de neiging van de klant geïdentificeerd om D365 Finance and Operations te kopen.  Klanten die neiging voor F&O tonen, staan in de hoofd categorieën zonder begeleiding.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|D365 CE-cluster|   Hiermee wordt de neiging van de klant geïdentificeerd om de klant betrokkenheid van D365 aan te schaffen.  Klanten die neiging voor CE weer geven, zijn de categorieën middel grote en kleine.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|D365 BC-cluster|   Hiermee wordt de neiging van de klant geïdentificeerd om D365 Business Central te kopen.  Klanten die neiging voor BC worden weer gegeven, zijn de categorieën middel grote en kleine.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|M365-cluster|  Hiermee wordt de neiging van de klant geïdentificeerd voor het aanschaffen van M365.  Clusters nu en evalueren moeten worden gericht op het feit dat ze meer rendement opleveren.  Nurture en Train klanten mogen alleen worden aangemerkt als er nog capaciteit is nadat het is bereikt en evalueren van klanten.|
|Licentie programma|   Hiermee wordt het type licentie programma voor de verlenging aangegeven|
|Overeenkomst-ID|  Overeenkomst-id|
|Eind datum van overeenkomst|    Eind datum van overeenkomst |
|Type verval datum|   Type verval datum|
|Verlopende omzet|  Omzet gekoppeld aan verlopen abonnementen|
|Bevat EA|    Hiermee wordt aangegeven of een vernieuwing een Enter prise Agreement (EA) of een EA-abonnement is|
|Heeft open|  Hiermee wordt aangegeven of een verlenging een open-of Open Value-overeenkomst is|
|Klant van Azure-verkoop| Hiermee wordt aangegeven of de klant verkoop neiging voor Azure weergeeft|
|M365-verkoop klant|  Hiermee wordt aangegeven of de klant verkoop neiging voor M365 weergeeft|
|RevSumDivisionName|    Hiermee wordt het product geïdentificeerd dat voor de verlenging is ingesteld|

## <a name="next-steps"></a>Volgende stappen

Zie [rapporten downloaden](pci-download-reports.md)voor rapporten.
