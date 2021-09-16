---
title: Definities van inzichtengegevens
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Het document bevat verschillende rapporten en hun gegevensdefinities, die u kunt downloaden van de Insights Rapport downloaden.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d1119152e601c0fa7f8bb080420181d1f52801db
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/16/2021
ms.locfileid: "127876727"
---
# <a name="export--data-definitions"></a>Exporteren : gegevensdefinities 

**Juiste rollen:** rapportviewer | Rapportviewer voor leidinggevenden

## <a name="introduction"></a>Introductie 

Met behulp van de hub Rapporten downloaden op Insights dashboard kunt u de onbewerkte gegevenssets exporteren. 

De verschillende rapporten, die u samen met de gegevensdefinities kunt downloaden, worden weergegeven in de volgende tabellen: 

### <a name="partner-profile-report"></a>**Partnerprofielrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| MPNId | Microsoft Partner Network-id (MPN) | 
| PartnerName | Naam van de partner | 
| PGA_MPNId | Id van de MPN van het globale partneraccount | 
| PGA_PartnerName | Globale accountnaam van partner | 
| Plaats | Plaats van de partnerlocatie | 
| Land/regio | Landlocatie van de partner | 
| HierarchyLevel | Geeft aan of het een globale MPN-id of locatie-MPN-id is | 

### <a name="customer-details-report"></a>**Rapport klantdetails**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId| Id van de MPN van het globale partneraccount|
| CustomerName| Naam van de klant|
| CustomerTenantId| Id van de tenant van de klant|
| CustomerTpid| Id van het bovenliggende bovenliggende klant|
| DUNSNumber|   Global Data Universal Number System Identifier van de klant|
| CustomerSegment | Klantsegment|
| TopSegment    | Segmentclassificatie op een hoger niveau van de klant|
| CustomerMarket|   Geografische markt van de klant|  
| CustomerStatus    | Klantstatus (actief of inactief)| 
| CustomerTenantName|   Naam van klant-tenant|
| CustomerTenantCountry|    Land van de tenant van de klant|
| TenantDomainName| Domeinnaam van klant-tenant|
| Product|  Het product dat aan de klant is verkocht door de MPN: O365, Dynamics 365, Enterprise Mobility + Security, Power BI of Microsoft Azure.|
| RawProductName|   Gedetailleerde productnaam die aan de klant is verkocht|
| SKU|  Product-SKU|
| Maand|    Maand waarvoor gebruik en omzet worden gerapporteerd|
| MPNId|    Id van Microsoft Partner Network (MPN)|
| PartnerName|  Naam van de partner|
| PartnerLocation|  Geografische locatie van partner|
| PartnerAttributionType|   Toeschrijvingstype van de partner| 
| SalesChannel| Verkoopkanaal|
| IsDuplicateRowForPGA| Voor meerdere partnervermeldingen onder één PGA wordt deze waarde ingesteld op 0 voor slechts één MPNId. Als de waarde is ingesteld op 1, wordt een dubbele rij aangegeven|
| AvailableSeats|   Beschikbare seats|
| BilledRevenueUSD| Gefactureerde omzet in Amerikaanse dollar|
| AzureConsumedRevenueUSD|  Omzet uit Azure-verbruik in USD|

### <a name="reseller-performance-report"></a>**Prestatierapport reseller**

> [!Note]
> Omzet- en ACR-gegevens (Consumed Revenue) van Azure zijn alleen beschikbaar voor gebruikers die rapportgebruikers van het management zijn.

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId | Id van de MPN van het globale partneraccount |
| ResellerMPNid | Reseller-Microsoft Partner Network-id | 
| ResellerName | Reseller name | 
| ResellerMarket | Resellerland van de markt | 
| IndirectProviderMPNId | Id van de indirecte provider Microsoft Partner Network | 
| IndirectProviderName | Indirecte providernaam | 
| Maand | Maand waarvoor gebruik en omzet worden gerapporteerd | 
| Product | Productnaam | 
| SubscriptionID | Id van het abonnement | 
| AvailableSeats | Aantal beschikbare seats | 
| Toegewezen toegewezen taken | Aantal toegewezen seats | 
| BilledRevenueUSD | Gefactureerde omzet in Amerikaanse dollars | 
| CustomerName | Naam van de klant | 
| CustomerTPid | Id van het bovenliggende bovenliggende klant | 
| CustomerSegment | Klantsegment | 
| CustomerMarket | Geografische markt van de klant | 
| ResellerStatus | Resellerstatus | 

### <a name="subscription-details-report"></a>**Rapport met abonnementsdetails**

>[!Note]
>Omzet- en ACR-gegevens zijn alleen beschikbaar voor gebruikers die executive rapport viewers zijn.

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
|PGAMpnId| Id van het globale partneraccount MPN |
|SubscriptionId | GUID van het abonnement|
|SubscriptionStartDate | Begindatum van het abonnement|
|SubscriptionEndDate | Einddatum van het abonnement|
|SubscriptionState | Status van het abonnement (actief of verloop)|
|Maand | Maand waarvoor gebruik en omzet worden gerapporteerd|
|IsAutoRenew | Geeft aan of het abonnement automatisch wordt verlengd (Ja of Nee)|
|CustomerName | Naam van de klant|
|CustomerTenantId | GUID van de klant|
|CustomerTpid | Bovenliggende id van klant|
|DUNSNumber| Global Data Universal Number System Identifier van de klant|
|CustomerSegment | Marktsegment van de klant|
|TopSegment| Segmentclassificatie op een hoger niveau van de klant|
|CustomerMarket | Geografische markt van de klant|
|ReportingProductName| Gedetailleerde productnaam|
|Product | Product verkocht aan de klant door de partner|
|RawProductName| Gedetailleerde productnaam verkocht aan de klant|
|ProductPartNumber| Onderdeelnummer van het product|
|SKU | SKU van het product|
|RevSumDivisionName| Naam van de producthiërarchie voor omzetrapportage|
|SolutionArea| Bedrijfstoepassingsclassificatie van het product|
|MPNId | Microsoft Partner Network id van de partner|
|PartnerName | Naam van de partner|
|PartnerLocation | Geografische locatie van de partner|
|PartnerAttributionType | Toeschrijvingstype voor het abonnement|
|SalesChannel | Verkoopkanaal: direct, CSP (Cloud Solution Provider), e.d.|
|PricingLevel| Prijspunt van de verkoop|
|EnrollmentNumber| Inschrijvingsnummer van het abonnement|
|IsDuplicateRowForPGA| Voor meerdere partnervermeldingen onder één PGA wordt deze waarde ingesteld op 0 voor slechts één MPNId. Als de waarde is ingesteld op 1, wordt een dubbele rij aangegeven|
|SubscriptionStartMonth| Beginmaand van het abonnement|
|ResellerID| Id van reseller|
|ResellerName| Reseller name|
|AvailableSeatsEOP| Algemeen beschikbare seats tot einde van periode|
|AvailableSeats | Beschikbaar zit zitverschil maand op maand|
|BilledRevenueUSD | Omzet in USD|
|AzureConsumedRevenueUSD| Omzet uit Azure-verbruik in USD|

### <a name="azure-usage-report"></a>**Azure-gebruiksrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
|PGAMpnId| Id van het globale partneraccount MPN|
|SubscriptionId| GUID van het abonnement|
|SubscriptionStartDate| De datum van het begin van het abonnement|
|SubscriptionEndDate| De datum van het einde van het abonnement|
|FirstUseDate| Datum waarop Azure-services het eerst zijn gebruikt|
|SubscriptionState| Huidige status van het abonnement (open, gesloten actief of in respijtperiode)|
|Maand| Datum geaggregeerd per maand|
|ServiceLevel1| Serviceniveau 1: komt overeen met servicepijler, zoals containers, databases, netwerken, enzovoort.|
|ServiceLevel2| Serviceniveau 2: komt overeen met de workload voor de servicepijler|
|ServiceLevel3| Servicenaam die wordt gebruikt door Azure.Microsoft.Com bij het aanbieden van Azure-aanbiedingen|
|ServiceLevel4| Logische groeperingen van functiesets op hoog niveau differentiëren binnen de service. Zoals Algemeen Virtual Machines, Geoptimaliseerd voor geheugen Virtual Machines, Single SQL Database, Elastic SQL Database, enzovoort. |
|ServiceGroup2| Veld revenue accountability (FRA) gebieden zoals AI, App Dev, IoT, enzovoort |
|ServiceGroup3| Aanvullende details voor FRA, zoals IoT Hub, Kaarten voor IoT FRA|
|ServiceInfluencer| PaaS-services die het verbruik van infrastructuurbronnen aanstrijden, zoals Service Fabric, Azure Databricks, AKS, enzovoort.|
|ComputeOS| Besturingssysteem voor de berekening|
|ComputeCoreSoftware| Compute Core Software|
|UsageUnits| Het aantal eenheden dat tijdens de factureringscyclus wordt gebruikt|
|UsageQuantity| Hoeveelheid gebruik van resource|
|CustomerName| Naam van de klant|
|CustomerTenantId| Tenant-id van de klant|
|CustomerTpid| Bovenliggende id van klant|
|CustomerSegment| Segment van de klant|
|CustomerMarket| Geografische markt van de klant|
|MPNId| Microsoft Partner Network id van de klant|
|PartnerName| Naam van de partner|
|PartnerLocation| Geografische landlocatie van de partner|
|PartnerAttributionType| Toeschrijvingstype van de partner|
|SalesChannel| Verkoopkanaal (Direct/CSP, Indirect/CSP, Direct, e.d.)  |
|EnrollmentNumber| Inschrijvingsnummer van het abonnement |
|IsACRDuplicateAtPGALevel| Voor meerdere partnervermeldingen onder één PGA wordt deze waarde ingesteld op 0 voor slechts één MPNId. Als de waarde is ingesteld op 1, wordt een dubbele rij aangegeven|
|ResellerID| Id van reseller|
|ResellerName| Reseller name|
|AdminType| Wanneer het type partnervermelding 'Partner Admin Link (PAL)' is, wordt in deze kolom de toegewezen rol in het abonnement van de klant aangegeven.|
|AssociationType| Type associatie|
|MonthlySubscriptionLevelACR| ACR op maandelijks abonnementsniveau|
|ACR_USD| Verbruikte azure-omzet (ACR) in Amerikaanse dollars|

### <a name="office-365-license-usage-report"></a>**Office 365 licentiegebruiksrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId | Id van de MPN van het globale partneraccount | 
| CustomerTenantId | Tenant-id van de klant | 
| CustomerTpid | Bovenliggende id van klant | 
| WorkloadName | Skype voor Bedrijven, Teams, Exchange Online | 
| Maand | Maand waarvoor gebruik wordt gerapporteerd | 
| PaidAvailableUnits | Aantal betaalde beschikbare eenheden | 
| MonthlyActiveUsers | Aantal maandelijks actieve gebruikers | 
| CustomerName | Naam van de klant | 
| CustomerMarket | Geografische landlocatie van de markt van de klant | 
| CustomerSegment | Klantsegment | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | Naam van de partner | 
| PartnerLocation | Geografische locatie van de partner | 
| PartnerAttributionType | Toeschrijvingstype van de partner | 
| IsDuplicateRowForPGA | Voor meerdere partnervermeldingen onder één PGA wordt deze waarde ingesteld op 0 voor slechts één MPNId. Als de waarde is ingesteld op 1, wordt een dubbele rij aangegeven|

### <a name="enterprise-mobility-license-usage-report"></a>**Gebruiksrapport voor Enterprise Mobility-licenties**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId| Id van het globale partneraccount MPN| 
| SubscriptionId | GUID van het abonnement| 
| SubscriptionStartDate | De datum van het begin van het abonnement| 
| SubscriptionEndDate | De datum waarop het abonnement eindigt| 
| SubscriptionStatus| Huidige status van het abonnement (open, gesloten, actief of in respijtperiode)| 
| Maand | Datum geaggregeerd per maand| 
| SKU| Product-SKU| 
| SKUId| SKU-id van het product| 
| FreeVsPaidSKU| Geeft gratis of betaalde SKU aan| 
| SalesModel| Verkoopkanaal dat wordt gebruikt voor het verkopen van het abonnement| 
| DetailedSalesModel| Gedetailleerd verkoopmodel voor het abonnement| 
| CustomerName| Naam van de klant| 
| CustomerTenantId | Tenant-id van de klant| 
| CustomerTpid | Bovenliggende id van klant| 
| CustomerSegment | Klantsegment| 
| CustomerMarket | Geografische landlocatie van de markt van de klant| 
| MPNId | Microsoft Partner Network ID| 
| PartnerName | Naam van de partner| 
| PartnerLocation | Geografische locatie van partner| 
| PartnerAttributionType | Toeschrijvingstype van partner| 
| PartnerHierarchy| Hiërarchie van partner (virtuele organisatie of headquarters of locatie)| 
| PaidAvailableUnits | Aantal betaalde beschikbare eenheden| 
| MonthlyActiveUsers | Aantal maandelijks actieve gebruikers| 
| AATPActiveUsage| Actief gebruik van Azure Advanced Threat Protection (AATP)| 
| MCASActiveUsage| Actief MCAS-gebruik| 
| AADPPaidAvailableUnits| Aantal betaalde beschikbare eenheden voor Azure Active Directory Premium (AADP)| 
| IntunePaidAvailableUnits| Aantal betaalde beschikbare eenheden voor Intune| 
| AzipPaidAvailableUnits| Aantal betaalde beschikbare eenheden voor Azip| 
| AADPMonthlyActiveUsers| Aantal maandelijks actieve gebruikers voor Azure Active Directory Premium (AADP)| 
| IntuneMonthlyActiveUsers| Aantal maandelijks actieve gebruikers voor Intune| 
| AzipMonthlyActiveUsers| Aantal maandelijks actieve gebruikers voor Azip| 
| MDM| MDM| 
| MAM| MAM| 
| SSPR| SSPR| 

### <a name="dynamics-365-license-usage-report"></a>**Gebruiksrapport voor Dynamics 365-licenties**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId | Id van het globale partneraccount MPN | 
| SubscriptionId | GUID van het abonnement | 
| SubscriptionStartDate | Begindatum van het abonnement | 
| SubscriptionEndDate | Einddatum van het abonnement | 
| SubscriptionStatus | Status van het abonnement | 
| Maand | Maand waarvoor gebruik wordt gerapporteerd | 
| RevSumDivisionName | Naam van de deling rev sum | 
| RevSumCategoryName | Naam van de rev sum-categorie | 
| SKU | SKU van het product | 
| SKUId | SKU-id van het product | 
| FreeVsPaidSKU | Geeft aan of het een gratis of betaalde SKU is | 
| SalesModel | Verkoopkanaal dat wordt gebruikt voor het verkopen van het abonnement | 
| DetailedSalesModel | Gedetailleerd verkoopmodel voor het abonnement | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | GUID van de tenant van de klant | 
| CustomerTpid | Bovenliggende id van klant | 
| CustomerSegment | Marktsegment van de klant | 
| CustomerMarket | Geografische markt van de klant | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | Naam van de partner | 
| PartnerLocation | Geografische landlocatie van de partner | 
| PartnerAttachType | Toeschrijvingstype voor het abonnement | 
| AvailableSeats |  Huidige betaalde beschikbare seats|
| ToegewezenSeats |   Huidige toegewezen seats|
| ActiveSeats | Huidige actieve seats|
| DeploymentOpportunity |   Implementatiekans is het aantal seats dat niet is toegewezen|
| ActiveUsagePercent |  Huidig actief gebruik als percentage van beschikbare seats |

### <a name="power-bi-license-usage-report"></a>**Power BI licentiegebruiksrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId | Id van de MPN van het globale partneraccount | 
| SubscriptionId | GUID van het abonnement | 
| SubscriptionStartDate | Begindatum van het abonnement | 
| SubscriptionEndDate | Einddatum van het abonnement | 
| SubscriptionStatus | Status van het abonnement (actief, inactief of in respijtperiode) | 
| Maand | Datum geaggregeerd per maand | 
| SKU | SKU van het product | 
| SKUId | SKU-id van het product | 
| FreeVsPaidSKU | Gratis of betaalde SKU-differentiator | 
| SalesModel | Verkoopmodel dat wordt gebruikt om het abonnement te verkopen | 
| DetailedSalesModel | Gedetailleerd verkoopmodel voor het abonnement | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | GUID van de tenant van de klant | 
| CustomerTpid | Id van het bovenliggende bovenliggende klant | 
| CustomerSegment | Marktsegment van de klant | 
| CustomerMarket | Geografische markt van de klant | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | Naam van de partner | 
| PartnerLocation | Geografische landlocatie van de partner | 
| PartnerAttachType | Toeschrijvingstype voor het abonnement | 
| PartnerHierarchy |    Hiërarchie van partner (virtuele organisatie of HeadQuarters of locatie)|
| AvailableSeats |  Huidige betaalde beschikbare seats|
| ToegewezenSeats |   Huidige toegewezen seats|
| ActiveSeats | Huidige actieve seats|
| DeploymentOpportunity |   Implementatiekans is het aantal seats dat niet is toegewezen|
| ActiveUsagePercent |  Huidig actief gebruik als percentage van beschikbare seats|

### <a name="teams-meetings-and-calls-report"></a>**Teams en aanroepen rapporteren**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId | Id van de MPN van het globale partneraccount | 
| CustomerTenantId | Tenant-id van de klant | 
| CustomerId | Id van het bovenliggende bovenliggende klant | 
| DateKey | Datum waarvan het gebruik wordt gerapporteerd
| Subworkload | Subworkload waarvoor gebruik wordt gerapporteerd (vergaderingen, oproepen of telefoonsystemen) | 
| Aantal vergadering | Aantal vergaderingen | 
| Duur van vergadering | Totale duur vergadering in uren | 

### <a name="teams-monthly-usage-report"></a>**Teams maandelijks gebruiksrapport maken**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId |    Id van het globale partneraccount MPN |
| CustomerTenantId |    Tenant-id van de klant|
| CustomerId |  Id van het bovenliggende bovenliggende klant|
| MonthKey |    Maand waarvoor gebruik wordt gerapporteerd|
| SubWorkload | Subworkload waarvoor gebruik wordt gerapporteerd (vergaderingen, oproepen of telefoonsystemen)|
| DesktopUsers |    Aantal gebruikers dat Teams desktopcomputer|
| MobileUsers | Aantal gebruikers dat Teams mobiel gebruikt|
| WebUsers |    Aantal gebruikers dat Teams op internet|
| AllUpParticiement |   Aantal unieke gebruikers van Teams voor de maand|

### <a name="teams-usage-3p-apps-report"></a>**Teams 3P-apps voor gebruik**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId  | Id van het globale partneraccount MPN |
| CustomerTenantId |    Tenant-id van de klant |
| CustomerId |  Bovenliggende id van klant |
| CustomerName |    Klantnaam |
| CustomerCountry | Land van klant |
| DateKey | Datum waarvan het gebruik wordt gerapporteerd |
| Appname | Naam van de Teams app |
| Aantal gebruikers |   Aantal gebruikers voor de app |

### <a name="training-details-report"></a>**Rapport met trainingsdetails**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId  | Id van het globale partneraccount MPN |
| TrainingActivityId | Id van de training | 
| TrainingTitle | Titel van de training | 
| TrainingType | Type training (certificering of examen) | 
| IndividualFirstName | Voornaam van de klant | 
| IndividualLastName | Achternaam van de klant | 
| Email | Persoonlijke e-mail-id van de klant | 
| CorpEmail | Office-e-mail-id van de klant | 
| TrainingCompletionDate | Voltooiingsdatum van de training | 
| Vervaldatum |  Vervaldatum van de certificering|
| ActivationStatus |    Status van de certificering|
| Maand | Maand waarvoor de gegevens worden gerapporteerd | 
| IcMCP | Geeft aan of de gebruiker een Microsoft Certified Professional (MCP) is | 
| MCPID | MCP-id van de gebruiker | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | Naam van de partner | 
| PartnerCityLocation | Geografische plaats van de partnerlocatie | 
| PartnerCountryLocation | Geografische landlocatie van de partner | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn rapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| PGAMpnId  | Id van het globale partneraccount MPN |
| UserName | Naam van de gebruiker | 
| UserId | GUID van de gebruiker | 
| TrainingName | Naam van de training | 
| TrainingType | Type training (module of leertraject) | 
| Producten | Product waarvoor de leermodule van toepassing is | 
| Rollen | Toepasselijke rollen van de training | 
| CompletionDate | Datum waarop de training is voltooid | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | Naam van de partner | 
| Land/regio | Geografische landlocatie van de partner | 

### <a name="competency-summary-and-history-report"></a>**Competentieoverzicht en geschiedenisrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CompetencyName | Naam van de competentie | 
| CompetencyLevel | Niveau van de competentie (Gold of Silver) | 
| CompetencyStatus | Huidige status van de competentie (actief, inactief of in respijtperiode) | 
| CompetencyStartDate | Begindatum van de competentie | 
| CompetencyEndDate | Einddatum van de competentie | 

### <a name="competency-performance-report"></a>**Rapport Competentieprestaties**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CompetencyName | Naam van de competentie | 
| CompetencyAttainmentOptionName | Naam van de optie voor het bereiken van competentie | 
| Maand | Maand waarvoor de metrische gegevens worden gerapporteerd | 
| MetricName | Naam van de metrische gegevens die relevant zijn voor de competentie | 
| MetricMonthlyContribution | Maandelijkse bijdrage van de metrische gegevens | 
| TTMAggregate | Geaggregeerde metrische gegevens voor de na 12 maanden | 
| AnniversaryYearAggregate | Geaggregeerde metrische gegevens voor het huidige jubileumjaar | 
| GoldThreshold | Prestatievereiste om te voldoen aan Gold-competentie | 
| SilverThreshold | Prestatievereiste om te voldoen aan Silver-competentie | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent - Microsoft 365 propensiteitsrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network ID | 
| Partnernaam | Naam van de partner | 
| Klant-ID | Id-nummer van de klant | 
| DUNS-nummer | Het nummer van Dun & Brad serienummer (D&B) van de klant die wordt scoren voor goedheid | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Organisatiegrootte | Grootte van de organisatie | 
| Branche | Branche waar de organisatie bij hoort | 
| Verticaal | De verticale positie van de klant die wordt scoren op basis van de normen van Microsoft, D&B en andere industriestandaarden | 
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochteronderneming van de klant die wordt scoren voor reensiteit | 
| Verkoopterritorium | Het verkoopgebied van de klant die wordt scoren op reensiteit | 
| Plaats | Geografische plaats van de organisatie | 
| Staat | Geografische statuslocatie van de organisatie | 
| Postcode | Postcode van de organisatie | 
| Land/regio | Geografische landlocatie van de organisatie | 
| Segment | Marktsegment | 
| Subsegment | Marktsubsegment | 
| Samenvatting SMC-type | SMC-type | 
| Top Unmanaged - Compute Base | Belangrijkste niet-mande klanten : rekenkracht | 
| Top Unmanaged - Gebruikersbasis | Belangrijkste niet-mande klanten - gebruiker | 
| IsNonProfit | Geeft aan of de organisatie non-profitorganisatie is (Ja of Nee) | 
| Extern werk inschakelen - Exchange Online | Klanten die een actief Exchange Online hebben, worden upsell aan Microsoft 365 | 
| Extern werk inschakelen - on-premises aanschaf (huidige versie) met Cloud Ascent-ondersteuning - +10 licenties | Klant met een huidige on-premises Office of Windows client. Dat wil zeggen dat de clientversie hoger is dan een end-of-life-versie (EOL). De klant heeft 10 of meer licenties. Klant die een reensiteitsscore heeft. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (huidige versie) met Cloud Ascent-ondersteuning - <10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 10 licenties. Klant die een reensiteitsscore heeft. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (huidige versie) zonder Cloud Ascent-ondersteuning - +10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft 10 of meer licenties. De klant heeft geen reactiviteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (huidige versie) zonder Cloud Ascent-ondersteuning - <10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 10 licenties. De klant heeft geen reactiviteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen : on-premises aanschaf (EOL-versie) met Cloud Ascent-ondersteuning - +10 licenties | Klant die een on-premises EOL-Office of Windows client (dat wil zeggen, een EOL-versie of eerder). De klant heeft 10 of meer licenties. De klant heeft een propensiteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen : on-premises aanschaf (EOL-versie) met Cloud Ascent-ondersteuning - <10 licenties | Klant die een on-premises EOL-Office of Windows client (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan 10 licenties. De klant heeft een propensiteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen : on-premises aanschaf (EOL-versie) zonder Cloud Ascent-ondersteuning - +10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een EOL-versie of eerder). De klant heeft 10 of meer licenties. De klant heeft geen reactiviteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen : on-premises aanschaf (EOL-versie) zonder Cloud Ascent-ondersteuning - <10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan 10 licenties. De klant heeft geen reactiviteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen: prospect met hoge mate van Microsoft 365 (Act NowithEvaluate) | Potentiële klant met hoge reactiviteit voor Microsoft 365 | 
| Extern werk inschakelen : concurreren (Zoom) met Microsoft 365 | Klant met Zoom en Microsoft 365, doel voor conversie naar Teams | 
| Extern werk inschakelen : concurreren (Zoom) zonder Microsoft 365 | Klant met Zoom, doel voor conversie naar Teams | 
| Kosten en beheer verlagen - Microsoft 365 E3 gericht op Microsoft 365 E5 | Bestaande klant met Microsoft 365 E3, doel voor Microsoft 365 E5 | 
| Kosten verlagen en beheren: Microsoft 365 Business Basic en Business Standard-klanten die zijn gericht op Microsoft 365 Business Premium | Bestaande Microsoft 365 Business Basic en Business Standard-klanten, doel voor Microsoft 365 Business Premium | 
| Organisatieproductiviteit transformeren - Surface propensity | Klant toont een gelijkenis voor Surface | 
| M365Cluster | Identificeert de wil van een klant om een Microsoft 365. Target Act Now en Evaluate clusters omdat ze een hoger rendement opleveren. Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted. | 
| M365Fit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste kleine of middelgrote bedrijven (SMB's) om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| M365Intent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Het scoren van intenties wordt over de passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
| SurfaceCluster | Identificeert de wil van een klant om Surface aan te schaffen door de aanbevelingen voor aanpassen en intentie in een cluster samen te brengen. Target Act Now en Evaluate clusters omdat ze een hoger rendement opleveren. Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted. | 
| SurfaceFit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB's om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| SurfaceIntent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Het scoren van intenties wordt over de passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
| O365Cluster | Identificeert de wil van de klant om een Office 365. Target Act Now en Evaluate clusters omdat ze een hoger rendement opleveren. Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted. | 
| O365Fit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB's om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| O365Intent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Het scoren van intenties wordt over de passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
| M365UpsellCustomer | Hiermee wordt aangegeven of de klant de verkoopaandedigheid voor de Microsoft 365 | 
| Heeft Google | Identificeert of de klant concurrerende signalen toont voor het bezit van Google-producten | 
| Heeft AWS | Identificeert of de klant concurrerende signalen toont voor het Amazon Web Services (AWS)-producten | 
| Heeft EA | Hiermee wordt aangegeven of een verlenging een Enterprise Agreement (EA) of een EA-abonnement is | 
| Is geopend | Hiermee wordt aangegeven of een verlenging een Open- of Open Value-overeenkomst is | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent - Dynamics 365-reensiteitsrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network-id (MPN) | 
| Partnernaam | Naam van de partner | 
| Klant-ID | Klant-id-nummer | 
| DUNS-nummer | Het Dun & Brad gaat over het nummer van de klant die wordt scoren voor goedheid | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Organisatiegrootte | Grootte van de organisatie | 
| Branche | Branche waar de organisatie deel van uit maakt | 
| Verticaal | De verticale van de klant die wordt scoren op basis van de normen van Microsoft, D&B en andere industriestandaarden
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochteronderneming van de klant die wordt scoren voor goedheid | 
| Verkoopterritorium | Het verkoopgebied van de klant die wordt scoren voor goedheid | 
| Plaats | Geografische plaatslocatie | 
| Staat | Geografische statuslocatie | 
| Postcode | Postcode van de organisatie | 
| Land/regio | Geografische landlocatie | 
| Segment | Marktsegment | 
| Subsegment | Marktsubsegment | 
| Samenvatting van SMC-type | De categorisatie van een klant: De belangrijkste onmanagede gebruikersbases zijn klanten met meer dan 300 werknemers, de belangrijkste onmanagede rekenbases zijn klanten met een potentieel van USD 10.000 in Azure voor drie jaar, middelgrote bedrijven zijn klanten met 25 werknemers of meer en kleine bedrijven zijn klanten met minder dan 25 werknemers. | 
| Top onmanaged - Rekenbasis | Belangrijkste onmanagede klanten - compute | 
| Top Onmanaged - Gebruikersbasis | Belangrijkste onmanagede klanten : gebruikers | 
| IsNonProfit | Geeft aan of de organisatie non-profitorganisatie is (Ja of Nee) | 
| Digitale verkoop activeren - Microsoft 365 - grootte van >= 25 seats (SalesPro-propensiteitsmodel) | Klant zonder Dynamics 365. Seatgrootte: 25+. Partner moet gericht zijn op cross-sell van Dynamics 365 SalesPro. | 
| Digitale verkoop activeren - Dynamics 365 SalesPro-reensiteit (nu actie ondernemen of evalueren) | Klanten met een hoge mate van eigenaarschap zonder Dynamics 365. Partner moet zich richten op Dynamics 365 SalesPro. | 
| Managing Financial Risk & Fraud - Dynamics on-premises install base - Navision (Business Central propensity model) | Bestaande klant met on-premises Navision. Partner moet zich richten op Dynamics 365 Business Central. | 
| Managing Financial Risk & Fraud - Dynamics on-premises install base - Dynamics AX (Dynamics 365 Finance + Operations propensity model) | Bestaande klant met on-premises AX. Partner moet zich richten op Dynamics 365 Finance + Operations. | 
| Managing Financial Risk & Fraud - Dynamics on-premises install base - Great Plains (Business Central propensity model) | Bestaande klant met on-premises Great Plains. Partner moet zich richten op Dynamics 365 Business Central. | 
| Managing Financial Risk & Fraud - Dynamics on-premises install base - Managing Financial Risk & Fraud - Dynamics on-premises install base - Managing Financial Risk & Fraud - Business Central propensity model) | Bestaande klant met on-premises Premise. Partner moet zich richten op Dynamics 365 Business Central. | 
| Managing Financial Risk & Fraud - Dynamics on-premises install base - Others (Business Central propensity model) | Bestaande klant met andere on-premises oplossingen die niet eerder worden vermeld. Partner moet zich richten op Dynamics 365 Business Central. | 
| Agile bedrijfsprocessen bouwen - Dynamics on-premises installatiebasis - AX/GP/SL/NAV/Other (Dynamics 365-bedrijfsmodel) | Agile bedrijfsprocessen bouwen - Dynamics on-premises installatiebasis - AX/GP/SL/NAV/Other (Dynamics 365-bedrijfsmodel) | 
| Agile bedrijfsprocessen bouwen - Dynamics-concurrentiebasis - Mendix/OutSystems/Salesforce (Dynamics 365-bedrijfsmodel) | Flexibele bedrijfsprocessen bouwen - Dynamics concurreert als basis - Mendix/OutSystems/Salesforce (Dynamics 365-bedrijfsmodel) | 
| Agile bedrijfsprocessen bouwen - Dynamics 365 Finance + Operations install base | Bestaande klanten van Dynamics 365 Finance + Operations. Partner voor doel Power Apps. | 
| Flexibele bedrijfsprocessen bouwen - Dynamics 365 Business Central-installatiebasis | Bestaande Klanten van Dynamics 365 Business Central. Partner voor doel Power Apps. | 
| Flexibele bedrijfsprocessen bouwen - Dynamics 365 Customer Engagement-installatiebasis | Bestaande Klanten van Dynamics 365 Customer Engagement. Partner voor doel Power Apps. | 
| Een Resilient Supply Chain bouwen - Windows en activeer de eerste Dynamics 365-workload als Dynamics 365 Supply Chain Management met klanten die geen Oracle of SAP ERP (enterprise resource planning) hebben | Doelklanten voor Dynamics 365 Supply Chain Management | 
| Een flexibele toeleveringsketen bouwen : Dynamics 365 Supply Chain Management en/of Retail of Commerce kruisverkopen aan bestaande Klanten van Dynamics 365 Customer Engagement | Bestaande Klanten van Dynamics 365 Customer Engagement zijn gericht op cross-selling dynamics 365 Supply Chain Management. | 
| Een flexibele toeleveringsketen bouwen : Dynamics 365 Supply Chain Management en/of Retail of Commerce kruisverkopen aan Dynamics 365 Customer Engagement en Oracle of SAP | Bestaande Klanten van Dynamics 365 Customer Engagement met Oracle of SAP als doel voor Dynamics 365 Supply Chain Management | 
| D365BCCluster | Identificeert de wil van de klant om Dynamics 365 Business Central aan te schaffen. Klanten die een eigenheid voor Business Central tonen, vallen in de categorieën Gemiddeld en Klein. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt u op Nurture en richt u op klanten alleen als er nog capaciteit is nadat u Zich hebt gericht op Nu reageren en Klanten evalueren. | 
| D365BCFit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| D365BCIntent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Het scoren van intenties wordt over de passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
| D365FOCluster | Identificeert de wil van de klant om Dynamics 365 Finance and Operations aan te schaffen. Klanten die een eigenaar voor Finance + Operations tonen, staan in de bovenste onmanagede categorieën. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt u op Nurture en richt u op klanten alleen als er nog capaciteit is nadat u Zich hebt gericht op Nu reageren en Klanten evalueren. | 
| D365FOFit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| D365FOIntent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Het scoren van intenties wordt over de passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
| D365CECluster | Identificeert de wil van de klant om Dynamics 365 Customer Engagement aan te schaffen. Klanten die klantbetrokkenheid tonen, vallen in de categorieën Gemiddeld en Klein. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt u op Nurture en richt u op klanten alleen als er nog capaciteit is nadat u Zich hebt gericht op Nu reageren en Klanten evalueren. | 
| D365CEFit | Geeft aan dat deze geschikt is voor Dynamics 365 Customer Engagement | 
| D365CEIntent | Geeft de intentie aan voor Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identificeert of de klant een open verlenging heeft voor Dynamics on-premises AX of CRM | 
| M365UpsellCustomer | Hiermee wordt aangegeven of de klant de verkoopaandedigheid voor de Microsoft 365 | 
| Heeft Google | Identificeert of de klant concurrerende signalen toont voor het bezit van Google-producten | 
| Heeft AWS | Identificeert of de klant concurrerende signalen toont voor het bezit van AWS-producten | 
| Heeft EA | Hiermee wordt aangegeven of een verlenging een EA- of EEN EA-abonnement is | 
| Is geopend | Hiermee wordt aangegeven of een verlenging een Open- of Open Value-overeenkomst is | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent - Azure-ondersteuningsrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network-id (MPN) | 
| Partnernaam | Naam van de partner | 
| Klant-ID | Klant-id-nummer | 
| DUNS-nummer | Het Dun & Brad serienummer van de klant die wordt scoren voor goedheid | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Organisatiegrootte | Grootte van de organisatie | 
| Branche | Branche | 
| Verticaal | De verticale van de klant die wordt scoren voor 'eigenheid', zoals aangegeven door Microsoft, D&B en andere industriestandaarden | 
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochteronderneming van de klant die wordt scoren voor goedheid | 
| Verkoopterritorium | Het verkoopgebied van de klant die wordt scoren voor goedheid | 
| Plaats | Geografische plaatslocatie | 
| Staat | Geografische statuslocatie | 
| Postcode | Postcode van de organisatie | 
| Land/regio | Geografische landlocatie | 
| Segment | Marktsegment | 
| Subsegment | Marktsubsegment | 
| Samenvatting van SMC-type | SMC-type | 
| Top onmanaged - Rekenbasis | Belangrijkste onmanagede klanten - compute | 
| Top Onmanaged - Gebruikersbasis | Belangrijkste onmanagede klanten : gebruikers | 
| IsNonProfit | Geeft aan of de organisatie non-profitorganisatie is (Ja of Nee) | 
| Migreren - EOL Windows Server - EOL Windows Server IB met Cloud Ascent-eigenheid - meer dan 5 licenties | Klant met een on-premises EOL-Windows Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft vijf of meer licenties. Klant die een reensiteitsscore heeft. Partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL Windows Server - EOL Windows Server IB met Cloud Ascent-eigenheid - <5 licenties | Klant met een on-premises EOL-Windows Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan vijf licenties. Klant die een reensiteitsscore heeft. Partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL Windows Server - EOL Windows Server IB zonder Cloud Ascent-eigenheid - 5+ licenties | Klant met een on-premises EOL-Windows Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft meer dan 5 licenties. De klant heeft geen reactiviteitsscore. Partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL Windows Server - EOL Windows Server IB zonder Cloud Ascent-toestemming - <5 licenties | Klant met een on-premises EOL-Windows Server (dat wil zeggen, een EOL-versie of eerder). Heeft minder dan 5 licenties. De klant heeft geen reactiviteitsscore. Partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL SQL - EOL SQL Server IB met Cloud Ascent-propensiteit - 5+ licenties | Klant met een on-premises EOL-SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft meer dan 5 licenties. De klant heeft een propensiteitsscore. Partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL SQL - EOL SQL Server IB met Cloud Ascent-propensiteit - <5 licenties | Klant met een on-premises EOL-SQL Server (dat wil zeggen, een EOL-versie of eerder). Heeft minder dan 5 licenties. Klant die een reensiteitsscore heeft. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL SQL - EOL SQL Server IB zonder Cloud Ascent-eigenheid - meer dan 5 licenties | Klant met een on-premises EOL-SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft vijf of meer licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL SQL - EOL SQL Server IB zonder Cloud Ascent-eigenheid - <5 licenties | Klant met een on-premises EOL-SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan vijf licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - On-premises Windows Server migreren - huidige Windows Server-IB met Cloud Ascent-propensiteit - meer dan 5 licenties | Klant met een huidige on-premises Windows Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft meer dan 5 licenties. De klant heeft een reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar on-premises Windows Server - huidige Windows Server-IB met Cloud Ascent-propensiteit - <5 licenties | Klant met een huidige on-premises Windows Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan vijf licenties. De klant heeft een reensiteitsscore voor Azure. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - On-premises Windows-server migreren - huidige Windows Server-IB zonder Cloud Ascent-propensiteit - meer dan 5 licenties | Klant met een huidige on-premises Windows Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft meer dan 5 licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - On-premises Windows Server migreren - huidige Windows Server-IB zonder Cloud Ascent-propensiteit - <5 licenties | Klant met een huidige on-premises Windows Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan vijf licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar Azure SQL of SQL virtuele machines (VM's) - huidige SQL Server IB met Cloud Ascent-ondersteuning - meer dan 5 licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft meer dan 5 licenties. De klant heeft een reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar Azure SQL of SQL-VM's - huidige SQL Server IB met Cloud Ascent-ondersteuning - <5 licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan vijf licenties. De klant heeft een reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar Azure SQL of SQL-VM's - huidige SQL Server IB zonder Cloud Ascent-ondersteuning - 5+ licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft meer dan 5 licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar Azure SQL of SQL-VM's - huidige SQL Server IB zonder Cloud Ascent-ondersteuning - <5 licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan vijf licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - OSS - Migreren naar Open Source Shakespeare (OSS) DB | Bestaande klant met een van de volgende producten: PostgreSQL, MySQL, MariaDB. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - OSS - Linux op Azure | Bestaande klant met Linux. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - SAP - SAP on Azure | Bestaande klant met SAP. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Windows Virtual Desktop - Extern bureaublad-services IB | Identificeert klanten met actieve Windows Extern bureaublad-services. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Windows Virtual Desktop - Modern werk kruisver verkopen aan Azure/WVD | Identificeert klanten Microsoft 365 en heeft geen Azure. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - VMware IB | Bestaande klant met het product: VMware. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Citrix IB | Bestaande klant met het product: Citrix Systems. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Innoveren - Analyse - IB Power BI met een hoge Azure-reensiteit | Klanten met een actief Power BI-abonnement, waaronder: Power BI - standalone Pro, Power BI - Azure Suites, Power BI - Office Suites, Power BI Suites - Microsoft 365 | 
| Inschakelen - DevOps met GitHub - Visual Studio/MSDN IB | Identificeert klanten met actieve Visual Studio versies | 
| Windows Standaardversie van server | Geeft de versie weer van Windows Server Standard-aankopen door de klant | 
| Windows Server Standard-licentie | Geeft het licentietype weer van Windows Server Standard-aankopen door de klant | 
| Windows Server Data Center-versie | Geeft de versie weer van Windows datacenteraankopen door de klant | 
| Windows Server Data Center-licentie | Geeft het licentietype weer van Windows datacenteraankopen door de klant | 
| AzureFit | Interne en externe gegevenspunten die firmographics definiëren. Score aanpassen maakt gebruik van een vergelijkbaar model voor onze beste SMB om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| AzureIntent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Intentiescores worden over elkaar heen in Passend om de clusters te definiëren. Intentiescores worden maandelijks bijgewerkt. | 
| AzureCluster | Identificeert de reensiteit van de klant om Azure aan te schaffen door de aanbevelingen voor Aanpassen en Intentie in een cluster samen te brengen. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Nu handelen hebt gericht en klanten evalueren. | 
| WindowsServerDataCenter_HasOpenRenewal | Identificeert of de klant een open verlenging heeft voor Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Identificeert of de klant een open verlenging heeft voor Windows Server Standard | 
| AzureUpsellCustomer | Identificeert of de klant verkoopaandedensiteit voor Azure laat zien | 
| Heeft Google | Identificeert of de klant concurrerende signalen toont voor het bezit van Google-producten | 
| Heeft AWS | Identificeert of de klant concurrerende signalen toont voor AWS-producten die eigenaar zijn | 
| Heeft EA | Hiermee wordt aangegeven of een verlenging een EA- of EEN EA-abonnement is | 
| Is geopend | Hiermee wordt aangegeven of een verlenging een Open- of Open Value-overeenkomst is | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent - rapport over verlenging van overeenkomst**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network ID | 
| Partnernaam | Naam van de partner | 
| Klant-ID | Klant-id-nummer | 
| DUNS-nummer | Het Dun & Brad gaat over het nummer van de klant die wordt scoren voor goedheid | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Organisatiegrootte | Grootte van de organisatie | 
| Branche | Branche | 
| Verticaal | De verticale positie van de klant die wordt scoren voor 'propensiteit', zoals aangegeven door Microsoft, D&B en andere industriestandaarden | 
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochteronderneming van de klant die wordt scoren voor reensiteit | 
| Verkoopterritorium | Het verkoopgebied van de klant die wordt scoren op reensiteit | 
| Plaats | Geografische plaatslocatie | 
| Staat | Geografische statuslocatie | 
| Postcode | Postcode van de organisatie | 
| Land/regio | Geografische landlocatie | 
| Segment | Marktsegment | 
| Subsegment | Marktsubsegment | 
| Samenvatting SMC-type | SMC-type | 
| Top Unmanaged - Compute Base | Belangrijkste niet-mande klanten : rekenkracht | 
| Top Unmanaged - Gebruikersbasis | Belangrijkste niet-mande klanten : gebruikers | 
| IsNonProfit | Geeft aan of de organisatie non-profitorganisatie is (Ja of Nee) | 
| Heeft Google | Identificeert of de klant concurrerende signalen toont voor AWS-producten die eigenaar zijn | 
| Heeft AWS | Identificeert of de klant concurrerende signalen toont voor AWS-producten die eigenaar zijn | 
| Azure-cluster | Identificeert de reensiteit van de klant om Azure aan te schaffen. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Nu handelen hebt gericht en klanten evalueren. | 
| D365 Finance + Operations Cluster | Identificeert de reensiteit van de klant om Dynamics 365 Finance and Operations aan te schaffen. Klanten die een reensiteit voor Finance + Operations tonen, worden in de bovenste onmanaged categorieën ingedeeld. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Nu handelen hebt gericht en klanten evalueren. | 
| D365 CE-cluster | Identificeert de reensiteit van de klant om Dynamics 365 Customer Engagement aan te schaffen. Klanten die klantbetrokkenheid tonen, vallen in de categorieën Gemiddeld en Klein. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Nu handelen hebt gericht en klanten evalueren. | 
| D365 BC-cluster | Identificeert de reensiteit van de klant om Dynamics 365 Business Central aan te schaffen. Klanten die een gelijkenis voor Business Central tonen, vallen in de categorieën Gemiddeld en Klein. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Nu handelen hebt gericht en klanten evalueren. | 
| Microsoft 365 Cluster | Identificeert de reensiteit van de klant om een Microsoft 365. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Nu handelen hebt gericht en klanten evalueren. | 
| Licentieprogramma | Identificeert het type licentieprogramma voor de verlenging | 
| Overeenkomst-id | Id van de overeenkomst | 
| Einddatum overeenkomst | Einddatum van de overeenkomst | 
| Verlooptype | Type verloopdatum | 
| Verlopende omzet | Omzet die is gekoppeld aan verlopen abonnementen | 
| Heeft EA | Hiermee wordt aangegeven of een verlenging een EA- of EEN EA-abonnement is | 
| Is geopend | Hiermee wordt aangegeven of een verlenging een Open- of Open Value-overeenkomst is | 
| Azure Upsell-klant | Identificeert of de klant verkoopaandedendheid voor Azure laat zien | 
| Microsoft 365 Upsell-klant | Hiermee wordt aangegeven of de klant de verkoopaandedigheid voor de Microsoft 365 | 
| RevSumDivisionName | Identificeert het product dat kan worden verlengd | 

### <a name="cpor-m365usage-report"></a>**CPOR-M365Usage-rapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-id van de klant | 
| CustomerName | Naam van de klant | 
| WorkloadName | Naam van de workload | 
| MonthlyActiveUsers | MAU (maandelijks actieve gebruikers) | 
| PaidAvailableUnits | PAU (betaalde beschikbare eenheden) | 
| ClaimId | Claim-id van de workload | 
| MpnId | Microsoft Partner Network-id (MPN) | 
| DateAssociated | Gekoppelde datum van de workload met de partner | 
| PartnerAttributionType | Type partnervermelding (CPOR) | 
| Datum | Datum (eerste van maand en jaar) waarvoor de gegevens worden geëxporteerd | 

## <a name="next-steps"></a>Volgende stappen

Zie Rapporten downloaden [voor meer informatie.](insights-download-reports.md)
