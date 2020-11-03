---
title: Eisen multi-factor Authentication (MFA) voor uw partner-Tenant
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe eisen MFA voor uw partner tenants uw toegang tot klant bronnen helpt beveiligen. Bevat voorbeeld scenario's.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b6985054e927dd777d61ae30bd435ab4c6c4ea8c
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133101"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Eisen multi-factor Authentication (MFA) voor uw partner-Tenant

**Van toepassing op**

- Alle partners in het Cloud Solution Provider-programma
- Alle leveranciers van het configuratie scherm
- Alle Advisors

**Betrokken rollen**

- Beheer agent
- Verkoop agent
- Helpdesk medewerker
- Factureringsbeheerder
- Globale beheerder

Dit artikel bevat gedetailleerde voor beelden en richt lijnen voor eisen multi-factor Authentication (MFA) in het partner centrum. Het doel van deze functie is om partners te helpen hun toegang tot klant bronnen te beveiligen tegen inbreuk op de referenties. Partners zijn verplicht MFA af te dwingen voor alle gebruikers accounts in hun partner Tenant, met inbegrip van gast gebruikers. Gebruikers worden verplicht om de MFA-verificatie te volt ooien voor de volgende gebieden:

- [Dash board van partner centrum](#partner-center-dashboard)
- [Partnercentrum-API](#partner-center-api)
- [Door de partner gedelegeerd beheer](#partner-delegated-administration)

Meer en voortdurende beveiligings-en privacy-veiligheids maatregelen zijn te vinden op onze belangrijkste prioriteiten en we blijven onze klanten en tenants helpen beveiligen. Alle partners die deel nemen aan het programma Cloud Solution Provider (CSP), leveranciers van het configuratie scherm (CPVs) en Advisor, moeten de vereisten voor de beveiliging van de partner implementeren om te blijven voldoen aan het [beleid](partner-security-requirements.md) .

Om partners te helpen hun bedrijven en klanten te beschermen tegen identiteits diefstal en onbevoegde toegang, hebben we extra beveiligings maatregelen geactiveerd voor partner tenants die MFA verplicht stellen en verifiëren. 

## <a name="partner-center-dashboard"></a>Dash board van partner centrum

Bepaalde pagina's in het dash board van de partner centrum worden beveiligd met MFA, waaronder:

- Alle pagina's op het tabblad **klanten** , bijvoorbeeld alle pagina's die toegankelijk zijn via de volgende URL: https://partner.microsoft.com/commerce/*
- Alle pagina's op het tabblad **ondersteuning > klant aanvragen** , bijvoorbeeld de pagina die wordt geopend onder https://partner.microsoft.com/dashboard/support/csp/customers/*
- Pagina Facturering

In de volgende tabel ziet u welke gebruikers typen zijn geautoriseerd voor toegang tot deze door MFA beveiligde pagina's (en die daarom worden beïnvloed door deze functie).


| Met MFA beveiligde pagina       | Beheerders agents      |  Verkoop medewerkers     |   Helpdesk medewerkers     | Globale beheerder      |  Factureringsbeheerder     | 
|---    |---    |---    |---    |---    |---    |
| Tabblad alle pagina's onder klanten      |   x    |    x   |  x     |       |       |
| Het tabblad alle pagina's onder ondersteuning > van klant aanvragen     | x      |       |    x   |       |       |
| Pagina Facturering     |   x    |       |       |    x   |   x    |

Als u probeert toegang te krijgen tot een van deze pagina's en u hebt geen MFA-verificatie eerder voltooid, moet u dit doen. Andere pagina's in het partner centrum, zoals de pagina overzicht, de pagina Service Health status controle vereist geen MFA.

## <a name="verification-examples"></a>Verificatie voorbeelden

Bekijk de volgende voor beelden om te laten zien hoe verificatie werkt in het dash board van de Partner Center.

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>Voor beeld 1: partner heeft Azure AD MFA geïmplementeerd

1. Jeroen werkt voor CSP contoso. Contoso heeft MFA geïmplementeerd voor al hun gebruikers onder contoso-partner-tenants met behulp van Azure Active Directory (Azure AD) MFA.

2. Jeroen start een nieuwe browser sessie en navigeert naar de overzichts pagina van het dash board van partner Center (dit is geen MFA-beveiligd). Het partner centrum stuurt Jeroen naar Azure AD om zich aan te melden.

3. Vanwege de bestaande Azure AD MFA-installatie van Contoso is Jeroen vereist om de MFA-verificatie te volt ooien. Bij geslaagde aanmelding en MFA-verificatie wordt Jeroen teruggeleid naar de overzichts pagina van het dash board van partner Center.

4. Jeroen probeert toegang te krijgen tot een van de met MFA beveiligde pagina's in het partner centrum. Omdat Jeroen de MFA-verificatie al heeft voltooid tijdens het aanmelden, heeft Jeroen toegang tot de pagina die is beveiligd met MFA zonder dat dit nodig is om de MFA-verificatie te door lopen.

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>Voor beeld 2: partner heeft MFA van derden geïmplementeerd met behulp van identiteits Federatie

1. Trent werkt voor CSP Wingtip. Wingtip heeft MFA geïmplementeerd voor al hun gebruikers onder Wingtip partner Tenant met behulp van MFA van derden, die is geïntegreerd met Azure AD via identiteits Federatie.

2. Trent start een nieuwe browser sessie en navigeert naar de overzichts pagina van het dash board van partner Center (dit is geen MFA-beveiligd). Het partner centrum leidt Trent naar Azure AD om zich aan te melden.

3. Omdat Wingtip is ingesteld als identiteits Federatie, stuurt Azure AD de Trent naar de federatieve id-provider om de aanmelding en MFA-verificatie te volt ooien. Nadat u zich hebt aangemeld en MFA hebt gecontroleerd, wordt Trent teruggeleid naar Azure AD en vervolgens naar de overzichts pagina van het dash board-partner centrum.

4. Trent probeert toegang te krijgen tot een van de met MFA beveiligde pagina's in het partner centrum. Omdat Trent de MFA-verificatie al heeft voltooid tijdens het aanmelden, heeft Trent toegang tot de pagina die is beveiligd met MFA zonder dat dit nodig is om de MFA-verificatie te door lopen.

### <a name="example-3-partner-hasnt-implemented-mfa"></a>Voor beeld 3: partner heeft geen MFA geïmplementeerd

1. John werkt voor CSP fabrikam. Fabrikam heeft geen MFA geïmplementeerd voor een gebruiker onder fabrikam partner Tenant.

2. John start een nieuwe browser sessie en navigeert naar de overzichts pagina van het dash board van partner Center (dit is geen MFA-beveiligd). Het partner centrum stuurt John naar Azure AD om zich aan te melden.

3. Omdat fabrikam geen MFA heeft geïmplementeerd, is John niet vereist om MFA-verificatie te volt ooien. Bij een geslaagde aanmelding wordt John omgeleid naar de overzichts pagina van het dash board van partner Center.

4. John probeert toegang te krijgen tot een van de met MFA beveiligde pagina's in het partner centrum. Omdat John geen MFA-verificatie heeft voltooid, stuurt het partner centrum John door naar Azure AD om de MFA-verificatie te volt ooien. Aangezien dit de eerste keer is dat John is vereist voor het volt ooien van MFA, wordt John ook gevraagd om [zich te registreren voor MFA](#mfa-registration-experience). Bij een succes volle MFA-registratie en MFA-verificatie heeft John nu toegang tot de pagina met MFA-beveiliging.

5. Een andere dag voordat fabrikam MFA implementeert voor alle gebruikers, John start een nieuwe browser sessie en navigeert naar de overzichts pagina van het dash board van partner Center (dit is niet MFA-beveiligd). Het partner centrum stuurt John naar Azure AD om zich aan te melden zonder MFA-prompt. 

6. John probeert toegang te krijgen tot een van de met MFA beveiligde pagina's in het partner centrum. Omdat John geen MFA-verificatie heeft voltooid, stuurt het partner centrum John door naar Azure AD om de MFA-verificatie te volt ooien. Omdat John een geregistreerde MFA heeft, wordt deze keer alleen gevraagd om de MFA-verificatie te volt ooien.

> [!NOTE]
>Actie: bedrijfs beheerders hebben [drie opties](partner-security-requirements.md#implementing-multi-factor-authentication) voor het implementeren van MFA.

## <a name="partner-center-api"></a>Partnercentrum-API

De partner centrum-API ondersteunt alleen app-only-verificatie en app +-gebruikers verificatie. 

Wanneer app + gebruikers verificatie wordt gebruikt, is voor het partner centrum MFA-verificatie vereist. Meer in het bijzonder, wanneer een partner toepassing een API-aanvraag naar het partner centrum wil verzenden, moet deze een toegangs token bevatten in de autorisatie-header van de aanvraag. 

> [!NOTE]
>Het [Framework van het veilige toepassings model](/partner-center/develop/enable-secure-app-model) is een schaalbaar Framework voor het verifiëren van CSP-partners en CPVs via de Microsoft Azure MFA-architectuur bij het aanroepen van partner Center-api's. U moet dit framework implementeren voordat u MFA op uw Tenant inschakelt. 

Wanneer het partner centrum een API-aanvraag ontvangt met een toegangs token dat is verkregen met behulp van app + gebruikers authenticatie, controleert de Partner Center-API of de *MFA* -waarde in de claim van de *verificatie methode Reference (AMR)* aanwezig is. U kunt een JWT-decoder gebruiken om te controleren of een toegangs token de verwachte waarde voor de verificatie methode verwijzing (AMR) bevat of niet:

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

Als de waarde aanwezig is, sluit het partner centrum aan dat de MFA-verificatie is voltooid en de API-aanvraag verwerkt. Als de waarde niet aanwezig is, wordt de aanvraag door de Partner Center-API afgewezen met het volgende antwoord:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Als App-Only verificatie wordt gebruikt, werken de Api's die ondersteuning bieden voor App-Only-verificatie voortdurend zonder MFA.

## <a name="partner-delegated-administration"></a>Door de partner gedelegeerd beheer

Partner accounts, met inbegrip van beheerders agents en helpdesk agenten, kunnen gebruikmaken van hun partner gedelegeerde beheerders bevoegdheden voor het beheren van klant bronnen via micro soft Online Services portals, opdracht regel interface (CLI) en Api's (met behulp van app + gebruikers verificatie).

### <a name="using-service-portals"></a>Service portals gebruiken

Bij het openen van micro soft Online Services-portals met behulp van de door de partner gedelegeerde beheerders bevoegdheden (namen van Administrators) voor het beheer van klant resources, moeten veel van deze portals interactief worden geverifieerd met de Azure AD-Tenant van de klant als verificatie context. de partner account is vereist om zich aan te melden bij de klant Tenant.

Wanneer Azure AD dergelijke verificatie aanvragen ontvangt, is het partner account vereist voor het volt ooien van de MFA-verificatie. Er zijn twee mogelijke gebruikers ervaringen, afhankelijk van het feit of de partner account een beheerde of federatieve identiteit is:

- Als het partner account een **beheerde** identiteit is, wordt de gebruiker rechtstreeks door Azure AD gevraagd om de MFA-verificatie te volt ooien. Als het partner account niet eerder is geregistreerd voor MFA met Azure AD, wordt de gebruiker gevraagd om de [MFA-registratie te volt ooien](#mfa-registration-experience) .

- Als het partner account een **federatieve** identiteit is, is de ervaring afhankelijk van de manier waarop de partner beheerder Federatie in azure AD heeft geconfigureerd. Bij het instellen van Federatie in azure AD kan de partner beheerder aangeven of de federatieve id-provider MFA ondersteunt of niet. Als dit het geval is, wordt de gebruiker door Azure AD omgeleid naar de federatieve id-provider om de MFA-verificatie te volt ooien. Anders vraagt Azure AD de gebruiker direct om de MFA-verificatie te volt ooien. Als het partner account niet eerder is geregistreerd voor MFA met Azure AD, wordt de gebruiker gevraagd om de [MFA-registratie te volt ooien](#mfa-registration-experience) .

De algemene ervaring is vergelijkbaar met het scenario waarin een Tenant van een eind gebruiker MFA voor de beheerders heeft geïmplementeerd. De Tenant van de klant heeft bijvoorbeeld de [standaard instellingen voor Azure AD-beveiliging](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)ingeschakeld. hiervoor zijn alle accounts met beheerders rechten nodig om zich aan te melden bij de klant TENANT met MFA-verificatie, met inbegrip van beheerders agents en helpdesk agenten. Voor test doeleinden kunnen partners de [standaard instellingen van de Azure AD-beveiliging](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) inschakelen in de Tenant van de klant en vervolgens proberen om toegang te krijgen tot de eigenaar van de klant.

> [!NOTE]
> Niet alle micro soft online service-portals vereisen dat partner accounts zich aanmelden bij de Tenant van de klant bij het openen van klant bronnen met behulp van gedelegeerde beheerders bevoegdheden van de partner. In plaats daarvan hebben ze alleen de partner accounts nodig om zich aan te melden bij de partner Tenant. Een voor beeld is het Exchange-beheer centrum. Na verloop van tijd kunnen deze portals worden gebruikt om te vereisen dat partner accounts worden aangemeld bij de Tenant van de klant bij het gebruik van gedelegeerde beheerders bevoegdheden voor de partner.

### <a name="using-service-apis"></a>Service-Api's gebruiken

Sommige micro soft Online Services-Api's (zoals Azure Resource Manager, Azure AD Graph, Microsoft Graph enz.) ondersteunen partners die gebruikmaken van gedelegeerde beheerders bevoegdheden voor het programmatisch beheren van klant resources. Om gebruik te maken van de door de partner gedelegeerde beheerders bevoegdheden met deze Api's, moet de partner toepassing een toegangs token bevatten in de autorisatie-header van de API-aanvraag, waarbij het toegangs token wordt verkregen door een partner gebruikers account te hebben om te verifiëren bij Azure AD, waarbij de klant Azure AD is ingesteld als verificatie context. De partner toepassing moet een gebruikers account van de partner aanmelden bij de Tenant van de klant.

Wanneer Azure AD als verificatie aanvraag wordt ontvangen, moet de partner gebruikers account van Azure AD de MFA-verificatie volt ooien. Als de partner gebruikers account voor MFA nog niet is geregistreerd, wordt het gebruikers account eerst gevraagd de MFA-registratie te volt ooien.

Alle partner toepassingen die zijn geïntegreerd met deze Api's met behulp van gedelegeerde beheerders bevoegdheden van de partner, worden beïnvloed door deze functie. Om ervoor te zorgen dat partner toepassingen zonder onderbreking met deze Api's kunnen blijven werken:

- De partner moet voor komen dat de niet-interactieve verificatie methode van de gebruiker met Azure AD wordt gebruikt om het toegangs token op te halen. Wanneer u niet-interactieve gebruikers verificatie methode gebruikt, zoals de [wachtwoord stroom](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), kan Azure AD de gebruiker niet vragen om MFA-verificatie te volt ooien. De partner moet overschakelen op het gebruik van interactieve verificatie methode voor gebruikers, zoals [OpenID Connect Connect flow](/azure/active-directory/develop/v1-protocols-openid-connect-code) .

- Tijdens de interactieve verificatie methode van de gebruiker moet de partner een partner gebruikers account gebruiken dat al is ingeschakeld voor MFA. Als u daarom wordt gevraagd door Azure AD, kan de partner MFA-registratie en MFA-verificatie volt ooien tijdens het aanmelden.

- Dit is vergelijkbaar met het scenario waarin een Tenant van een eind gebruiker MFA voor de beheerders heeft geïmplementeerd. De Tenant van de klant heeft bijvoorbeeld de [standaard instellingen voor Azure AD-beveiliging](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)ingeschakeld. hiervoor zijn alle gebruikers accounts met beheerders rechten nodig om zich aan te melden bij de Tenant van de klant met MFA-verificatie, met inbegrip van beheerders agents en helpdesk agenten. Voor test doeleinden kunnen partners de [standaard instellingen van Azure AD-beveiliging](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) inschakelen in de Tenant van de klant en vervolgens proberen om via een programma toegang te krijgen tot de Tenant van de klant.

### <a name="mfa-registration-experience"></a>MFA-registratie-ervaring

Als tijdens de MFA-verificatie het partner account voor MFA nog niet is geregistreerd, wordt de gebruiker door Azure AD gevraagd de MFA-registratie te volt ooien:

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA-registratie stap 1":::

Nadat u op **volgende** hebt geklikt, wordt de gebruiker gevraagd om te kiezen uit een lijst met verificatie methoden.

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA-registratie stap 1":::

Na een geslaagde registratie is de gebruiker verplicht om de MFA-verificatie te volt ooien op basis van de door de gebruiker gekozen verificatie.
 
## <a name="list-of-common-issues"></a>Lijst met veelvoorkomende problemen

Lees, voordat u een [technische uitzonde ring](#how-to-submit-a-request-for-technical-exception) van de MFA-vereiste toepast, de lijst met veelvoorkomende problemen die door andere partners zijn gerapporteerd om te begrijpen of uw aanvraag geldig is.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Probleem 1: partner heeft meer tijd nodig om MFA voor hun partner agenten te implementeren
Een partner is niet gestart of is nog steeds in het proces van het implementeren van MFA voor hun partner agenten die toegang nodig hebben tot micro soft Online Services-portals met behulp van gedelegeerde beheer bevoegdheden voor het beheren van klant resources. De partner heeft meer tijd nodig om de MFA-implementatie te volt ooien. Is dit een geldige reden voor een technische uitzonde ring?

**Antwoord** : Nee. De partner moet plannen maken om MFA voor hun gebruikers te implementeren om onderbrekingen te voor komen.

> [!NOTE]
> Hoewel de partner geen MFA voor hun partner agenten heeft geïmplementeerd, kunnen de partner agents nog steeds toegang krijgen tot portals van micro soft Online Services met behulp van de gedelegeerde beheer bevoegdheden van de partner, mits deze de MFA-registratie en MFA-verificatie kunnen volt ooien wanneer u wordt gevraagd om u aan te melden bij de klant Tenant Bij het volt ooien van MFA-registratie wordt de gebruiker niet automatisch voor MFA ingeschakeld.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Probleem 2: partner heeft geen MFA geïmplementeerd voor gebruikers accounts die geen gedelegeerde beheerders bevoegdheden gebruiken
Een partner heeft sommige gebruikers in hun partner tenants die geen toegang nodig hebben tot micro soft Online Services-portals om klanten resources te beheren met gemachtigde beheer bevoegdheden. De partner is bezig met het implementeren van MFA voor deze gebruikers en heeft meer tijd nodig om te volt ooien. Is dit een geldige reden voor een technische uitzonde ring?

**Antwoord** : Nee. Omdat deze gebruikers accounts geen door de partner gedelegeerde beheer bevoegdheden gebruiken om klant resources te beheren, hoeven ze zich niet aan te melden bij de Tenant van de klant. Deze worden niet beïnvloed door Azure AD waarvoor MFA-verificatie is vereist bij het aanmelden bij de klant Tenant.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Probleem 3: partner heeft geen MFA geïmplementeerd voor gebruikers service accounts
Een partner heeft sommige gebruikers accounts in hun partner tenants die door apparaten als service accounts worden gebruikt. Dit zijn accounts met weinig bevoegdheden waarvoor geen portals voor Access Partner Center of micro soft Online Services zijn vereist voor het beheren van klant resources met behulp van overgedragen beheer bevoegdheden van de partner. Is dit een geldige reden voor een technische uitzonde ring?

**Antwoord** : Nee. Omdat deze gebruikers accounts geen door de partner gedelegeerde beheer bevoegdheden gebruiken om klant resources te beheren, hoeven ze zich niet aan te melden bij de Tenant van de klant. Deze worden niet beïnvloed door Azure AD waarvoor MFA-verificatie is vereist bij het aanmelden bij de klant Tenant.

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Probleem 4: partner kan geen MFA implementeren met behulp van de MS Authenticator-app
Een partner heeft het beleid ' schoon bureau ', zodat werk nemers hun persoonlijke mobiele apparaten niet op hun werk gebied kunnen zetten. Zonder toegang tot hun persoonlijke mobiele apparaten kunnen de werk nemers de MS Authenticator-app niet installeren. Dit is de enige MFA-verificatie die wordt ondersteund door de standaard instellingen van Azure AD. Is dit een geldige reden voor een technische uitzonde ring?

**Antwoord** : Nee, dit is geen geldige reden voor een technische uitzonde ring. De partner moet rekening houden met de volgende alternatieven, zodat hun werk nemers de MFA-verificatie kunnen volt ooien bij het openen van het partner centrum:
- De partner kan zich ook aanmelden voor Azure AD Premium of MFA-oplossingen van derden (compatibel met Azure AD), die aanvullende verificatie methoden kunnen bieden.

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Probleem 5: partner kan geen MFA implementeren vanwege het gebruik van verouderde verificatie protocollen
Een partner heeft een aantal partner agenten die nog steeds gebruikmaken van verouderde verificatie protocollen, die niet compatibel zijn met MFA. De gebruikers gebruiken bijvoorbeeld nog steeds Outlook 2010, dat is gebaseerd op verouderde verificatie protocollen. Door MFA in te scha kelen voor deze partner agenten wordt het gebruik van verouderde verificatie protocollen verstoord.

**Antwoord** : Nee, dit is geen geldige reden voor een technische uitzonde ring. Het gebruik van verouderde verificatie protocollen wordt sterk aangemoedigd vanwege mogelijke beveiligings implicaties omdat deze protocollen niet kunnen worden beveiligd met MFA-verificatie en veel meer gevoelig zijn voor de inbreuk op de referenties. Als u het gebruik van verouderde verificatie protocollen niet meer kunt gebruiken, moeten partners zich aanmelden voor Azure AD Premium, dat het gebruik van toepassings wachtwoorden ondersteunt. Toepassings wachtwoorden zijn eenmalig door het systeem gegenereerde wacht woorden en zijn doorgaans sterker dan door mensen gegenereerde wacht woorden. Met behulp van toepassings wachtwoorden kunnen partners MFA voor hun gebruikers implementeren, terwijl ze terugvallen op toepassings wachtwoorden voor verouderde verificatie protocollen.

Lees het bericht over de [Basic-verificatie en Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) voor meer informatie over het meest recente abonnement op ondersteuning voor verouderde verificatie voor Outlook en volg de blog van het [Exchange-team](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) om het nieuwe nieuws te ontvangen. 

> [!NOTE]
> Hoewel de partner geen MFA voor hun partner agenten heeft geïmplementeerd, kunnen de partner agents nog steeds toegang krijgen tot portals van micro soft Online Services met behulp van de gedelegeerde beheer bevoegdheden van de partner, mits deze de MFA-registratie en MFA-verificatie kunnen volt ooien wanneer u wordt gevraagd om u aan te melden bij de klant Tenant Bij het volt ooien van MFA-registratie wordt de gebruiker niet automatisch voor MFA ingeschakeld.

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Probleem 6: partner heeft een MFA van derden geïmplementeerd die niet wordt herkend door Azure AD
Een partner heeft MFA geïmplementeerd voor hun gebruikers met behulp van een MFA-oplossing van derden. De partner kan de MFA-oplossing van derden echter niet op de juiste manier configureren voor het door sturen naar Azure AD waardoor MFA-verificatie is voltooid tijdens gebruikers verificatie. Is dit een geldige reden voor een technische uitzonde ring?

**Antwoord** : Ja, dit probleem kan worden beschouwd als een geldige reden voor een technische uitzonde ring. Voordat u een aanvraag voor een technische uitzonde ring indient, moet u bevestigen dat de MFA-oplossing van derden niet kan worden geconfigureerd om de *authenticationmethodsreferences* -claim (met de waarde *Multipleauthn* ) naar Azure ad te laten stromen om aan te geven dat de MFA-verificatie is voltooid tijdens de gebruikers verificatie. Bij het indienen van een aanvraag voor een technische uitzonde ring moet u details opgeven over de gebruikte MFA-oplossing van derden en de methode voor integratie (bijvoorbeeld via identiteits Federatie of het aangepaste besturings element van Azure AD) aanduiden, en de volgende informatie opgeven in de aanvraag voor technische uitzonde ringen als ondersteunende documenten:

- De MFA-configuraties van derden.

- Het resultaat van [het testen van de vereisten voor de partner beveiliging](/powershell/partnercenter/test-partner-security-requirements) die worden uitgevoerd door het MFA-account van derden.

- De aankoop order van de MFA-oplossing van derden die u gebruikt of die u wilt gebruiken.

## <a name="how-to-submit-a-request-for-technical-exception"></a>Een aanvraag indienen voor een technische uitzonde ring

Partners kunnen van toepassing zijn op een technische uitzonde ring om MFA-verificatie te onderdrukken als er technische problemen met micro soft Online Services optreden en er geen bruikbare oplossingen of tijdelijke oplossingen zijn. Bekijk de [lijst met veelvoorkomende problemen](#list-of-common-issues) in de vorige sectie voordat u dit doet.

Een aanvraag indienen voor een technische uitzonde ring:

1. Meld u aan bij Partner Center als globale beheerder of beheer agent.

2. Maak een nieuwe partner service aanvraag door te **navigeren naar ondersteunings**  >  **aanvragen voor partners** en te klikken op **nieuwe aanvraag** .

3. Zoeken naar **MFA-aanvraag voor uitzonde ring** in het zoekvak; of selecteer **CSP** uit categorie, selecteer **accounts, onboarding, toegang tot** onderwerp en selecteer vervolgens **MFA-aanvraag voor uitzonde ring** in het subonderwerp en selecteer **volgende stap** .

4. Geef de gevraagde details op voor het indienen van een service aanvraag voor een technische uitzonde ring en klik op **verzenden** .

Micro soft kan Maxi maal drie werk dagen duren om een antwoord te geven op een aanvraag voor technische uitzonde ring.

## <a name="next-steps"></a>Volgende stappen

 - [Status van partner beveiligings vereisten](partner-security-compliance.md)