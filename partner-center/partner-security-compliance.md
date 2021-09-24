---
title: Statusrapport van beveiligingsvereisten
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Meer informatie over het controleren van de naleving van uw beveiligingsvereisten met het statusrapport van de beveiligingsvereisten en Partner Center MFA-rapport
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 7f28f6333542fb1a2f11b9cc48c00777f1977c1a
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/24/2021
ms.locfileid: "128366047"
---
# <a name="security-requirements-status-report"></a>Statusrapport van beveiligingsvereisten

**Juiste rollen:** CPV-| Globale beheerder

In dit artikel wordt het statusrapport van de beveiligingsvereisten in Partner Center. Dit rapport bevat metrische gegevens over naleving [van de beveiligingsvereisten van](partner-security-requirements.md) partners voor meervoudige verificatie (MFA) voor gebruikers in uw partner-tenant.

Voor toegang tot dit rapport in [Partner Center](https://partner.microsoft.com/dashboard)gaat u **naar Instellingen**  >  **Accountinstellingen**  >  **Beveiligingsvereisten.** Het rapport wordt dagelijks bijgewerkt en geeft aanmeldingsgegevens van de afgelopen zeven dagen weer.

>[!NOTE]
>Het statusrapport van de beveiligingsvereisten wordt alleen ondersteund in Partner Center. Het is niet beschikbaar in de Microsoft Cloud for US Government of Microsoft Cloud Duitsland. We raden u ten zeerste aan dat alle partners die via een soevereine cloud (Amerikaanse overheid en Duitsland) werken, onmiddellijk aan deze nieuwe beveiligingsvereisten voldoen. Deze partners zijn momenteel echter niet vereist om te voldoen aan de nieuwe beveiligingsvereisten. Microsoft geeft in de toekomst aanvullende informatie over het afdwingen van deze beveiligingsvereisten voor onafhankelijke clouds.

## <a name="security-status-metrics"></a>Metrische gegevens over de beveiligingsstatus

Het statusrapport van de beveiligingsvereisten biedt inzicht in de implementatie van MFA van partners en biedt metrische gegevens over MFA-configuratie en Partner Center activiteiten op partnerten tenants. In de volgende secties worden deze metrische gegevens gedetailleerder uitgelegd.

### <a name="mfa-configuration-on-a-partner-tenant"></a>MFA-configuratie op een partner-tenant

Het metrische percentage ingeschakelde gebruikersaccounts met MFA dat wordt afgedwongen met behulp van de hier vermelde **opties:** toont het percentage ingeschakelde gebruikersaccounts op uw partner-tenant dat MFA heeft afgedwongen. U kunt een van deze [MFA-opties gebruiken om naleving](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) te bereiken. Deze gegevens worden dagelijks vastgelegd en gerapporteerd. Bijvoorbeeld:

- Contoso is een CSP-partner met 110 gebruikersaccounts in de tenant. 10 van deze gebruikersaccounts zijn uitgeschakeld. 
- Van de overige 100 gebruikersaccounts worden 90 afgedwongen MFA met behulp van de opgegeven [MFA-opties](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started). De metrische gegevens tonen daarom 90%. 

### <a name="partner-center-requests-with-mfa"></a>Partner Center aanvragen met MFA

Telkens wanneer uw werknemers zich aanmelden bij Partner Center om te werken of, via API's, gegevens op te halen of te verzenden via Partner Center, wordt hun beveiligingsstatus op de proef gesteld en bij te houden. Ook zijn uw toepassingen en toepassingen van configuratieschermleveranciers opgenomen in het bijhouden van beveiligingsstatussen. Deze gegevens worden weergegeven in metrische gegevens onder Percentage aanvragen voor **Partner Center met MFA** en weerspiegelt de afgelopen zeven dagen.

#### <a name="dashboard-mfa-verification"></a>MFA-verificatie op dashboard

De metrische **gegevens via Partner Center-portal** zijn gerelateerd aan activiteiten in Partner Center dashboard. Het meet het percentage bewerkingen dat is uitgevoerd door gebruikers die de MFA-verificatie hebben voltooid. Bijvoorbeeld:

- Contoso is een CSP-partner met twee beheerdersagents, Jane en John.
- Op de eerste dag heeft Jane zich aangemeld bij het Partner Center zonder MFA-verificatie en drie bewerkingen uitgevoerd.
- Op de tweede dag heeft John zich aangemeld bij Partner Center dashboard zonder MFA-verificatie en vijf bewerkingen uitgevoerd.
- Op de derde dag heeft Jane zich aangemeld bij het Partner Center dashboard met MFA-verificatie en twee bewerkingen uitgevoerd.
- Er zijn geen bewerkingen uitgevoerd door een van beide agent op de resterende vier dagen.
- Van de tien bewerkingen die in het tijdvenster van zeven dagen zijn uitgevoerd, zijn er twee uitgevoerd door de gebruiker met MFA-verificatie. Daarom toont het metrische gegevens 20%.

Gebruik het bestand **Portal-aanvragen** zonder MFA om te begrijpen welke gebruiker zich heeft aangemeld bij Partner Center dashboard zonder MFA-verificatie en de tijd van het laatste bezoek tijdens het rapportagevenster.

#### <a name="appuser-mfa-verification"></a>MFA-verificatie voor app en gebruiker

De metrische gegevens **via API of SDK** zijn gerelateerd aan App+User-verificatie via Partner Center API-aanvragen. Het meet het percentage API-aanvragen dat is gedaan met behulp van een toegangs token met MFA-claim. Bijvoorbeeld:

- Fabrikam is een CSP-partner en heeft een CSP-toepassing die gebruikmaakt van een combinatie van App+User-verificatie en verificatiemethoden voor alleen apps.
- Op de eerste dag heeft de toepassing drie API-aanvragen gedaan, die werden geback-token dat is verkregen via de verificatiemethode App+User zonder MFA-verificatie.
- Op de tweede dag heeft de toepassing vijf API-aanvragen gedaan, die werden gebacked door een toegangs token dat is verkregen met behulp van verificatie alleen voor apps.
- Op de derde dag heeft de toepassing twee API-aanvragen gedaan, die werden geback-token dat is verkregen met behulp van de verificatiemethode App+User met MFA-verificatie.
- Er zijn geen bewerkingen uitgevoerd door een van beide agent op de resterende vier dagen.
- De vijf API-aanvragen op de tweede dag, die werden gebacked door een toegangsken dat is verkregen via alleen-app-verificatie, worden weggelaten uit de metrische gegevens omdat deze geen gebruikmaakt van gebruikersreferenties. Van de resterende vijf bewerkingen werden twee van deze twee back-outs gemaakt door een toegangs token dat is verkregen met MFA-verificatie. De metrische gegevens tonen daarom 40%.

Als u wilt weten welke app- en gebruikersactiviteiten leiden tot de niet-100% voor deze metrische gegevens, gebruikt u bestanden:

- **Samenvatting van API-aanvragen** om inzicht te krijgen in de algehele MFA-status per toepassing.
- **Alle API-aanvragen** om inzicht te krijgen in de details van elke API-aanvraag van gebruikers van uw tenant. Het resultaat is beperkt tot maximaal 10.000 meest recente aanvragen voor een betere downloadervaring.

## <a name="actions-for-mfa-status-below-100"></a>Acties voor de MFA-status lager dan 100%

Sommige partners die MFA hebben geïmplementeerd, zien mogelijk metrische rapportgegevens onder de 100%. Om te begrijpen waarom, zijn hier enkele factoren om rekening mee te houden.

> [!NOTE]
> U moet samenwerken met iemand uit uw organisatie die bekend is met identiteitsbeheer en MFA-implementatie voor uw partner-tenant.

### <a name="implemented-mfa-for-your-partner-tenant"></a>MFA geïmplementeerd voor uw partner-tenant

U moet MFA implementeren voor uw partner-tenant om naleving te bereiken. Zie Security requirements for using Partner Center or Partner Center APIs (Beveiligingsvereisten voor het gebruik van Partner Center- of [Partner Center-API's) voor](partner-security-requirements.md)meer informatie over het implementeren van MFA.

>[!NOTE]
> Metrische MFA-gegevens worden dagelijks berekend en houden rekening met bewerkingen die in de afgelopen zeven dagen zijn uitgevoerd. Als u de MFA-implementatie voor uw partner-tenant pas onlangs hebt voltooid, geven de metrische gegevens mogelijk nog geen 100% weer.

### <a name="verify-mfa-on-all-user-accounts"></a>MFA controleren op alle gebruikersaccounts

Begrijpen of uw huidige MFA-implementatie alle gebruikersaccounts of slechts enkele omvat. Sommige MFA-oplossingen zijn op beleid gebaseerd en bieden ondersteuning voor gebruikersuitsluiting, terwijl u voor andere oplossingen mogelijk per gebruiker expliciet MFA moet inschakelen. Controleer of u geen enkele gebruiker hebt uitgesloten van uw huidige MFA-implementatie. Elk gebruikersaccount dat is uitgesloten en zich aanmeldt bij Partner Center om CSP-, CPV- of Advisor-gerelateerde activiteiten uit te voeren, kan ertoe leiden dat de metrische gegevens niet 100% zijn.

### <a name="review-your-mfa-conditions"></a>Uw MFA-voorwaarden controleren

Begrijpen of uw huidige implementatie alleen MFA onder specifieke voorwaarden afdwingt. Sommige MFA-oplossingen bieden flexibiliteit om MFA alleen af te dwingen wanneer aan bepaalde voorwaarden wordt voldaan. De gebruiker heeft bijvoorbeeld toegang vanaf een onbekend apparaat of een onbekende locatie. Een gebruiker die is ingeschakeld voor MFA, maar geen MFA-verificatie hoeft te voltooien bij het openen van Partner Center, kan ertoe leiden dat de metrische gegevens niet 100% zijn.

>[!NOTE]
>Voor partners die MFA hebben geïmplementeerd met standaardinstellingen voor Azure AD-beveiliging, is het belangrijk te weten dat voor niet-beheerdersgebruikersaccounts meervoudige verificatie wordt afgedwongen op basis van risico. Gebruikers wordt alleen tijdens riskante aanmeldingspogingen om MFA gevraagd (bijvoorbeeld wanneer de gebruiker zich aanmeldt vanaf een andere locatie). Bovendien hebben gebruikers maximaal 14 dagen de tijd om zich te registreren voor MFA. Gebruikers die de MFA-registratie niet hebben voltooid, worden niet om MFA-verificatie tijdens de periode van 14 dagen gesteld. Daarom wordt verwacht dat de metrische gegevens mogelijk niet 100% zijn voor partners die MFA hebben geïmplementeerd met de standaardinstellingen voor Azure AD-beveiliging.

### <a name="review-third-party-mfa-configurations"></a>MFA-configuraties van derden controleren

Als u een MFA-oplossing van derden gebruikt, moet u bepalen hoe u deze integreert met Azure AD. Over het algemeen zijn er twee methoden, waaronder federatie en aangepaste besturingselementen:

* **Identiteitsfederatie:** wanneer Azure AD een verificatieaanvraag ontvangt, leidt Azure AD de gebruiker om naar de federatief-id-provider voor verificatie. Als de verificatie is geslaagd, stuurt de federatief-id-provider de gebruiker terug naar Azure AD, samen met een SAML-token. Het SAML-token moet de claim *authenticationmethodsreferences* (met de waarde *multipleauthn)* bevatten om ervoor te zorgen dat Azure AD kan herkennen dat de gebruiker de MFA-verificatie heeft voltooid bij het verifiëren bij de federatieve id-provider. Controleer of de federatief-id-provider de uitgifte van een dergelijke claim ondersteunt. Zo ja, controleer dan of de federatief-id-provider is geconfigureerd om dit te doen. Als de claim ontbreekt, weet Azure AD (en daarom Partner Center) niet dat de gebruiker de MFA-verificatie heeft voltooid en dat het ontbreken van de claim ertoe kan leiden dat de metrische gegevens niet 100% zijn.

* **Aangepast beheer:** aangepast beheer van Azure AD kan niet worden gebruikt om te bepalen of een gebruiker de MFA-verificatie heeft voltooid via een MFA-oplossing van derden. Als gevolg hiervan wordt elke gebruiker die de verificatie van MFA via een aangepast besturingselement heeft voltooid, altijd weergegeven in Azure AD (en op zijn beurt Partner Center) dat de MFA-verificatie niet is voltooid. Waar mogelijk wordt u aangeraden over te schakelen naar identiteitsfederatie in plaats van Aangepast besturingselement wanneer u integreert met Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Bepalen welke gebruikers zich hebben aangemeld bij Partner Center zonder MFA

Het kan handig zijn om te bepalen welke gebruikers zich aanmelden bij Partner Center zonder MFA-verificatie en deze te verifiëren met uw huidige MFA-implementatie. U kunt het [aanmeldingsrapport van Azure AD gebruiken om](/azure/active-directory/reports-monitoring/concept-sign-ins) erachter te komen of een gebruiker de MFA-verificatie al dan niet heeft voltooid. Azure AD-aanmeldingsrapport is momenteel alleen beschikbaar voor partners die zich hebben geabonneerd op Azure AD Premium of een O365-SKU, waaronder Azure AD Premium (bijvoorbeeld EMS).

## <a name="next-steps"></a>Volgende stappen

- [Partner Center community van beveiligingsadviesgroep](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Beveiligingsvereisten voor Partnercentrum](partner-security-requirements.md)
- [Partner Center veelgestelde vragen over beveiligingsvereisten](partner-security-requirements-faq.yml)
