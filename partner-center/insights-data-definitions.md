---
title: Definities van inzichtengegevens
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Het document bevat verschillende rapporten en hun gegevensdefinities, die u kunt downloaden van de Insights Rapport downloaden.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c77f5eb97771c4768f76b8d35c0d4493c5070ff2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376781"
---
# <a name="export--data-definitions"></a>Exporteren : gegevensdefinities 

**Juiste rollen:** Rapportviewer | Rapportviewer voor leidinggevenden

## <a name="introduction"></a>Introductie 

Met behulp van de hub Rapporten downloaden op Insights dashboard kunt u de onbewerkte gegevenssets exporteren. 

De verschillende rapporten die u samen met de gegevensdefinities kunt downloaden, worden vermeld in de volgende tabellen: 

### <a name="partner-profile-report"></a>**Partnerprofielrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| MPNId | Microsoft Partner Network-id (MPN)| 
| PartnerName | Naam van de partner | 
| PGA_MPNId | Id van het globale partneraccount MPN | 
| PGA_PartnerName | Naam globale partneraccount | 
| Plaats | Plaats van de partnerlocatie | 
| Land/regio | Landlocatie van de partner | 
| HierarchyLevel | Geeft aan of het een globale MPN-id of locatie-MPN-id is | 

### <a name="customer-details-report"></a>**Rapport klantdetails**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | Id van de tenant van de klant | 
| CustomerTpid | Id van het bovenliggende bovenliggende klant | 
| CustomerSegment | Klantsegment | 
| CustomerMarket | Geografische markt van de klant | 
| CustomerStatus | Klantstatus (actief of inactief) | 
| Product | Het product dat aan de klant is verkocht via MPN: Office 365, Dynamics 365, Enterprise Mobility and Security, Power BI of Microsoft Azure | 
| SKU | Product-SKU | 
| Maand | Maand waarvoor gebruik en omzet worden gerapporteerd | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | Naam van de partner | 
| PartnerLocation | Geografische locatie van de partner | 
| PartnerAttributionType | Toeschrijvingstype van de partner | 
| SalesChannel | Verkoopkanaal | 
| AvailableSeats | Beschikbare seats | 
| RevenueUSD | Omzet in Amerikaanse dollars | 

### <a name="reseller-performance-report"></a>**Prestatierapport reseller**

> [!Note]
> Gegevens over omzet en door Azure verbruikte omzet (ACR) zijn alleen beschikbaar voor gebruikers die een executive rapport hebben.

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| ResellerMPNid | Id van Microsoft Partner Network reseller | 
| ResellerName | Reseller name | 
| ResellerMarket | Land van de reseller van de markt | 
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
| SubscriptionId | GUID van het abonnement | 
| SubscriptionStartDate | Begindatum van het abonnement | 
| SubscriptionEndDate | Einddatum van het abonnement | 
| SubscriptionState | Status van het abonnement (actief of verloop) | 
| Maand | Maand waarvoor gebruik en omzet worden gerapporteerd | 
| IsAutoRenew | Geeft aan of het abonnement automatisch wordt verlengen (Ja of Nee) | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | GUID van de klant | 
| CustomerTpid | Bovenliggende id van klant | 
| CustomerSegment | Marktsegment van de klant | 
| CustomerMarket | Geografische markt van de klant | 
| Product | Product verkocht aan de klant door de partner | 
| SKU | SKU van het product | 
| MPNId | Microsoft Partner Network id van de partner | 
| PartnerName | Naam van de partner | 
| PartnerLocation | Geografische locatie van de partner | 
| PartnerAttributionType | Toeschrijvingstype voor het abonnement | 
| SalesChannel | Verkoopkanaal: direct, Cloud Solution Provider (CSP), e.d. | 
| AvailableSeats | Huidige beschikbare seat | 
| RevenueUSD | Omzet in Amerikaanse dollars | 
| Inschrijvings-id | Inschrijvings-id van het abonnement | 

### <a name="azure-usage-report"></a>**Azure-gebruiksrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| SubscriptionId | GUID van het abonnement | 
| SubscriptionStartDate | De datum van het begin van het abonnement | 
| SubscriptionEndDate | De datum van het einde van het abonnement | 
| SubscriptionState | Huidige status van het abonnement (open, gesloten, actief of in respijtperiode) | 
| Maand | Datum geaggregeerd per maand | 
| ServiceName | Naam van de Azure-service | 
| MeterCategory | Naam van de metercategorie | 
| UsageUnits | Het aantal eenheden dat wordt gebruikt tijdens de factureringscyclus | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | Tenant-id van de klant | 
| CustomerTpid | Bovenliggende id van klant | 
| CustomerSegment | Segment van de klant | 
| CustomerMarket | Geografische markt van de klant | 
| MPNId | Microsoft Partner Network-id van de klant | 
| PartnerName | Naam van de partner | 
| PartnerLocation | Geografische landlocatie van de partner | 
| PartnerAttributionType | Toeschrijvingstype van de partner | 
| SalesChannel | Verkoopkanaal (Direct/CSP, Indirect/CSP, Direct, e.d.) | 
| ACR_USD | Verbruikte ACR (Azure Consumed Revenue) in Amerikaanse dollars | 
| Inschrijvings-id | Inschrijvings-id van het Azure-abonnement | 

### <a name="office-365-license-usage-report"></a>**Office 365 licentiegebruiksrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
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

### <a name="enterprise-mobility-license-usage-report"></a>**Gebruiksrapport voor Enterprise Mobility-licenties**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-id van de klant | 
| CustomerTpid | Bovenliggende id van klant | 
| WorkloadName | Naam van de Enterprise Mobility + Security workload (EMS) | 
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

### <a name="dynamics-365-license-usage-report"></a>**Gebruiksrapport voor Dynamics 365-licenties**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
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
| AvailableSeats | Huidige beschikbare seat | 
| Toegewezen toegewezen taken | Huidige toegewezen seat | 
| ActiveSeats | Huidige actieve seats | 
| ImplementatieOpportunity | Huidige implementatiekans | 
| ActiveUsagePercent | Huidig actief gebruikspercentage | 

### <a name="power-bi-license-usage-report"></a>**Power BI licentiegebruiksrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
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
| AvailableSeats | Huidige beschikbare seats | 
| ToegewezenSeats | Huidige toegewezen seats | 
| ActiveSeats | Huidige actieve seats | 
| DeploymentOpportunity | Huidige implementatiekans | 
| ActiveUsagePercent | Huidig actief gebruikspercentage | 

### <a name="teams-meetings-and-calls-report"></a>**Teams en aanroepen rapporteren**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-id van de klant | 
| CustomerTpid | Id van het bovenliggende bovenliggende klant | 
| Maand | Maand waarvoor gebruik wordt gerapporteerd | 
| Subworkload | Subworkload waarvoor gebruik wordt gerapporteerd (vergaderingen, oproepen of telefoonsystemen) | 
| Aantal vergadering | Aantal vergaderingen | 
| Duur van vergadering | Totale duur vergadering in uren | 

### <a name="teams-monthly-usage-report"></a>**Teams maandelijks gebruiksrapport maken**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-id van de klant | 
| CustomerTpid | Id van het bovenliggende bovenliggende klant | 
| Maand | Maand waarvoor gebruik wordt gerapporteerd | 
| Subworkload | Subworkload waarvoor gebruik wordt gerapporteerd (vergaderingen, oproepen of telefoonsystemen) | 
| Desktopgebruikers | Aantal gebruikers dat Teams bureaublad | 
| Mobiele gebruikers | Aantal gebruikers dat mobiele Teams gebruiken | 
| Webgebruikers | Aantal gebruikers dat gebruik Teams op internet | 
| AllUpParticiici | Aantal unieke gebruikers van Teams voor de maand | 

### <a name="teams-usage-3p-apps-report"></a>**Teams rapport met 3P-apps voor gebruik**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-id van de klant | 
| CustomerTpid | Bovenliggende id van klant | 
| Maand | Maand waarvoor gebruik wordt gerapporteerd | 
| Naam van 3P-app | Naam van de Teams app | 
| Aantal gebruikers | Aantal gebruikers voor de app | 


### <a name="training-details-report"></a>**Rapport met trainingsdetails**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| TrainingActivityId | Id van de training | 
| TrainingTitle | Titel van de training | 
| TrainingType | Type training (certificering of examen) | 
| IndividualFirstName | Voornaam van de klant | 
| IndividualLastName | Achternaam van de klant | 
| E-mail | Persoonlijke e-mail-id van de klant | 
| CorpEmail | Office e-mail-id van de klant | 
| TrainingCompletionDate | Voltooiingsdatum van de training | 
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
| UserName | Naam van de gebruiker | 
| UserId | GUID van de gebruiker | 
| TrainingName | Naam van de training | 
| TrainingType | Type training (module of leertraject) | 
| Producten | Product waarvoor de leermodule van toepassing is | 
| Rollen | Toepasselijke rollen van de training | 
| CompletionDate | De datum waarop de training is voltooid | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | Naam van de partner | 
| Land/regio | Geografische landlocatie van de partner | 

### <a name="competency-summary-and-history-report"></a>**Competentieoverzicht en geschiedenisrapport**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| CompetencyName | Naam van de competentie | 
| CompetencyLevel | Niveau van de competentie (Goud of Zilver) | 
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
| MPN-id | Microsoft Partner Network-id | 
| Partnernaam | Naam van de partner | 
| Klant-ID | Id-nummer van de klant | 
| DUNS-nummer | Het nummer van Dun & Brad serienummer (D&B) van de klant die wordt scoren voor goedheid | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Organisatiegrootte | Grootte van de organisatie | 
| Branche | Branche waar de organisatie bij hoort | 
| Verticaal | De verticale positie van de klant die wordt scoren op reensiteit, zoals aangegeven door Microsoft, D&B en andere industriestandaarden | 
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
| Extern werk inschakelen - doel-Exchange Online | Klanten die een actief Exchange Online hebben, worden upsell aan Microsoft 365 | 
| Extern werk inschakelen - on-premises aanschaf (huidige versie) met Cloud Ascent-ondersteuning - +10 licenties | Klant met een huidige on-premises Office of Windows client. Dat wil zeggen dat de clientversie hoger is dan een end-of-life-versie (EOL). De klant heeft 10 of meer licenties. Klant die een reensiteitsscore heeft. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (huidige versie) met Cloud Ascent-ondersteuning - <10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 10 licenties. Klant die een reensiteitsscore heeft. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (huidige versie) zonder Cloud Ascent-ondersteuning - +10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft 10 of meer licenties. De klant heeft geen reensiteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (huidige versie) zonder Cloud Ascent-ondersteuning - <10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 10 licenties. De klant heeft geen reensiteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (EOL-versie) met Cloud Ascent-ondersteuning - +10 licenties | Klant die een on-premises EOL-Office of Windows client (dat wil zeggen, een EOL-versie of eerder). De klant heeft 10 of meer licenties. De klant heeft een reensiteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (EOL-versie) met Cloud Ascent-ondersteuning - <10 licenties | Klant die een on-premises EOL-Office of Windows client (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan 10 licenties. De klant heeft een reensiteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (EOL-versie) zonder Cloud Ascent-ondersteuning - +10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een EOL-versie of eerder). De klant heeft 10 of meer licenties. De klant heeft geen reensiteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen - on-premises aanschaf (EOL-versie) zonder Cloud Ascent-ondersteuning - <10 licenties | Klant met een huidige on-premises Office of Windows client (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan 10 licenties. De klant heeft geen reensiteitsscore. Partner moet worden gericht op conversie naar Microsoft 365. | 
| Extern werk inschakelen : prospect met hoge mate van Microsoft 365 (Act NowithEvaluate) | Prospect-klant met hoge mate van Microsoft 365 | 
| Extern werk inschakelen : concurreren (Zoom) met Microsoft 365 | Klant met Zoom en Microsoft 365, doel voor conversie naar Teams | 
| Extern werk inschakelen : concurreren (Zoom) zonder Microsoft 365 | Klant met Zoom, doel voor conversie naar Teams | 
| Kosten verlagen en beheren - Microsoft 365 E3 gericht op Microsoft 365 E5 | Bestaande klant met Microsoft 365 E3, doel voor Microsoft 365 E5 | 
| Kosten en beheer verlagen - Microsoft 365 Business Basic en Business Standard-klanten die zijn gericht op Microsoft 365 Business Premium | Bestaande Microsoft 365 Business Basic en Business Standard-klanten, doel voor Microsoft 365 Business Premium | 
| Organisatieproductiviteit transformeren - Surface propensity | Klant toont een gelijkenis voor Surface | 
| M365Cluster | Identificeert de reensiteit van een klant om een Microsoft 365. Target Act Now en Evaluate clusters omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat de klanten Nu reageren en evalueren zijn gericht. | 
| M365Fit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste kleine of middelgrote bedrijven (SMB's) om klanten te vergelijken en te zien of ze geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| M365Intent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Intentiescores worden over elkaar heen in Passend om de clusters te definiëren. Intentiescores worden maandelijks bijgewerkt. | 
| SurfaceCluster | Identificeert de wil van een klant om Surface aan te schaffen door de aanbevelingen voor aanpassen en intentie in een cluster samen te brengen. Target Act Now en Evaluate clusters omdat ze een hoger rendement opleveren. Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted. | 
| SurfaceFit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB's om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| SurfaceIntent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Intent scoring wordt over elkaar heen relativeren bij Passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
| O365Cluster | Identificeert de wil van de klant om een Office 365. Target Act Now en Evaluate clusters omdat ze een hoger rendement opleveren. Target Nurture and Educate customers only if there is still capacity after Act Now and Evaluate customers are targeted. | 
| O365Fit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB's om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| O365Intent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Intent scoring wordt over elkaar heen relativeren bij Passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
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
| DUNS-nummer | Het Dun & Brad serienummer van de klant die wordt scoren voor goedheid | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Organisatiegrootte | Grootte van de organisatie | 
| Branche | Branche waar de organisatie deel van uit maakt | 
| Verticaal | De verticale positie van de klant die wordt scoren voor goedheid, zoals aangegeven door Microsoft, D&B en andere industriestandaarden
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochteronderneming van de klant die wordt scoren voor goedheid | 
| Verkoopterritorium | Het verkoopgebied van de klant die wordt scoren voor goedheid | 
| Plaats | Geografische plaatslocatie | 
| Staat | Geografische statuslocatie | 
| Postcode | Postcode van de organisatie | 
| Land/regio | Geografische landlocatie | 
| Segment | Marktsegment | 
| Subsegment | Marktsubsegment | 
| Samenvatting SMC-type | De categorisatie van een klant: De belangrijkste onmanagede gebruikersbases zijn klanten met meer dan 300 werknemers, de belangrijkste on-mande rekenbases zijn klanten met een potentieel van USD 10.000 in Azure voor drie jaar, middelgrote bedrijven zijn klanten met 25 werknemers of meer en kleine bedrijven zijn klanten met minder dan 25 werknemers. | 
| Top Onmanaged - Compute Base | Belangrijkste onmanagede klanten : rekenkracht | 
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
| Agile bedrijfsprocessen bouwen - Dynamics-concurrentiebasis - Mendix/OutSystems/Salesforce (Dynamics 365-bedrijfsmodel) | Flexibele bedrijfsprocessen bouwen - Dynamics-concurrentiebasis - Mendix/OutSystems/Salesforce (Dynamics 365-bedrijfsmodel) | 
| Agile bedrijfsprocessen bouwen - Dynamics 365 Finance + Operations install base | Bestaande klanten van Dynamics 365 Finance + Operations. Partner voor doel Power Apps. | 
| Flexibele bedrijfsprocessen bouwen - Dynamics 365 Business Central-installatiebasis | Bestaande Klanten van Dynamics 365 Business Central. Partner voor doel Power Apps. | 
| Flexibele bedrijfsprocessen bouwen - Dynamics 365 Customer Engagement-installatiebasis | Bestaande Klanten van Dynamics 365 Customer Engagement. Partner voor doel Power Apps. | 
| Een Resilient Supply Chain bouwen - Windows en activeer de eerste Dynamics 365-workload als Dynamics 365 Supply Chain Management met klanten die geen Oracle of SAP ERP (enterprise resource planning) hebben | Doelklanten voor Dynamics 365 Supply Chain Management | 
| Een flexibele toeleveringsketen bouwen : Dynamics 365 Supply Chain Management en/of Retail of Commerce kruisverkopen aan bestaande Klanten van Dynamics 365 Customer Engagement | Bestaande Klanten van Dynamics 365 Customer Engagement zijn gericht op cross-selling dynamics 365 Supply Chain Management. | 
| Een flexibele toeleveringsketen bouwen : Dynamics 365 Supply Chain Management en/of Retail of Commerce kruisverkopen aan Dynamics 365 Customer Engagement en Oracle of SAP | Bestaande Klanten van Dynamics 365 Customer Engagement met Oracle of SAP als doel voor Dynamics 365 Supply Chain Management | 
| D365BCCluster | Identificeert de wil van de klant om Dynamics 365 Business Central aan te schaffen. Klanten die een zakelijkheid voor Business Central tonen, vallen in de categorieën Gemiddeld en Klein. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich hebt gericht op Nu reageren en Klanten evalueren. | 
| D365BCFit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| D365BCIntent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Intent scoring wordt over elkaar heen relativeren bij Passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
| D365FOCluster | Identificeert de wil van de klant om Dynamics 365 Finance and Operations aan te schaffen. Klanten die een eigenaar voor Finance + Operations tonen, staan in de bovenste onmanagede categorieën. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich hebt gericht op Nu reageren en Klanten evalueren. | 
| D365FOFit | Interne en externe gegevenspunten die firmographics definiëren. Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft-cloudproducten. Passend scoren wordt elk kwartaal bijgewerkt. | 
| D365FOIntent | Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie. Intent scoring wordt over elkaar heen relativeren bij Passend om de clusters te definiëren. Het scoren van intenties wordt maandelijks bijgewerkt. | 
| D365CECluster | Identificeert de wil van de klant om Dynamics 365 Customer Engagement aan te schaffen. Klanten die klantbetrokkenheid tonen, vallen in de categorieën Gemiddeld en Klein. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich hebt gericht op Nu reageren en Klanten evalueren. | 
| D365CEFit | Geeft aan dat deze geschikt is voor Dynamics 365 Customer Engagement | 
| D365CEIntent | Geeft de intentie aan voor Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identificeert of de klant een open verlenging heeft voor Dynamics on-premises AX of CRM | 
| M365UpsellCustomer | Hiermee wordt aangegeven of de klant de verkoopaandedigheid voor de Microsoft 365 | 
| Heeft Google | Identificeert of de klant concurrerende signalen toont voor het bezit van Google-producten | 
| Heeft AWS | Identificeert of de klant concurrerende signalen toont voor het in bezit hebben van AWS-producten | 
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
| Verticaal | De verticale van de klant die wordt scoren voor goedheid, zoals aangegeven door Microsoft, D&B en andere industriestandaarden | 
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochteronderneming van de klant die wordt scoren voor goedheid | 
| Verkoopterritorium | Het verkoopgebied van de klant die wordt scoren voor goedheid | 
| Plaats | Geografische plaatslocatie | 
| Staat | Geografische statuslocatie | 
| Postcode | Postcode van de organisatie | 
| Land/regio | Geografische landlocatie | 
| Segment | Marktsegment | 
| Subsegment | Marktsubsegment | 
| SMC-type Samenvatting | SMC-type | 
| Top Unmanaged - Compute Base | Belangrijkste niet-mande klanten : rekenkracht | 
| Top Unmanaged - Gebruikersbasis | Belangrijkste niet-mande klanten : gebruikers | 
| IsNonProfit | Geeft aan of de organisatie non-profitorganisatie is (Ja of Nee) | 
| Migreren - EOL Windows Server - EOL Windows Server IB met Cloud Ascent-eigenheid - meer dan 5 licenties | Klant met een on-premises EOL-Windows Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft vijf of meer licenties. Klant die een reensiteitsscore heeft. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL Windows Server - EOL Windows Server IB met Cloud Ascent-propensiteit - <5 licenties | Klant met een on-premises EOL-Windows Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan vijf licenties. Klant die een reensiteitsscore heeft. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL Windows Server - EOL Windows Server IB zonder Cloud Ascent-eigenheid - meer dan 5 licenties | Klant met een on-premises EOL-Windows Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft meer dan 5 licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL Windows Server - EOL Windows Server IB zonder Cloud Ascent-propensiteit - <5 licenties | Klant met een on-premises EOL-Windows Server (dat wil zeggen, een EOL-versie of eerder). Heeft minder dan 5 licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL SQL - EOL SQL Server IB met Cloud Ascent-eigenheid - meer dan 5 licenties | Klant met een on-premises EOL-SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft meer dan 5 licenties. De klant heeft een reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL SQL - EOL SQL Server IB met Cloud Ascent-eigenheid - <5 licenties | Klant met een on-premises EOL-SQL Server (dat wil zeggen, een EOL-versie of eerder). Heeft minder dan 5 licenties. Klant die een reensiteitsscore heeft. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL SQL - EOL SQL Server IB zonder Cloud Ascent-eigenheid - meer dan 5 licenties | Klant met een on-premises EOL-SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft vijf of meer licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - EOL SQL - EOL SQL Server IB zonder Cloud Ascent-propensiteit - <5 licenties | Klant met een on-premises EOL-SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan vijf licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - On-premises Windows Server migreren - huidige Windows Server-IB met Cloud Ascent-propensiteit - meer dan 5 licenties | Klant met een huidige on-premises Windows Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft meer dan 5 licenties. De klant heeft een reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - On-premises Windows Server migreren - huidige Windows Server-IB met Cloud Ascent-propensiteit - <5 licenties | Klant met een huidige on-premises Windows Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan vijf licenties. De klant heeft een reensiteitsscore voor Azure. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - On-premises Windows Server migreren - huidige Windows Server-IB zonder Cloud Ascent-propensiteit - meer dan 5 licenties | Klant met een huidige on-premises Windows Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft meer dan 5 licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - On-premises Windows Server migreren - huidige Windows Server-IB zonder Cloud Ascent-propensiteit - <5 licenties | Klant met een huidige on-premises Windows Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan vijf licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar Azure SQL of SQL virtuele machines (VM's) - huidige SQL Server IB met Cloud Ascent-ondersteuning - meer dan 5 licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft meer dan 5 licenties. De klant heeft een reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar Azure SQL of SQL-VM's - huidige SQL Server IB met Cloud Ascent-ondersteuning - <5 licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan vijf licenties. De klant heeft een reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar Azure SQL of SQL-VM's - huidige SQL Server IB zonder Cloud Ascent-ondersteuning - 5+ licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft meer dan 5 licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Migreren naar Azure SQL of SQL-VM's - huidige SQL Server IB zonder Cloud Ascent-ondersteuning - <5 licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan vijf licenties. De klant heeft geen reensiteitsscore. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - OSS - Migreren naar Open Source Shakespeare (OSS) DB | Bestaande klant met een van de volgende producten: PostgreSQL, MySQL, MariaDB. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - OSS - Linux op Azure | Bestaande klant met Linux. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - SAP - SAP on Azure | Bestaande klant met SAP. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Windows Virtual Desktop - Extern bureaublad-services IB | Identificeert klanten met actieve Windows Extern bureaublad-services. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
| Migreren - Windows Virtual Desktop - modern werk kruisver verkopen aan Azure/WVD | Identificeert klanten Microsoft 365 en heeft geen Azure. De partner moet deze klant als doel hebben voor migratie naar Azure. | 
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
| AzureCluster | Identificeert de reensiteit van de klant om Azure aan te schaffen door de aanbevelingen voor Aanpassen en Intentie in een cluster samen te brengen. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich richt op Nu reageren en Klanten evalueren. | 
| WindowsServerDataCenter_HasOpenRenewal | Identificeert of de klant een open verlenging heeft voor Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Identificeert of de klant een open verlenging heeft voor Windows Server Standard | 
| AzureUpsellCustomer | Identificeert of de klant verkoopaandedensiteit voor Azure laat zien | 
| Heeft Google | Identificeert of de klant concurrerende signalen toont voor het bezit van Google-producten | 
| Heeft AWS | Identificeert of de klant concurrerende signalen toont voor AWS-producten die eigenaar zijn | 
| Heeft EA | Hiermee wordt aangegeven of een verlenging een EA- of EEN EA-abonnement is | 
| Is geopend | Hiermee wordt aangegeven of een verlenging een Overeenkomst voor open of open waarde is | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent - rapport over verlenging van overeenkomst**

| Kolomnaam | Gegevensbeschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network-id | 
| Partnernaam | Naam van de partner | 
| Klant-ID | Klant-id-nummer | 
| DUNS-nummer | Het Dun & Brad gaat over het nummer van de klant die wordt scoren voor goedheid | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Organisatiegrootte | Grootte van de organisatie | 
| Branche | Branche | 
| Verticaal | De verticale positie van de klant die wordt scoren op reensiteit, zoals aangegeven door Microsoft, D&B en andere industriestandaarden | 
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
| Azure-cluster | Identificeert de reensiteit van de klant om Azure aan te schaffen. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich richt op Nu reageren en Klanten evalueren. | 
| D365 Finance + Operations Cluster | Identificeert de reensiteit van de klant om Dynamics 365 Finance and Operations aan te schaffen. Klanten die een eigenheid voor Finance + Operations hebben, vallen in de bovenste onmanagede categorieën. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich richt op Nu reageren en Klanten evalueren. | 
| D365 CE-cluster | Identificeert de reensiteit van de klant om Dynamics 365 Customer Engagement aan te schaffen. Klanten die klantbetrokkenheid tonen, vallen in de categorieën Gemiddeld en Klein. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich richt op Nu reageren en Klanten evalueren. | 
| D365 BC-cluster | Identificeert de reensiteit van de klant om Dynamics 365 Business Central aan te schaffen. Klanten die een eigenheid voor Business Central hebben, vallen in de categorieën Gemiddeld en Klein. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich richt op Nu reageren en Klanten evalueren. | 
| Microsoft 365 Cluster | Identificeert de reensiteit van de klant om een Microsoft 365. Target Act Now en Evaluate-clusters, omdat ze een hoger rendement opleveren. Richt klanten alleen op Nurture en Opleiden als er nog capaciteit is nadat u Zich richt op Nu reageren en Klanten evalueren. | 
| Licentieprogramma | Identificeert het type licentieprogramma voor de verlenging | 
| Overeenkomst-id | Id van de overeenkomst | 
| Einddatum overeenkomst | Einddatum van de overeenkomst | 
| Verlooptype | Type verloopdatum | 
| Verlopende omzet | Omzet die is gekoppeld aan verlopende abonnementen | 
| Heeft EA | Hiermee wordt aangegeven of een verlenging een EA- of EEN EA-abonnement is | 
| Is geopend | Hiermee wordt aangegeven of een verlenging een Open- of Open Value-overeenkomst is | 
| Azure Upsell-klant | Identificeert of de klant verkoopaandedensiteit voor Azure laat zien | 
| Microsoft 365 Upsell-klant | Hiermee wordt aangegeven of de klant verkoopaandigheid voor de Microsoft 365 | 
| RevSumDivisionName | Identificeert het product dat kan worden verlengd | 

## <a name="next-steps"></a>Volgende stappen

Zie Rapporten downloaden [voor meer informatie.](insights-download-reports.md)
