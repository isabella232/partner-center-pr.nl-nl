---
title: Beveiligingsvereisten van partners
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Introduceert beveiligingsvereisten van partners om Multi-Factor Authentication (MFA) in te schakelen en het framework veilig toepassingsmodel gebruiken.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 73d508b8a8dabacaf65037c905fd31929a0f2522
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114837336"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Beveiligingsvereisten voor het gebruik Partner Center of Partner Center API's

**Juiste rollen:** alle Partner Center gebruikers

In dit artikel worden de verplichte beveiligingsvereisten beschreven voor adviseurs, Configuratiescherm-leveranciers en partners die deelnemen aan het Cloud Solution Provider-programma, evenals verificatieopties en andere beveiligingsoverwegingen. Privacybeveiliging en -beveiliging zijn een van onze belangrijkste prioriteiten. We weten dat de beste verdediging preventie is en dat we alleen zo sterk zijn als onze zwakste koppeling. Daarom hebben we iedereen in ons ecosysteem nodig om actie te ondernemen en ervoor te zorgen dat de juiste beveiligingsbescherming is gewaarborgd.

## <a name="mandatory-security-requirements"></a>Verplichte beveiligingsvereisten

Partners die de verplichte beveiligingsvereisten niet implementeren, kunnen het Cloud Solution Provider-programma niet uitvoeren of tenants van klanten beheren met gedelegeerde beheerdersrechten. Daarnaast kunnen partners die de beveiligingsvereisten niet implementeren hun deelname aan programma's in gevaar brengen. De voorwaarden die zijn gekoppeld aan de beveiligingsvereisten van de partner zijn toegevoegd aan de Microsoft Partner-overeenkomst. Voor advisors gelden dezelfde contractuele vereisten.

Om u en uw klanten te beschermen, moeten partners onmiddellijk de volgende acties uitvoeren:  

1. **Schakel Meervoudige verificatie (MFA) in voor alle gebruikersaccounts in uw partner-tenant.** U moet MFA afdwingen voor alle gebruikersaccounts in uw partner-tenant(s). Gebruikers moeten worden op de proef gesteld door MFA wanneer ze zich aanmelden bij commerciële cloudservices van Microsoft of wanneer ze in het Cloud Solution Provider-programma werken via Partner Center of via API's.

2. **Gebruik het veilig toepassingsmodel framework**. Alle partners die integreren met Partner Center API's, moeten het [veilig toepassingsmodel framework gebruiken](/partner-center/develop/enable-secure-app-model) voor toepassingen met een app- en gebruikersver auth-model.

    > [!IMPORTANT]
    > We raden partners ten zeerste aan de veilig toepassingsmodel te implementeren voor integratie met een Microsoft-API, zoals Azure Resource Manager of Microsoft Graph, of bij het gebruik van automatisering, zoals PowerShell met behulp van gebruikersreferenties, om onderbrekingen te voorkomen wanneer MFA wordt afgedwongen.

Deze beveiligingsvereisten helpen uw infrastructuur te beschermen en de gegevens van uw klanten te beschermen tegen mogelijke beveiligingsrisico's, zoals het identificeren van diefstal of andere fraudeincidenten.  

## <a name="implementing-multi-factor-authentication"></a>Meervoudige verificatie implementeren

Om te voldoen aan de beveiligingsvereisten van de partner, moet u MFA implementeren en afdwingen voor elk gebruikersaccount in uw partner-tenant. U kunt dit op een van de volgende manieren doen:

- Implementeert [Azure Active Directory (Azure AD)-standaardinstellingen voor beveiliging.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults) Zie de volgende [sectie voor meer informatie.](#security-defaults)

- Koop Azure Active Directory Premium voor elk gebruikersaccount. Zie Plan [an Azure AD Multi-Factor Authentication deployment (Een Azure AD Multi-Factor Authentication-implementatie plannen) voor meer informatie.](/azure/active-directory/authentication/howto-mfa-getstarted)

- Gebruik een oplossing van derden om MFA af te dwingen voor elk gebruikersaccount in uw partner-tenant. Zie hoe de beveiligingsvereisten worden afgedwongen om ervoor te zorgen dat de oplossing de verwachte oplossing [biedt.](#how-the-requirements-are-enforced)

> [!NOTE]
> Hoewel meervoudige verificatie niet contractueel vereist is voor een soevereine cloud (Amerikaanse overheid en Duitsland), wordt u ten zeerste aangeraden deze beveiligingsvereisten in te stellen.

### <a name="security-defaults"></a>Standaardinstellingen voor de beveiliging

Een van de opties die partners kunnen kiezen om MFA-vereisten te implementeren, is het inschakelen van standaardinstellingen voor beveiliging in Azure AD. Standaardinstellingen voor beveiliging bieden een basisbeveiligingsniveau zonder extra kosten. Lees hoe u MFA inschakelen voor uw organisatie met Azure AD en de belangrijkste overwegingen hieronder voordat u de standaardinstellingen voor beveiliging inschakelen.

- Partners die al basislijnbeleid hebben aangenomen, moeten actie ondernemen om over te stappen op de standaardinstellingen voor beveiliging.

- Standaardinstellingen voor beveiliging zijn de algemene beschikbaarheidsvervanging van het basislijnbeleid voor previews. Zodra een partner de standaardinstellingen voor beveiliging heeft ingeschakeld, kan deze geen basislijnbeleid meer inschakelen.

- Met de standaardinstellingen voor beveiliging worden alle beleidsregels in één keer ingeschakeld.

- Voor partners die [voorwaardelijke toegang gebruiken,](/azure/active-directory/conditional-access/concept-conditional-access-policy-common) [zijn de standaardinstellingen voor beveiliging niet beschikbaar.](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)

- Verouderde verificatie wordt op dit moment niet geblokkeerd. Omdat de meeste gebeurtenissen met betrekking tot gecompromitteerde identiteiten afkomstig zijn van een aanmeldingspoging met behulp van verouderde verificatie, wordt partners echter aangeraden om af te zien van deze oudere protocollen.

- Azure AD Verbinding maken synchronisatieaccount is uitgesloten van de standaardinstellingen voor beveiliging.

Lees Overview [of Azure AD Multi-Factor Authentication for your organization (Overzicht van Azure AD Multi-Factor Authentication voor uw](/azure/active-directory/authentication/concept-mfa-get-started) organisatie) en What are security [defaults? (Wat zijn standaardinstellingen voor beveiliging?) voor gedetailleerde informatie.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)

> [!NOTE]
> Standaardinstellingen voor Azure AD-beveiliging zijn de ontwikkeling van het basisbeschermingsbeleid vereenvoudigd. Als u het basisbeveiligingsbeleid al hebt ingeschakeld, wordt het ten zeerste aanbevolen om de [standaardinstellingen voor beveiliging in te stellen.](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)

## <a name="implementation-considerations"></a>Afwegingen bij de implementatie

Omdat deze vereisten van toepassing zijn op alle gebruikersaccounts in uw partner-tenant, moet u verschillende zaken overwegen om een soepele implementatie te garanderen. Identificeer bijvoorbeeld gebruikersaccounts in Azure AD die geen MFA kunnen uitvoeren, en toepassingen en apparaten in uw organisatie die geen ondersteuning bieden voor moderne verificatie.

Voordat u een actie gaat uitvoeren, raden we u aan de volgende validaties te voltooien. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>Hebt u een toepassing of apparaat die het gebruik van moderne verificatie niet ondersteunt?

Wanneer u MFA afdwingt, worden protocollen voor het gebruik van verouderde verificatie, zoals IMAP, POP3, SMTP en andere, geblokkeerd omdat ze geen ondersteuning bieden voor MFA. Als u deze beperking wilt aanpakken, gebruikt u de [functie app-wachtwoorden](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) om ervoor te zorgen dat de toepassing of het apparaat nog steeds wordt geverifieerd. Bekijk de [overwegingen voor het gebruik van app-wachtwoorden](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) om te bepalen of deze kunnen worden gebruikt in uw omgeving.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>Hebt u Office 365 gebruikers met licenties die zijn gekoppeld aan uw partnerten tenant?

Voordat u een oplossing implementeert, raden we u aan te bepalen welke versies van Microsoft Office gebruikers in uw partnerten tenant gebruiken. Er is een kans dat uw gebruikers verbindingsproblemen ervaren met toepassingen zoals Outlook. Voordat u MFA afdwingt, is het belangrijk om ervoor te zorgen dat u Outlook 2013 SP1 of hoger gebruikt en dat moderne verificatie is ingeschakeld in uw organisatie. Zie Moderne verificatie inschakelen in Exchange Online voor [meer Exchange Online.](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) 

Als u moderne verificatie wilt inschakelen voor apparaten met Windows die Microsoft Office 2013 hebben geïnstalleerd, moet u twee registersleutels maken. Zie [Moderne verificatie inschakelen voor Office 2013 op Windows apparaten.](/office365/admin/security-and-compliance/enable-modern-authentication)

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>Is er een beleid waardoor een van uw gebruikers hun mobiele apparaten niet kan gebruiken terwijl ze werken?

Het is belangrijk om bedrijfsbeleid te identificeren dat voorkomt dat werknemers mobiele apparaten gebruiken tijdens het werken, omdat dit van invloed is op de MFA-oplossing die u implementeert. Er zijn oplossingen, zoals de oplossingen die worden geleverd door de implementatie van [standaardinstellingen](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)voor Azure AD-beveiliging, die alleen het gebruik van een ver authenticator-app voor verificatie toestaan. Als uw organisatie een beleid heeft dat het gebruik van mobiele apparaten verhindert, kunt u een van de volgende opties overwegen:

- Implementeer een OPP-toepassing (Time-Based One-Time Base Password) die kan worden uitgevoerd op een beveiligd systeem.

- Implementeert een oplossing van derden die MFA afdwingt voor elk gebruikersaccount in de partnerten tenant dat de meest geschikte verificatieoptie biedt.

- Koop [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) voor de betrokken gebruikers.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>Welke automatisering of integratie hebt u nodig om gebruikersreferenties te gebruiken voor verificatie?

Omdat we MFA afdwingen voor elke gebruiker, met inbegrip van serviceaccounts, in uw partnermap, is dit van invloed op automatisering of integratie die gebruikmaakt van gebruikersreferenties voor verificatie. Het is dus belangrijk dat u identificeert welke accounts in deze situaties worden gebruikt. Bekijk de volgende lijst met voorbeeldtoepassingen of -services om rekening mee te houden:

- Configuratiescherm dat wordt gebruikt voor het inrichten van resources namens uw klanten

- Integratie met elk platform dat wordt gebruikt voor facturering (in verband met het CSP-programma) en het ondersteunen van uw klanten

- PowerShell-scripts die gebruikmaken van de modules Az, AzureRM, Azure AD, MS Online en andere modules

De bovenstaande lijst is niet uitgebreid. Het is dus belangrijk dat u een volledige evaluatie van een toepassing of service in uw omgeving die gebruikmaakt van gebruikersreferenties voor verificatie. Als u wilt voldoen aan de vereiste voor MFA, moet u waar mogelijk de richtlijnen in veilig toepassingsmodel [framework](/partner-center/develop/enable-secure-app-model) implementeren.

## <a name="accessing-your-environment"></a>Toegang tot uw omgeving

Als u meer inzicht wilt krijgen in wat of wie zich authenticeert zonder dat u om MFA wordt aangeraden, raden we u aan de aanmeldingsactiviteit te bekijken. Via Azure Active Directory Premium kunt u het aanmeldingsrapport gebruiken. Zie Rapporten voor aanmeldingsactiviteiten in de Azure Active Directory portal voor [meer informatie over dit onderwerp.](/azure/active-directory/reports-monitoring/concept-sign-ins) Als u geen Azure Active Directory Premium hebt of als u op zoek bent naar een manier om deze aanmeldingsactiviteit te verkrijgen via PowerShell, moet u de cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) van de [Partner Center PowerShell-module](https://www.powershellgallery.com/packages/PartnerCenter/) gebruiken.

## <a name="how-the-requirements-are-enforced"></a>Hoe de vereisten worden afgedwongen

Beveiligingsvereisten van partners worden afgedwongen door Azure AD, en op hun beurt Partner Center, door te controleren op de aanwezigheid van de MFA-claim om te identificeren dat MFA-verificatie heeft plaatsgevonden. Vanaf 18 november 2019 heeft Microsoft aanvullende beveiligingsmaatregelen (voorheen bekend als 'technische afdwinging') geactiveerd voor tenants van partners.

Na activering wordt gebruikers in de partner-tenant gevraagd om MFA-verificatie te voltooien wanneer ze een beheerder uitvoeren namens (AOBO)-bewerkingen, toegang tot de Partner Center-portal of het aanroepen van Partner Center API's. Zie [Multi-Factor Authentication (MFA) voor uw partner-tenant](partner-security-requirements-mandating-mfa.md)voor meer informatie. 

Partners die niet aan de vereisten voldoen, moeten deze maatregelen zo snel mogelijk implementeren om bedrijfsonderbrekingen te voorkomen. Als u de standaardinstellingen Azure Active Directory Multi-Factor Authentication of Azure AD-beveiliging gebruikt, hoeft u geen aanvullende acties uit te voeren.

Als u een MFA-oplossing van derden gebruikt, bestaat de kans dat de MFA-claim niet wordt uitgegeven. Als deze claim ontbreekt, kan Azure AD niet bepalen of de verificatieaanvraag is gevraagd door MFA. Lees Testing the Partner Security Requirements (De beveiligingsvereisten van de partner testen) voor meer informatie over het controleren van de oplossing die de verwachte claim [uitkeert.](/powershell/partnercenter/test-partner-security-requirements) 

> [!IMPORTANT]
> Als uw oplossing van derden de verwachte claim niet uit geeft, moet u samenwerken met de leverancier die de oplossing heeft ontwikkeld om te bepalen welke acties moeten worden ondernomen.

## <a name="resources-and-samples"></a>Resources en voorbeelden

Zie de volgende bronnen voor ondersteuning en voorbeeldcode:

- [Partner Center Security Guidance Group community](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): De community Partner Center Security Guidance Group is een online community waar u meer te weten kunt komen over aanstaande gebeurtenissen en waar u eventuele vragen kunt stellen.
- [Partner Center .NET-voorbeelden:](https://github.com/microsoft/partner-center-dotnet-samples)deze GitHub-opslagplaats bevat voorbeelden, ontwikkeld met .NET, die laten zien hoe u het framework veilig toepassingsmodel implementeren.
- [Partner Center Java-voorbeelden:](https://github.com/microsoft/partner-center-java-samples)deze GitHub-opslagplaats bevat voorbeelden, ontwikkeld met behulp van Java, die laten zien hoe u het framework veilig toepassingsmodel implementeren.
- [Partner Center PowerShell - Multi-Factor Authentication:](/powershell/partnercenter/multi-factor-auth)in dit artikel over Multi-Factor Authentication vindt u meer informatie over het implementeren van het veilig toepassingsmodel framework met behulp van PowerShell.

## <a name="next-steps"></a>Volgende stappen

- [Multi-Factor Authentication (MFA) voor uw partner-tenant verplichten](partner-security-requirements-mandating-mfa.md)