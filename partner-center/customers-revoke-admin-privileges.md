---
title: De beheerdersbevoegdheden van een klant verkrijgen
ms.topic: how-to
ms.date: 12/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Verkrijg de machtigingen die u nodig hebt om de service of het abonnement van een klant namens hen te beheren. Meer informatie over hoe machtigingen worden verleend, ingetrokken en beheerd.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: 779e76d6bb3e8df679a5ca6fa8ce441e42529161
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147289"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant

**Juiste rollen:** beheeragent | Verkoopagent

Als u de service of het abonnement van een klant namens hen wilt beheren, moet de klant u beheerdersmachtigingen voor die service verlenen. Als u beheerdersmachtigingen van een klant wilt krijgen, moet u hen een aanvraag voor een resellerrelatie sturen. Nadat de klant uw aanvraag heeft goedgekeurd, kunt u zich aanmelden bij de beheerportal van de service en de service namens de klant beheren. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Een klant uitnodigen om een resellerrelatie met u tot stand te stellen

1.  Selecteer **Klanten** en selecteer vervolgens **Een resellerrelatie aanvragen.**

2.  Bekijk op de volgende pagina het concept-e-mailbericht. U kunt het conceptbericht openen in de standaardtoepassing voor e-mail, of u kunt het bericht kopiëren naar het klembord en in een e-mailbericht plakken. 

    >[!IMPORTANT]
    >U kunt de tekst in het e-mailbericht bewerken, maar vergeet niet om de koppeling op te nemen, aangezien deze is gepersonaliseerd om de klant rechtstreeks naar uw account te brengen. 
    
3.  Selecteer **Gereed** wanneer u deze stap hebt voltooid.

4.  Verzend het e-mailbericht naar uw klant.

5.  Nadat de klant uw uitnodiging heeft geaccepteerd,  wordt deze weergegeven op de pagina Klanten en kunt u de service voor de klant van hieruit inrichten en beheren.

6.  Als u het account, de services, gebruikers en licenties van de klant wilt beheren, vouwt u de record van de klant uit door de pijl-omlaag bij de naam te selecteren en vervolgens de beheerportal te selecteren voor de service die u wilt beheren.

>[!IMPORTANT]  
>Klanten kunnen beheerdersmachtigingen opnieuw toewijzen of verwijderen in de beheerportal van een service. U moet de klant echter informeren dat het verwijderen van uw beheerdersmachtigingen betekent dat u niet langer namens hen een serviceaanvraag voor Microsoft kunt openen. U kunt dit soort serviceaanvragen pas namens de klant openen als u uw overeenkomst met de klant hebt gesloten.

Uw klanten kunnen in de Office 365-beheerportal zien welke van hun partners beheerdersbevoegdheden hebben voor hun tenant. Om dit te doen:

1. De klant moet zich aanmelden bij de Office 365-beheerportal als globale beheerder.

2. Selecteer **Instellingen**  >  **Partnerrelaties.**

3. Op de **pagina Partnerrelaties** ziet de klant een lijst met de partners met wie ze werken en de partners die gedelegeerde beheerdersbevoegdheden hebben gekregen voor hun tenant.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Klanten kunnen de gedelegeerde beheerdersbevoegdheden van een partner beheren 

Uw klant kan besluiten om uw gedelegeerde beheerdersbevoegdheden te verwijderen uit hun tenant, maar de relatie met u te behouden voor abonnements- en licentievernieuwingsdoeleinden. Klanten beheren rechten en machtigingen voor hun Office 365-accounts op de **pagina Partnerrelaties** in het Office 365-beheercentrum. Op deze pagina kunnen klanten:

- Zien met welke partners ze een relatie hebben en met welke partners beheerdersbevoegdheden zijn gedelegeerd

- De gedelegeerde beheerdersbevoegdheden van een partner uit de tenant verwijderen

Gedelegeerde beheerbevoegdheden van een partner verwijderen:

1. Selecteer op **de pagina** Partnerrelaties de partner van belang.
2. Selecteer in het detailvenster **Gedelegeerde beheerder verwijderen.**
3. Selecteer Verwijderen in het **bevestigingsvenster.**

>[!IMPORTANT]  
>Azure AD-roltoewijzingen aan de partner zijn impliciet. Als u probeert de leden van de Azure AD-rollen weer te geven met behulp van de Azure AD-portal/PowerShell/Graph, wordt de partner niet geretourneerd. Als u wilt weten of de partners zijn toegewezen aan Azure AD-rollen, raadpleegt u de pagina Partnerrelaties in de Office 365-beheerportal om erachter te komen of gedelegeerde beheermachtiging is verleend aan de partner of niet.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Gedelegeerde beheerdersbevoegdheden in Azure AD 

Er zijn twee beveiligingsgroepen, beheerdersagents en helpdeskmedewerkers, in de Azure AD-tenant van de partner die worden gebruikt voor gedelegeerd beheer. Wanneer een klant gedelegeerde beheerrechten verleent aan een partner:

- De beheerdersagentgroep wordt toegewezen aan de rol Globale beheerder in de Azure AD-tenant van de klant.

- De groep Helpdeskagent wordt toegewezen aan de rol Helpdeskbeheerder in de Azure AD-tenant van de klant.

Op basis van de toegewezen directoryrollen kunnen leden van beide groepen zich namens de klant aanmelden bij de Azure AD-tenant en O365-services van de klant.

Als uw klant gedelegeerde beheerdersbevoegdheden verwijdert, worden de Azure AD-roltoewijzingen verwijderd en kunt u de Azure AD-tenant van de klant niet meer beheren.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-abonnementen en resourcebeheer

Elk Azure-abonnement heeft een eigen set resourcebeheerrollen. Voordat een CSP-partner het Azure-abonnement van een klant kan beheren, moet de partner worden toegewezen aan een of meer rollen onder het Azure-abonnement. Met name:

- Wanneer een klant een reselleruitnodiging accepteert en gedelegeerde beheerrechten verleent aan een partner, krijgt de partner niet automatisch toegang tot bestaande Azure-abonnementen onder de tenant van de klant.

- Wanneer de CSP-partner een nieuw Azure-abonnement voor de klant indeelt, krijgt de groep Beheerdersagenten onder de tenant van de CSP-partner automatisch de rol Eigenaar toegewezen onder het abonnement. Op basis van deze roltoewijzing hebben leden van de groep toegang tot en beheer van resources onder het abonnement.

- Wanneer een klant gedelegeerde beheerdersbevoegdheden verwijdert van een partner met behulp van de Office 365-portal, kan de partner nog steeds het Azure-abonnement van de klant beheren zolang de partner nog steeds is toegewezen aan een of meer rollen in het abonnement. Als u wilt voorkomen dat de partner het Azure-abonnement beheert, moet de klant de roltoewijzing verwijderen.

## <a name="windows-autopilot"></a>Windows Autopilot

Vanuit Partner Center kunnen CSP-partners Autopilot-profielen voor hun klanten beheren zonder gedelegeerde beheerdersbevoegdheden onder deze omstandigheden: 

- Als een klant gedelegeerde beheerbevoegdheden verwijdert, maar een resellerrelatie met u behoudt, kunt u autopilot-profielen voor deze klanten blijven beheren.

- U kunt klantapparaten beheren die u of een andere partner heeft toegevoegd. 

- U kunt geen apparaten beheren die uw klant heeft toegevoegd via de Microsoft Store voor Bedrijven, Microsoft Store voor Onderwijs of Microsoft Intune Portal.

Zie Setup van apparaten vereenvoudigen met autopilot [voor meer informatie Windows Autopilot.](autopilot.md)

>[!IMPORTANT]  
>De huidige Autopilot-beheerervaring in Partner Center mogelijk blijven wijzigen. Op het moment dat dit artikel werd gepubliceerd, worden de volgende wijzigingen in aanmerking genomen:

- De partner moet gedelegeerde beheerrechten van de klant krijgen voordat de partner profielen kan toevoegen/bijwerken/verwijderen en profiel kan toepassen/verwijderen van apparaten in de tenant van de klant.

- Aan de partner moet gedelegeerde beheerrechten worden verleend door de klant voordat de partner apparaten kan verwijderen die zijn toegevoegd door andere partners of door de klant in de tenant van de klant. Anders kan de partner alleen apparaten verwijderen die eerder door dezelfde partner zijn toegevoegd.
