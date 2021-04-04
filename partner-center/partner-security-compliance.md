---
title: Status rapport van beveiligings vereisten
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het controleren van de beveiligings vereisten die voldoen aan het status rapport van de beveiligings vereisten en het partner centrum MFA-rapport
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: d56b9675ea405b29190f68420037ea9a92f3d831
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086546"
---
# <a name="security-requirements-status-report"></a>Status rapport van beveiligings vereisten

**Juiste rollen**
- CPV-beheerder
- Globale beheerder

In dit artikel wordt het status rapport voor beveiligings vereisten in partner centrum uitgelegd. Dit rapport bevat metrische gegevens over de naleving van vereisten voor de beveiliging van de [partner](partner-security-requirements.md) voor multi-factor Authentication (MFA) voor gebruikers in uw partner Tenant.

Als u dit rapport in [partner centrum](https://partner.microsoft.com/dashboard)wilt openen, gaat u naar **instellingen**  >  **account instellingen**  >  **beveiligings vereisten status**. Het rapport wordt dagelijks bijgewerkt en weerspiegelt de aanmeldings gegevens van de afgelopen zeven dagen.

>[!NOTE]
>Het rapport status van beveiligings vereisten wordt alleen ondersteund in partner centrum. Het is niet beschikbaar in de Microsoft Cloud voor de Amerikaanse overheid of Microsoft Cloud Duitsland. We raden u ten zeerste aan dat alle partners die via een soevereine Cloud handelen (Amerikaanse overheid en Duitsland), deze nieuwe beveiligings vereisten onmiddellijk aannemen. Deze partners zijn momenteel echter niet vereist om te voldoen aan de nieuwe beveiligings vereisten. Micro soft geeft in de toekomst aanvullende informatie over de afdwinging van deze beveiligings vereisten voor soevereine Clouds.

## <a name="security-status-metrics"></a>Metrische gegevens van beveiligings status

Het rapport status van beveiligings vereisten biedt inzicht in de partner MFA-implementatie en biedt metrische configuratie-en partner centrum-activiteiten op partner tenants. In de volgende secties worden deze metrische gegevens gedetailleerd beschreven.

### <a name="mfa-configuration-on-a-partner-tenant"></a>MFA-configuratie op een partner-Tenant

Het metrieke **percentage van ingeschakelde gebruikers accounts met MFA dat wordt afgedwongen met behulp van de opties die hier worden weer gegeven:** toont het percentage ingeschakelde gebruikers accounts in uw partner TENANT waarvoor MFA is afgedwongen. U kunt een van deze [MFA-opties](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) gebruiken om te voldoen aan de vereisten. Deze gegevens worden dagelijks vastgelegd en gerapporteerd. Bijvoorbeeld:

- Contoso is een CSP-partner met 110 gebruikers accounts in de Tenant, 10 van deze gebruikers accounts zijn uitgeschakeld. 
- Van de rest van 100 gebruikers accounts, 90 worden MFA afgedwongen met behulp van de meegeleverde [MFA-opties](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). De metriek toont daarom 90%. 

### <a name="partner-center-requests-with-mfa"></a>Partner centrum-aanvragen met MFA

Telkens wanneer uw werk nemers zich aanmelden bij het partner centrum om te werken of, via Api's, gegevens ophalen of verzenden via het partner centrum, zijn de beveiligings status vraag en bijgehouden. Ook inbegrepen bij het bijhouden van de beveiligings status zijn uw toepassingen en alle toepassingen van het configuratie scherm. Deze gegevens worden weer gegeven in metrieken onder **het percentage aanvragen voor partner centrum met MFA** en de afgelopen zeven dagen.

#### <a name="dashboard-mfa-verification"></a>Dashboard-MFA-verificatie

De metrische gegevens **via de Partner Center-Portal** zijn gerelateerd aan activiteiten in het dash board van de partner centrum. Hiermee wordt het percentage van de bewerkingen gemeten die zijn gemaakt door gebruikers die MFA-verificatie hebben voltooid. Bijvoorbeeld:

- Contoso is een CSP-partner met twee beheerders agenten, Jeroen en John.
- Op de eerste dag heeft Jeroen aangemeld bij het Partner Center-dash board zonder MFA-verificatie en werden er drie bewerkingen uitgevoerd.
- Op de tweede dag is Jan aangemeld bij het Partner Center-dash board zonder MFA-verificatie en werden er vijf bewerkingen uitgevoerd.
- Op de derde dag heeft Jeroen aangemeld bij het Partner Center-dash board met MFA-verificatie en twee bewerkingen uitgevoerd.
- Er zijn voor de resterende vier dagen geen bewerkingen uitgevoerd door een van de agents.
- Van de tien verwerkingen die in het venster van zeven dagen zijn gemaakt, zijn er twee gedaan door de gebruiker met MFA-verificatie. De metriek toont daarom 20%.

Gebruik de aanvragen voor bestands **portals zonder MFA** om te begrijpen welke gebruiker zich heeft aangemeld bij het Partner Center-dash board zonder MFA-verificatie en de tijd van de laatste bezoek tijdens het rapportage venster.

#### <a name="appuser-mfa-verification"></a>App + gebruikers-MFA-verificatie

De metrische gegevens **via API of SDK** zijn gerelateerd aan app + gebruikers verificatie via partner Center API-aanvragen. Hiermee wordt het percentage van API-aanvragen gemeten dat is gemaakt met behulp van een toegangs token met MFA-claim. Bijvoorbeeld:

- Fabrikam is een CSP-partner die een CSP-toepassing heeft die gebruikmaakt van een combi natie van app + gebruikers authenticatie en app-only-verificatie methoden.
- Op de eerste dag heeft de toepassing drie API-aanvragen gedaan, die werden ondersteund door een toegangs token dat is verkregen via de authenticatie methode voor apps en gebruikers zonder MFA-verificatie.
- Op de tweede dag hebben de toepassing vijf API-aanvragen uitgevoerd, die werden ondersteund door een toegangs token dat is verkregen met behulp van app-only-verificatie.
- Op de derde dag hebben de toepassing twee API-aanvragen gedaan, die werden ondersteund door een toegangs token dat is verkregen met behulp van app + gebruikers verificatie methode met MFA-verificatie.
- Er zijn voor de resterende vier dagen geen bewerkingen uitgevoerd door een van de agents.
- De vijf API-aanvragen op de tweede dag, die worden ondersteund door een toegangs token dat is verkregen via verificatie op basis van een app, worden wegge laten uit de metriek omdat het geen gebruik maakt van gebruikers referenties. Van de resterende vijf bewerkingen werden twee hiervan ondersteund door een toegangs token dat is verkregen met MFA-verificatie. De metriek toont daarom 40%.

Als u wilt weten welke app + gebruikers activiteiten resulteert in het niet-100% op deze metrische gegevens, gebruikt u bestanden:

- **Overzicht van API-aanvragen** om inzicht te krijgen in de algehele MFA-status per toepassing.
- **Alle API-aanvragen** om inzicht te krijgen in de details van de API-aanvragen van gebruikers van uw Tenant, is het resultaat beperkt tot maxi maal 10.000 meest recente aanvragen voor betere download ervaring.

## <a name="actions-for-mfa-status-below-100"></a>Acties voor de MFA-status onder 100%

Sommige partners die MFA hebben geïmplementeerd, zien mogelijk metrische rapport gegevens onder 100%. Als u wilt weten waarom, moet u rekening houden met de volgende factoren.

> [!NOTE]
> U moet samen werken met iemand van uw organisatie die vertrouwd is met Identity Management en MFA-implementatie voor uw partner Tenant.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Geïmplementeerde MFA voor uw partner-Tenant

U moet MFA implementeren voor de partner-Tenant om naleving te bereiken. Zie [beveiligings vereisten voor het gebruik van partner Center of partner Center api's](partner-security-requirements.md)voor meer informatie over het implementeren van MFA.

>[!NOTE]
> MFA-metrische gegevens worden dagelijks berekend en worden uitgevoerd in de afgelopen zeven dagen. Als u alleen een MFA-implementatie hebt voltooid voor uw partner-Tenant, worden de metrische gegevens mogelijk nog niet 100% weer gegeven.

### <a name="verify-mfa-on-all-user-accounts"></a>MFA controleren op alle gebruikers accounts

Krijg inzicht in de huidige MFA-implementatie voor alle gebruikers accounts of alleen enkele. Sommige MFA-oplossingen zijn op beleid gebaseerde en ondersteunen gebruikers uitsluiting, terwijl anderen mogelijk verplicht zijn om MFA expliciet in te scha kelen op basis van per gebruiker. Controleer of u geen gebruikers hebt uitgesloten van uw huidige MFA-implementatie. Elk gebruikers account dat wordt uitgesloten en zich aanmeldt bij het partner centrum voor het uitvoeren van alle activiteit CSP-, CPV-of Advisor-gerelateerde activiteiten kan ertoe leiden dat de metrische gegevens niet 100% zijn.

### <a name="review-your-mfa-conditions"></a>Uw MFA-voor waarden controleren

Begrijp of uw huidige implementatie alleen MFA afdwingt onder specifieke voor waarden. Sommige MFA-oplossingen bieden flexibiliteit om alleen MFA af te dwingen wanneer aan bepaalde voor waarden wordt voldaan. Bijvoorbeeld: de gebruiker is toegang tot een onbekend apparaat of een onbekende locatie. Een gebruiker die is ingeschakeld voor MFA maar niet vereist is om MFA-verificatie te volt ooien bij het openen van het partner centrum, kan de metrische gegevens niet 100%.

>[!NOTE]
>Voor partners die MFA met de standaard instellingen van Azure AD-beveiliging hebben geïmplementeerd, is het belang rijk te weten dat voor niet-beheerders gebruikers accounts multi-factor Authentication wordt afgedwongen op basis van risico. Gebruikers wordt alleen om MFA gevraagd tijdens Risk ante pogingen (bijvoorbeeld wanneer de gebruiker zich vanaf een andere locatie aanmeldt). Daarnaast hebben gebruikers Maxi maal 14 dagen de tijd om te registreren voor MFA. Gebruikers die geen MFA-registratie hebben voltooid, worden tijdens de periode van 14 dagen niet voor MFA-verificatie gecontroleerd. Daarom is het mogelijk dat de metrische gegevens niet 100% zijn voor partners die MFA hebben geïmplementeerd met behulp van de standaard instellingen van Azure AD.

### <a name="review-third-party-mfa-configurations"></a>MFA-configuraties van derden controleren

Als u een MFA-oplossing van derden gebruikt, moet u bepalen hoe u deze integreert met Azure AD. Over het algemeen zijn er twee methoden, waaronder Federatie-en aangepaste besturings elementen:

* **Identiteits Federatie** : wanneer Azure AD een verificatie aanvraag ontvangt, wordt de gebruiker door Azure AD omgeleid naar de federatieve id-provider voor verificatie. Bij een geslaagde verificatie stuurt de federatieve id-provider de gebruiker terug naar Azure AD, samen met een SAML-token. Om ervoor te zorgen dat Azure AD herkent dat de gebruiker de MFA-verificatie heeft voltooid bij het verifiëren van de federatieve id-provider, moet het SAML-token de *authenticationmethodsreferences* -claim (met de waarde *multipleauthn*) bevatten. Controleer of de provider voor federatieve identiteiten ondersteuning biedt voor het verlenen van een dergelijke claim. Als dit het geval is, controleert u of de federatieve id-provider hiervoor is geconfigureerd. Als de claim ontbreekt, weet Azure AD (en daarom is het partner centrum) niet dat de gebruiker de MFA-verificatie heeft voltooid en dat de claim ontbreekt, waardoor de metriek niet 100% is.

* **Aangepast besturings element** : aangepast Azure AD-besturings element kan niet worden gebruikt om te bepalen of een gebruiker de MFA-verificatie heeft voltooid via een MFA-oplossing van derden. Als gevolg hiervan wordt een gebruiker die MFA-verificatie via een aangepast besturings element heeft voltooid, altijd weer gegeven voor Azure AD (en in Partner Center), omdat de MFA-verificatie niet is voltooid. Als dat mogelijk is, kunt u het beste overschakelen naar het gebruik van identiteits Federatie in plaats van aangepast besturings element wanneer u integreert met Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Bepalen welke gebruikers zijn aangemeld bij partner centrum zonder MFA

Het kan handig zijn om te bepalen welke gebruikers zich aanmelden bij het partner centrum zonder MFA-verificatie en ze te verifiëren met uw huidige MFA-implementatie. U kunt het [aanmeldings rapport van Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) gebruiken om erachter te komen of een gebruiker de MFA-verificatie heeft voltooid of niet. Het aanmeldings rapport van Azure AD is momenteel alleen beschikbaar voor partners die zich hebben geabonneerd op Azure AD Premium of een O365-SKU, met inbegrip van Azure AD Premium (bijvoorbeeld EMS).

## <a name="next-steps"></a>Volgende stappen

- [Groeps Community voor de beveiligings richtlijnen van partner centrum](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Beveiligingsvereisten voor Partnercentrum](partner-security-requirements.md)
- [Veelgestelde vragen over beveiligings vereisten voor Partner Center](partner-security-requirements-faq.md)
