---
title: Rollen en machtigingen & toewijzen aan gebruikers
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Ontdek welke rollen het beste zijn voor de gebruikers van uw bedrijf die commerciële transacties, verwijzingen, incentives of MPN-lidmaatschappen beheren in Partner Center.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 7638a35b5aa583cd3a7c3b40833123402df7cb70
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126245680"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Gebruikersrollen en -machtigingen toewijzen aan de gebruikers van een bedrijf die in een Partner Center

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | MPN-partnerbeheerder

U hebt uw partnerprofiel ingesteld, inclusief juridische naam en adres, ondersteuningsdetails, btw-vrijstellingen, bankgegevens en de primaire contactpersoon voor uw bedrijf. Volgende stap: stel uw gebruikers in met wachtwoorden en rollen, zodat ze met u aan de slag Partner Center gaan.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Uw werknemers instellen voor werk in Partner Center

U bepaalt de soorten toegang die uw gebruikers moeten Partner Center aan de hand van de rollen en machtigingen die u ze geeft. Rollen zijn gerelateerd aan de programma's waar uw bedrijf bij betrokken is. Als uw bedrijf bijvoorbeeld een Cloud Solution Provider-bedrijf (CSP) is, hebt u niet alleen de standaard tenantbeheerrollen van Azure Active Directory (Azure AD), zoals globale beheerder, maar hebt u ook rollen nodig die specifiek zijn voor het CSP-programma. Elk programma heeft specifieke rollen.

>[!Note]
> Azure AD-tenantrollen zijn globale beheerder, gebruikersbeheerder en CSP-rollen. Niet-Azure AD-rollen zijn rollen die de tenant niet beheren, en ze omvatten MPN-partnerbeheerder (Microsoft Partner Network), bedrijfsprofielbeheerder, verwijzingsbeheerder, incentive-beheerder en incentive-gebruiker. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Commerciële transacties beheren in Partner Center (Azure AD- en CSP-rollen)

|**Role**|**Wat ze kunnen doen**|**Meer informatie**|
|----------------------------------|---|:---------------------------------|
|Globale beheerder|* Heeft toegang tot alle Microsoft-account/services met volledige bevoegdheden|[Uw Partner Center-account beheren](partner-center-account-setup.md)
|      |* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt
||* Overeenkomsten, prijslijsten en aanbiedingen weergeven
||* Partnergebruikers weergeven, maken en beheren|
||  Facturering, facturen en recon-bestanden weergeven, maken en beheren
|Beheerder van gebruikersbeheer   | * Gebruikers weergeven, maken en beheren|[Uw voordelen Microsoft Partner Network en aanbiedingen voor lidmaatschap beheren in Partner Center](manage-your-partner-network-benefits.md)
||* Alles weergeven partnerprofielen
||* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt
|Factureringsbeheerder | - Facturering, facturen en recon-bestanden weergeven, maken en beheren|[Uw rekening lezen](billing.md)
||* Prijzen weergeven
||* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt
|Standaardgebruiker|  De Mijn profiel   |[Uw wachtwoord opnieuw instellen](reset-my-pasword.md)
|Beheeragent | * Klantbeheer|[Communiceren met uw klanten](connect-with-your-customers.md)
||* Apparaatlijst toevoegen aan de Partner Center
||* Profielen maken en toepassen op apparaten
||* Abonnementsbeheer
||* Service health and service requests for customers (Status- en serviceaanvragen voor klanten)
||* Gedelegeerde beheerdersbevoegdheden aanvragen
||* Prijzen en aanbiedingen weergeven
||* Facturering
||* Beheer namens een klant
||* Een reseller met toegevoegde waarde registreren
||* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt|
|Verkoopagent | * Klantbeheer|[Factureringsondersteuning bieden voor uw klanten en helpen bij het beantwoorden van hun vragen over facturering](provide-billing-support.md)
||* Apparaatlijst toevoegen aan de Partner Center
||* Abonnementsbeheer
||* Ondersteuningstickets weergeven
||* Een relatie met een klant aanvragen
||* Prijzen en aanbiedingen weergeven
||* Leads van klanten beheren
||* De klantovereenkomst weergeven
||* Een reseller met toegevoegde waarde registreren
||* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt|
|Helpdeskagent| * Een klant zoeken en weergeven|[Problemen naar Microsoft escaleren en leren welke problemen geschikter zijn voor escalatie van Microsoft](escalate-problems-to-microsoft.md)
||* Klantgegevens bewerken
||* Problemen van klanten met facturerings- of abonnementsbeheer oplossen
||* Ondersteuning aanvragen namens klanten 
||* Problemen met abonnementen en facturering namens klanten beheren
||* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Configuratiescherm Vendor (CPV). (CSP-rol en niet-Azure AD-rol)

CPV's ontwikkelen apps die door CSP-partners kunnen worden gebruikt om hun systemen te integreren met Partner Center API's. 

|**Role**   |**Wat u kunt doen**|**Meer informatie**|
|------------------------------|:----------------------------|----|
|Globale beheerder| Uw CPV-profiel (Configuratiescherm Vendor) weergeven en beheren|[Registreren als een Configuratiescherm leverancier om CSP-partnersystemen te integreren met Partner Center API's](enroll-as-cpv.md)
||Uw gebruikers weergeven en beheren die toegang nodig hebben tot CPV-mogelijkheden|

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Gastgebruiker (moet worden toegevoegd aan de Azure AD-tenant)

|**Gastgebruiker**   | **Rollen**|
|---------------------------|:--------------------|
||MPN-partnerbeheerder|
||Bedrijfsprofielbeheerder|
||Verwijzingsbeheerder|


## <a name="manage-mpn-membership-and-your-company"></a>MPN-lidmaatschap en uw bedrijf beheren 

Deze rollen zijn geen Azure AD-rollen. Deze rollen beheren het bedrijf in plaats van de tenant.

|**Role** | **Wat u kunt doen**|**Meer informatie**|
|----------------------------|:----------------------------|-----|
|MPN-partnerbeheerder|* Aanvragen voor partnerservice weergeven, maken en beheren|[Een abonnement op Microsoft Action Pack of een Silver- of Gold-competentie kopen of verlengen](mpn-get-action-pack.md)
||* Juridische, bedrijfs-, zakelijke en MPN-profielen weergeven
||* Gebruikersdetails en hun vaardigheden weergeven
||* Competenties weergeven
||* Voordelen weergeven en beheren
||* MPN-aanbiedingen weergeven en kopen
||* MpN-aanbiedingen bestelgeschiedenis en facturen weergeven
||* Indicatorgegevens voor partnerbijdragen weergeven
||* Kan werken in het hulpprogramma Voor validatie van validatie|
||* Klantgegevensanalyses weergeven
||* Andere gebruikersrollen binnen het bedrijf weergeven, maar kunnen geen rollen toewijzen
||* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt
|Accountbeheerder| Locaties toevoegen|[Locaties beheren](manage-locations.md)
|| Profielen beheren die betrekking hebben op de accounts die u beheert 
||* Rollen voor gebruikers in tenant toewijzen aan niet-Azure AD-rollen 
||* Locaties inschrijven bij programma's
||* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt

## <a name="manage-referrals"></a>Verwijzingen beheren

|**Role** | **Wat u kunt doen**|**Meer informatie**
|------------------------------|:-------------------------|---|
|Verwijzingsbeheerder|Maak en beheer alles op het tabblad Verwijzingen in Partner Center|[Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
||    Kan alle kansen en leads voor co-verkoop weergeven en bewerken
||    Kan teamleden toewijzen voor een deal
||    Kan bedrijfsprofielen weergeven en bewerken
||    Kan deals weergeven en registreren voor verkoopkansen die zijn gemarkeerd als gewonnen en in aanmerking komen voor dealregistratie
||    Kan ondersteuningstickets maken en weergeven
|Verwijzingsgebruiker|Verkoopkansen voor co-verkoop alleen maken en beheren als ze deel uitmaken van het team |[Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
||    Kan kansen voor co-verkoop creëren voor de locaties waar de rol aan hen is toegewezen.
||    Kan deals weergeven en registreren voor verkoopkansen die zijn gemarkeerd als gewonnen en in aanmerking komen voor dealregistratie als ze teamlid zijn.
||    Kan ondersteuningstickets maken en weergeven
|Bedrijfsprofielbeheerder|Bedrijfsprofielen maken en beheren | [Bedrijfsprofielen beheren](create-a-marketing-profile.md)
||    Kan ondersteuningstickets maken en weergeven

Naast de nieuwe gebruikersrol verwijzingen introduceren we ook het locatiebereik voor deals. In de onderstaande tabel wordt de toegang tot deals op basis van de locatie uitgelegd.

|**Scope** | **Wat u kunt doen** |
|------------------------------|:-------------------------|
|Hele bedrijf | Zowel beheerders als gebruikers hebben toegang tot het maken van deals voor elke locatie in hun bedrijf|
|| Verwijzingsbeheerder heeft toegang om alle deals weer te geven en te bewerken |
|| Verwijzingsgebruikers hebben alleen toegang om alle deals te bekijken en te bewerken als ze deel uitmaken van het team |
|Een of meer locaties | Zowel beheerders als gebruikers hebben toegang tot het maken van deals voor de toegewezen locatie in hun bedrijf|
|| Verwijzingsbeheerder heeft toegang tot het weergeven en bewerken van alle deals die horen bij de toegewezen locaties|
|| Verwijzingsgebruikers hebben toegang tot het weergeven en bewerken van alle deals die horen bij de toegewezen locaties als ze deel uitmaken van het team|

## <a name="manage-incentives"></a>Incentives beheren

|**Role** | **Wat u kunt doen**|**Meer informatie**
|------------------------------|:-------------------------|---|
|Incentives-beheerder|* Incentives initiëren en beheren |[Gebruik deze resources om aan de slag te gaan met incentives](incentives-get-started-intro.md)
||* Kan alle aspecten van incentives-programma's weergeven en bewerken
||* Kan bank- en belastinggegevens bekijken en bewerken
||* Verdiensten voor inkomend en co-op-resultaat weergeven
||* Toegangsondersteuning
||* Incentives-betalingen betwisten|
|Incentives-gebruiker|* Kan incentives-programma's weergeven
||* Kan incentives-claims bekijken en initiëren
||* Verdiensten voor inkomend en co-op-resultaat weergeven
||* Ondersteuningstickets maken voor de Partner Center
||* Partnerondersteuningstickets weergeven die u maakt

## <a name="view-partner-center-insights-data"></a>Gegevens Partner Center Insights weergeven

|**Role** | **Wat u kunt doen**|**Meer informatie**|
|------------------------------|:-------------------------|---|
|Rapportviewer voor leidinggevenden|Toegang tot alle rapportagesets, partnerondersteuningstickets maken, partnerondersteuningstickets weergeven die u maakt|[Overzicht van dashboardrapporten die beschikbaar zijn in Partner Center Insights](insights-overview-report.md)
|Rapportviewer|Toegang tot gegevensrapporten, met uitzondering van omzet en persoonlijke gegevens van klanten en werknemers, partnerondersteuningstickets maken, partnerondersteuningstickets weergeven die u maakt|

## <a name="next-steps"></a>Volgende stappen

- [Gebruikersaccounts maken en rollen en machtigingen toewijzen](create-user-accounts-and-set-permissions.md)
- [Uw accountgegevens controleren wanneer u zich inschrijft voor een nieuw Partner Center-programma](verification-responses.md)
