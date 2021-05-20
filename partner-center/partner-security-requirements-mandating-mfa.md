---
title: Meervoudige verificatie (MFA) voor uw partner-tenant verplichten
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe het verplicht stellen van MFA voor uw partnerten tenants u helpt uw toegang tot klantresources te beveiligen. Bevat voorbeeldscenario's.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b1b02967209ba36088b0c7bb7487428ab08b8a37
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152576"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Meervoudige verificatie (MFA) voor uw partner-tenant verplichten

**Juiste rollen:** beheeragent | Verkoopagent | Helpdeskagent | Factureringsbeheerders | Globale beheerder

Dit artikel bevat gedetailleerde voorbeelden en richtlijnen voor het bepalen van meervoudige verificatie (MFA) in Partner Center. Het doel van deze functie is om partners te helpen hun toegang tot klantbronnen te beveiligen tegen gecompromitteerd referenties. Partners moeten MFA afdwingen voor alle gebruikersaccounts in hun partner-tenant, inclusief gastgebruikers. Gebruikers moeten MFA-verificatie voltooien voor de volgende gebieden:

- [Partner Center Dashboard](#partner-center-dashboard)
- [Partnercentrum-API](#partner-center-api)
- [Gedelegeerd beheer van partners](#partner-delegated-administration)

Betere en voortdurende beveiliging en privacybeveiliging zijn een van onze belangrijkste prioriteiten en we blijven partners helpen hun klanten en tenants te beschermen. Alle partners die deelnemen aan het Cloud Solution Provider(CSP)-programma, Configuratiescherm Vendors (CPV's) en advisors moeten de [beveiligingsvereisten](partner-security-requirements.md) van de partner implementeren om compatibel te blijven.

Om partners te helpen hun bedrijf en klanten te beschermen tegen identiteitsdiefstal en onbevoegde toegang, hebben we extra beveiligingsbeveiliging geactiveerd voor partnerten tenants die MFA verplichten en verifiëren. 

## <a name="partner-center-dashboard"></a>Partner Center dashboard

Bepaalde pagina's in Partner Center dashboard worden beveiligd met MFA, waaronder:

- Alle pagina's **op het** tabblad Klanten, bijvoorbeeld alle pagina's die toegankelijk zijn via de volgende URL: https://partner.microsoft.com/commerce/*
- Alle pagina's op **het tabblad > aanvragen** van klanten, bijvoorbeeld de pagina die wordt gebruikt onder https://partner.microsoft.com/dashboard/support/csp/customers/*
- Pagina Facturering

In de volgende tabel ziet u welke gebruikerstypen zijn gemachtigd voor toegang tot deze met MFA beveiligde pagina's (en worden daarom beïnvloed door deze functie).


| Pagina met MFA-bescherming       | Beheerdersagents      |  Verkoopmedewerkers     |   Helpdeskmedewerkers     | Globale beheerder      |  Factureringsbeheerder     | 
|---    |---    |---    |---    |---    |---    |
| Alle pagina's op het tabblad Klanten      |   x    |    x   |  x     |       |       |
| Alle pagina's onder het tabblad > klantenaanvragen     | x      |       |    x   |       |       |
| Pagina Facturering     |   x    |       |       |    x   |   x    |

Als u toegang probeert te krijgen tot een van deze pagina's en u de MFA-verificatie nog niet eerder hebt voltooid, moet u dit doen. Andere pagina's Partner Center, zoals de pagina Overzicht, Service Health pagina Statuscontrole vereist geen MFA.

## <a name="verification-examples"></a>Verificatievoorbeelden

Als u wilt laten zien hoe verificatie werkt in Partner Center dashboard, kunt u de volgende voorbeelden bekijken.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Voorbeeld 1: Partner heeft Azure AD MFA geïmplementeerd

1. Jane werkt voor CSP Contoso. Contoso heeft MFA geïmplementeerd voor al hun gebruikers onder de tenant van de Contoso-partner met behulp van Azure Active Directory (Azure AD) MFA.

2. Jane start een nieuwe browsersessie en navigeert naar Partner Center overzichtspagina van het dashboard (die niet met MFA is beveiligd). Partner Center Jane omgeleid naar Azure AD om zich aan te melden.

3. Vanwege de bestaande Azure AD MFA-installatie door Contoso is Jane vereist om MFA-verificatie te voltooien. Na een geslaagde aanmelding en MFA-verificatie wordt Jane teruggeleid naar Partner Center dashboardoverzichtspagina.

4. Jane probeert toegang te krijgen tot een van de pagina's met MFA-Partner Center. Omdat Jane de MFA-verificatie al eerder heeft voltooid tijdens het aanmelden, heeft Jane toegang tot de pagina met MFA-bescherming zonder dat ze MFA-verificatie opnieuw moet door te voeren.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Voorbeeld 2: Partner heeft externe MFA geïmplementeerd met behulp van identiteitsfederatie

1. Het werkt voor CSP Wingtip. Wingtip heeft MFA geïmplementeerd voor al hun gebruikers onder De tenant van de Wingtip-partner met behulp van MFA van derden, dat is geïntegreerd met Azure AD via identiteitsfederatie.

2. Met Een nieuwe browsersessie wordt een nieuwe browsersessie gestart en Partner Center naar de overzichtspagina van het dashboard (die niet met MFA is beveiligd). Partner Center omgeleid naar Azure AD om u aan te melden.

3. Omdat Wingtip identiteitsfederatie heeft ingesteld, leidt Azure ADPrinter om naar de federatief-id-provider om aanmelding en MFA-verificatie te voltooien. Na een geslaagde aanmelding en MFA-verificatie wordt Hij teruggeleid naar Azure AD en vervolgens naar Partner Center dashboardoverzichtspagina.

4. Er wordt geprobeerd toegang te krijgen tot een van de met MFA beveiligde pagina's in Partner Center. Omdat Tijdens het aanmelden MFA-verificatie al is voltooid inPrinter, heeftPrint toegang tot de met MFA beveiligde pagina zonder dat MFA-verificatie opnieuw moet worden uitgevoerd.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Voorbeeld 3: Partner heeft MFA niet geïmplementeerd

1. John werkt voor CSP Fabrikam. Fabrikam heeft MFA niet geïmplementeerd voor een gebruiker onder de tenant van de Fabrikam-partner.

2. John start een nieuwe browsersessie en navigeert naar Partner Center overzichtspagina van het dashboard (die niet met MFA is beveiligd). Partner Center John omgeleid naar Azure AD om zich aan te melden.

3. Omdat Fabrikam MFA niet heeft geïmplementeerd, hoeft John de MFA-verificatie niet te voltooien. Na een geslaagde aanmelding wordt John teruggeleid naar de Partner Center dashboard.

4. John probeert toegang te krijgen tot een van de met MFA beveiligde pagina's in Partner Center. Omdat John de MFA-verificatie niet heeft voltooid, Partner Center John omgeleid naar Azure AD om de MFA-verificatie te voltooien. Omdat dit de eerste keer is dat John MFA moet voltooien, wordt John ook gevraagd om zich [te registreren voor MFA.](#mfa-registration-experience) Na een geslaagde MFA-registratie en MFA-verificatie heeft John nu toegang tot de pagina met MFA-bescherming.

5. Nog een dag voordat Fabrikam MFA implementeert voor elke gebruiker, start John een nieuwe browsersessie en navigeert hij naar de overzichtspagina van het Partner Center-dashboard (die niet met MFA is beveiligd). Partner Center john omgeleid naar Azure AD om zich aan te melden zonder MFA-prompt. 

6. John probeert toegang te krijgen tot een van de pagina's met MFA-Partner Center. Omdat John de MFA-verificatie niet heeft voltooid, Partner Center John omgeleid naar Azure AD om de MFA-verificatie te voltooien. Omdat John MFA heeft geregistreerd, wordt hij deze keer alleen gevraagd om de MFA-verificatie te voltooien.

> [!NOTE]
>Actie: Bedrijfsbeheerders hebben [drie opties voor](partner-security-requirements.md#implementing-multi-factor-authentication) het implementeren van MFA.

## <a name="partner-center-api"></a>Partnercentrum-API

De Partner Center-API ondersteunt zowel app-only verificatie als app+gebruikersverificatie. 

Wanneer app- en gebruikersverificatie wordt gebruikt, Partner Center MFA-verificatie vereist. Om precies te zijn: wanneer een partnertoepassing een API-aanvraag naar Partner Center wil verzenden, moet deze een toegangs token bevatten in de autorisatie-header van de aanvraag. 

> [!NOTE]
>Het [veilig toepassingsmodel](/partner-center/develop/enable-secure-app-model) framework is een schaalbaar framework voor het authenticeren van CSP-partners en CPV's via de Microsoft Azure MFA-architectuur bij het aanroepen Partner Center API's. U moet dit framework implementeren voordat u MFA in uw tenant inschakelen. 

Wanneer Partner Center een API-aanvraag ontvangt met een toegangs token dat is verkregen met app- en gebruikersverificatie, controleert de Partner Center-API of de *MFA-waarde* aanwezig is in de CLAIM Authentication *Method Reference (AMR).* U kunt een JWT-decoder gebruiken om te controleren of een toegangsteken de verwachte amr-waarde (Authentication Method Reference) bevat of niet:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Als de waarde aanwezig is, Partner Center de MFA-verificatie voltooid en wordt de API-aanvraag verwerkt. Als de waarde niet aanwezig is, Partner Center API de aanvraag met het volgende antwoord:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Wanneer App-Only verificatie wordt gebruikt, werken de API's die ondersteuning bieden App-Only verificatie continu zonder MFA.

## <a name="partner-delegated-administration"></a>Gedelegeerd beheer van partners

Partneraccounts, waaronder beheerdersagents en helpdeskmedewerkers, kunnen hun gedelegeerde beheerdersbevoegdheden van de partner gebruiken om klantresources te beheren via Microsoft Online Services-portals, opdrachtregelinterface (CLI) en API's (met behulp van App+Gebruikersverificatie).

### <a name="using-service-portals"></a>Serviceportals gebruiken

Wanneer u toegang hebt tot Microsoft Online Services-portals met behulp van de gedelegeerde beheerdersbevoegdheden van de partner (Admin-On-Behalf-Of) voor het beheren van klantresources, is voor veel van deze portals vereist dat het partneraccount interactief wordt geverifieerd, met de Azure AD-tenant van de klant ingesteld als verificatiecontext: het partneraccount is vereist voor aanmelding bij de tenant van de klant.

Wanneer Azure AD dergelijke verificatieaanvragen ontvangt, moet het partneraccount MFA-verificatie voltooien. Er zijn twee mogelijke gebruikerservaringen, afhankelijk van of het partneraccount een beheerde of federatief identiteit is:

- Als het partneraccount een **beheerde** identiteit is, wordt de gebruiker rechtstreeks door Azure AD gevraagd om de MFA-verificatie te voltooien. Als het partneraccount niet eerder is geregistreerd voor MFA bij Azure AD, wordt de gebruiker gevraagd om eerst [de MFA-registratie te](#mfa-registration-experience) voltooien.

- Als het partneraccount een **federatief** identiteit is, is de ervaring afhankelijk van hoe de partnerbeheerder federatie in Azure AD heeft geconfigureerd. Bij het instellen van federatie in Azure AD kan de partnerbeheerder aan Azure AD aangeven of de federatie-id-provider MFA al dan niet ondersteunt. Zo ja, dan leidt Azure AD de gebruiker om naar de federatief-id-provider om de MFA-verificatie te voltooien. Anders wordt de gebruiker rechtstreeks door Azure AD gevraagd om de MFA-verificatie te voltooien. Als het partneraccount niet eerder is geregistreerd voor MFA bij Azure AD, wordt de gebruiker gevraagd om eerst [de MFA-registratie te](#mfa-registration-experience) voltooien.

De algehele ervaring is vergelijkbaar met het scenario waarin een tenant van een eindklant MFA heeft geïmplementeerd voor de beheerders. De tenant van de klant heeft bijvoorbeeld [standaardinstellingen](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)voor Azure AD-beveiliging ingeschakeld, waarvoor alle accounts met beheerdersrechten zijn vereist om zich aan te melden bij de tenant van de klant met MFA-verificatie, inclusief beheerdersagents en helpdeskmedewerkers. Voor testdoeleinden kunnen partners de [standaardinstellingen](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) voor Azure AD-beveiliging inschakelen in de tenant van de klant en vervolgens proberen gedelegeerde beheerdersbevoegdheden van de partner te gebruiken om toegang te krijgen tot de tenant van de klant.

> [!NOTE]
> Niet alle Microsoft Online Service Portals vereisen partneraccounts om zich aan te melden bij de tenant van de klant bij het openen van klantresources met behulp van gedelegeerde beheerdersbevoegdheden van de partner. In plaats daarvan hebben ze alleen de partneraccounts nodig om zich aan te melden bij de partner-tenant. Een voorbeeld is het Exchange-beheercentrum. Na een periode verwachten we dat voor deze portals partneraccounts moeten worden gebruikt om zich aan te melden bij de tenant van de klant wanneer partner gedelegeerde beheerdersbevoegdheden worden gebruikt.

### <a name="using-service-apis"></a>Service-API's gebruiken

Sommige Microsoft Online Services-API's (zoals Azure Resource Manager, Azure AD Graph, Microsoft Graph enzovoort) ondersteunen partners die gedelegeerde beheerdersbevoegdheden van partners gebruiken om klantresources programmatisch te beheren. Als u gedelegeerde beheerdersbevoegdheden van de partner wilt gebruiken met deze API's, moet de partnertoepassing een toegangs token bevatten in de header Autorisatie van DE API-aanvraag, waarbij het toegangsken wordt verkregen door een partnergebruikersaccount te hebben om te verifiëren met Azure AD, waarbij azure AD van de klant is ingesteld als verificatiecontext. De partnertoepassing moet een partnergebruikersaccount hebben om zich aan te melden bij de tenant van de klant.

Wanneer Azure AD een dergelijke verificatieaanvraag ontvangt, heeft Azure AD het partnergebruikersaccount nodig om de MFA-verificatie te voltooien. Als het partnergebruikersaccount nog niet eerder is geregistreerd voor MFA, wordt het gebruikersaccount gevraagd om eerst de MFA-registratie te voltooien.

Alle partnertoepassingen die zijn geïntegreerd met deze API's met behulp van gedelegeerde beheerdersbevoegdheden van de partner, worden beïnvloed door deze functie. Om ervoor te zorgen dat partnertoepassingen zonder onderbreking met deze API's kunnen blijven werken:

- Partner moet voorkomen dat niet-interactieve gebruikersverificatiemethode met Azure AD wordt gebruikt om het toegangs token te verkrijgen. Wanneer u niet-interactieve gebruikersverificatiemethode zoals [Wachtwoordstroom](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)gebruikt, kan de gebruiker niet worden gevraagd MFA-verificatie te voltooien. De partner moet overschakelen naar een interactieve gebruikersverificatiemethode, [zoals OpenID Connect stroom.](/azure/active-directory/develop/v1-protocols-openid-connect-code)

- Tijdens de interactieve gebruikersverificatiemethode moet de partner een partnergebruikersaccount gebruiken dat al is ingeschakeld voor MFA. Als dit wordt gevraagd door Azure AD, kan de partner ook de MFA-registratie en MFA-verificatie tijdens het aanmelden voltooien.

- Dit is vergelijkbaar met het scenario waarin een tenant van een eindklant MFA heeft geïmplementeerd voor de beheerders. De tenant van de klant heeft bijvoorbeeld [de standaardinstellingen](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)voor Azure AD-beveiliging ingeschakeld. Hiervoor zijn alle gebruikersaccounts met beheerdersrechten vereist om zich met MFA-verificatie aan te melden bij de tenant van de klant, inclusief beheerdersagents en helpdeskmedewerkers. Voor testdoeleinden kunnen partners de [standaardinstellingen](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) voor Azure AD-beveiliging inschakelen in de tenant van de klant en vervolgens proberen gedelegeerde beheerdersbevoegdheden van de partner te gebruiken om programmatisch toegang te krijgen tot de tenant van de klant.

### <a name="mfa-registration-experience"></a>MFA-registratie-ervaring

Als tijdens MFA-verificatie het partneraccount nog niet eerder is geregistreerd voor MFA, wordt de gebruiker door Azure AD gevraagd om eerst de MFA-registratie te voltooien:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA-registratie stap 1":::

Nadat u op **Volgende hebt** geklikt, wordt de gebruiker gevraagd om te kiezen uit een lijst met verificatiemethoden.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA-registratie stap 2":::

Na een geslaagde registratie moet de gebruiker de MFA-verificatie voltooien op basis van de verificatie die door de gebruiker is gekozen.
 
## <a name="list-of-common-issues"></a>Lijst met veelvoorkomende problemen

Voordat u een technische [uitzondering op de](#how-to-submit-a-request-for-technical-exception) MFA-vereiste aanvraagt, bekijkt u de lijst met veelvoorkomende problemen die zijn gerapporteerd door andere partners om te begrijpen of uw aanvraag geldig is.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Probleem 1: Partner heeft meer tijd nodig om MFA te implementeren voor hun partneragents
Een partner is nog niet gestart of is nog bezig met het implementeren van MFA voor hun partneragents die toegang nodig hebben tot Microsoft Online Services-portals met behulp van gedelegeerde beheerdersbevoegdheden van partners om klantresources te beheren. De partner heeft meer tijd nodig om de MFA-implementatie te voltooien. Is dit probleem een geldige reden voor een technische uitzondering?

**Antwoord:** Nee. Partner moet plannen maken voor het implementeren van MFA voor hun gebruikers om onderbrekingen te voorkomen.

> [!NOTE]
> Hoewel de partner MFA niet heeft geïmplementeerd voor hun partneragents, hebben de partneragents nog steeds toegang tot Microsoft Online Services-portals met behulp van gedelegeerde beheerdersbevoegdheden van partners, mits ze MFA-registratie en MFA-verificatie kunnen voltooien wanneer hier om wordt gevraagd tijdens het aanmelden bij de tenant van de klant. Als u MFA-registratie voltooit, wordt de gebruiker niet automatisch ingeschakeld voor MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Probleem 2: Partner heeft geen MFA geïmplementeerd voor gebruikersaccounts die geen gedelegeerde beheerdersbevoegdheden gebruiken
Een partner heeft een aantal gebruikers in hun partnerten tenants die geen toegang nodig hebben tot Microsoft Online Services-portals voor het beheren van klantresources met behulp van gedelegeerde beheerdersbevoegdheden van partners. De partner is bezig met het implementeren van MFA voor deze gebruikers en heeft meer tijd nodig om te voltooien. Is dit probleem een geldige reden voor een technische uitzondering?

**Antwoord:** Nee. Omdat deze gebruikersaccounts geen gedelegeerde beheerdersbevoegdheden van partners gebruiken voor het beheren van klantresources, zijn ze niet verplicht om zich aan te melden bij de tenant van de klant. Deze worden niet beïnvloed door azure AD waarvoor MFA-verificatie is vereist tijdens het aanmelden bij de tenant van de klant.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Probleem 3: Partner heeft geen MFA geïmplementeerd voor gebruikersserviceaccounts
Een partner heeft een aantal gebruikersaccounts in hun partnerten tenants, die door apparaten worden gebruikt als serviceaccounts. Dit zijn accounts met beperkte bevoegdheden waarvoor geen toegang is Partner Center microsoft Online Services-portals voor het beheren van klantresources met behulp van gedelegeerde beheerdersbevoegdheden van partners. Is dit probleem een geldige reden voor een technische uitzondering?

**Antwoord:** Nee. Omdat deze gebruikersaccounts geen gedelegeerde beheerdersbevoegdheden van partners gebruiken voor het beheren van klantresources, zijn ze niet vereist om zich aan te melden bij de tenant van de klant. Ze worden niet beïnvloed door azure AD waarvoor MFA-verificatie is vereist tijdens het aanmelden bij de tenant van de klant.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Probleem 4: De partner kan MFA niet implementeren met behulp van de MS Authenticator-app
Een partner heeft 'clean desk'-beleid, waardoor werknemers hun persoonlijke mobiele apparaten niet naar hun werkgebied kunnen brengen. Zonder toegang tot hun persoonlijke mobiele apparaten kunnen de werknemers de MS Authenticator-app niet installeren. Dit is de enige MFA-verificatie die wordt ondersteund door de standaardinstellingen voor Azure AD-beveiliging. Is dit probleem een geldige reden voor een technische uitzondering?

**Antwoord:** Nee, dit is geen geldige reden voor een technische uitzondering. De partner moet de volgende alternatieven overwegen, zodat hun werknemers nog steeds MFA-verificatie kunnen voltooien bij het openen van Partner Center:
- Partner kan zich ook registreren voor Azure AD Premium MFA-oplossingen van derden (compatibel met Azure AD) die aanvullende verificatiemethoden kunnen bieden.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Probleem 5: Partner kan MFA niet implementeren vanwege het gebruik van verouderde verificatieprotocollen
Een partner heeft een aantal partneragents die nog steeds gebruikmaken van verouderde verificatieprotocollen, die niet compatibel zijn met MFA. De gebruikers gebruiken bijvoorbeeld nog steeds Outlook 2010, dat is gebaseerd op verouderde verificatieprotocollen. Het inschakelen van MFA voor deze partneragenten verstoort het gebruik van verouderde verificatieprotocollen.

**Antwoord:** Nee, dit is geen geldige reden voor een technische uitzondering. Partners worden ten zeerste aangeraden af te stappen van het gebruik van verouderde verificatieprotocollen vanwege mogelijke gevolgen voor de beveiliging, omdat deze protocollen niet kunnen worden beveiligd met MFA-verificatie en veel vatbaarder zijn voor referentierisico's. Als het gebruik van verouderde verificatieprotocollen geen optie is, kunnen partners overwegen zich aan te melden voor Azure AD Premium, dat het gebruik van toepassingswachtwoorden ondersteunt. Toepassingswachtwoorden zijn een een keer door het systeem gegenereerde wachtwoorden en zijn meestal sterker dan door mensen gegenereerde wachtwoorden. Met behulp van toepassingswachtwoorden kunnen partners MFA implementeren voor hun gebruikers, terwijl ze alleen voor verouderde verificatieprotocollen terugvallen op toepassingswachtwoorden.

Lees het bericht over de [Basisverificatie](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) en Exchange Online voor meer informatie over het meest recente plan voor het ondersteunen van verouderde verificatie voor Outlook en volg de blog van het [Exchange-team](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) voor het volgende nieuws. 

> [!NOTE]
> Hoewel de partner MFA niet heeft geïmplementeerd voor hun partneragents, hebben de partneragents nog steeds toegang tot Microsoft Online Services-portals met behulp van gedelegeerde beheerdersbevoegdheden van partners, mits ze MFA-registratie en MFA-verificatie kunnen voltooien wanneer hier om wordt gevraagd tijdens het aanmelden bij de tenant van de klant. Als u MFA-registratie voltooit, wordt de gebruiker niet automatisch ingeschakeld voor MFA.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Probleem 6: De partner heeft externe MFA geïmplementeerd die niet wordt herkend door Azure AD
Een partner heeft MFA geïmplementeerd voor hun gebruikers met behulp van een MFA-oplossing van derden. De partner kan de MFA-oplossing van derden echter niet correct configureren om aan Azure AD door te geven dat MFA-verificatie is voltooid tijdens de gebruikersverificatie. Is dit een geldige reden voor een technische uitzondering?

**Antwoord:** Ja, dit probleem kan worden beschouwd als een geldige reden voor een technische uitzondering. Voordat u een aanvraag voor technische uitzondering indient, moet u bij de provider van de MFA-oplossing van derden bevestigen dat de MFA-oplossing niet kan worden geconfigureerd om de claim *authenticationmethodsreferences* (met de waarde *multipleauthn*) naar Azure AD te sturen om aan te geven dat MFA-verificatie is voltooid tijdens de gebruikersverificatie. Tijdens het indienen van een aanvraag voor technische uitzondering, moet u details opgeven van de gebruikte MFA-oplossing van derden en de integratiemethode aangeven (bijvoorbeeld via identiteitsfederatie of het gebruik van Aangepast beheer van Azure AD), en de volgende informatie in de aanvraag voor technische uitzonderingen opgeven als de ondersteunende documenten:

- De MFA-configuraties van derden.

- Het resultaat van [Test the Partner Security Requirements running](/powershell/partnercenter/test-partner-security-requirements) by the third-party MFA enabled account.

- De inkooporder van de MFA-oplossing van derden die u gebruikt of die u wilt gebruiken.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Een aanvraag indienen voor een technische uitzondering

Partners kunnen een technische uitzondering aanvragen om MFA-verificatie te onderdrukken als ze technische problemen ondervinden met Microsoft Online Services en er geen haalbare oplossing of tijdelijke oplossing is. Bekijk voordat u dit doet de [lijst met veelvoorkomende problemen](#list-of-common-issues) in de vorige sectie.

Een aanvraag voor een technische uitzondering indienen:

1. Meld u aan Partner Center globale beheerder of beheerderagent.

2. Maak een nieuwe partnerserviceaanvraag door te navigeren naar **Ondersteuningsaanvragen**  >  **van ondersteuningspartners** en Nieuwe **aanvraag te selecteren.**

3. Zoeken naar **MFA - Aanvraag voor uitzondering** in het zoekvak; of selecteer **CSP** in Categorie, selecteer **vervolgens Accounts, Onboarding, Toegang** vanuit onderwerp, selecteer **vervolgens MFA - Aanvraag** voor uitzondering van het subonderwerp en selecteer vervolgens volgende **stap.**

4. Geef de details op die zijn aangevraagd om een serviceaanvraag voor technische uitzondering in te dienen en selecteer **Verzenden.**

Het kan tot drie werkdagen duren voordat Microsoft een reactie geeft op een aanvraag voor technische uitzonderingen.

## <a name="next-steps"></a>Volgende stappen

 - [Status van beveiligingsvereisten van partner](partner-security-compliance.md)