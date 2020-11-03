---
title: Rollen & machtigingen toewijzen aan gebruikers
ms.topic: article
ms.date: 09/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over welke rollen het meest geschikt zijn voor de gebruikers van uw bedrijf die commerciële trans acties, verwijzingen, prikkels of MPN-lidmaatschappen in het partner centrum beheren.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 32df86887ccbea5d18d1bd8c7c34add2b1ab60e4
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/13/2020
ms.locfileid: "92528668"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Gebruikers rollen en-machtigingen toewijzen aan gebruikers van een bedrijf die moeten werken in het partner centrum

**Juiste rollen**

- Globale beheerder
- Gebruikersbeheerder
- MPN-partner beheerder

U hebt uw partner profiel ingesteld, inclusief de juridische naam en het adres, de ondersteunings Details, de bestands belasting, de Bank gegevens en de primaire contact persoon van uw bedrijf. Volgende stap: laat uw gebruikers instellen met wacht woorden en rollen, zodat ze met u kunnen werken in het partner centrum.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Uw werk nemers instellen om te werken in het partner centrum

U bepaalt welke soorten toegang uw gebruikers hebben voor het partner centrum door de rollen en machtigingen die u hebt. Rollen zijn gerelateerd aan de Program ma's waarmee uw bedrijf is betrokken. Als uw bedrijf bijvoorbeeld een Cloud Solution Provider (CSP)-bedrijf is, hebt u niet alleen de standaard Azure Active Directory Tenant beheer rollen, zoals globale beheerder, maar hebt u ook rollen nodig die specifiek zijn voor het CSP-programma. Elk programma heeft specifieke rollen.

>[!Note]
> Azure Active Directory Tenant rollen zijn onder andere globale beheerder, gebruikers beheerder en CSP-rollen. Niet-Azure-Active-Directory-functies zijn de rollen die de Tenant niet beheren, en ze omvatten MPN admin, bedrijfs profiel beheerder, verwijzings beheerder, prikkel beheerder en gebruikers met prikkel. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Commerciële trans acties beheren in Partner Center (Azure AD-en CSP-functies)

|**Role**|**Wat ze kunnen doen**|**Meer informatie**|
|----------------------------------|---|:---------------------------------|
|Globale beheerder|* Kan toegang krijgen tot alle Microsoft-account/services met volledige bevoegdheden|[Uw Partner Center-account beheren](partner-center-account-setup.md)
|      |* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt
||* Overeenkomsten, prijs lijsten en aanbiedingen weer geven
||* Partner gebruikers weer geven, maken en beheren|
||  Facturerings-, factuur-en afstemmings bestanden weer geven, maken en beheren
|Beheerder van gebruikers beheer   | * Gebruikers weer geven, maken en beheren|[De voor delen en aanbiedingen van uw Microsoft Partner Network lidmaatschap beheren in het partner centrum](manage-your-partner-network-benefits.md)
||* Alle partner profielen weer geven
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt
|Factureringsbeheerder | -Facturerings-, factuur-en afstemmings bestanden weer geven, maken en beheren|[Uw rekening lezen](billing.md)
||* Prijs weer geven
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt
|Standaard gebruiker|  Mijn profiel weer geven   |[Uw wachtwoord opnieuw instellen](reset-my-pasword.md)
|Beheer agent | * Klant beheer|[Maak verbinding met uw klanten](connect-with-your-customers.md)
||* Apparaten lijst toevoegen aan het partner centrum
||* Profielen maken en Toep assen op apparaten
||* Abonnements beheer
||* Service status-en service aanvragen voor klanten
||* Gemachtigde beheerder bevoegdheden aanvragen
||* Prijs en aanbiedingen weer geven
||* Facturering
||* Namens een klant beheren
||* Een wederverkoper met toegevoegde waarde registreren
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt|
|Verkoop agent | * Klant beheer|[Ondersteuning voor facturering voor uw klanten bieden en helpen bij het beantwoorden van vragen over facturering](provide-billing-support.md)
||* Apparaten lijst toevoegen aan het partner centrum
||* Abonnements beheer
||* Ondersteunings tickets weer geven
||* Een relatie met een klant aanvragen
||* Prijs en aanbiedingen weer geven
||* Leads van klanten beheren
||* De klant overeenkomst weer geven
||* Een reseller met toegevoegde waarde registreren
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt|
|Helpdesk medewerker| * Een klant zoeken en weer geven|[Problemen naar micro soft escaleren en leren welke problemen meer geschikt zijn voor micro soft-escalatie](escalate-problems-to-microsoft.md)
||* Klant Details bewerken
||* Hulp bij het oplossen van problemen met klanten met facturering of abonnements beheer
||* Ondersteuning aanvragen namens klanten 
||* Abonnementen en problemen met facturering namens klanten beheren
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Configuratie scherm leverancier (CPV). (CSP-functie en niet-Azure AD-rol)

CPVs ontwikkel apps die worden gebruikt door de Cloud Solution Provider (CSP)-partners om hen in staat te stellen hun systemen te integreren met partner Center-Api's. 

|**Role**   |**Wat u kunt doen**|**Meer informatie**|
|------------------------------|:----------------------------|----|
|Globale beheerder| Uw CPV-profiel weer geven en beheren|[Inschrijven als leverancier van het configuratie scherm om de CSP-partner systemen te helpen integreren met partner Center-Api's](enroll-as-cpv.md)
||Uw gebruikers weer geven en beheren die toegang moeten hebben tot de CPV-mogelijkheden|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Gast gebruiker (moet worden toegevoegd aan de Azure Active Directory Tenant)

|**Gast gebruiker**   | **Rollen**|
|---------------------------|:--------------------|
||MPN-partner beheerder|
||Account beheerder|
||Prikkel beheerder|
||Bedrijfs profiel beheerder|
||Beheerder van verwijzingen|


## <a name="manage-mpn-membership-and-your-company"></a>MPN-lidmaatschap en uw bedrijf beheren 

Deze rollen zijn niet Azure Active Directory rollen. Deze rollen beheren het bedrijfs bedrijf in plaats van de Tenant.

|**Role** | **Wat u kunt doen**|**Meer informatie**|
|----------------------------|:----------------------------|-----|
|MPN-partner beheerder|* Aanvragen voor partner services weer geven, maken en beheren|[Een abonnement op Microsoft Action Pack of een Silver- of Gold-competentie kopen of verlengen](mpn-get-action-pack.md)
||* Juridische, bedrijfs-, Business-en MPN-profielen weer geven
||* Gebruikers gegevens en hun vakkennis gegevens weer geven
||* Competenties weer geven
||* Voor delen weer geven en beheren
||* MPN-aanbiedingen weer geven en kopen
||* MPN weer geven bevat order geschiedenis en facturen
||* Gegevens van de bijdrage indicator van de partner weer geven
||* Kan worden gebruikt in het hulp programma voor validatie van boek stukken|
||* Analyse van klant gegevens weer geven
||* Andere gebruikers rollen in het bedrijf weer geven, maar kan geen rollen toewijzen
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt
|Accountbeheerder| Locaties toevoegen|[Locaties beheren](manage-locations.md)
|| Profielen beheren die betrekking hebben op de accounts waarmee u beheerder bent 
||* Rollen voor gebruikers in een Tenant toewijzen aan niet-Azure-Active Directory-rollen 
||* Locaties registreren in Program ma's
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt


## <a name="manage-referrals"></a>Verwijzingen beheren 

|**Role**|**Wat u kunt doen**|**Meer informatie**|
|-----------------------------|:------------------------|---|
|Beheerder van verwijzingen       |* Zakelijke profielen weer geven, maken en beheren|[Verschillende leads beheren, zoals vragen van klanten, gekwalificeerde marketingleads en gekwalificeerde verkoopleads](manage-leads.md)
||* Verwijzingen ontvangen en beheren
||* Verwijzingen voor verkopen weer geven, maken en beheren|
||* Aanvragen voor partner services weer geven, maken en beheren
|Bedrijfs profiel beheerder   |* Bedrijfs profiel weer geven, maken en beheren |[Een bedrijfs profiel maken](create-a-marketing-profile.md)
||* Aanvragen voor partner services weer geven, maken en beheren
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt|

## <a name="manage-incentives"></a>Prikkels beheren 

|**Role** | **Wat u kunt doen**|**Meer informatie**
|------------------------------|:-------------------------|---|
|Prikkel beheerder|* Initieert en beheert prikkels |[Gebruik deze bronnen om u te helpen aan de slag te gaan met prikkels](incentives-get-started-intro.md)
||* Kan alle aspecten van prikkel Programma's weer geven en bewerken
||* Kan Bank-en belasting gegevens weer geven en bewerken
||* Kortingen en mede-op-winst weer geven
||* Ondersteuning voor toegang
||* Betalings stimulansen voor geschillen|
|Prikkel gebruiker|* Kan prikkel Programma's weer geven
||* Kan prikkel claims weer geven en initiëren
||* Kortingen en mede-op-winst weer geven
||* Ondersteunings tickets maken voor het partner centrum
||* Partner-ondersteunings tickets weer geven die u maakt

## <a name="view-partner-center-insights-data"></a>Partner Center Insights-gegevens weer geven

|**Role** | **Wat u kunt doen**|**Meer informatie**|
|------------------------------|:-------------------------|---|
|Rapport Viewer Executive|Toegang tot alle rapport gegevens sets, partner-ondersteunings tickets maken, partner-ondersteunings tickets weer geven die u hebt gemaakt|[Overzicht van Dashboard rapporten die beschikbaar zijn in Partner Center Insights](pci-overview-report.md)
|Rapport viewer|Toegang tot gegevens rapporten met uitzonde ring van de persoonlijke gegevens van de klant en de werk nemer, het maken van partner-ondersteunings tickets, het weer geven van partners die u maakt|

## <a name="next-steps"></a>Volgende stappen

- [Gebruikersaccounts maken en rollen en machtigingen toewijzen](create-user-accounts-and-set-permissions.md)
- [Uw account gegevens verifiëren wanneer u zich registreert in een nieuw partner centrum-programma](verification-responses.md)
