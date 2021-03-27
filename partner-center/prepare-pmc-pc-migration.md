---
title: Verplaatsen van partner centrum voor partners
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bekijk nuttige informatie en veelgestelde vragen voordat u uw bedrijf verplaatst van het partner lidmaatschaps centrum naar het partner centrum.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b267f89ec1c7b27e87eaaf3d7b594ebbd0fd6942
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633876"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Bereid u voor op uw overstap van Partner Membership Center (PMC) naar het partner centrum

**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikers beheer
- Verkoop agent
- Beheer agent

We verhuizen het lidmaatschaps beheer van het Partner Membership Center (PMC) naar het partner centrum, de enkele bestemming voor het beheren van uw zakelijke relatie met micro soft. We willen dat uw overstap naar partner centrum zo efficiënt en eenvoudig mogelijk is. We hebben een aantal gebieden geïdentificeerd waarvan het partner centrum afwijkt van PMC en we denken dat u ze wilt begrijpen en voor bereidingen voor u hebt gemaakt voordat u de verhuizing maakt.

## <a name="account-and-identity-setup"></a>Account-en identiteits instellingen

Hieronder vindt u antwoorden op veelgestelde vragen over het instellen van accounts en identiteiten.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Wat is een Azure Active Directory-werk account (Azure AD)?

Een Azure-werk account is een toegewezen en geïsoleerde virtuele weer gave van uw bedrijf in de open bare Azure-Cloud die u voor u hebt gemaakt wanneer u zich abonneert op een micro soft-Cloud service zoals Azure, Microsoft Intune of Office 365.

Uw werk account fungeert als host voor uw Azure AD-gebruikers en de informatie hierover: hun e-mail adres, wacht woord, profiel gegevens, machtigingen enzovoort. Het werk account bevat ook groepen, toepassingen en andere informatie die betrekking heeft op een bedrijf en de beveiliging ervan. 

Uw werk-e-mail maakt deel uit van uw Azure Active Directory-Tenant. Als u een account in het partner centrum wilt hebben, moet u een AAD-Tenant hebben. Lees [uw Directory maken in azure AD](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)voor meer informatie over Azure Active Directory.

In het partner centrum gebruikt u uw zakelijke e-mail adres om u aan te melden bij uw account, niet uw persoonlijke e-mail adres.

- Uw werk account: john@contoso.com
- Uw persoonlijke account: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Welk account moet u aanmelden bij het partner centrum als u een AAD-Tenant met micro soft hebt (bijvoorbeeld voor Office 365) en u ook een Tenant hebt voor uw CSP-bedrijf?

U kunt zich aanmelden bij het partner centrum met het CSP-account of uw MPN werk-e-mail account. Als u zich aanmeldt met uw CSP-werk-e-mail, worden de MPN-en CSP-programma gegevens weer gegeven in de linkernavigatiebalk op het dash board. Als u zich aanmeldt met uw MPN Azure AD-Tenant werk-e-mail, ziet u alleen de informatie over het MPN-programma. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Als u uw bestaande Office 365 Azure AD-Tenant niet wilt gebruiken voor het partner centrum, kunt u een nieuwe Tenant maken voordat u migreert van PMC.

Er kunnen veel redenen zijn waarom u geen bestaande Azure AD-Tenant wilt gebruiken om uw partner centrum-account in te stellen. Ga naar het [Azure Portal](https://ms.portal.azure.com/#home) om een nieuwe Azure AD-Tenant te maken voordat u begint met de migratie naar het partner centrum. Volg de richt lijnen in [een nieuwe Tenant maken in azure Active Directory](/azure/active-directory/develop/quickstart-create-new-tenant). Gebruik de nieuwe AAD-Tenant om uw partner centrum-account in te stellen. U moet een globale beheerder zijn om de Tenant te maken. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Gebruikers rollen, inclusief gast gebruikers rollen in het partner centrum

Het partner centrum heeft verschillende typen rollen, afhankelijk van de typen werk die moeten worden uitgevoerd. Er zijn rollen als globale beheerder die Azure AD-rollen zijn. Sommige rollen zijn specifiek voor Program ma's, zoals het programma of prikkels van de Cloud service provider, en er zijn rollen die specifiek zijn voor MPN. Als u wilt weten wat alle functies van het partner centrum zijn, lees dan [gebruikers rollen en machtigingen toewijzen](permissions-overview.md).

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Wat gebeurt er met mijn gebruikers rollen wanneer ze van PMC naar het partner centrum gaan?

Met uitzonde ring van de MPN Global admin of het primaire programma waarmee de migratie wordt verricht, raken alle gebruikers in PMC hun beheerders rollen kwijt. De persoon die de migratie voltooit, moet rollen toewijzen in het partner centrum. De rollen in het partner centrum verschillen van de rollen in PMC. Lees [gebruikers rollen en-machtigingen toewijzen] (permissions-overview.md en [overstappen van PMC naar partner Center](move-pmc-pc-map.md#user-roles) voor meer informatie over gebruikers rollen in het partner centrum.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Wat is het verschil tussen mijn bedrijfs profiel en mijn bedrijfs profiel?

Uw bedrijfs profiel bevat informatie over uw bedrijf met adres, locaties, primaire contact persoon, Bank en belasting gegevens.

Uw bedrijfs profiel is de manier waarop u zichzelf aan klanten presenteert en is een marketing pagina waarin uw logo wordt weer gegeven, Details over uw bedrijfs focus, uw expertise, enzovoort.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Wat betekent het samen voegen van accounts voor mijn account?

Als u dezelfde Azure AD-Tenant gebruikt voor het migreren van meerdere MPN-accounts naar het partner centrum, wordt deze automatisch door het systeem herkend en wordt u gevraagd om uw accounts samen te voegen. Dit geldt ook als er meerdere domeinen zijn gekoppeld aan dezelfde Azure AD-Tenant. 

U kunt nog steeds besluiten om te migreren naar het partner centrum met behulp van afzonderlijke AAD-tenants, maar dit resulteert in een geïsoleerde evaluatie van uw competenties en extra aanschaf kosten. Lees [uw bedrijfs accounts samen voegen](consolidate-accounts.md) voor meer informatie over het samen voegen van accounts

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Als ik meerdere AAD-tenants en één MPN-account heb, kan ik deze dan koppelen aan partner Center?

Ja, in het partner centrum kunt u meerdere Azure AD-tenants koppelen aan het account van één partner centrum.
Lees [uw bedrijfs accounts samen voegen](consolidate-accounts.md) voor meer informatie over het samen voegen van accounts

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Zijn er beperkingen om meerdere Azure AD-tenants toe te voegen aan één partner centrum-account?

Als de Azure AD-Tenant al is gekoppeld aan een bestaand Partner Center-account, kan deze niet worden gekoppeld aan nieuwe partner centrum-accounts met behulp van de functie multitenancy. Een andere manier om dit te zien is, een Azure AD-Tenant kan alleen worden gekoppeld aan één partner centrum-account, maar aan een partner centrum-account kunnen meerdere tenants zijn gekoppeld.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migratie van lidmaatschap van Microsoft Partner Network (MPN) 

Zie de volgende antwoorden op veelgestelde vragen over de migratie van MPN-lidmaatschap.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Wie kan de overstap van PMC naar partner Center uitvoeren?

De MPN van uw bedrijf of de contact persoon van het primaire programma (deze twee rollen worden vaak door dezelfde persoon bewaard) kan de verplaatsing initiëren en uitvoeren.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Wordt de persoon die de migratie uitvoert de primaire contact persoon van het juridisch Profiel van het bedrijf in Partner Center?

Niet noodzakelijkerwijs moet de primaire contact persoon echter iemand zijn die toestemming heeft om overeenkomsten te ondertekenen.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Kan micro soft mijn MPN-lidmaatschap voor mij migreren?

Nee. Micro soft kan u niet helpen uw lidmaatschaps account naar het partner centrum te verplaatsen. U moet uw account verplaatsen door u aan te melden bij PMC met uw werk account (aanmeldings referenties) om het migratie proces te starten. Nadat u de stappen voor het verplaatsen van uw account hebt voltooid, kunt u beginnen met het beheren van uw lidmaatschap en gebruikers rollen en machtigingen toewijzen aan uw team, zodat ze toegang hebben tot voor delen en het lidmaatschap kunnen beheren. 

Micro soft migreert automatisch de huidige competenties, voor delen, locatie-informatie, Bank/belasting gegevens voor prikkels en MCP-koppelingen, waaronder partner University Access.

### <a name="how-will-the-renewal-policy-change"></a>Hoe wordt het vernieuwings beleid gewijzigd?

In partner centrum is het vernieuwings venster van uw jubileum datum tot en met de volgende 30 dagen.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Blijven onze vaardig heden ongewijzigd nadat we naar het partner centrum zijn verplaatst?

Ja, de vaardig heden worden niet beïnvloed door het verplaatsen naar partner Center. Neem contact op met de [ondersteuning](https://partner.microsoft.com/support)als u merkt dat er verschillen zijn.

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Zullen mijn voor delen (inclusief Cloud voordelen, technische ondersteuning, software voordelen, Visual Studio) worden gewijzigd nadat ze zijn verplaatst?

Uw in aanmerking komende voor delen worden niet gewijzigd. Neem contact op met de [ondersteuning](https://partner.microsoft.com/support)als u merkt dat er verschillen zijn.

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Zullen onze micro soft-accounts waaraan de toewijzingen van Visual Studio voor delen worden toegepast, worden gehonoreerd?

Ja. Visual Studio-voor delen die aan Msa's worden toegewezen, worden geaccepteerd en bewaard. Ze worden ook bewaard na verlenging in het partner centrum. Als u echter een MSA-toewijzing verwijdert die eenmaal in het partner centrum is gemigreerd, kan deze niet meer worden toegevoegd aan het partner centrum.

In het partner centrum kan een partner werk accounts en gast gebruikers accounts toevoegen, die MSA zijn van dezelfde Tenant waar de partner MPN-beheerder is in de Azure AD-Tenant. Als de partner een globale beheerder is in meerdere Azure AD-tenants en al deze tenants zijn gekoppeld aan hetzelfde partner centrum-account, mag de partner gebruikers toevoegen aan al deze tenants in de voor delen van Visual Studio en toewijzingen op basis van Azure-gebruik.

Hoewel gast gebruikers met behulp van de MPN-beheerder of globale beheerder kunnen worden toegewezen op gebruik gebaseerde abonnementen van Visual Studio, kunnen gast gebruikers zich niet aanmelden bij het partner centrum met hun MSA. Gast gebruikers kunnen zich echter aanmelden bij Azure en Visual Studio om hun toegewezen voor delen te valideren en te gebruiken.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Hoe moeten we onze MCP-koppelingen en onze partner University-toegang beheren?

Er zijn geen wijzigingen in MCP-koppelingen die van PMC worden verplaatst. Nieuwe werk nemers na het verplaatsen naar het partner centrum moeten echter worden gekoppeld in het partner centrum. Al uw partner University-machtigingen voor bestaande gebruikers blijven behouden, maar nieuwe mede werkers moeten naar [het trainings centrum](https://partner.microsoft.com/training) gaan voor informatie over het verkrijgen van toegang tot partner University.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>MCP-gegevens Hoe kan ik weer geven nadat ik mijn partner centrum heb verplaatst?

Selecteer **competenties** in het Linkernavigatie-navigatie venster op het dash board. Op de pagina **competenties** kunt u het rapport met vaardig heden downloaden. In het rapport met vaardig heden worden uw gebruikers vermeld die de vaardig heden hebben behaald die relevant zijn voor de competenties en Program ma's in het partner centrum. Als uw gebruikers vaardig heden hebben opgedaan, maar deze vaardig heden niet relevant zijn voor de vaardig heden die u aan het werk bent, worden ze niet weer gegeven in het rapport.

### <a name="are-customer-references-used-in-partner-center"></a>Worden klant verwijzingen gebruikt in Partner Center?

Nee, u hebt geen klant verwijzingen nodig om te voldoen aan de competentie vereisten in het partner centrum.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Neemt de partner van record koppelingen over naar het partner centrum?

Ja, er is geen wijziging in de partner van de record. Meer informatie over [het koppelen van uw partner-id aan uw klanten](/azure/billing/billing-partner-admin-link-started).

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Is er sprake van prikkels vanwege de overstap naar partner Center?

Nee, er is geen invloed op prikkels als u uw account hebt verplaatst zonder de locaties te consolideren. Als uw bedrijf meerdere accounts in PMC heeft en, wanneer u overstapt naar partner Center, u besluit om een globaal account samen te voegen, is het niet mogelijk om te stimuleren, maar er kan een vertraging optreden bij het uitvallen van een stimulans. 

Als u niet alle PMC-accounts verplaatst die zijn betrokken bij prikkel Programma's, kunt u geen prikkels meer verdienen die zijn gekoppeld aan deze accounts.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Wat zijn de prikkel rollen in Partner Center?

Prikkel rollen in partner centrum zijn op locatie gebaseerd en omvatten prikkel beheerder en prikkel gebruiker. Zie [gebruikers rollen en machtigingen toewijzen](permissions-overview.md)voor meer informatie over wat die rollen kunnen doen.

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Kunnen beheerders voor stimulansen worden toegewezen op het niveau van globale en locatie?

Ja. U kunt een stimulanss beheerder toewijzen als stimulans beheerder voor alle locaties of elke locatie kan een eigen stimulans beheerder hebben.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Kunnen prikkels worden betaald op het niveau van de globale of locatie?

Prikkels worden alleen betaald op locatie niveau.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Over verwijzingen, hoeveel bedrijfs profielen kunnen we maken?

Uw bedrijf kan net zoveel zakelijke profielen maken als u nodig hebt om de belangen van uw bedrijf volledig te vertegenwoordigen. In elk bedrijfs profiel kunt u Maxi maal vijf locaties, één locatie per land, weer geven. Elk van de bedrijfs profielen kan verwijzingen ontvangen voor elk van zijn locaties.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Hoe worden verwijzingen toegewezen, welke wijzigingen kan ik verwachten? Als ik bijvoorbeeld een wereld wijd bedrijf op de ene markt en locaties op andere markten heb, hoe worden er verwijzingen worden toegewezen?

Verwijzingen worden toegewezen op basis van de zoek parameters die de klant definieert. Ongeacht of u één locatie of veel hebt, als de klant een gewenste locatie heeft opgegeven en u een bedrijf hebt dat aan de andere para meters voldoet, gaat de verwijzing naar die locatie.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Ik Migreer naar het partner centrum vanuit Rusland. Ik krijg een fout bericht over web direct. Hoe kan ik wilt u door gaan met de migratie?

Als er een fout bericht wordt weer gegeven omdat u deelneemt aan het web direct-programma, moet u het volgende doen:

1. Meld u aan bij de portal. Azure.com en maak een nieuwe Azure AD-Tenant. Lees [een nieuwe Azure AD-Tenant maken](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)voor meer informatie.

2. Nadat u de nieuwe Azure AD-Tenant hebt gemaakt, gebruikt u deze om te migreren van het partner lidmaatschaps centrum naar het partner centrum of om te registreren als een net nieuw in partner centrum.