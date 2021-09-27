---
title: Rollen en machtigingen toewijzen aan gebruikers
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Ontdek welke rollen het beste zijn voor de gebruikers van uw bedrijf die commerciële transacties, verwijzingen, incentives of MPN-lidmaatschappen beheren in Partner Center.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 46d17de1ba7572c72162cfd38143ed9aa084c5c7
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075777"
---
# <a name="assign-roles-and-permissions-to-users"></a>Rollen en machtigingen toewijzen aan gebruikers

**Juiste rollen:** Globale | Gebruikersbeheerbeheer | MPN-partnerbeheerder

U hebt uw partnerprofiel ingesteld, inclusief juridische naam en adres, ondersteuningsgegevens, btw-vrijstellingen, bankgegevens en de primaire contactpersoon voor uw bedrijf. De volgende stap bestaat uit het instellen van wachtwoorden en rollen voor uw gebruikers, zodat ze in een Partner Center kunnen gaan werken.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Uw werknemers instellen om in een Partner Center

U bepaalt de soorten toegang die uw gebruikers moeten Partner Center de rollen en machtigingen die u hen geeft. Rollen zijn gerelateerd aan de programma's waar uw bedrijf bij betrokken is. Als uw bedrijf bijvoorbeeld een Cloud Solution Provider-bedrijf (CSP) is, hebt u niet alleen de standaard tenantbeheerrollen voor Azure Active Directory (Azure AD), zoals globale beheerder, maar hebt u ook rollen nodig die specifiek zijn voor het CSP-programma. Elk programma heeft specifieke rollen.

> [!NOTE]
> Azure AD-tenantrollen zijn globale beheerders, gebruikersbeheerders en CSP-rollen. Niet-Azure AD-rollen zijn rollen die de tenant niet beheren, en ze omvatten MPN-partnerbeheerder (Microsoft Partner Network), bedrijfsprofielbeheerder, verwijzingsbeheerder, incentive-beheerder en incentive-gebruiker. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Commerciële transacties beheren in Partner Center (Azure AD- en CSP-rollen)

|**Role**|**Wat ze kunnen doen**| **Werkruimte** | **Meer informatie**|
|----------------------------------|---|---|:---------------------------------|
|Globale beheerder|* Heeft toegang tot alle Microsoft-account/services met volledige bevoegdheden| Accountinstellingen | [Uw Partner Center-account beheren](partner-center-account-setup.md) |
||* Ondersteuningstickets maken voor Partner Center | Help en ondersteuning |
||* Partnerondersteuningstickets weergeven die u maakt | Help en ondersteuning |
||* Overeenkomsten, prijslijsten en aanbiedingen weergeven | Prijzen |
||* Partnergebruikers weergeven, maken en beheren | Accountinstellingen |
||  Facturering, facturen en reconbestanden weergeven, maken en beheren | Billing |
| Beheerder van gebruikersbeheer   | * Gebruikers weergeven, maken en beheren| Voordelen | [Uw voordelen Microsoft Partner Network en aanbiedingen in uw Partner Center](manage-your-partner-network-benefits.md)
||* Alles weergeven partnerprofielen | Customers |
||* Ondersteuningstickets maken voor de Partner Center | Help en ondersteuning |
||* Partnerondersteuningstickets weergeven die u maakt | Help en ondersteuning |
|Factureringsbeheerder | - Facturering, facturen en reconbestanden weergeven, maken en beheren| Billing | [Uw rekening lezen](billing.md)
||* Prijzen weergeven | Billing |
||* Ondersteuningstickets maken voor de Partner Center | Help en ondersteuning |
||* Partnerondersteuningstickets weergeven die u maakt | Help en ondersteuning |
|Standaardgebruiker|  Mijn profiel weergeven   | Accountinstellingen | [Uw wachtwoord opnieuw instellen](reset-my-pasword.md)
|Beheeragent | * Klantbeheer| Customers | [Communiceren met uw klanten](connect-with-your-customers.md)
||* Apparaatlijst toevoegen aan de Partner Center | Accountinstellingen |
||* Profielen maken en toepassen op apparaten | Accountinstellingen |
||* Abonnementsbeheer | Accountinstellingen |
||* Service health and service requests for customers (Status- en serviceaanvragen voor klanten) | Help en ondersteuning |
||* Gedelegeerde beheerdersbevoegdheden aanvragen | Accountinstellingen |
||* Prijzen en aanbiedingen weergeven | Prijzen |
||* Facturering | Billing |
||* Beheer namens een klant | Accountinstellingen |
||* Een reseller met toegevoegde waarde registreren | Accountinstellingen |
||* Ondersteuningstickets maken voor de Partner Center | Help en ondersteuning |
||* Partnerondersteuningstickets weergeven die u maakt | Help en ondersteuning |
|Verkoopagent | * Klantbeheer| Billing | [Factureringsondersteuning bieden voor uw klanten en hulp bieden bij het beantwoorden van hun vragen over facturering](provide-billing-support.md)
||* Apparaatlijst toevoegen aan de Partner Center | Accountinstellingen |
||* Abonnementsbeheer | Accountinstellingen |
||* Ondersteuningstickets weergeven | Help en ondersteuning |
||* Een relatie met een klant aanvragen | Customers |
||* Prijzen en aanbiedingen weergeven | Prijzen |
||* Leads van klanten beheren | Verwijzingen |
||* De klantovereenkomst weergeven | Customers |
||* Een reseller met toegevoegde waarde inschrijven | Accountinstellingen |
||* Ondersteuningstickets maken voor de Partner Center | Help en ondersteuning |
||* Partnerondersteuningstickets weergeven die u maakt | Help en ondersteuning |
|Helpdeskagent| * Een klant zoeken en weergeven| Help en ondersteuning | [Problemen naar Microsoft escaleren en leren welke problemen geschikter zijn voor escalatie van Microsoft](escalate-problems-to-microsoft.md)
||* Klantgegevens bewerken  | Help en ondersteuning |
||* Hulp bij het oplossen van klantproblemen met facturerings- of abonnementsbeheer | Help en ondersteuning |
||* Ondersteuning aanvragen namens klanten | Help en ondersteuning |
||* Abonnementen en factureringsproblemen namens klanten beheren | Billing |
||* Ondersteuningstickets maken voor de Partner Center | Help en ondersteuning |
||* Partnerondersteuningstickets weergeven die u maakt  | Help en ondersteuning |

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Configuratiescherm Vendor (CPV). (CSP-rol en niet-Azure AD-rol)

CPV's ontwikkelen apps voor gebruik door CSP-partners, zodat ze hun systemen kunnen integreren met Partner Center API's.

|**Role**                   | **Wat u kunt doen**      | **Werkruimte** | **Meer informatie**|
|------------------------------|:----------------------------|---------------|---------------|
|Globale beheerder| Uw CPV-profiel (Configuratiescherm Vendor) weergeven en beheren|  | [Registreren als een Configuratiescherm leverancier om CSP-partnersystemen te integreren met Partner Center API's](enroll-as-cpv.md)
||Uw gebruikers weergeven en beheren die toegang nodig hebben tot CPV-mogelijkheden |  |

### <a name="guest-user-must-be-added-to-the-azure-ad-tenant"></a>Gastgebruiker (moet worden toegevoegd aan de Azure AD-tenant)

| **Gastgebruiker**    | **Rollen**            |
|----------------------|:------------------------|
|                      | MPN-partnerbeheerder       |
|                      | Bedrijfsprofielbeheerder  |
|                      | Verwijzingsbeheerder         |

## <a name="manage-mpn-membership-and-your-company"></a>MPN-lidmaatschap en uw bedrijf beheren

Deze rollen zijn **geen** Azure AD-rollen. Ze worden gebruikt om het bedrijf te beheren in plaats van de tenant.

| **Role** | **Wat u kunt doen** | **Werkruimte** | **Meer informatie**|
|----------------------------|:----------------------------|-----|
|MPN-partnerbeheerder|* Partnerserviceaanvragen weergeven, maken en beheren| Lidmaatschap | [Een abonnement op Microsoft Action Pack of een Silver- of Gold-competentie kopen of verlengen](mpn-get-action-pack.md) |
| |* Juridische, bedrijfs-, zakelijke en MPN-profielen weergeven | Accountinstellingen |
| |* Gebruikersdetails en hun vaardigheden weergeven | Lidmaatschap |
| |* Competenties weergeven | Lidmaatschap |
| |* Voordelen weergeven en beheren | Voordelen |
| |* MPN-aanbiedingen weergeven en kopen | Lidmaatschap |
| |* MpN-aanbiedingen bestelgeschiedenis en facturen weergeven | Lidmaatschap |
| |* Indicatorgegevens voor partnerbijdragen weergeven | Lidmaatschap |
| |* Kan werken in het hulpprogramma Voor validatie van validatie | Lidmaatschap |
| |* Klantgegevensanalyses weergeven | Inzichten |
| |* Andere gebruikersrollen binnen het bedrijf weergeven, maar kunnen geen rollen toewijzen | Accountinstellingen |
| |* Ondersteuningstickets maken voor de Partner Center | Help en ondersteuning |
| |* Partnerondersteuningstickets weergeven die u maakt | Help en ondersteuning |
| Accountbeheerder| Locaties toevoegen| Accountinstellingen | [Locaties beheren](manage-locations.md)
| |* Profielen beheren die betrekking hebben op de accounts die u beheert | Accountinstellingen |
| |* Rollen voor gebruikers in tenant toewijzen aan niet-Azure AD-rollen | Accountinstellingen |
| |* Locaties inschrijven bij programma's |  |
| |* Ondersteuningstickets maken voor de Partner Center | Help en ondersteuning |
| |* Partnerondersteuningstickets weergeven die u maakt | Help en ondersteuning |

## <a name="manage-referrals"></a>Verwijzingen beheren

|**Role** | **Wat u kunt doen**| **Werkruimte** | **Meer informatie** |
|------------------------------|:---|-----------------------|---|
|Verwijzingsbeheerder|Maak en beheer alles op het tabblad Verwijzingen in Partner Center| Verwijzingen | [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
||    Kan alle kansen en leads voor co-verkoop weergeven en bewerken | Verwijzingen |
||    Kan teamleden toewijzen voor een deal | Verwijzingen |
||    Kan bedrijfsprofielen weergeven en bewerken | Verwijzingen |
||    Kan deals weergeven en registreren voor verkoopkansen die zijn gemarkeerd als gewonnen en in aanmerking komen voor dealregistratie | Verwijzingen |
||    Kan ondersteuningstickets maken en weergeven | Help en ondersteuning |
|Verwijzingsgebruiker|Verkoopkansen voor co-verkoop alleen maken en beheren als ze deel uitmaken van het team | Verwijzingen | [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
||    Kan kansen voor co-verkoop creëren voor de locaties waar de rol aan hen is toegewezen. | Verwijzingen |
||    Kan deals weergeven en registreren voor verkoopkansen die zijn gemarkeerd als gewonnen en in aanmerking komen voor dealregistratie als ze teamlid zijn. | Verwijzingen |
||    Kan ondersteuningstickets maken en weergeven | Help en ondersteuning |
|Bedrijfsprofielbeheerder|Bedrijfsprofielen maken en beheren | Verwijzingen | [Bedrijfsprofielen beheren](create-a-marketing-profile.md)
||    Kan ondersteuningstickets maken en weergeven | Help en ondersteuning |

Naast de nieuwe gebruikersrol verwijzingen introduceren we ook het locatiebereik voor deals. In de onderstaande tabel wordt de toegang tot deals op basis van de locatie uitgelegd.

|**Scope** | **Wat u kunt doen** | **Werkruimte** |
|------------------------------|:-----------------|--------|
|Hele bedrijf | Zowel beheerders als gebruikers hebben toegang tot het maken van deals voor elke locatie in hun bedrijf| Verwijzingen |
|| Verwijzingsbeheerder heeft toegang om alle deals weer te geven en te bewerken | Verwijzingen |
|| Verwijzingsgebruikers hebben alleen toegang om alle deals te bekijken en te bewerken als ze deel uitmaken van het team | Verwijzingen |
|Een of meer locaties | Zowel beheerders als gebruikers hebben toegang tot het maken van deals voor de toegewezen locatie in hun bedrijf| Verwijzingen |
|| Verwijzingsbeheerder heeft toegang tot het weergeven en bewerken van alle deals die horen bij de toegewezen locaties| Verwijzingen |
|| Verwijzingsgebruikers hebben toegang tot het weergeven en bewerken van alle deals die horen bij de toegewezen locaties als ze deel uitmaken van het team| Verwijzingen |

## <a name="manage-incentives"></a>Incentives beheren

|**Role** | **Wat u kunt doen**| **Werkruimte** | **Meer informatie** |
|---------|:-------------------|---------------|----------------|
|Incentives-beheerder|* Incentives initiëren en beheren | Incentives | [Gebruik deze resources om aan de slag te gaan met incentives](incentives-get-started-intro.md) |
||* Kan alle aspecten van incentives-programma's weergeven en bewerken | Incentives |
||* Kan bank- en belastinggegevens bekijken en bewerken | Incentives |
||* Verdiensten voor inkomend en co-op-resultaat weergeven | Incentives |
||* Toegangsondersteuning | Help en ondersteuning |
||* Incentives-betalingen betwisten | Incentives |
|Incentives-gebruiker|* Kan incentives-programma's weergeven | Incentives ||
||* Kan incentives-claims bekijken en initiëren | Incentives |
||* Verdiensten voor inkomend en co-op-resultaat weergeven | Incentives |
||* Ondersteuningstickets maken voor de Partner Center | Help en ondersteuning |
||* Partnerondersteuningstickets weergeven die u maakt | Help en ondersteuning |

## <a name="view-partner-center-insights-data"></a>Gegevens Partner Center Insights weergeven

|**Role** | **Wat u kunt doen** | **Werkruimte** | **Meer informatie** |
|---------|:--------------------|---------------|----------------|
|Rapportviewer voor leidinggevenden|Toegang tot alle rapportagesets, partnerondersteuningstickets maken, partnerondersteuningstickets weergeven die u maakt| Inzichten | [Overzicht van dashboardrapporten die beschikbaar zijn in Partner Center Insights](insights-overview-report.md) |
|Rapportviewer|Toegang tot gegevensrapporten, met uitzondering van omzet en persoonlijke gegevens van klanten en werknemers, partnerondersteuningstickets maken, partnerondersteuningstickets weergeven die u maakt | Inzichten | |

## <a name="next-steps"></a>Volgende stappen

- [Gebruikersaccounts maken en rollen en machtigingen toewijzen](create-user-accounts-and-set-permissions.md)
- [Uw accountgegevens controleren wanneer u zich inschrijft voor een nieuw Partner Center-programma](verification-responses.md)
