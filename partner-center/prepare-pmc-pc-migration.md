---
title: Verplaatsen van Partner Membership Center
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Bekijk nuttige informatie en veelgestelde vragen voordat u uw bedrijf verplaatst van Partner Membership Center naar Partner Center.
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 7f533240d5236f03fe277d4c6dfa02ed1c58b63c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855009"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Voorbereiden op de overstap van Partner Membership Center (PMC) naar Partner Center

**Juiste rollen:** Globale | Gebruikersbeheerbeheer | Verkoopagent | Beheeragent

Lidmaatschapsbeheer wordt verplaatst van Partner Membership Center (PMC) naar de Partner Center: de enige bestemming voor het beheren van uw zakelijke relatie met Microsoft. We willen dat uw overstap Partner Center zo efficiënt en eenvoudig mogelijk is. We hebben een aantal gebieden geïdentificeerd waar de Partner Center verschilt van PMC en we denken dat u deze wilt begrijpen en voorbereiden voordat u de overstap maakt.

## <a name="account-and-identity-setup"></a>Account en identiteit instellen

Hieronder vindt u antwoorden op veelvoorkomende vragen over het instellen van een account en identiteit.

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Wat is een Azure Active Directory(Azure AD)-werkaccount?

Een Azure-werkaccount is een toegewezen en geïsoleerde virtuele weergave van uw bedrijf in de openbare Azure-cloud die voor u wordt gemaakt wanneer u zich abonneert op een Microsoft-cloudservice zoals Azure, Microsoft Intune of Office 365.

Uw werkaccount host uw Azure AD-gebruikers en de informatie over hen, zoals hun e-mailadres, wachtwoorden, profielgegevens, machtigingen, en meer. Het werkaccount bevat ook groepen, toepassingen en andere informatie met betrekking tot een bedrijf en de beveiliging ervan. 

Uw werke-mail maakt deel uit van uw Azure Active Directory-tenant. Als u een account in Partner Center, moet u een AAD-tenant hebben. Lees Uw directory maken in Azure AD Azure Active Directory [meer informatie over uw account.](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)

In Partner Center gebruikt u uw werk-e-mail om u aan te melden bij uw account, niet uw persoonlijke e-mailadres.

- Uw werkaccount: john@contoso.com
- Uw persoonlijke account: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Met welk account moet u zich aanmelden bij Partner Center als u een AAD-tenant hebt met Microsoft (bijvoorbeeld voor Office 365) en u ook een tenant voor uw CSP-bedrijf hebt?

U kunt zich aanmelden Partner Center met het CSP-account of uw MPN-werk-e-mailaccount. Als u ervoor kiest om u aan te melden met uw CSP-werke-mail, wordt in het linkernavigatievenster op het dashboard zowel MPN- als CSP-programmagegevens weergegeven. Als u zich met de werk-e-mail van uw MPN Azure AD-tenant hebt aanmelden, ziet u alleen de programmagegevens van uw MPN. 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>Als u uw bestaande Office 365 Azure AD-tenant niet wilt gebruiken voor Partner Center, kunt u een nieuwe tenant maken voordat u migreert van PMC.

Er kunnen verschillende redenen zijn waarom u geen bestaande Azure AD-tenant wilt gebruiken om uw Partner Center instellen. Voordat u begint met migreren naar Partner Center, gaat u naar de [Azure Portal](https://ms.portal.azure.com/#home) een nieuwe Azure AD-tenant te maken. Volg de instructies in [Een nieuwe tenant maken in Azure Active Directory.](/azure/active-directory/develop/quickstart-create-new-tenant) Gebruik de nieuwe AAD-tenant om uw Partner Center instellen. U moet een globale beheerder zijn om de tenant te kunnen maken. 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>Gebruikersrollen, waaronder gastgebruikersrollen in Partner Center

Partner Center heeft verschillende soorten rollen, afhankelijk van de typen werk die moeten worden uitgevoerd. Er zijn rollen zoals globale beheerders die Azure AD-rollen zijn. Sommige rollen zijn specifiek voor programma's zoals het cloudserviceproviderprogramma of incentives, en er zijn rollen die specifiek zijn voor MPN. Als u wilt weten wat alle Partner Center zijn, leest u [Gebruikersrollen en -machtigingen toewijzen.](permissions-overview.md)

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>Wat gebeurt er met de rollen van mijn gebruikers wanneer ze van PMC naar Partner Center?

Met uitzondering van de contactpersoon van de globale beheerder van het MPN of het primaire programma die de migratie heeft uitgevoerd, verliezen alle gebruikers in PMC hun beheerdersrollen. De persoon die de migratie voltooit, moet rollen toewijzen in Partner Center. De rollen in Partner Center verschillen van de rollen in PMC. Lees [Gebruikersrollen en -machtigingen toewijzen](permissions-overview.md en Verplaatsen van [PMC](move-pmc-pc-map.md#user-roles) naar Partner Center voor meer informatie over gebruikersrollen in Partner Center.

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>Wat is het verschil tussen mijn bedrijfsprofiel en mijn bedrijfsprofiel?

Uw bedrijfsprofiel is de informatie over uw bedrijf, waaronder het adres, de locaties, de primaire contactpersoon, de bank en de belastinggegevens.

Uw bedrijfsprofiel is de manier waarop u zich aan klanten presenteert. Dit is een marketingpagina waarop uw logo, details over uw zakelijke focus, uw expertise, enzovoort worden weergegeven.

### <a name="what-does-account-consolidation-mean-for-my-account"></a>Wat betekent accountconsolidatie voor mijn account?

Als u dezelfde Azure AD-tenant gebruikt om meerdere MPN-accounts te migreren naar Partner Center, herkent het systeem dat automatisch en wordt u gevraagd uw accounts te consolideren. Dit geldt zelfs als er meerdere domeinen zijn gekoppeld aan dezelfde Azure AD-tenant. 

U kunt nog steeds besluiten om te migreren naar Partner Center afzonderlijke AAD-tenants, maar houd er rekening mee dat dit resulteert in een geïsoleerde evaluatie van uw competenties en extra aankoopkosten. Lees Uw bedrijfsaccounts consolideren voor meer informatie [over accountconsolidatie](consolidate-accounts.md)

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>Als ik meerdere AAD-tenants en één MPN-account heb, is het dan mogelijk om deze te koppelen in Partner Center?

Ja, in Partner Center kunt u meerdere Azure AD-tenants koppelen aan een Partner Center account.
Lees Uw bedrijfsaccounts consolideren voor meer informatie [over accountconsolidatie](consolidate-accounts.md)

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>Gelden er beperkingen voor het toevoegen van meerdere Azure AD-tenants aan één Partner Center account?

Als de Azure AD-tenant al is gekoppeld aan een bestaand Partner Center-account, kan deze niet worden gekoppeld aan nieuwe Partner Center-accounts met behulp van de functie voor meerdere tenants. Een andere manier om dit te zien is: een Azure AD-tenant kan alleen worden gekoppeld aan één Partner Center-account, maar aan een Partner Center-account kunnen meerdere tenants zijn gekoppeld.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>migratie Microsoft Partner Network (MPN) lidmaatschap 

Zie de volgende antwoorden op veelvoorkomende vragen over de migratie van MPN-lidmaatschappen.

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>Wie kan de overstap van PMC naar Partner Center?

De globale beheerder van het MPN van uw bedrijf of de contactpersoon voor het primaire programma (deze twee rollen worden vaak in bezit van dezelfde persoon) kan de overstap initiëren en uitvoeren.

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>Wordt de persoon die de migratie voltooit de primaire contactpersoon in het juridische profiel van het bedrijf in Partner Center?

Niet noodzakelijkerwijs moet de primaire contactpersoon echter iemand zijn die is autorisatie heeft om overeenkomsten te ondertekenen.

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Kan Microsoft mijn MPN-lidmaatschap voor mij migreren?

Nee. Microsoft kan u niet helpen bij het verplaatsen van uw lidmaatschapsaccount naar het partnercentrum. U moet uw account verplaatsen door u aan te melden bij PMC met uw werkaccount (aanmeldingsreferenties) om het migratieproces te starten. Nadat u de stappen voor het verplaatsen van uw account hebt voltooid, kunt u beginnen met het beheren van uw lidmaatschap en gebruikersrollen en -machtigingen toewijzen aan uw team, zodat ze toegang hebben tot voordelen en kunnen helpen bij het beheren van het lidmaatschap. 

Microsoft migreert automatisch de huidige competenties, voordelen, locatiegegevens, bank-/belastinginformatie voor incentives en MCP-associaties, waaronder toegang tot Partner University.

### <a name="how-will-the-renewal-policy-change"></a>Hoe wordt het vernieuwingsbeleid gewijzigd?

In Partner Center is het vernieuwingsvenster van uw jubileumdatum tot de volgende 30 dagen.

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>Blijven onze competenties ongewijzigd nadat we naar de Partner Center?

Ja, competenties worden niet beïnvloed door de overstap naar Partner Center. Neem contact op met ondersteuning als u discrepanties [ziet.](https://partner.microsoft.com/support)

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>Veranderen mijn voordelen (inclusief cloudvoordelen, technische ondersteuning, softwarevoordelen, Visual Studio) na de overstap?

Uw in aanmerking komende voordelen worden niet gewijzigd. Neem contact op met ondersteuning als u discrepanties [ziet.](https://partner.microsoft.com/support)

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Worden onze Microsoft-accounts met Visual Studio voordeeltoewijzingen gehonoreerd?

Ja. Visual Studio voordelen die aan MSP's zijn toegewezen, worden gehonoreerd en behouden. Ze blijven ook behouden na verlenging in Partner Center. Als u echter een MSA-toewijzing verwijdert nadat deze is gemigreerd in Partner Center, kan deze niet opnieuw worden toegevoegd aan Partner Center.

In Partner Center kan een partner werkaccounts en gastgebruikersaccounts toevoegen, die MSA zijn van dezelfde tenant waarin de partner MPN-beheerder is in de Azure AD-tenant. Als de partner een globale beheerder is in meerdere Azure AD-tenants en al deze tenants zijn gekoppeld aan hetzelfde Partner Center-account, mag de partner gebruikers in al deze tenants toevoegen aan de Visual Studio-voordelen en toewijzingen op basis van Azure-gebruik.

Hoewel aan gastgebruikers op gebruik gebaseerde abonnementen van Visual Studio kunnen worden toegewezen door de MPN-beheerder of globale beheerder, kunnen gastgebruikers zich niet aanmelden bij Partner Center met hun MSA. Gastgebruikers kunnen zich echter aanmelden bij Azure en Visual Studio hun toegewezen voordelen te valideren en te gebruiken.

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>Hoe moeten we onze MCP-verbanden en de toegang tot onze Partner University beheren?

Er zijn geen wijzigingen in MCP-verbanden die vanuit PMC worden verplaatst. Nieuwe werknemers na de overstap naar Partner Center moeten echter worden gekoppeld in Partner Center. Alle machtigingen van uw Partner University voor bestaande gebruikers blijven bestaan, maar nieuwe werknemers moeten naar het [trainingscentrum](https://partner.microsoft.com/training) gaan voor informatie over het verkrijgen van toegang tot Partner University.

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>Hoe kan ik MCP-gegevens weergeven zodra ik naar Partner Center?

Selecteer **Competenties** in het linkernavigatiepaneel op het dashboard. Op de **pagina Competenties** kunt u het vaardighedenrapport downloaden. Het vaardighedenrapport vermeldt uw gebruikers die vaardigheden hebben verkregen die relevant zijn voor de competenties en programma's in Partner Center. Als uw gebruikers vaardigheden hebben opgedaan, maar deze vaardigheden niet relevant zijn voor de competenties waar u mee werkt, worden ze niet vermeld in het rapport.

### <a name="are-customer-references-used-in-partner-center"></a>Worden klantverwijzingen gebruikt in Partner Center?

Nee, u hebt geen klantverwijzingen nodig om te voldoen aan de competentievereisten in Partner Center.

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>Worden Partner of Record nu verplaatst naar Partner Center?

Ja, er is geen wijziging in Partner of Record. Meer informatie over het [koppelen van uw partner-id aan uw klanten.](/azure/billing/billing-partner-admin-link-started)

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>Is er een impact op incentives vanwege de overstap naar Partner Center?

Nee, er zijn geen gevolgen voor incentives als u uw account hebt verplaatst zonder locaties te consolideren. Als uw bedrijf meerdere accounts in PMC heeft en wanneer u overstapt naar Partner Center besluit u te consolideren in een wereldwijd account, zal er geen verlies zijn in incentives, maar kan er een vertraging in de uitbetaling van incentives zijn. 

Als u niet al uw PMC-accounts verplaatst die betrokken zijn bij incentives-programma's, kunt u stoppen met het verdienen van incentives die aan die accounts zijn gekoppeld.

### <a name="what-are-the-incentive-roles-in-partner-center"></a>Wat zijn de incentive-rollen in Partner Center?

Incentive-rollen in Partner Center zijn gebaseerd op locatie en omvatten Incentives-beheerder en Incentives-gebruiker. Zie Gebruikersrollen en -machtigingen toewijzen voor meer informatie over wat deze rollen [kunnen doen.](permissions-overview.md)

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>Kunnen incentives-beheerders worden toegewezen op globaal en locatieniveau?

Ja. U kunt een incentives-beheerder toewijzen als incentives-beheerder voor alle locaties of elke locatie kan een eigen incentives-beheerder hebben.

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>Kunnen incentives worden betaald op globaal of locatieniveau?

Incentives worden alleen op locatieniveau betaald.

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>Hoeveel bedrijfsprofielen kunnen we maken met betrekking tot verwijzingen?

Uw bedrijf kan zoveel bedrijfsprofielen maken als u nodig hebt om de interesses van uw bedrijf volledig te vertegenwoordigen. In elk bedrijfsprofiel kunt u maximaal vijf locaties opgeven, één locatie per land. Elk van de bedrijfsprofielen kan verwijzingen ontvangen voor elk van de locaties.

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>Hoe worden verwijzingen toegewezen en welke wijzigingen kan ik verwachten? Als ik bijvoorbeeld een wereldwijd bedrijf heb op de ene markt en locaties in andere markten, hoe worden verwijzingen dan toegewezen?

Verwijzingen worden toegewezen op basis van de zoekparameters die de klant definieert. Ongeacht of u één of veel locaties hebt, als de klant een gewenste locatie op geeft en u daar een bedrijf hebt dat voldoet aan de andere parameters, gaat de verwijzing naar die locatie.

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>Ik migreert naar Partner Center vanuit Rusland. Ik krijg een foutbericht over Web Direct. Hoe kan ik doorgaan met de migratie?

Als u een foutbericht ontvangt omdat u deelneemt aan het Web Direct-programma, moet u het volgende doen:

1. Meld u aan bij de portal. Azure.com en maak een nieuwe Azure AD-tenant. Lees Create [a new Azure AD tenant (Een nieuwe Azure AD-tenant maken) voor meer informatie.](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)

2. Nadat u de nieuwe Azure AD-tenant hebt gemaakt, gebruikt u deze om te migreren van Partner Membership Center naar Partner Center of om u in te schrijven als een nieuw net in Partner Center.