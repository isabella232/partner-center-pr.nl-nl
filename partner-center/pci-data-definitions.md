---
title: Definities van inzichtengegevens
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: In het document worden verschillende rapporten en hun gegevens definities weer gegeven, die u kunt downloaden via de rapport pagina inzichten downloaden.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861390"
---
# <a name="export--data-definitions"></a>Exporteren – gegevens definities 

 **Juiste rollen** 

- Rapport viewer 
- Rapport Viewer Executive 

## <a name="introduction"></a>Inleiding 

U kunt de onbewerkte gegevens sets exporteren met behulp van de hub voor het downloaden van rapporten op het Insights-dash board. 

De verschillende rapporten, die u samen met hun gegevens definities kunt downloaden, worden weer gegeven in de volgende tabellen: 

### <a name="partner-profile-report"></a>**Partner profiel rapport**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| MPNId | Id van Microsoft Partner Network (MPN) | 
| PartnerName | De naam van de partner | 
| PGA_MPNId | Id van het globale account van de partner MPN | 
| PGA_PartnerName | Globale account naam partner | 
| Plaats | Locatie van de plaats van de partner | 
| Land | Land locatie van de partner | 
| HierarchyLevel | Geeft aan of het een globale MPN-ID of locatie MPN-ID is | 

### <a name="customer-details-report"></a>**Rapport klant Details**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | Id van de Tenant van de klant | 
| CustomerTpid | Id van het bovenste bovenliggende item van de klant | 
| CustomerSegment | Klant segment | 
| CustomerMarket | Geografische markt van de klant | 
| CustomerStatus | Klant status (actief of inactief) | 
| Product | Het product dat aan de klant wordt verkocht door MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI of Microsoft Azure | 
| SKU | Product-SKU | 
| Maand | Maand waarvoor het gebruik en de opbrengst worden gerapporteerd | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | De naam van de partner | 
| Databasenames | Geografische locatie van de partner | 
| PartnerAttributionType | Het type toewijzing van de partner | 
| SalesChannel | Verkoop kanaal | 
| AvailableSeats | Beschik bare stoelen | 
| RevenueUSD | Omzet in Amerikaanse dollars | 

### <a name="reseller-performance-report"></a>**Rapport reseller performance**

> [!Note]
> Opbrengst-en ACR-gegevens zijn alleen beschikbaar voor gebruikers die een leidinggevende rapport kijkers hebben.

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| ResellerMPNid | ID Microsoft Partner Network wederverkoper | 
| ResellerName | Reseller name | 
| ResellerMarket | Land van wederverkoper van de markt | 
| IndirectProviderMPNId | Id van de indirecte provider Microsoft Partner Network | 
| IndirectProviderName | Naam van de indirecte provider | 
| Maand | Maand waarvoor het gebruik en de opbrengst worden gerapporteerd | 
| Product | Productnaam | 
| SubscriptionID | Id van het abonnement | 
| AvailableSeats | Aantal beschik bare seats | 
| AssignedSeats | Aantal toegewezen stoelen | 
| BilledRevenueUSD | Gefactureerde omzet in Amerikaanse dollars | 
| CustomerName | Naam van de klant | 
| CustomerTPid | Id van het bovenste bovenliggende item van de klant | 
| CustomerSegment | Klant segment | 
| CustomerMarket | Geografische markt van de klant | 
| ResellerStatus | Reseller-status | 

### <a name="subscription-details-report"></a>**Rapport abonnements Details**

>[!Note]
>Opbrengst-en ACR-gegevens zijn alleen beschikbaar voor gebruikers die een leidinggevende rapport kijkers hebben.

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| SubscriptionId | GUID van het abonnement | 
| Subscription | Begin datum van het abonnement | 
| SubscriptionEndDate | Eind datum van het abonnement | 
| Subscription State | De status van het abonnement (actief of verloop) | 
| Maand | Maand waarvoor het gebruik en de opbrengst worden gerapporteerd | 
| IsAutoRenew | Hiermee wordt aangegeven of het abonnement wordt verlengd (ja of Nee) | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | GUID van de klant | 
| CustomerTpid | Bovenliggende id van de klant | 
| CustomerSegment | Markt segment van de klant | 
| CustomerMarket | Geografische markt van de klant | 
| Product | Product dat door de partner aan de klant wordt verkocht | 
| SKU | SKU van het product | 
| MPNId | Microsoft Partner Network-ID van de partner | 
| PartnerName | De naam van de partner | 
| Databasenames | Geografische locatie van de partner | 
| PartnerAttributionType | Type toewijzing voor het abonnement | 
| SalesChannel | Kanaal van de verkoop-direct, CSP (Cloud Solution Provider), enzovoort | 
| AvailableSeats | Huidige beschik bare seat | 
| RevenueUSD | Omzet in Amerikaanse dollars | 
| Inschrijvings-ID | Inschrijvings-ID van het abonnement | 

### <a name="azure-usage-report"></a>**Azure-gebruiks rapport**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| SubscriptionId | GUID van het abonnement | 
| Subscription | De begin datum van het abonnement | 
| SubscriptionEndDate | De eind datum van het abonnement | 
| Subscription State | Huidige status van het abonnement (open, gesloten, actief of in respijt periode) | 
| Maand | Datum samengevoegd per maand | 
| ServiceName | De naam van de Azure-service | 
| MeterCategory | Naam van de meter categorie | 
| UsageUnits | Het aantal eenheden dat wordt gebruikt tijdens de facturerings cyclus | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | Tenant-ID van de klant | 
| CustomerTpid | Bovenliggende ID van de klant | 
| CustomerSegment | Segment van de klant | 
| CustomerMarket | Geografische markt van de klant | 
| MPNId | Microsoft Partner Network ID van de klant | 
| PartnerName | De naam van de partner | 
| Databasenames | Locatie van het geografische land van de partner | 
| PartnerAttributionType | Het type toewijzing van de partner | 
| SalesChannel | Kanaal van de verkoop (direct/CSP, indirect/CSP, direct, enzovoort) | 
| ACR_USD | Azure-verbruikte omzet (ACR) in Amerikaanse dollars | 
| Inschrijvings-ID | Inschrijvings-ID van het Azure-abonnement | 

### <a name="office-365-license-usage-report"></a>**Gebruiks rapport van het Office 365-licentie**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-ID van de klant | 
| CustomerTpid | Bovenliggende ID van de klant | 
| Workload | Skype voor bedrijven, teams, Exchange Online | 
| Maand | Maand waarvoor het gebruik wordt gerapporteerd | 
| PaidAvailableUnits | Aantal betaalde beschik bare eenheden | 
| MonthlyActiveUsers | Aantal maandelijkse actieve gebruikers | 
| CustomerName | Naam van de klant | 
| CustomerMarket | Locatie van het geografische land van de markt van de klant | 
| CustomerSegment | Klant segment | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | De naam van de partner | 
| Databasenames | Geografische locatie van de partner | 
| PartnerAttributionType | Het type toewijzing van de partner | 

### <a name="enterprise-mobility-license-usage-report"></a>**Gebruiks rapport voor Enter prise Mobility License**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-ID van de klant | 
| CustomerTpid | Bovenliggende ID van de klant | 
| Workload | Naam van de workload van de Enterprise Mobility + Security (EMS) | 
| Maand | Maand waarvoor het gebruik wordt gerapporteerd | 
| PaidAvailableUnits | Aantal betaalde beschik bare eenheden | 
| MonthlyActiveUsers | Aantal maandelijkse actieve gebruikers | 
| CustomerName | Naam van de klant | 
| CustomerMarket | Locatie van het geografische land van de markt van de klant | 
| CustomerSegment | Klant segment | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | De naam van de partner | 
| Databasenames | Geografische locatie van de partner | 
| PartnerAttributionType | Het type toewijzing van de partner | 

### <a name="dynamics-365-license-usage-report"></a>**Gebruiks rapport voor Dynamics 365-licentie**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| SubscriptionId | GUID van het abonnement | 
| Subscription | Begin datum van het abonnement | 
| SubscriptionEndDate | Eind datum van het abonnement | 
| SubscriptionStatus | Status van het abonnement | 
| Maand | Maand waarvoor het gebruik wordt gerapporteerd | 
| RevSumDivisionName | Naam van de verdeling van de Rev-som | 
| RevSumCategoryName | Naam van de categorie voor de opbrengst som | 
| SKU | SKU van het product | 
| SKUId | SKU-ID van het product | 
| FreeVsPaidSKU | Geeft aan of het een gratis of betaalde SKU is | 
| SalesModel | Verkoop kanaal dat wordt gebruikt voor het verkopen van het abonnement | 
| DetailedSalesModel | Gedetailleerd verkoop model voor het abonnement | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | GUID van de Tenant van de klant | 
| CustomerTpid | Bovenliggende id van de klant | 
| CustomerSegment | Markt segment van de klant | 
| CustomerMarket | Geografische markt van de klant | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | De naam van de partner | 
| Databasenames | Locatie van het geografische land van de partner | 
| PartnerAttachType | Type toewijzing voor het abonnement | 
| AvailableSeats | Huidige beschik bare seat | 
| AssignedSeats | Huidige toegewezen seat | 
| ActiveSeats | Huidige actieve stoelen | 
| DeploymentOpportunity | Huidige implementatie opportuniteit | 
| ActiveUsagePercent | Huidig actief gebruiks percentage | 

### <a name="power-bi-license-usage-report"></a>**Gebruiks rapport van Power BI licentie**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| SubscriptionId | GUID van het abonnement | 
| Subscription | Begin datum van het abonnement | 
| SubscriptionEndDate | Eind datum van het abonnement | 
| SubscriptionStatus | Status van het abonnement (actief, inactief of in respijt periode) | 
| Maand | Datum samengevoegd per maand | 
| SKU | SKU van het product | 
| SKUId | SKU-ID van het product | 
| FreeVsPaidSKU | Gratis of betaalde SKU onderscheid | 
| SalesModel | Verkoop model dat wordt gebruikt om het abonnement te verkopen | 
| DetailedSalesModel | Gedetailleerd verkoop model voor het abonnement | 
| CustomerName | Naam van de klant | 
| CustomerTenantId | GUID van de Tenant van de klant | 
| CustomerTpid | Id van het bovenste bovenliggende item van de klant | 
| CustomerSegment | Markt segment van de klant | 
| CustomerMarket | Geografische markt van de klant | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | De naam van de partner | 
| Databasenames | Locatie van het geografische land van de partner | 
| PartnerAttachType | Type toewijzing voor het abonnement | 
| AvailableSeats | Huidige beschik bare stoelen | 
| AssignedSeats | Huidig toegewezen stoelen | 
| ActiveSeats | Huidige actieve stoelen | 
| DeploymentOpportunity | Huidige implementatie opportuniteit | 
| ActiveUsagePercent | Huidig actief gebruiks percentage | 

### <a name="teams-meetings-and-calls-report"></a>**Team vergaderingen en oproep rapporten**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-ID van de klant | 
| CustomerTpid | Id van het bovenste bovenliggende item van de klant | 
| Maand | Maand waarvoor het gebruik wordt gerapporteerd | 
| Subbelasting | Subwerk belasting waarvoor het gebruik wordt gerapporteerd (vergaderingen, aanroepen of telefoon systemen) | 
| Aantal vergaderingen | Aantal vergaderingen | 
| Duur van vergadering | Totale duur van de vergadering in uren | 

### <a name="teams-monthly-usage-report"></a>**Rapport maandelijks gebruik van teams**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-ID van de klant | 
| CustomerTpid | Id van het bovenste bovenliggende item van de klant | 
| Maand | Maand waarvoor het gebruik wordt gerapporteerd | 
| Subbelasting | Subwerk belasting waarvoor het gebruik wordt gerapporteerd (vergaderingen, aanroepen of telefoon systemen) | 
| Bureaublad gebruikers | Aantal gebruikers die teams op bureau blad gebruiken | 
| Mobiele gebruikers | Aantal gebruikers die teams op mobiele apparaten gebruiken | 
| Webgebruikers | Aantal gebruikers die teams op het web gebruiken | 
| AllUpParticipants | Aantal unieke gebruikers van teams voor de maand | 

### <a name="teams-usage-3p-apps-report"></a>**Rapport over het gebruik van 3P-apps**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| CustomerTenantId | Tenant-ID van de klant | 
| CustomerTpid | Bovenliggende ID van de klant | 
| Maand | Maand waarvoor het gebruik wordt gerapporteerd | 
| Naam van de 3P-app | De naam van de teams-app | 
| Aantal gebruikers | Aantal gebruikers voor de app | 


### <a name="training-details-report"></a>**Rapport met trainings Details**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| TrainingActivityId | Id van de training | 
| TrainingTitle | Titel van de training | 
| TrainingType | Type training (certificering of examen) | 
| IndividualFirstName | Voor naam van de klant | 
| IndividualLastName | Achternaam van de klant | 
| Email | Persoonlijke e-mail-ID van de klant | 
| CorpEmail | Office-e-mail-ID van de klant | 
| TrainingCompletionDate | Voltooiings datum van de training | 
| Maand | Maand waarvoor de gegevens worden gerapporteerd | 
| IcMCP | Hiermee wordt aangegeven of de gebruiker een micro soft Certified Professional (MCP) is | 
| MCPID | MCP-ID van de gebruiker | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | De naam van de partner | 
| PartnerCityLocation | Locatie van de geografische plaats van de partner | 
| PartnerCountryLocation | Locatie van het geografische land van de partner | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn rapport**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| UserName | De naam van de gebruiker | 
| UserId | GUID van de gebruiker | 
| Opleidingsnaam | De naam van de training | 
| TrainingType | Type training (module of leer traject) | 
| Producten | Product waarvoor de leer module van toepassing is | 
| Rollen | Toepasselijke rollen van de training | 
| CompletionDate | Voltooiings datum van de training | 
| MPNId | Id van Microsoft Partner Network | 
| PartnerName | De naam van de partner | 
| Land | Locatie van het geografische land van de partner | 

### <a name="competency-summary-and-history-report"></a>**Het rapport competentie samen vatting en geschiedenis**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| CompetencyName | Naam van de competentie | 
| CompetencyLevel | Niveau van de competentie (goud of zilver) | 
| CompetencyStatus | Huidige status van de competentie (actief, inactief of in respijt periode) | 
| CompetencyStartDate | Begin datum van de competentie | 
| CompetencyEndDate | De eind datum van de competentie | 

### <a name="competency-performance-report"></a>**Rapport over competentie prestaties**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| CompetencyName | Naam van de competentie | 
| CompetencyAttainmentOptionName | Naam van de optie competentie-verhoudingen | 
| Maand | De maand waarvoor de metrische gegevens worden gerapporteerd | 
| MetricName | De naam van de metriek die relevant is voor de competentie | 
| MetricMonthlyContribution | Maandelijkse bijdrage van de metriek | 
| TTMAggregate | Cumulatieve metrische gegevens voor de periode van 12 maanden | 
| AnniversaryYearAggregate | Cumulatieve metrische gegevens voor het huidige jubileum jaar | 
| GoldThreshold | Prestatie vereiste om te voldoen aan de Gold-competentie | 
| SilverThreshold | Prestatie vereiste om te voldoen aan de Silver-competentie | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Neiging-rapport in aflopende Cloud-Microsoft 365**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network-ID | 
| Partner naam | De naam van de partner | 
| Klant-ID | Id-nummer van de klant | 
| DUNS-nummer | & het Bradstreet-nummer (D&B) van de klant die wordt beoordeeld op neiging | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Grootte van org | Grootte van de organisatie | 
| Branche | Branche waarvan de organisatie deel uitmaakt | 
| Verticaal | De verticale van de klant die wordt beoordeeld op neiging, zoals wordt geïdentificeerd door micro soft, D&B en andere industrie normen | 
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochter onderneming van de klant die wordt gescoord voor neiging | 
| Verkoopterritorium | Het verkoop gebied van de klant die wordt beoordeeld op neiging | 
| Plaats | Locatie van geografische plaats van de organisatie | 
| Staat | Locatie van de geografische staat van de organisatie | 
| Postcode | Post code van de organisatie | 
| Land | Locatie van het geografische land van de organisatie | 
| Segment | Markt segment | 
| Subsegment | Subsegment van de markt | 
| Overzicht van SMC-typen | SMC-type | 
| Top niet-beheerd-Compute base | Top unmanaged Customers – compute | 
| Boven onbeheerd: gebruikers basis | Belangrijkste onbeheerde klanten – gebruiker | 
| IsNonProfit | Hiermee wordt aangegeven of de organisatie geen winst is (ja of Nee) | 
| Externe werk doelen inschakelen voor Exchange Online | Klanten die een actief Exchange Online-abonnement hebben, verkopen aan Microsoft 365 | 
| On-premises aanschaf op afstand inschakelen (huidige versie) met neiging-+ 10-licenties in de Cloud | Klant die een huidige on-premises Office-of Windows-client heeft. Dat wil zeggen dat de client versie later is dan een EOL-versie (End-of-Life). De klant heeft 10 of meer licenties. Klant die een neiging score heeft. De partner moet gericht zijn op de conversie naar Microsoft 365. | 
| On-premises aanschaf op afstand inschakelen (huidige versie) met <neiging 10 licenties voor de Cloud | Klant met een actuele on-premises Office-of Windows-client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 10 licenties. Klant die een neiging score heeft. De partner moet gericht zijn op de conversie naar Microsoft 365. | 
| On-premises aanschaf op afstand inschakelen (huidige versie) zonder Cloud neiging-+ 10 licenties | Klant met een actuele on-premises Office-of Windows-client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft 10 of meer licenties. De klant heeft geen neiging score. De partner moet gericht zijn op de conversie naar Microsoft 365. | 
| On-premises aanschaf op afstand inschakelen (huidige versie) zonder Cloud neiging-<10 licenties | Klant met een actuele on-premises Office-of Windows-client (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 10 licenties. De klant heeft geen neiging score. De partner moet gericht zijn op de conversie naar Microsoft 365. | 
| On-premises aanschaf op afstand (EOL-versie) inschakelen met Cloud neiging-+ 10 licenties | Klant met een EOL on-premises Office of een Windows-client (dat wil zeggen, een EOL-versie of eerder). De klant heeft 10 of meer licenties. De klant heeft een neiging score. De partner moet gericht zijn op de conversie naar Microsoft 365. | 
| On-premises aanschaf op afstand inschakelen (EOL-versie) met neiging-<10-licenties in de Cloud | Klant met een EOL on-premises Office of een Windows-client (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan 10 licenties. De klant heeft een neiging score. De partner moet gericht zijn op de conversie naar Microsoft 365. | 
| On-premises aanschaf op afstand (EOL-versie) inschakelen zonder Cloud neiging-+ 10-licenties | Klant die een huidige on-premises Office-of Windows-client heeft (dat wil zeggen, een EOL-versie of eerder). De klant heeft 10 of meer licenties. De klant heeft geen neiging score. De partner moet gericht zijn op de conversie naar Microsoft 365. | 
| On-premises aanschaf op afstand (EOL-versie) inschakelen zonder Cloud neiging-<10-licenties | Klant die een huidige on-premises Office-of Windows-client heeft (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan 10 licenties. De klant heeft geen neiging score. De partner moet gericht zijn op de conversie naar Microsoft 365. | 
| Externe werk inschakelen-neiging-prospect voor Microsoft 365 (Act NowithEvaluate) | Prospect klant met hoge neiging voor Microsoft 365 | 
| Extern werk inschakelen-concurrentie beding (inzoomen) met Microsoft 365 | Klant met zoom en Microsoft 365, doel voor conversie naar teams | 
| Extern werk inschakelen-concurrentie beding (inzoomen) zonder Microsoft 365 | Klant met Inzoomen, doel voor conversie naar teams | 
| Kosten verlagen en beheren Microsoft 365 E3 gericht op Microsoft 365 E5 | Bestaande klant met Microsoft 365 E3, Target voor Microsoft 365 E5 | 
| Kosten verlagen en beheren Microsoft 365 Business Basic-en Business Standard-klanten die zijn gericht op Microsoft 365 Business Premium | Bestaande Microsoft 365 Business Basic-en Business Standard-klanten, streef voor Microsoft 365 Business Premium | 
| De productiviteit van de organisatie neiging | Klant toont een neiging voor het Opper vlak | 
| M365Cluster | Identificeert de neiging van een klant om Microsoft 365 aan te schaffen. Richt nu op Act en evalueer clusters omdat ze een hoger rendement opleveren. Richt Nurturee en Train klanten alleen als er nog steeds capaciteit is nadat u nu aan de slag hebt en klanten te evalueren. | 
| M365Fit | Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een lookalike-model voor onze beste kleine of middel grote bedrijven (Smb's) om klanten te vergelijken en te zien of ze geschikt zijn voor micro soft-Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt. | 
| M365Intent | Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De beoordeling van de intentie bevindt zich in de breedte om de clusters te definiëren. Beoordeling van de intentie is maandelijks bijgewerkt. | 
| SurfaceCluster | Identificeert de neiging van een klant voor het aanschaffen van het Opper vlak door de aanpassings-en intentie aanbevelingen in een cluster te consolideren. Richt nu op Act en evalueer clusters omdat ze een hoger rendement opleveren. Richt Nurturee en Train klanten alleen als er nog steeds capaciteit is nadat u nu aan de slag hebt en klanten te evalueren. | 
| SurfaceFit | Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een lookalike-model voor onze beste Smb's om klanten te vergelijken en te zien of het geschikt is voor micro soft-Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt. | 
| SurfaceIntent | Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De beoordeling van de intentie bevindt zich in de breedte om de clusters te definiëren. Beoordeling van de intentie is maandelijks bijgewerkt. | 
| O365Cluster | Identificeert de neiging van de klant om Office 365 aan te schaffen. Richt nu op Act en evalueer clusters omdat ze een hoger rendement opleveren. Richt Nurturee en Train klanten alleen als er nog steeds capaciteit is nadat u nu aan de slag hebt en klanten te evalueren. | 
| O365Fit | Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een lookalike-model voor onze beste Smb's om klanten te vergelijken en te zien of het geschikt is voor micro soft-Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt. | 
| O365Intent | Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De beoordeling van de intentie bevindt zich in de breedte om de clusters te definiëren. Beoordeling van de intentie is maandelijks bijgewerkt. | 
| M365UpsellCustomer | Hiermee wordt aangegeven of de klant verkoop neiging voor Microsoft 365 weergeeft | 
| Heeft Google | Hiermee wordt aangegeven of de klant concurrerende signalen weergeeft voor Google-producten die eigenaar zijn | 
| Heeft AWS | Hiermee wordt aangegeven of de klant concurrerende signalen weergeeft voor producten van eigenaar Amazon Web Services (AWS) | 
| Bevat EA | Hiermee wordt aangegeven of een vernieuwing een Enter prise Agreement (EA) of een EA-abonnement is | 
| Heeft open | Hiermee wordt aangegeven of een verlenging een open-of open-waarde-overeenkomst is | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Neiging-rapport in de Cloud-Dynamics 365**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network-ID | 
| Partner naam | De naam van de partner | 
| Klant-ID | Klant-id-nummer | 
| DUNS-nummer | Het Bradstreet-nummer van de inbel netwerk-& van de klant die wordt gescoord voor neiging | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Grootte van org | Grootte van de organisatie | 
| Branche | Branche waarvan de organisatie deel uitmaakt | 
| Verticaal | De verticale van de klant die wordt beoordeeld op neiging, zoals wordt geïdentificeerd door micro soft, D&B en andere industrie normen
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochter onderneming van de klant die wordt gescoord voor neiging | 
| Verkoopterritorium | Het verkoop gebied van de klant die wordt beoordeeld op neiging | 
| Plaats | Locatie van geografische plaats | 
| Staat | Locatie van geografische status | 
| Postcode | Post code van de organisatie | 
| Land | Locatie van geografisch land | 
| Segment | Markt segment | 
| Subsegment | Subsegment van de markt | 
| Overzicht van SMC-typen | De categorisatie van een klant: de belangrijkste onbeheerde gebruikers bases zijn klanten met 300 + werk nemers, de belangrijkste onbeheerde reken bases zijn klanten met USD10, 000 in azure-potentieel van drie jaar, middel grote bedrijven zijn klanten met 25 werk nemers of meer en kleine bedrijven zijn klanten met minder dan 25 werk nemers. | 
| Top niet-beheerd-Compute base | Top unmanaged Customers – compute | 
| Boven onbeheerd: gebruikers basis | Belangrijkste onbeheerde klanten – gebruikers | 
| IsNonProfit | Hiermee wordt aangegeven of de organisatie geen winst is (ja of Nee) | 
| Digitale verkoop activeren-Microsoft 365-Seat-grootte >= 25 seats (SalesPro neiging model) | Klant zonder Dynamics 365. Grootte van Seat: 25 +. Partner moet gericht zijn op het cross-sell van Dynamics 365 SalesPro. | 
| Digitale verkoop activeren-Dynamics 365 SalesPro neiging (Act Now of evaluate) | Klanten met een hoge neiging zonder Dynamics 365. Partner moet gericht zijn op Dynamics 365 SalesPro. | 
| Financieel risico beheren & fraude-Dynamics on-premises installatie base-Navision (Business Central neiging model) | Bestaande klant met on-premises Navision. De partner moet gericht zijn op Dynamics 365 Business Central. | 
| Financieel risico beheren & fraude-Dynamics on-premises install base-Dynamics AX (Dynamics 365 Financiën + Operations neiging model) | Bestaande klant met on-premises AX. De partner moet gericht zijn op Dynamics 365 Finance +-bewerkingen. | 
| Financieel risico beheren & fraude-Dynamics on-premises install base-Great Plains (Business Central neiging model) | Bestaande klant met on-premises Great Plains. De partner moet gericht zijn op Dynamics 365 Business Central. | 
| Financieel risico beheren & fraude-Dynamics on-premises install base-Solomon (Business Central neiging model) | Bestaande klant met on-premises Solomon. De partner moet gericht zijn op Dynamics 365 Business Central. | 
| Financieel risico beheren & fraude-Dynamics on-premises install base-overige (Business Central neiging model) | Bestaande klant met andere on-premises oplossingen die niet eerder zijn vermeld. De partner moet gericht zijn op Dynamics 365 Business Central. | 
| Flexibele bedrijfs processen bouwen-Dynamics on-premises install base-AX/GP/SL/NAV/Overig (Dynamics 365 neiging model) | Flexibele bedrijfs processen bouwen-Dynamics on-premises install base-AX/GP/SL/NAV/Overig (Dynamics 365 neiging model) | 
| Flexibele bedrijfs processen bouwen-Dynamics-concurrentie Mendix/Outsystems/Sales Force (Dynamics 365 neiging model) | Flexibele bedrijfs processen bouwen-Dynamics-concurrentie Mendix/Outsystems/Sales Force (Dynamics 365 neiging model) | 
| Flexibele bedrijfs processen bouwen-basis voor Dynamics 365 Finance + Operations-installatie | Bestaande Dynamics 365 Finance + Operations-klanten. Partner om Power-apps te richten. | 
| Flexibele bedrijfs processen bouwen-basis installatie van Dynamics 365 Business Central | Bestaande Dynamics 365 Business Central-klanten. Partner om Power-apps te richten. | 
| Flexibele bedrijfs processen bouwen-basis voor Dynamics 365-klant betrokkenheid installeren | Bestaande klanten van Dynamics 365 Customer engagement. Partner om Power-apps te richten. | 
| Bouw een robuuste toeleverings keten-Windows en activeer de eerste Dynamics 365-workload als Dynamics 365 supply chain management met niet-Oracle of SAP ERP-klanten (Enter prise resource planning) | Doel klanten voor Dynamics 365 Supply Chain Management | 
| Bouw een robuuste toeleverings keten met een cross-sell van Dynamics 365 supply chain management en/of retail of Commerce aan bestaande klanten van Dynamics 365 Customer engagement | Bestaande Dynamics 365 Customer engagement-klanten te richten op het cross-sell Dynamics 365 supply chain management. | 
| Bouw een robuuste toeleverings keten voor een cross-sell van Dynamics 365 supply chain management en/of retail of Commerce aan Dynamics 365 Customer engagement en Oracle of SAP | Bestaande Dynamics 365 Customer engagement-klanten met Oracle of SAP naar target voor Dynamics 365 Supply Chain Management | 
| D365BCCluster | Identificeert de neiging van de klant om Dynamics 365 Business Central te kopen. Klanten die een neiging voor Business Central weer geven, zijn de categorieën middel grote en kleine. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| D365BCFit | Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een lookalike-model voor onze beste SMB om klanten te vergelijken en te zien of het geschikt is voor micro soft-Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt. | 
| D365BCIntent | Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De beoordeling van de intentie bevindt zich in de breedte om de clusters te definiëren. Beoordeling van de intentie is maandelijks bijgewerkt. | 
| D365FOCluster | Identificeert de neiging van de klant om Dynamics 365-Financiën en-bewerkingen te kopen. Klanten die een neiging voor Financiën +-bewerkingen tonen, staan in de hoofd categorieën zonder begeleiding. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| D365FOFit | Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een lookalike-model voor onze beste SMB om klanten te vergelijken en te zien of het geschikt is voor micro soft-Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt. | 
| D365FOIntent | Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De beoordeling van de intentie bevindt zich in de breedte om de clusters te definiëren. Beoordeling van de intentie is maandelijks bijgewerkt. | 
| D365CECluster | Identificeert de neiging van de klant om de klant betrokkenheid van Dynamics 365 aan te schaffen. Klanten die een neiging voor klant betrokkenheid tonen, zijn de categorieën middel grote en kleine. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| D365CEFit | Geeft aan dat de klant betrokkenheid voor Dynamics 365 wordt aangepast | 
| D365CEIntent | Geeft het doel aan voor Dynamics 365-klant betrokkenheid | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Hiermee wordt aangegeven of de klant een openstaande verlenging heeft voor Dynamics on-premises AX of CRM | 
| M365UpsellCustomer | Hiermee wordt aangegeven of de klant verkoop neiging voor Microsoft 365 weergeeft | 
| Heeft Google | Hiermee wordt aangegeven of de klant concurrerende signalen weergeeft voor Google-producten die eigenaar zijn | 
| Heeft AWS | Hiermee wordt aangegeven of de klant concurrerende signalen weergeeft voor AWS-producten van eigenaar | 
| Bevat EA | Hiermee wordt aangegeven of een vernieuwing een EA-of EA-abonnement is | 
| Heeft open | Hiermee wordt aangegeven of een verlenging een open-of open-waarde-overeenkomst is | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud, schuine-Azure neiging-rapport**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network-ID | 
| Partner naam | De naam van de partner | 
| Klant-ID | Klant-id-nummer | 
| DUNS-nummer | Het Bradstreet-nummer van de inbel netwerk-& van de klant die wordt gescoord voor neiging | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Grootte van org | Grootte van de organisatie | 
| Branche | Branche | 
| Verticaal | De verticale van de klant die wordt beoordeeld op neiging, zoals wordt geïdentificeerd door micro soft, D&B en andere industrie normen | 
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochter onderneming van de klant die wordt gescoord voor neiging | 
| Verkoopterritorium | Het verkoop gebied van de klant die wordt beoordeeld op neiging | 
| Plaats | Locatie van geografische plaats | 
| Staat | Locatie van geografische status | 
| Postcode | Post code van de organisatie | 
| Land | Locatie van geografisch land | 
| Segment | Markt segment | 
| Subsegment | Subsegment van de markt | 
| Overzicht van SMC-typen | SMC-type | 
| Top niet-beheerd-Compute base | Top unmanaged Customers – compute | 
| Boven onbeheerd: gebruikers basis | Belangrijkste onbeheerde klanten – gebruikers | 
| IsNonProfit | Hiermee wordt aangegeven of de organisatie geen winst is (ja of Nee) | 
| Migrate-EOL Windows Server-EOL Windows Server IB met Cloud neiging-5 + licenties | Klant met een on-premises Windows Server-EOL (dat wil zeggen, een EOL-versie of eerder). De klant heeft 5 of meer licenties. Klant die een neiging score heeft. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB met Cloud neiging-<5-licenties | Klant met een on-premises Windows Server-EOL (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan 5 licenties. Klant die een neiging score heeft. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB zonder Cloud neiging-5 + licenties | Klant met een on-premises Windows Server-EOL (dat wil zeggen, een EOL-versie of eerder). De klant heeft meer dan vijf licenties. De klant heeft geen neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-EOL Windows Server-EOL Windows Server IB zonder Cloud neiging-<5 licenties | Klant met een on-premises Windows Server-EOL (dat wil zeggen, een EOL-versie of eerder). Heeft minder dan 5 licenties. De klant heeft geen neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB met Cloud neiging-5 + licenties | Klant met een EOL on-premises SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft 5 licenties. De klant heeft een neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB met neiging-<5-licenties in de Cloud | Klant met een EOL on-premises SQL Server (dat wil zeggen, een EOL-versie of eerder). Heeft minder dan 5 licenties. Klant die een neiging score heeft. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB zonder Cloud neiging-5 + licenties | Klant met een EOL on-premises SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft 5 of meer licenties. De klant heeft geen neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-EOL SQL-EOL SQL Server IB zonder Cloud neiging-<5-licenties | Klant met een EOL on-premises SQL Server (dat wil zeggen, een EOL-versie of eerder). De klant heeft minder dan 5 licenties. De klant heeft geen neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migreren: on-premises Windows Server-huidige Windows Server IB met Cloud neiging-5 + licenties migreren | Klant die een huidige on-premises Windows Server heeft (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft 5 licenties. De klant heeft een neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migratie migreren: on-premises Windows Server-huidige Windows Server IB met Cloud neiging-<5-licenties | Klant die een huidige on-premises Windows Server heeft (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 5 licenties. De klant heeft een neiging-score voor Azure. De partner moet deze klant richten op de migratie naar Azure. | 
| Migreren: on-premises Windows Server-huidige Windows Server IB zonder Cloud neiging-5 + licenties migreren | Klant die een huidige on-premises Windows Server heeft (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft 5 licenties. De klant heeft geen neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migratie migreren: on-premises Windows Server-huidige Windows Server IB zonder Cloud neiging-<5-licenties | Klant die een huidige on-premises Windows Server heeft (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 5 licenties. De klant heeft geen neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migreren: migreren naar Azure SQL of SQL virtual machines (Vm's)-huidige SQL Server IB met Cloud neiging-5 + licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft 5 licenties. De klant heeft een neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migreren: migreren naar Azure SQL of SQL-Vm's-huidige SQL Server IB met clouding neiging-<5-licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 5 licenties. De klant heeft een neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migreren: migreren naar Azure SQL of SQL-Vm's-huidige SQL Server IB zonder Cloud neiging-5 + licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft 5 licenties. De klant heeft geen neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migreren: migreren naar Azure SQL of SQL-Vm's-huidige SQL Server IB zonder Cloud neiging-<5-licenties | Klant met een huidige on-premises SQL Server (dat wil zeggen, een versie die hoger is dan EOL). De klant heeft minder dan 5 licenties. De klant heeft geen neiging score. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-OSS-Migrate to open source Shakespeare (OSS) DB | Bestaande klant met een van de volgende concurrentie producten: PostgreSQL, MySQL, MariaDB. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-OSS-Linux op Azure | Bestaande klant met Linux. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-SAP-SAP on Azure | Bestaande klant met SAP. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-Windows virtueel bureau blad-Extern bureaublad-services IB | Identificeert klanten met actieve Windows Extern bureaublad-services. De partner moet deze klant richten op de migratie naar Azure. | 
| Migreren-Windows virtueel bureau blad-moderne werk door verkopen aan Azure-WVD | Identificeert klanten met Microsoft 365 en heeft geen Azure. De partner moet deze klant richten op de migratie naar Azure. | 
| Migreren-VMware IB | Bestaande klant met het product: VMware. De partner moet deze klant richten op de migratie naar Azure. | 
| Migrate-Citrix IB | Bestaande klant met het product: Citrix Systems. De partner moet deze klant richten op de migratie naar Azure. | 
| Innoveren-analyses-Power BI IB met hoge Azure neiging | Klanten met en actief Power BI abonnement met inbegrip van: Power BI-zelfstandige Pro, Power BI-Azure-suites, Power BI Office-suites, Power BI suites-Microsoft 365 | 
| Enable-DevOps met GitHub-Visual Studio/MSDN IB | Identificeert klanten met actieve Visual Studio-versies | 
| Windows Server Standard-versie | Geeft de versie van Windows Server Standard-aankopen door de klant weer | 
| Windows Server Standard-licentie | Geeft het licentie type weer van Windows Server Standard-aankopen door de klant | 
| Windows Server Data Center-versie | Geeft de versie van Windows Data Center-aankopen door de klant weer | 
| Windows Server Data Center-licentie | Geeft het licentie type weer van Windows Data Center-aankopen door de klant | 
| AzureFit | Interne en externe gegevens punten die firmographics definiëren. Het aanpassen van scores maakt gebruik van een lookalike-model voor onze beste SMB om klanten te vergelijken en te zien of het geschikt is voor micro soft-Cloud producten. Het afstemmen van scores wordt per kwar taal bijgewerkt. | 
| AzureIntent | Signalen met betrekking tot sociale media en het online gedrag van een klant definiëren intentie. De beoordeling van de intentie bevindt zich in de breedte om de clusters te definiëren. Beoordeling van de intentie is maandelijks bijgewerkt. | 
| AzureCluster | Identificeert de neiging van de klant om Azure aan te schaffen door de aanpassings-en intentie aanbevelingen in een cluster te consolideren. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| WindowsServerDataCenter_HasOpenRenewal | Hiermee wordt aangegeven of de klant een openstaande verlenging heeft voor Windows Server Data Center | 
| WindowsServerStandard_HasOpenRenewal | Hiermee wordt aangegeven of de klant een openstaande verlenging heeft voor Windows Server Standard | 
| AzureUpsellCustomer | Hiermee wordt aangegeven of de klant verkoop neiging voor Azure weergeeft | 
| Heeft Google | Hiermee wordt aangegeven of de klant concurrerende signalen weergeeft voor Google-producten die eigenaar zijn | 
| Heeft AWS | Hiermee wordt aangegeven of de klant concurrerende signalen weergeeft voor AWS-producten van eigenaar | 
| Bevat EA | Hiermee wordt aangegeven of een vernieuwing een EA-of EA-abonnement is | 
| Heeft open | Hiermee wordt aangegeven of een verlenging een open-of open-waarde-overeenkomst is | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Neiging rapport voor het verlengen van de Cloud**

| Kolomnaam | Gegevens beschrijving | 
| :--------- | :--------- | 
| MPN-id | Microsoft Partner Network-ID | 
| Partner naam | De naam van de partner | 
| Klant-ID | Klant-id-nummer | 
| DUNS-nummer | Het Bradstreet-nummer van de inbel netwerk-& van de klant die wordt gescoord voor neiging | 
| Accountnaam | Naam van het account | 
| Domain | Domein van het account | 
| Grootte van org | Grootte van de organisatie | 
| Branche | Branche | 
| Verticaal | De verticale van de klant die wordt beoordeeld op neiging, zoals wordt geïdentificeerd door micro soft, D&B en andere industrie normen | 
| Gebied | Geografisch gebied van de locatie | 
| Dochteronderneming | De dochter onderneming van de klant die wordt gescoord voor neiging | 
| Verkoopterritorium | Het verkoop gebied van de klant die wordt beoordeeld op neiging | 
| Plaats | Locatie van geografische plaats | 
| Staat | Locatie van geografische status | 
| Postcode | Post code van de organisatie | 
| Land | Locatie van geografisch land | 
| Segment | Markt segment | 
| Subsegment | Subsegment van de markt | 
| Overzicht van SMC-typen | SMC-type | 
| Top niet-beheerd-Compute base | Top unmanaged Customers – compute | 
| Boven onbeheerd: gebruikers basis | Belangrijkste onbeheerde klanten – gebruikers | 
| IsNonProfit | Hiermee wordt aangegeven of de organisatie geen winst is (ja of Nee) | 
| Heeft Google | Hiermee wordt aangegeven of de klant concurrerende signalen weergeeft voor AWS-producten van eigenaar | 
| Heeft AWS | Hiermee wordt aangegeven of de klant concurrerende signalen weergeeft voor AWS-producten van eigenaar | 
| Azure-cluster | Identificeert de neiging van de klant om Azure aan te schaffen. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| D365 Finance + Operations-cluster | Identificeert de neiging van de klant om Dynamics 365-Financiën en-bewerkingen te kopen. Klanten die een neiging voor Financiën +-bewerkingen tonen, staan in de hoofd categorieën zonder begeleiding. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| D365 CE-cluster | Identificeert de neiging van de klant om de klant betrokkenheid van Dynamics 365 aan te schaffen. Klanten die een neiging voor klant betrokkenheid tonen, zijn de categorieën middel grote en kleine. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| D365 BC-cluster | Identificeert de neiging van de klant om Dynamics 365 Business Central te kopen. Klanten die een neiging voor Business Central weer geven, zijn de categorieën middel grote en kleine. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| Microsoft 365 cluster | Identificeert de neiging van de klant om Microsoft 365 aan te schaffen. Richt nu op Act en evalueer clusters, omdat ze een hoger rendement opleveren. Richt nurture en Train klanten alleen als er nog capaciteit is nadat u nu aan de slag gaat en klanten te evalueren. | 
| Licentie programma | Hiermee wordt het type licentie programma voor de verlenging geïdentificeerd | 
| Overeenkomst-ID | Id van de overeenkomst | 
| Eind datum van overeenkomst | Eind datum van de overeenkomst | 
| Type verval datum | Type verval datum | 
| Verlopende omzet | Omzet gekoppeld aan verlopen abonnementen | 
| Bevat EA | Hiermee wordt aangegeven of een vernieuwing een EA-of EA-abonnement is | 
| Heeft open | Hiermee wordt aangegeven of een verlenging een open-of open-waarde-overeenkomst is | 
| Klant van Azure-verkoop | Hiermee wordt aangegeven of de klant verkoop neiging voor Azure weergeeft | 
| Klant Microsoft 365 verkoop | Hiermee wordt aangegeven of de klant verkoop neiging voor Microsoft 365 weergeeft | 
| RevSumDivisionName | Hiermee wordt het product geïdentificeerd dat is voor verlenging | 

## <a name="next-steps"></a>Volgende stappen

Zie [down load rapporten](pci-download-reports.md)voor meer informatie.
