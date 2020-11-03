---
title: Status van partner beveiligings vereisten
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over de nieuwe verplichte vereisten voor betere beveiliging voor Advisor, leveranciers van het configuratie scherm en partners in het Cloud Solution Provider-programma.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b6c2d56a0747ddf2bd1a821886e371ed698a4a1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528528"
---
# <a name="partner-security-requirements-status---get-answers-and-check-reports-about-current-status"></a>Status van de partner beveiligings vereisten: antwoorden ophalen en rapporten over de huidige status controleren

**Van toepassing op**

- Alle partners in het Cloud Solution Provider-programma
  - Directe factuur
  - Indirecte provider
  - Indirecte wederverkoper
- Alle leveranciers van het configuratie scherm
- Alle Advisors

**Juiste gebruikers**
- Alle ingeschakelde gebruikers, inclusief gast gebruikers

Grotere veiligheids maatregelen en beveiliging zijn onder de meest voorkomende prioriteiten. We weten dat de beste verdediging voor komen en dat we alleen even sterk zijn als onze zwakste koppeling. Daarom hebben we iedereen in ons ecosysteem nodig om te reageren en om ervoor te zorgen dat de juiste beveiligings beveiligingen aanwezig zijn. Om partners en klanten te helpen beschermen, introduceren we een reeks verplichte beveiligings vereisten voor adviseurs, leveranciers van configuratie schermen en partners die deel nemen aan het Cloud Solution Provider-programma.

Vanaf 1 augustus 2019 zijn alle partners vereist voor het afdwingen van multi-factor Authentication voor alle gebruikers, inclusief service accounts, in hun partner Tenant. Lees vereisten voor de [beveiliging van partners](partner-security-requirements.md)voor meer informatie over de nieuwe beveiligings beleidsregels.

We willen er zeker van zijn dat elke gebruiker een MFA-uitdaging voor elke afzonderlijke verificatie heeft. Deze ervaring kan worden bereikt via een van de volgende manieren:

- Azure AD Premium implementeren om ervoor te zorgen dat MFA wordt afgedwongen voor elke gebruiker
- Implementatie van de [standaard instellingen voor Azure AD-beveiliging](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementatie van een oplossing van derden om ervoor te zorgen dat MFA wordt afgedwongen voor elke gebruiker

## <a name="partner-security-requirements-status"></a>Status van partner beveiligings vereisten

Met dit rapport kunt u de status van beveiligings vereisten controleren door een manier te bieden om te zien waar u zich ook bevindt. De tracering wordt regel matig bijgewerkt.

>[!NOTE]
>Het status rapport van de partner beveiligings vereisten wordt alleen ondersteund in het partner centrum. Het is niet beschikbaar in de Microsoft Cloud voor de Amerikaanse overheid of Microsoft Cloud Duitsland. We raden u ten zeerste aan dat alle partners die via een soevereine Cloud communiceren (21Vianet, Amerikaanse overheid en Duitsland), deze nieuwe beveiligings vereisten onmiddellijk aannemen. Deze partners zijn echter niet verplicht om te voldoen aan de nieuwe beveiligings vereisten met ingang van 1 augustus 2019. Micro soft geeft in de toekomst aanvullende informatie over de afdwinging van deze beveiligings vereisten voor soevereine Clouds.

## <a name="multi-factor-authentication-mfa-report"></a>Rapport multi-factor Authentication (MFA)

Het partner centrum MFA-rapport biedt inzicht in de partner MFA-implementatie door twee soorten metrische gegevens op te geven op basis van MFA-configuratie en partner Center-activiteiten van de CSP-Tenant: 

### <a name="mfa-configuration-on-a-csp-tenant"></a>MFA-configuratie op een CSP-Tenant

Deze metrische gegevens zijn gerelateerd aan de MFA-configuratie op een CSP-Tenant die dagelijks is vastgelegd en gerapporteerd. Hiermee wordt het percentage ingeschakelde gebruikers accounts met MFA afgedwongen met behulp van een van deze [MFA-opties](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). Bijvoorbeeld:

- Contoso is een CSP-partner met 110 gebruikers accounts in de Tenant, 10 van deze gebruikers accounts zijn uitgeschakeld. 
- Van de rest van 100 gebruikers accounts, 90 worden MFA afgedwongen met behulp van de meegeleverde [MFA-opties](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). De metriek toont daarom 90%. 

### <a name="partner-center-activities-with-mfa"></a>Partner Center-activiteiten met MFA

Telkens wanneer uw werk nemers zich aanmelden bij het partner centrum om te werken of, via Api's, gegevens ophalen of verzenden via het partner centrum, zijn de beveiligings status vraag en bijgehouden. Ook inbegrepen bij het bijhouden van de beveiligings status, zijn uw toepassingen en alle toepassingen van het configuratie scherm. De weer gegeven status geldt voor de afgelopen zeven dagen.

#### <a name="mfa-verification-completed-by-users"></a>MFA-verificatie voltooid door gebruikers

Deze metrische gegevens zijn gerelateerd aan activiteiten in het dash board van de partner centrum. Hiermee wordt het percentage van de bewerkingen gemeten die zijn gemaakt door gebruikers die MFA-verificatie hebben voltooid. Bijvoorbeeld:

- Contoso is een CSP-partner met twee beheerders agenten, Jeroen en John.
- Op de eerste dag heeft Jeroen aangemeld bij het Partner Center-dash board zonder MFA-verificatie en werden er drie bewerkingen uitgevoerd.
- Op de tweede dag is Jan aangemeld bij het Partner Center-dash board zonder MFA-verificatie en werden er vijf bewerkingen uitgevoerd.
- Op de derde dag heeft Jeroen aangemeld bij het Partner Center-dash board met MFA-verificatie en twee bewerkingen uitgevoerd.
- Er zijn voor de resterende vier dagen geen bewerkingen uitgevoerd door een van de agents.
- Van de tien verwerkingen die in het 7-dagen venster zijn gemaakt, werden er twee gedaan door de gebruiker met MFA-verificatie. De metriek toont daarom 20%.

Gebruik de aanvragen voor bestands **portals zonder MFA** om te begrijpen welke gebruiker zich heeft aangemeld bij het Partner Center-dash board zonder MFA-verificatie en de tijd van de laatste bezoek tijdens het rapportage venster.

#### <a name="appuser-authentication"></a>App + gebruikers authenticatie

Deze metriek is gerelateerd aan het gebruik van partner Center API-aanvragen die zijn gemaakt met behulp van app + gebruikers authenticatie. Hiermee wordt het percentage van API-aanvragen gemeten dat is gemaakt met behulp van een toegangs token met MFA-claim. Bijvoorbeeld:

- Fabrikam is een CSP-partner die een CSP-toepassing heeft die gebruikmaakt van een combi natie van app + gebruikers authenticatie en app-only-verificatie methoden.
- Op de eerste dag heeft de toepassing drie API-aanvragen gedaan, die werden ondersteund door een toegangs token dat is verkregen via de authenticatie methode voor apps en gebruikers zonder MFA-verificatie.
- Op de tweede dag hebben de toepassing vijf API-aanvragen uitgevoerd, die werden ondersteund door een toegangs token dat is verkregen met behulp van app-only-verificatie.
- Op de derde dag hebben de toepassing twee API-aanvragen gedaan, die werden ondersteund door een toegangs token dat is verkregen met behulp van app + gebruikers verificatie methode met MFA-verificatie.
- Er zijn voor de resterende vier dagen geen bewerkingen uitgevoerd door een van de agents.
- De vijf API-aanvragen op de tweede dag, die worden ondersteund door een toegangs token dat is verkregen via verificatie op basis van een app, worden wegge laten uit de metriek omdat het geen gebruik maakt van gebruikers referenties. Van de resterende vijf bewerkingen werden twee hiervan ondersteund door een toegangs token dat is verkregen met MFA-verificatie. De metriek toont daarom 40%.

Als u wilt weten welke app + gebruikers activiteiten resulteert in het niet-100% op deze metrische gegevens, gebruikt u bestanden:

- **Overzicht van API-aanvragen** om inzicht te krijgen in de algehele MFA-status per toepassing.
- **Alle API-aanvragen** om inzicht te krijgen in de details van de API-aanvragen van gebruikers van uw Tenant, is het resultaat beperkt tot maxi maal 10.000 meest recente aanvragen voor betere download ervaring.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>Wat moet ik doen als de metrische gegevens in het MFA-rapport niet 100% zijn

Het is mogelijk dat de metrische gegevens onder het Partner Center MFA-rapport niet 100% zijn voor partners die MFA hebben geïmplementeerd. Als u wilt weten waarom, moet u rekening houden met de volgende factoren.

> [!NOTE]
> U moet samen werken met iemand van uw organisatie die vertrouwd is met Identity Management en MFA-implementatie voor uw partner Tenant.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>Hebt u MFA geïmplementeerd voor uw partner-Tenant?

Als dat niet het geval is, moet u eerst MFA implementeren voor uw partner Tenant. Raadpleeg voor meer informatie over het implementeren van MFA de artikel [partner beveiligings vereiste](partner-security-requirements.md).

### <a name="have-you-only-recently-completed-mfa-implementation"></a>Hebt u alleen onlangs de MFA-implementatie voltooid?

De metrische gegevens worden dagelijks berekend en er wordt rekening gehouden met de bewerkingen die in de afgelopen zeven dagen worden uitgevoerd. Als u alleen de MFA-implementatie voor uw partner Tenant hebt voltooid, zijn de metrische gegevens mogelijk niet 100%.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>Zijn bepaalde gebruikers accounts uitgesloten van de MFA-implementatie?

Krijg inzicht in de huidige MFA-implementatie voor alle gebruikers accounts of alleen enkele. Sommige MFA-oplossingen zijn op beleid gebaseerde en ondersteunen gebruikers uitsluiting, terwijl anderen mogelijk verplicht zijn om MFA expliciet in te scha kelen op basis van per gebruiker. Controleer of u geen gebruikers hebt uitgesloten van uw huidige MFA-implementatie. Elk gebruikers account dat wordt uitgesloten en zich aanmeldt bij partner centrum voor het uitvoeren van een CSP-gerelateerde activiteit, kan de metrische gegevens niet 100%.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>Is MFA alleen vereist wanneer aan bepaalde voor waarden wordt voldaan?

Begrijp of uw huidige implementatie alleen MFA afdwingt onder specifieke voor waarden. Sommige MFA-oplossingen bieden flexibiliteit om alleen MFA af te dwingen wanneer aan bepaalde voor waarden wordt voldaan. Bijvoorbeeld: de gebruiker is toegang tot een onbekend apparaat of een onbekende locatie. Een gebruiker die is ingeschakeld voor MFA maar niet vereist is om MFA-verificatie te volt ooien bij het openen van het partner centrum, kan de metrische gegevens niet 100%.

>[!NOTE]
>Voor partners die MFA met de standaard instellingen van Azure AD-beveiliging hebben geïmplementeerd, is het belang rijk te weten dat voor niet-beheerders gebruikers accounts multi-factor Authentication wordt afgedwongen op basis van risico. Gebruikers wordt alleen om MFA gevraagd tijdens Risk ante pogingen (bijvoorbeeld wanneer de gebruiker zich vanaf een andere locatie aanmeldt). Daarnaast hebben gebruikers Maxi maal 14 dagen de tijd om te registreren voor MFA. Gebruikers die geen MFA-registratie hebben voltooid, worden tijdens de periode van 14 dagen niet voor MFA-verificatie gecontroleerd. Daarom is het mogelijk dat de metrische gegevens niet 100% zijn voor partners die MFA hebben geïmplementeerd met behulp van de standaard instellingen van Azure AD.

### <a name="are-you-using-third-party-mfa-solution"></a>Maakt u gebruik van een MFA-oplossing van derden?

Als u een MFA-oplossing van derden gebruikt, moet u bepalen hoe u deze integreert met Azure AD. Over het algemeen zijn er twee methoden, waaronder Federatie-en aangepaste besturings elementen:

* **Identiteits Federatie** : wanneer Azure AD een verificatie aanvraag ontvangt, wordt de gebruiker door Azure AD omgeleid naar de federatieve id-provider voor verificatie. Bij een geslaagde verificatie stuurt de federatieve id-provider de gebruiker terug naar Azure AD, samen met een SAML-token. Om ervoor te zorgen dat Azure AD herkent dat de gebruiker de MFA-verificatie heeft voltooid bij het verifiëren van de federatieve id-provider, moet het SAML-token de *authenticationmethodsreferences* -claim (met de waarde *multipleauthn* ) bevatten. Controleer of de provider voor federatieve identiteiten ondersteuning biedt voor het verlenen van een dergelijke claim. Als dit het geval is, controleert u of de federatieve id-provider hiervoor is geconfigureerd. Als de claim ontbreekt, weet Azure AD (en daarom is het partner centrum) niet dat de gebruiker de MFA-verificatie heeft voltooid en dat de claim ontbreekt, waardoor de metriek niet 100% is.

* **Aangepast besturings element** : aangepast Azure AD-besturings element kan niet worden gebruikt om te bepalen of een gebruiker de MFA-verificatie heeft voltooid via een MFA-oplossing van derden. Als gevolg hiervan wordt een gebruiker die MFA-verificatie via een aangepast besturings element heeft voltooid, altijd weer gegeven voor Azure AD (en in Partner Center), omdat de MFA-verificatie niet is voltooid. Als dat mogelijk is, kunt u het beste overschakelen naar het gebruik van identiteits Federatie in plaats van aangepast besturings element wanneer u integreert met Azure AD.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Identificeren welke gebruikers zich hebben aangemeld bij partner centrum zonder MFA

Het kan handig zijn om te bepalen welke gebruikers zich aanmelden bij het partner centrum zonder MFA-verificatie en ze te verifiëren met uw huidige MFA-implementatie. U kunt het [aanmeldings rapport van Azure AD](/azure/active-directory/reports-monitoring/concept-sign-ins) gebruiken om erachter te komen of een gebruiker de MFA-verificatie heeft voltooid of niet. Het aanmeldings rapport van Azure AD is momenteel alleen beschikbaar voor partners die zich hebben geabonneerd op Azure AD Premium of een O365-SKU, met inbegrip van Azure AD Premium (bijvoorbeeld EMS).

## <a name="next-steps"></a>Volgende stappen

- [Groeps Community voor de beveiligings richtlijnen van partner centrum](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Beveiligings vereisten voor Partner Center](partner-security-requirements.md)
- [Veelgestelde vragen over beveiligings vereisten voor Partner Center](partner-security-requirements-faq.md)