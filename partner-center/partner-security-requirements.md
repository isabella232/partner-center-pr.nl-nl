---
title: Beveiligings vereisten voor partners
ms.topic: article
ms.date: 10/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Introduceert de partner vereisten om multi-factor Authentication (MFA) in te scha kelen en het Framework van het veilige toepassings model te gebruiken.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c92e8c9a9a08582d89ef478a4600f737a548b787
ms.sourcegitcommit: 2847efac28d3bff24ed37cdfaa88ff4be06705c8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/27/2020
ms.locfileid: "92680383"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Partner beveiligings vereisten voor partners die partner Center-of partner Center-Api's gebruiken

**Van toepassing op**

- Alle partners in het Cloud Solution Provider-programma
  - Directe factuur
  - Indirecte provider
  - Indirecte wederverkoper
- Alle leveranciers van het configuratie scherm
- Alle Advisors

**Juiste gebruikers**

- Alle ingeschakelde gebruikers, inclusief gast gebruikers

Grotere veiligheids maatregelen en beveiliging zijn onder de meest voorkomende prioriteiten. We weten dat de beste verdediging voor komen en dat we alleen even sterk zijn als onze zwakste koppeling. Daarom hebben we iedereen in ons ecosysteem nodig om te reageren en te zorgen dat de juiste beveiligings beveiligingen aanwezig zijn. Om partners en klanten te helpen beschermen, introduceren we een reeks verplichte beveiligings vereisten voor Advisor, leveranciers van het configuratie scherm en partners die deel nemen aan het programma voor Cloud solution provider.

## <a name="overview"></a>Overzicht

Partners zijn verplicht multi-factor Authentication af te dwingen voor alle gebruikers accounts in hun partner Tenant. De voor waarden die zijn gekoppeld aan de beveiligings vereisten van de partner zijn toegevoegd aan de micro soft-partner overeenkomst. Aangezien deze betrekking heeft op Advisor, zijn dezelfde contractuele vereisten van kracht.

Partners die de verplichte beveiligings vereisten niet implementeren, kunnen geen trans acties uitvoeren in het Cloud Solution Provider-programma of de tenants van klanten beheren die gebruikmaken van gedelegeerde beheerders rechten, zodra deze vereisten worden afgedwongen. Daarnaast kunnen partners die de beveiligings vereisten niet implementeren, hun deelname nemen aan Program ma's die risico lopen.  

Om u en uw klanten te beschermen, moeten partners onmiddellijk de volgende acties uitvoeren:  

1. **Schakel multi-factor Authentication (MFA) in voor alle gebruikers accounts in uw partner Tenant** . Alle gebruikers accounts in uw partner-Tenant (s) moeten worden aangestuurd door multi-factor Authentication (MFA) wanneer ze zich aanmelden bij commerciële Cloud Services van micro soft of wanneer ze in het Cloud Solution Provider-programma schrijven via het partner centrum of via Api's.

2. **Het Framework van het veilige toepassings model aannemen** . Het Framework van het veilige toepassings model aannemen. Alle partners die zijn geïntegreerd met de Partner Center-API, moeten het beveiligde Framework voor toepassings modellen voor alle toepassingen van app + gebruikers authenticatie model aannemen.

    > [!IMPORTANT]
    > We raden u ten zeerste aan dat partners het beveiligde toepassings model implementeren voor de integratie met een micro soft-API, zoals Azure Resource Manager, Microsoft Graph of het gebruik van Automation zoals Power shell met gebruikers referenties, om onderbrekingen te voor komen wanneer MFA wordt afgedwongen.

Door Multi-Factor Authentication (MFA) in te scha kelen en het Framework van het veilige toepassings model te gebruiken, wordt uw infra structuur beschermd en worden de gegevens van uw klanten beschermd tegen mogelijke beveiligings Risico's, zoals het identificeren van dief stal of andere fraude incidenten.  

## <a name="actions-that-you-need-to-take"></a>Acties die u moet uitvoeren

Als u wilt voldoen aan de vereisten voor de beveiliging van de partner, moet u multi-factor Authentication afdwingen voor elk gebruikers account in uw partner Tenant. U kunt dit op een van de volgende manieren doen:

- Implementatie van [Azure AD-beveiligings standaards](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Aankoop Azure Active Directory Premium voor elk gebruikers account. Zie [een Cloud implementatie van Azure multi-factor Authentication plannen](/azure/active-directory/authentication/howto-mfa-getstarted)voor meer informatie.

- Het gebruik van een oplossing van derden voor het afdwingen van multi-factor Authentication voor elk gebruikers account in uw partner Tenant. Zie [hoe de beveiligings vereisten worden afgedwongen](#how-the-requirements-are-enforced)om ervoor te zorgen dat de oplossing de verwachte oplossing zal bieden.

> [!NOTE]
> Hoewel multi-factor Authentication niet contractueel is vereist voor een soevereine Cloud (21Vianet, Amerikaanse overheid en Duitsland), is het raadzaam deze beveiligings vereisten aan te passen.

## <a name="security-defaults"></a>Standaardinstellingen voor de beveiliging

Beleid voor standaard instellingen van beveiliging is een van de [Opties](#actions-that-you-need-to-take) die partners kunnen kiezen voor het implementeren van MFA voor de beveiligings vereisten, afhankelijk van hun bedrijfs behoeften. Het biedt een basis niveau van beveiliging zonder extra kosten. Lees hoe u MFA inschakelt voor uw organisatie met Azure AD en de belangrijkste aandachtspunten voordat u de standaard instellingen voor beveiliging inschakelt.

- Basislijn beleid blijft in de komende maanden en wordt aan het einde van februari 2020 afgeschaft.

- Partners die al een basislijn beleid hebben aangenomen, moeten actie ondernemen om over te gaan naar de standaard instellingen van de beveiliging.

- Standaard instellingen voor beveiliging zijn de algemene beschikbaarheids vervanging van de preview-Baseline-beleids regels. Zodra een partner de standaard instellingen voor beveiliging inschakelt, kunnen ze geen basislijn beleidsregels meer inschakelen.

- Met de standaard instellingen voor beveiliging worden alle beleids regels tegelijk ingeschakeld.

- Voor partners die gebruikmaken van [voorwaardelijke toegang](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), [zijn de standaard instellingen voor beveiliging niet beschikbaar](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Het blok keren van verouderde verificatie wordt op dit moment niet afgedwongen voor partners. Omdat de meeste gebeurtenissen met betrekking tot aangetaste identiteiten echter afkomstig zijn van aanmeldings pogingen met behulp van verouderde verificatie, worden partners aangemoedigd om deze oudere protocollen te verlaten.

- Azure AD Connect synchronisatie account wordt uitgesloten van de standaard instellingen voor beveiliging.

- Lees [multi-factor Authentication inschakelen voor uw organisatie](/azure/active-directory/authentication/concept-mfa-get-started) en [Azure Active Directory standaard instellingen](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)voor de beveiliging voor gedetailleerde informatie.

> [!NOTE]
> De standaard instellingen van Azure AD zijn de ontwikkeling van het Baseline-beveiligings beleid vereenvoudigd. Als u het Baseline-beveiligings beleid al hebt ingeschakeld, wordt u ten zeerste aangeraden de standaard instellingen voor beveiliging in te scha kelen.

Als u wilt overstappen van basislijn beleidsregels naar standaard instellingen voor beveiliging, lees dan de [standaard instellingen voor beveiliging?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Overweging

Omdat deze vereisten van toepassing zijn op alle gebruikers accounts in uw partner-Tenant, moet u rekening houden met verschillende dingen om te zorgen voor een soepele implementatie, met inbegrip van het identificeren van gebruikers accounts in Azure Active Directory die geen multi-factor Authentication kunnen uitvoeren, evenals toepassingen en apparaten die worden gebruikt door uw organisatie die geen ondersteuning bieden voor moderne verificatie.

Voordat u een actie uitvoert, raden we u aan de volgende validaties uit te voeren: 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Hebt u een toepassing of apparaat dat geen ondersteuning biedt voor het gebruik van moderne authenticatie?

Wanneer u de verouderde verificatie van multi-factor Authentication afdwingt, worden protocollen zoals IMAP, POP3, SMTP, enzovoort, geblokkeerd omdat ze geen ondersteuning bieden voor multi-factor Authentication. Om ervoor te zorgen dat de toepassing of het apparaat nog steeds kan worden geverifieerd, kan de functie worden gebruikt om te voor komen dat de [app wacht woorden](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) kent. Bekijk de overwegingen voor het gebruik van app-wacht woorden die [hier](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) worden beschreven om te bepalen of ze kunnen worden gebruikt in uw omgeving.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>Hebt u de beschikking over de Office 365 van de licenties die zijn gekoppeld aan uw partner-Tenant?

Voordat u een oplossing implementeert, wordt u aangeraden te bepalen welke versie van Microsoft Office wordt gebruikt door gebruikers in uw partner Tenant. Er is een kans dat uw gebruikers connectiviteits problemen ondervinden met toepassingen zoals Outlook. Voordat u multi-factor Authentication afdwingt, is het belang rijk om ervoor te zorgen dat Outlook 2013 SP1 of hoger wordt gebruikt en dat voor uw organisatie moderne authenticatie is ingeschakeld. Zie voor meer informatie [moderne verificatie inschakelen in Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Als u moderne verificatie wilt inschakelen voor apparaten met Windows, waarop Microsoft Office 2013 is geïnstalleerd, moet u twee register sleutels maken. Zie [moderne authenticatie inschakelen voor Office 2013 op Windows-apparaten](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Is er een beleid dat voor komt dat uw gebruikers hun mobiele apparaten kunnen gebruiken tijdens het werken?

Het is belang rijk dat u bedrijfs beleid identificeert waarmee wordt voor komen dat werk nemers mobiele apparaten kunnen gebruiken tijdens het werken, omdat dit van invloed is op de multi-factor Authentication-oplossing die u implementeert. Er zijn oplossingen, zoals de implementatie van de [standaard instellingen voor Azure AD-beveiliging](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), die alleen het gebruik van een verificator-app voor verificatie toestaan. Als uw organisatie een beleid voor het gebruik van mobiele apparaten heeft voor komen, kunt u een van de volgende opties gebruiken:

- Een op tijd gebaseerde mobiele TOTP-toepassing (base Password) implementeren die op een beveiligd systeem kan worden uitgevoerd

- Implementeer een oplossing van derden die multi-factor Authentication afdwingt voor elk gebruikers account in de partner Tenant die de meest geschikte verificatie optie biedt

- [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) -licenties aanschaffen voor de betrokken gebruikers

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Welke automatisering of integratie moet u gebruiken om gebruikers referenties te gebruiken voor verificatie?

Omdat de vereiste is om MFA af te dwingen voor elke gebruiker, inclusief service accounts, in uw partner Directory, wordt de automatisering of integratie van de gebruikers referenties voor verificatie beïnvloed. Het is dus belang rijk dat u bepaalt welke accounts in deze situaties worden gebruikt. Raadpleeg de volgende lijst met voor beelden van toepassingen of services die u moet overwegen:

- Configuratie scherm dat wordt gebruikt om resources namens uw klanten in te richten

- Integratie met elk platform dat wordt gebruikt voor facturering (zoals het hoort bij het CSP-programma) en het ondersteunen van uw klanten

- Power shell-scripts die gebruikmaken van AZ, AzureRM, Azure AD, MS online, enzovoort.

De bovenstaande lijst is niet volledig. Het is dus belang rijk dat u een volledige evaluatie uitvoert van elke toepassing of service in uw omgeving die gebruikmaakt van de gebruikers referenties voor verificatie. Voor concurreren met de vereiste voor multi-factor Authentication moet u waar mogelijk de richt lijnen in het Framework van het [veilige toepassings model](/partner-center/develop/enable-secure-app-model) implementeren.

## <a name="accessing-your-environment"></a>Toegang tot uw omgeving

U wordt aangeraden de aanmeldings activiteit te bekijken als u meer wilt weten over wat of wie verificatie uitvoert zonder dat deze wordt aangevraagd voor multi-factor Authentication. Via Azure Active Directory Premium kunt u gebruikmaken van het aanmeld rapport. Zie voor meer informatie over dit onderwerp de [rapporten voor aanmeldings activiteiten in de Azure Active Directory Portal](/azure/active-directory/reports-monitoring/concept-sign-ins). Als u niet beschikt over Azure Active Directory Premium, of als u op zoek bent naar een manier om deze aanmeldings activiteit te verkrijgen via Power shell, moet u gebruikmaken van de cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity)  van de Power shell-module van [Partner Center](https://www.powershellgallery.com/packages/PartnerCenter/) .

## <a name="how-the-requirements-are-enforced"></a>Hoe de vereisten worden afgedwongen

De beveiligings vereisten van de partner worden afgedwongen door Azure Active Directory en in het partner centrum, door te controleren of de MFA-claim aanwezig is om te identificeren dat de verificatie van de multi-factor Authentication is uitgevoerd. Gestart op 18 november 2019, micro soft heeft aanvullende beveiligings maatregelen (voorheen bekend als ' technische afdwinging ') ingeschakeld voor partner tenants.

Bij de activering worden gebruikers in de partner-Tenant gevraagd om verificatie van multi-factor Authentication (MFA) te volt ooien bij het uitvoeren van een beheerder namens (ADMINISTRATE)-bewerkingen, toegang te krijgen tot de Partner Center-portal of de API voor Partner Center. Zie [eisen multi-factor Authentication (MFA) voor uw partner Tenant](partner-security-requirements-mandating-mfa.md)voor meer informatie. 

Partners die niet aan de vereisten voldoen, moeten deze maat regelen zo spoedig mogelijk implementeren om bedrijfs onderbrekingen te voor komen. 

Als u Azure Multi-Factor Authentication of de standaard instellingen van Azure AD gebruikt, zijn er geen aanvullende acties die u moet uitvoeren.

Als u een multi-factor Authentication-oplossing van derden gebruikt, is het mogelijk dat de MFA-claim niet kan worden uitgegeven. Als deze claim ontbreekt, kan Azure Active Directory niet bepalen of de verificatie aanvraag door multi-factor Authentication wordt aangevraagd. Lees [de vereisten voor de partner beveiliging testen](/powershell/partnercenter/test-partner-security-requirements)voor meer informatie over hoe u kunt controleren of uw oplossing de verwachte claim afgeeft. 

> [!IMPORTANT]
> Als uw oplossing van derden de verwachte claim niet uitgeeft, moet u samen werken met de leverancier die de oplossing heeft ontwikkeld om te bepalen welke acties moeten worden uitgevoerd.

## <a name="resources-and-support"></a>Resources en ondersteuning

Raadpleeg de volgende bronnen voor ondersteuning en voorbeeld code:

- [Partner centrum-Community voor beveiligings richtlijnen](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): de groeps Gemeenschap voor de beveiligings richtlijnen van de partner centrum is een online community waar u meer informatie kunt vinden over aanstaande gebeurtenissen en u vragen hebt die u mogelijk hebt.
- [Partner centrum .net](https://github.com/microsoft/partner-center-dotnet-samples)-voor beelden: deze github-opslag plaats bevat voor beelden die zijn ontwikkeld met behulp van .net, die laat zien hoe u het beveiligde Framework voor het toepassings model kunt implementeren.
- Java-voor beelden voor het [partner centrum](https://github.com/microsoft/partner-center-java-samples): deze github-opslag plaats bevat voor beelden die zijn ontwikkeld met behulp van Java, die laat zien hoe u het beveiligde Framework voor het toepassings model kunt implementeren.
- [Partner centrum Power shell-multi-factor Authentication](/powershell/partnercenter/multi-factor-auth): dit multi-factor Authentication artikel bevat informatie over het implementeren van het Framework van het veilige toepassings model met behulp van Power shell.