---
title: Rollen & machtigingen toewijzen aan gebruikers
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over welke rollen het meest geschikt zijn voor de gebruikers van uw bedrijf die commerciële trans acties, verwijzingen, prikkels of MPN-lidmaatschappen in het partner centrum beheren.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 964c0e6be3003c2b3c9da8828d6e896e2fff82f9
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756460"
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
|Beheer agent | * Klant beheer|[Communiceren met uw klanten](connect-with-your-customers.md)
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

|**Role** | **Wat u kunt doen**|**Meer informatie**
|------------------------------|:-------------------------|---|
|Beheerder van verwijzingen|Alles op het tabblad verwijzingen maken en beheren in het partner centrum|[Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
||    Kan alle verkoop kansen en potentiële klanten weer geven en bewerken
||    Kan team leden toewijzen aan een deal
||    Kan zakelijke profielen weer geven en bewerken
||    Kan deals weer geven en registreren voor verkoop kansen die zijn gemarkeerd als binnengehaald en die in aanmerking komen voor de registratie van deals
||    Kan ondersteunings tickets maken en weer geven
|Referenties gebruiker|Maak en beheer alleen verkoop kansen als deze deel uitmaken van het team |[Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
||    Kan verkoop kansen maken voor de locaties waaraan de rol is toegewezen.
||    Kan deals weer geven en registreren voor verkoop kansen die zijn gemarkeerd als binnengehaald en die in aanmerking komen voor de registratie van deals als ze een teamlid zijn.
||    Kan ondersteunings tickets maken en weer geven
|Bedrijfs profiel beheerder|Zakelijke profielen maken en beheren | [Zakelijke profielen beheren](create-a-marketing-profile.md)
||    Kan ondersteunings tickets maken en weer geven

In combi natie met de nieuwe referrals gebruikersrol maken we ook kennis met het bereik van de locatie voor deals. De volgende tabel geeft uitleg over de deals-toegang op basis van de locatie.

|**Scope** | **Wat u kunt doen** |
|------------------------------|:-------------------------|
|Het hele bedrijf | Zowel beheerders als gebruikers hebben toegang tot het maken van deals voor elke locatie in het bedrijf|
|| Verwijzings beheerder heeft toegang om alle deals weer te geven en te bewerken |
|| Referentie gebruikers hebben toegang tot het weer geven en bewerken van alle deals alleen als ze deel uitmaken van het team |
|Een of meer locaties | Zowel beheerders als gebruikers hebben toegang tot het maken van deals voor de toegewezen locatie in het bedrijf|
|| Verwijzings beheerder heeft toegang om alle deals weer te geven en te bewerken die horen bij de toegewezen locaties|
|| Verwijzings gebruikers hebben toegang tot het weer geven en bewerken van alle deals die tot de toegewezen locaties behoren als ze deel uitmaken van het team|

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
