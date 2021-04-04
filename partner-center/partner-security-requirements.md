---
title: Beveiligings vereisten voor partners
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Introduceert de beveiligings vereisten van de partner om multi-factor Authentication (MFA) in te scha kelen en het Framework van het veilige toepassings model te gebruiken.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b7fa76999d2e071f80c0175a8dfcbc1afe527bfc
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087056"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Beveiligings vereisten voor het gebruik van partner Center of partner Center-Api's

**Juiste rollen**

- Alle gebruikers van het partner centrum

In dit artikel worden de verplichte beveiligings vereisten voor Advisor, de leveranciers van configuratie schermen en partners die deel nemen aan het Cloud Solution Provider-programma, beschreven, evenals verificatie opties en andere beveiligings overwegingen. Privacy-en beveiligings maatregelen zijn gebaseerd op onze belangrijkste prioriteiten. We weten dat de beste verdediging voor komen en dat we alleen even sterk zijn als onze zwakste koppeling. Daarom hebben we iedereen in ons ecosysteem nodig om te reageren en te zorgen dat de juiste beveiligings beveiligingen aanwezig zijn.

## <a name="mandatory-security-requirements"></a>Verplichte beveiligings vereisten

Partners die de verplichte beveiligings vereisten niet implementeren, kunnen geen trans acties uitvoeren in het Cloud Solution Provider-programma of klanten tenants beheren met gedelegeerde beheerders rechten. Daarnaast kunnen partners die de beveiligings vereisten niet implementeren, hun deelname nemen aan Program ma's die risico lopen. De voor waarden die zijn gekoppeld aan de beveiligings vereisten van de partner zijn toegevoegd aan de micro soft-partner overeenkomst. Aangezien deze betrekking heeft op Advisor, zijn dezelfde contractuele vereisten van kracht.

Om u en uw klanten te beschermen, moeten partners onmiddellijk de volgende acties uitvoeren:  

1. **Schakel multi-factor Authentication (MFA) in voor alle gebruikers accounts in uw partner Tenant**. U moet MFA afdwingen voor alle gebruikers accounts in uw partner-Tenant (s). Gebruikers moeten worden aangevraagd door MFA wanneer ze zich aanmelden bij commerciële Cloud Services van micro soft of wanneer ze in het Cloud Solution Provider-programma transacten via het partner centrum of via Api's.

2. **Het Framework van het veilige toepassings model aannemen**. Alle partners die zijn geïntegreerd met partner centrum-Api's moeten het [beveiligde Framework voor toepassings modellen](/partner-center/develop/enable-secure-app-model) voor alle toepassingen van de app en het gebruikers verificatie model aannemen.

    > [!IMPORTANT]
    > We raden u ten zeerste aan dat partners het beveiligde toepassings model implementeren voor integratie met een micro soft-API, zoals Azure Resource Manager of Microsoft Graph, of wanneer er automatiserings mogelijkheden zoals Power shell met gebruikers referenties worden gebruikt om onderbrekingen te voor komen wanneer MFA wordt afgedwongen.

Deze beveiligings vereisten helpen bij het beschermen van uw infra structuur en het beschermen van de gegevens van uw klanten tegen mogelijke beveiligings Risico's, zoals het identificeren van dief stal of andere fraude incidenten.  

## <a name="implementing-multi-factor-authentication"></a>Multi-factor Authentication implementeren

Als u wilt voldoen aan de vereisten voor de beveiliging van de partner, moet u MFA implementeren en afdwingen voor elk gebruikers account in uw partner Tenant. U kunt dit op een van de volgende manieren doen:

- Implementeer de [standaard instellingen voor beveiliging van Azure Active Directory (Azure AD)](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Meer informatie vindt u in de [volgende sectie](#security-defaults).

- Aankoop Azure Active Directory Premium voor elk gebruikers account. Zie [een Azure AD multi-factor Authentication-implementatie plannen](/azure/active-directory/authentication/howto-mfa-getstarted)voor meer informatie.

- Gebruik een oplossing van derden voor het afdwingen van MFA voor elk gebruikers account in uw partner Tenant. Zie [hoe de beveiligings vereisten worden afgedwongen](#how-the-requirements-are-enforced)om ervoor te zorgen dat de oplossing de verwachte oplossing zal bieden.

> [!NOTE]
> Hoewel multi-factor Authentication niet contractueel is vereist voor een soevereine Cloud (Amerikaanse overheid en Duitsland), is het raadzaam deze beveiligings vereisten aan te passen.

### <a name="security-defaults"></a>Standaardinstellingen voor de beveiliging

Een van de opties die partners kunnen kiezen om MFA-vereisten te implementeren, is door de standaard instellingen voor beveiliging in azure AD in te scha kelen. Standaard instellingen voor beveiliging bieden gratis beveiliging, zonder extra kosten. Lees hoe u MFA inschakelt voor uw organisatie met Azure AD en de belangrijkste aandachtspunten voordat u de standaard instellingen voor beveiliging inschakelt.

- Partners die al een basislijn beleid hebben aangenomen, moeten actie ondernemen om over te gaan naar de standaard instellingen van de beveiliging.

- Standaard instellingen voor beveiliging zijn de algemene beschikbaarheids vervanging van de preview-Baseline-beleids regels. Zodra een partner de standaard instellingen voor beveiliging inschakelt, kunnen ze geen basislijn beleidsregels meer inschakelen.

- Met de standaard instellingen voor beveiliging worden alle beleids regels tegelijk ingeschakeld.

- Voor partners die gebruikmaken van [voorwaardelijke toegang](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), [zijn de standaard instellingen voor beveiliging niet beschikbaar](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- Er wordt op dit moment geen verouderde verificatie geblokkeerd. Omdat de meeste gebeurtenissen met betrekking tot aangetaste identiteiten echter afkomstig zijn van een aanmeldings poging met behulp van verouderde verificatie, worden partners aangemoedigd om deze oudere protocollen te verlaten.

- Azure AD Connect synchronisatie account wordt uitgesloten van de standaard instellingen voor beveiliging.

Lees [overzicht van Azure AD-multi-factor Authentication voor uw organisatie](/azure/active-directory/authentication/concept-mfa-get-started) en [Wat zijn de standaard instellingen voor beveiliging?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)voor gedetailleerde informatie.

> [!NOTE]
> De standaard instellingen van Azure AD zijn de ontwikkeling van het Baseline-beveiligings beleid vereenvoudigd. Als u het Baseline-beveiligings beleid al hebt ingeschakeld, wordt u ten zeerste aangeraden de [standaard instellingen voor beveiliging](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)in te scha kelen.

## <a name="implementation-considerations"></a>Afwegingen bij de implementatie

Omdat deze vereisten van toepassing zijn op alle gebruikers accounts in uw partner-Tenant, moet u rekening houden met verschillende dingen om te zorgen voor een soepele implementatie. U kunt bijvoorbeeld gebruikers accounts in azure AD identificeren die geen MFA en toepassingen en apparaten in uw organisatie kunnen uitvoeren die moderne verificatie niet ondersteunen.

Voordat u een actie uitvoert, raden we u aan de volgende validaties uit te voeren. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Hebt u een toepassing of apparaat dat geen ondersteuning biedt voor het gebruik van moderne authenticatie?

Wanneer u MFA afdwingt, worden verouderde verificatie protocollen zoals IMAP, POP3, SMTP en anderen geblokkeerd omdat ze geen ondersteuning bieden voor MFA. Als u deze beperking wilt aanpakken, gebruikt u de functie voor [app-wacht woorden](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) om te controleren of de toepassing of het apparaat nog steeds wordt geverifieerd. Bekijk de [overwegingen voor het gebruik van app-wacht woorden](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) om te bepalen of ze kunnen worden gebruikt in uw omgeving.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Hebt u Office 365-gebruikers met licenties die zijn gekoppeld aan uw partner-Tenant?

Voordat u een oplossing implementeert, kunt u het beste bepalen welke versies van Microsoft Office gebruikers in uw partner-Tenant worden gebruikt. Er is een kans dat uw gebruikers connectiviteits problemen ondervinden met toepassingen zoals Outlook. Voordat u MFA afdwingt, is het belang rijk om ervoor te zorgen dat u Outlook 2013 SP1 of hoger gebruikt en dat voor uw organisatie moderne authenticatie is ingeschakeld. Zie voor meer informatie [moderne verificatie inschakelen in Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Als u moderne verificatie wilt inschakelen voor apparaten waarop Windows wordt uitgevoerd waarop Microsoft Office 2013 is geïnstalleerd, moet u twee register sleutels maken. Zie [moderne authenticatie inschakelen voor Office 2013 op Windows-apparaten](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Is er een beleid dat voor komt dat uw gebruikers hun mobiele apparaten kunnen gebruiken tijdens het werken?

Het is belang rijk dat u bedrijfs beleid identificeert waarmee wordt voor komen dat werk nemers mobiele apparaten kunnen gebruiken tijdens het werken, omdat dit invloed heeft op de MFA-oplossing die u implementeert. Er zijn oplossingen, zoals de implementatie van de [standaard instellingen voor Azure AD-beveiliging](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), die alleen het gebruik van een verificator-app voor verificatie toestaan. Als uw organisatie een beleid voor het gebruik van mobiele apparaten heeft voor komen, kunt u een van de volgende opties gebruiken:

- Implementeer een op tijd gebaseerde mobiele TOTP-toepassing (basis wachtwoord) die op een beveiligd systeem kan worden uitgevoerd.

- Implementeer een oplossing van derden die MFA afdwingt voor elk gebruikers account in de partner Tenant met de meest geschikte verificatie optie.

- Koop [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) -licenties voor de betrokken gebruikers.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Welke automatisering of integratie moet u gebruiken om gebruikers referenties te gebruiken voor verificatie?

Omdat we MFA afdwingen voor elke gebruiker, inclusief service accounts, in uw partner Directory, is dit van invloed op elke automatisering of integratie waarbij gebruikers referenties worden gebruikt voor verificatie. Het is dus belang rijk dat u bepaalt welke accounts in deze situaties worden gebruikt. Raadpleeg de volgende lijst met voor beelden van toepassingen of services die u moet overwegen:

- Configuratie scherm dat wordt gebruikt om resources namens uw klanten in te richten

- Integratie met elk platform dat wordt gebruikt voor facturering (zoals het hoort bij het CSP-programma) en het ondersteunen van uw klanten

- Power shell-scripts die gebruikmaken van AZ, AzureRM, Azure AD, MS online en andere modules

De bovenstaande lijst is niet volledig. Het is dus belang rijk dat u een volledige evaluatie uitvoert van elke toepassing of service in uw omgeving die gebruikmaakt van gebruikers referenties voor verificatie. Voor concurreren met de vereiste voor MFA moet u waar mogelijk de richt lijnen in het raam werk van het [veilige toepassings model](/partner-center/develop/enable-secure-app-model) implementeren.

## <a name="accessing-your-environment"></a>Toegang tot uw omgeving

U wordt aangeraden de aanmeldings activiteit te controleren om te zien wat of wie verificatie uitvoert zonder te worden aangevraagd voor MFA. Via Azure Active Directory Premium kunt u het aanmeld rapport gebruiken. Zie voor meer informatie over dit onderwerp [aanmeldings activiteiten rapporten in de Azure Active Directory Portal](/azure/active-directory/reports-monitoring/concept-sign-ins). Als u niet beschikt over Azure Active Directory Premium, of als u op zoek bent naar een manier om deze aanmeldings activiteit via Power shell te verkrijgen, moet u de cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) van de [Power shell](https://www.powershellgallery.com/packages/PartnerCenter/) -module van partner Center gebruiken.

## <a name="how-the-requirements-are-enforced"></a>Hoe de vereisten worden afgedwongen

Beveiligings vereisten voor partners worden afgedwongen door Azure AD en in Partner Center, door te controleren of de MFA-claim aanwezig is om te identificeren dat de MFA-verificatie is uitgevoerd. Vanaf 18 november 2019 heeft micro soft aanvullende beveiligings maatregelen (voorheen bekend als "technische afdwinging") voor het partner tenants geactiveerd.

Bij de activering worden gebruikers in de partner-Tenant gevraagd om de MFA-verificatie te volt ooien bij het uitvoeren van een beheerder namens (ADMINISTRATE)-bewerkingen, toegang te krijgen tot de portal van het partner centrum of door Partner Center-Api's aan te roepen. Zie [eisen multi-factor Authentication (MFA) voor uw partner Tenant](partner-security-requirements-mandating-mfa.md)voor meer informatie. 

Partners die niet aan de vereisten voldoen, moeten deze maat regelen zo spoedig mogelijk implementeren om bedrijfs onderbrekingen te voor komen. Als u Azure Active Directory Multi-Factor Authentication of de standaard instellingen van Azure AD gebruikt, zijn er geen aanvullende acties die u moet uitvoeren.

Als u een MFA-oplossing van derden gebruikt, is het mogelijk dat de MFA-claim niet kan worden uitgegeven. Als deze claim ontbreekt, kan Azure AD niet bepalen of de verificatie aanvraag is aangevraagd door MFA. Lees [de vereisten voor de partner beveiliging testen](/powershell/partnercenter/test-partner-security-requirements)voor meer informatie over hoe u kunt controleren of uw oplossing de verwachte claim afgeeft. 

> [!IMPORTANT]
> Als uw oplossing van derden de verwachte claim niet uitgeeft, moet u samen werken met de leverancier die de oplossing heeft ontwikkeld om te bepalen welke acties moeten worden uitgevoerd.

## <a name="resources-and-samples"></a>Bronnen en voor beelden

Raadpleeg de volgende bronnen voor ondersteuning en voorbeeld code:

- [Partner centrum-Community voor beveiligings richtlijnen](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): de groeps Gemeenschap voor de beveiligings richtlijnen van de partner centrum is een online community waar u meer informatie kunt vinden over aanstaande gebeurtenissen en u vragen hebt die u mogelijk hebt.
- [Partner centrum .net](https://github.com/microsoft/partner-center-dotnet-samples)-voor beelden: deze github-opslag plaats bevat voor beelden die zijn ontwikkeld met behulp van .net, die laat zien hoe u het beveiligde Framework voor het toepassings model kunt implementeren.
- Java-voor beelden voor het [partner centrum](https://github.com/microsoft/partner-center-java-samples): deze github-opslag plaats bevat voor beelden die zijn ontwikkeld met behulp van Java, die laat zien hoe u het beveiligde Framework voor het toepassings model kunt implementeren.
- [Partner centrum Power shell-multi-factor Authentication](/powershell/partnercenter/multi-factor-auth): dit multi-factor Authentication artikel bevat informatie over het implementeren van het Framework van het veilige toepassings model met behulp van Power shell.

## <a name="next-steps"></a>Volgende stappen

- [Eisen multi-factor Authentication (MFA) voor uw partner-Tenant](partner-security-requirements-mandating-mfa.md)