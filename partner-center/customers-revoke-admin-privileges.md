---
title: De beheerders bevoegdheden van een klant verkrijgen
ms.topic: how-to
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Verkrijg de machtigingen die u nodig hebt voor het beheren van de service of het abonnement van een klant in hun naam. Meer informatie over hoe machtigingen worden verleend, ingetrokken en beheerd.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.openlocfilehash: dcfc552016560ecc3167deebf96f7a75a72048bc
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/04/2020
ms.locfileid: "92528124"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Machtigingen voor het beheren van de service of het abonnement van een klant verkrijgen

**Van toepassing op**

- Partnercentrum

**Juiste rollen**

- Beheer agent
- Verkoop agent

Voor het beheren van de service of het abonnement van een klant in hun naam, moet de klant u beheerders machtigingen voor die service verlenen. Als u beheerders machtigingen van een klant wilt ophalen, kunt u een e-mail verzenden naar een reseller-relatie aanvraag. Nadat de klant uw aanvraag heeft goedgekeurd, kunt u zich aanmelden bij de beheer portal van de service en de service namens de klant beheren. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Een klant uitnodigen om een reseller-relatie met u te maken

1.  Selecteer **klanten** en selecteer vervolgens **een reseller-relatie aanvragen** .

2.  Bekijk op de volgende pagina het concept-e-mailbericht. U kunt het conceptbericht openen in de standaardtoepassing voor e-mail, of u kunt het bericht kopiëren naar het klembord en in een e-mailbericht plakken. 

    >[!IMPORTANT]
    >U kunt de tekst in het e-mailbericht bewerken, maar vergeet niet om de koppeling op te nemen, aangezien deze is gepersonaliseerd om de klant rechtstreeks naar uw account te brengen. 
    
3.  Selecteer **gereed** wanneer u deze stap hebt voltooid.

4.  Verzend het e-mail bericht naar uw klant.

5.  Nadat de klant uw uitnodiging heeft geaccepteerd, wordt deze weer gegeven op uw **klanten** pagina en kunt u de service van daaruit inrichten en beheren.

6.  Als u het account, de services, gebruikers en licenties van de klant wilt beheren, vouwt u de record van de klant uit door de pijl-omlaag bij de naam te selecteren en selecteert u vervolgens de beheer portal voor de service die u wilt beheren.

>[!IMPORTANT]  
>Klanten kunnen beheerders machtigingen opnieuw toewijzen of verwijderen in de beheer portal van een service. Tenzij en totdat u de overeenkomst met de klant opnieuw hebt door lopen, blijft u verantwoordelijk voor het leveren van klanten ondersteuning en het naleven van de voor waarden van de overeenkomst in de Cloud reseller, zelfs nadat een klant de beheerders machtigingen opnieuw heeft toegewezen of verwijderd. Als de klant hulp nodig heeft, neemt u contact op met micro soft ondersteuning om een service aanvraag namens de klant te openen.

Uw klanten kunnen nagaan of hun partners beheerders bevoegdheden voor hun Tenant hebben in de Office 365-beheer Portal. Om dit te doen:

1. De klant moet zich aanmelden bij de Office 365-beheer portal als globale beheerder.

2. Selecteer **instellingen**  >  **partner relaties** .

3. Op de pagina **partner relaties** wordt de klant een lijst weer gegeven met de partners met wie ze werken en de gebruikers aan wie de bevoegdheden voor gedelegeerd beheer zijn verleend voor hun Tenant.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Klanten kunnen de gedelegeerde beheerders bevoegdheden van een partner beheren 

Uw klant kan besluiten uw gedelegeerde beheerders bevoegdheden te verwijderen van hun Tenant, maar de relatie met u te behouden voor het vernieuwen van het abonnement en de licentie. Klanten beheren rechten en machtigingen voor hun Office 365-accounts op de pagina **partner relaties** in het Office 365-beheer centrum. Op deze pagina kunnen klanten het volgende doen:

- Bekijk met welke partners ze een relatie hebben en welke partners gedelegeerde beheerders bevoegdheden hebben

- De machtigingen voor gedelegeerd beheer van een partner van de Tenant verwijderen

Machtigingen voor gedelegeerd beheer van een partner verwijderen:

1. Selecteer op de pagina **partner relaties** de partner van belang.
2. Selecteer in het detail venster **gedelegeerde beheerder verwijderen** .
3. Selecteer **verwijderen** in het bevestigings venster.

>[!IMPORTANT]  
>Toewijzingen van Azure AD-rollen aan de partner zijn impliciet. Als u probeert om de leden van de Azure AD-rollen te vermelden met behulp van Azure AD-Portal/Power shell/Graph, wordt de partner niet geretourneerd. Als u wilt weten of de partners zijn toegewezen aan Azure AD-rollen, moet u verwijzen naar de pagina partner relaties in de Office 365-beheer Portal om erachter te komen of de bevoegdheid gedelegeerd beheer is verleend aan de partner.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Gedelegeerde beheerders bevoegdheden in azure AD 

Er zijn twee beveiligings groepen, beheerders agenten en helpdesk agenten in de Azure AD-Tenant van de partner die worden gebruikt voor gedelegeerd beheer. Wanneer een klant de bevoegdheid gedelegeerd beheer verleent aan een partner:

- De groep Administrator agent is toegewezen aan de rol van globale beheerder in de Azure AD-Tenant van de klant.

- De agent groep helpdesk wordt toegewezen aan de beheerdersrol van de helpdesk beheerder in de Azure AD-Tenant van de klant.

Op basis van de toegewezen Directory functies kunnen leden van beide groepen zich aanmelden bij de Azure AD-Tenant en O365-services van de klant met behulp van hun partner referenties en beheerder namens de klant.

Als uw klant gedelegeerde beheerders bevoegdheden verwijdert, worden de toewijzingen van Azure AD-rollen verwijderd en kunt u de Azure AD-Tenant van de klant niet meer beheren.

### <a name="azure-subscriptions-and-resource-management"></a>Azure-abonnementen en resource beheer

Elk Azure-abonnement heeft een eigen set resource management-rollen. Voordat een CSP-partner het Azure-abonnement van een klant kan beheren, moet de partner worden toegewezen aan een of meer rollen onder het Azure-abonnement. Specifiek:

- Wanneer een klant een uitnodiging voor een wederverkoper accepteert en gedelegeerde beheer bevoegdheid verleent aan een partner, krijgt de partner niet automatisch toegang tot de bestaande Azure-abonnementen onder de Tenant van de klant.

- Wanneer de CSP-partner een nieuw Azure-abonnement voor de klant aanbiedt, wordt de groep Administrator-agents onder de Tenant van de CSP-partner automatisch toegewezen aan de eigenaar van het abonnement. Op basis van deze roltoewijzing kunnen leden van de groep resources onder het abonnement openen en beheren.

- Wanneer een klant gedelegeerde beheer rechten van een partner met behulp van Office 365 Portal verwijdert, kan de partner nog steeds het Azure-abonnement van de klant beheren, zolang de partner nog steeds is toegewezen aan een of meer functies onder het abonnement. Als u wilt voor komen dat de partner het Azure-abonnement beheert, moet de klant de roltoewijzing verwijderen.

## <a name="windows-autopilot"></a>Windows Autopilot

Vanuit Partner Center kunnen CSP-partners auto pilot-profielen beheren voor hun klanten zonder gedelegeerde beheerders bevoegdheden onder deze omstandigheden: 

- Als een klant gedelegeerde beheer bevoegdheden verwijdert, maar een wederverkoper met u houdt, kunt u de auto pilot-profielen voor hen blijven beheren.

- U kunt klant apparaten beheren die u of een andere partner hebt toegevoegd. 

- U kunt geen apparaten beheren die uw klant heeft toegevoegd via de Microsoft Store voor bedrijven, Microsoft Store voor onderwijs of Microsoft Intune Portal.

Zie voor meer informatie over automatische pilot het [apparaat instellen vereenvoudigen met Windows auto pilot](autopilot.md).

>[!IMPORTANT]  
>De huidige automatische pilot-ervaring in het partner centrum kan worden gewijzigd. Op het moment van publicatie van dit artikel worden de volgende wijzigingen in overweging genomen:

- Aan de partner moet een gedelegeerde beheer bevoegdheid worden verleend door de klant voordat de partner profielen kan toevoegen, bijwerken of verwijderen en profiel kan Toep assen op of verwijderen van apparaten in de Tenant van de klant.

- Aan de partner moet een gedelegeerde beheer bevoegdheid worden verleend door de klant voordat de partner apparaten kan verwijderen die door andere partners of door de klant in de Tenant van de klant worden toegevoegd. Anders kan de partner alleen apparaten verwijderen die eerder zijn toegevoegd door dezelfde partner.
