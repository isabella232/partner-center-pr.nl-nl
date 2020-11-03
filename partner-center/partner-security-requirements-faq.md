---
title: Veelgestelde vragen over beveiligings vereisten voor partners
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Veelgestelde vragen over de beveiligings vereisten van de partner: wat het zijn, hoe partners ze moeten implementeren en hoe u weet of u eraan hebt voldaan.'
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f60b6e2624bd4f9020181a936842bdb46db8aa9
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133045"
---
# <a name="common-questions-about-partner-security-requirements"></a>Veelgestelde vragen over de beveiligings vereisten van partners

**Van toepassing op**

- Partnercentrum

**Juiste gebruikers**

- Alle ingeschakelde gebruikers, inclusief gast gebruikers


In dit artikel vindt u antwoorden op enkele veelgestelde vragen over de [beveiligings vereisten](partner-security-requirements.md)van de partner.

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Wat zijn de beveiligings vereisten van de partner en waarom moeten partners deze implementeren?

Meer en voortdurende beveiligings-en privacy-veiligheids maatregelen zijn te vinden op onze belangrijkste prioriteiten en we blijven onze klanten en tenants helpen beveiligen. We blijven een geavanceerder en uitgebreid aantal beveiligings aanvallen zien, voornamelijk gerelateerd aan incidenten met betrekking tot identiteits inbreuken. Als preventieve controles een belang rijke rol spelen in een algemene verdedigings strategie om beveiligings aanvallen te tegen gaan, hebben we [verplichte beveiligings vereisten](partner-security-requirements.md) geïntroduceerd in 2019. Alle partners die deel nemen aan het programma Cloud Solution Provider (CSP), leveranciers van het configuratie scherm en Advisor, moeten de vereisten implementeren om te blijven voldoen aan het beleid.

### <a name="what-are-the-key-timelines-and-milestones"></a>Wat zijn de belangrijkste tijd lijnen en mijl palen?

De voor waarden die zijn gekoppeld aan deze beveiligings vereisten, waaronder tijd lijnen en mijl palen, zijn opgenomen in de [micro soft-partner overeenkomst](microsoft-partner-agreement.md). U moet deze beveiligings vereisten zo snel mogelijk implementeren om te blijven voldoen aan uw deelname aan het CSP-programma.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Wat gebeurt er als de beveiligings vereisten van de partner niet worden geïmplementeerd?

Voor de micro soft-partner overeenkomst moet u multi-factor Authentication afdwingen voor gebruikers accounts en het veilige toepassings model voor interactie met de Partner Center API aannemen. 

Partners die zich niet houden aan deze beveiligings procedures, kunnen de mogelijkheid tot het maken van een Transact in het cryptografie programma of het beheren van de tenants van klanten met gedelegeerde beheerders rechten kwijt raken.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Zijn de beveiligings vereisten van toepassing op alle geographs?

Ja, de beveiligings vereisten zijn van toepassing op alle geographs. We raden u ten zeerste aan alle partners door middel van een soevereine Cloud (Amerikaanse overheid en Duitsland) te handelen en deze nieuwe beveiligings vereisten onmiddellijk aan te nemen. Deze partners zijn momenteel echter niet vereist om te voldoen aan de beveiligings vereisten. Micro soft geeft in de toekomst aanvullende informatie over de afdwinging van deze beveiligings vereisten voor soevereine Clouds.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Is het mogelijk een uitsluiting voor een account te krijgen?

Nee, het is niet mogelijk om een gebruikers account uit te sluiten van de vereiste voor het afdwingen van multi-factor Authentication (MFA). Gezien de zeer beschermde aard van een partner, vereist de micro soft-partner overeenkomst dat multi-factor Authentication wordt afgedwongen voor elk gebruikers account in uw partner Tenant.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Hoe kan ik weet ik of ik aan de beveiligings vereisten van de partner heb voldaan?

U moet de volgende stappen uitvoeren:

- U moet voldoen aan alle vereisten die worden beschreven in de [beveiligings vereisten](partner-security-requirements.md)van de partner.
- U moet ervoor zorgen dat alle gebruikers accounts in uw partner-Tenant multi-factor Authentication hebben afgedwongen.

Om u te helpen bij het identificeren van de belangrijkste gebieden waar u acties kunt ondernemen, bieden we het [status rapport voor beveiligings vereisten](https://partner.microsoft.com/commerce/security/compliance) dat beschikbaar is via partner centrum.

Zie de status van de [partner beveiligings vereisten](partner-security-compliance.md) voor meer informatie over het status rapport.

## <a name="required-actions"></a>Vereiste acties

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Wat zijn de belangrijkste acties die ik moet uitvoeren om aan de vereisten te voldoen?

Alle partners in het CSP-programma (directe factuur, indirecte provider en indirecte wederverkoper), adviseurs en de leveranciers van het configuratie scherm moeten voldoen aan de vereisten.

1. **MFA afdwingen voor alle gebruikers**

    Alle partners in het CSP-programma, de Advisor en de leveranciers van het configuratie scherm zijn verplicht MFA af te dwingen voor alle gebruikers in hun partner Tenant.

    Aanvullende overwegingen:

    - Indirecte providers moeten samen werken met indirecte wederverkopers om het partner centrum uit te kunnen voeren als ze dit nog niet hebben gedaan en hun wederverkopers aanmoedigen om te voldoen aan de vereisten.
    - Azure MFA wordt voor alle gebruikers in de partner-Tenant gratis beschikbaar gesteld via de standaard instellingen van Azure AD-beveiliging met de enige verificatie methode van een verificator-toepassing die ondersteuning biedt voor eenmalige wacht woorden (mobiele TOTP).
    - Aanvullende verificatie methoden zijn beschikbaar via de [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) sku's, als andere methoden zoals een telefoon gesprek of SMS-bericht vereist zijn.
    - Partners kunnen ook gebruikmaken van een MFA-oplossing van derden voor elk account bij het openen van micro soft-commerciële Cloud Services.

2. **Het Framework van het veilige toepassings model aannemen**

    Alle partners die aangepaste integratie hebben ontwikkeld met behulp van Api's (zoals Azure Resource Manager, Microsoft Graph, Partner Center-API enzovoort) of aangepaste automatisering met hulpprogram ma's van Power shell, moeten het [beveiligde Application model-Framework](/partner-center/develop/enable-secure-app-model) aannemen om te integreren met micro soft-Cloud Services. Als u dit niet doet, kan dit leiden tot een onderbreking vanwege een MFA-implementatie. De volgende bronnen bevatten een overzicht en richt lijnen voor het aannemen van het model.

    - [Overzicht van veilig toepassings model](/partner-center/develop/enable-secure-app-model)
    - [Partner centrum: hand leiding voor beveiligde toepassings modellen](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partners in het CSP-programma: .NET-voorbeeld code voor het inschakelen van een veilig toepassings model](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partners in het CSP-programma: Java-voorbeeld code voor het inschakelen van een veilig toepassings model](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Verificatie document van partner centrum](/partner-center/develop/partner-center-authentication)
    - [Document Power shell Multi-Factor Authentication (MFA) van partner Center](/powershell/partnercenter/multi-factor-auth)

    Neem contact op met de leverancier als u een configuratie scherm gebruikt met betrekking tot de goed keuring van het Framework van het veilige toepassings model.

    Leveranciers van het configuratie scherm zijn vereist voor de [onboarding](enroll-as-cpv.md) van het partner centrum als leverancier van het configuratie scherm en beginnen de implementatie van deze vereiste onmiddellijk te starten. Raadpleeg het [partner centrum: Secure Application model-Framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Leveranciers van het configuratie scherm moeten de toestemming van de CSP-partners accepteren en beheren in plaats van referenties en alle bestaande referenties van de CSP-partners opschonen.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-multi-factor-authentication-mfa"></a>Wat is multi-factor Authentication (MFA)?

MFA is een beveiligings mechanisme, waarbij individuen worden geverifieerd via meer dan één vereiste beveiligings-en validerings procedure. Het werkt met twee of meer van de volgende verificatie methoden:

- Iets dat u kent (doorgaans een wacht woord)
- Iets dat u hebt (een vertrouwd apparaat dat niet eenvoudig kan worden gedupliceerd, zoals een telefoon)
- Iets dat u bent (biometrie)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Wat zijn de kosten voor het inschakelen van MFA?

Micro soft biedt geen kosten voor MFA via de implementatie van Azure AD-beveiligings standaards. De enige verificatie optie die beschikbaar is via deze versie van MFA is een verificator-toepassing. Als een telefoon gesprek of SMS-bericht vereist is, moet een [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) licentie worden aangeschaft. U kunt ook een oplossing van derden gebruiken om MFA te bieden voor elke gebruiker in uw partner-Tenant. in dit geval is het uw verantwoordelijkheid om ervoor te zorgen dat uw MFA-oplossing wordt afgedwongen en dat u compatibel bent.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Welke acties moet ik ondernemen als ik al een MFA-oplossing heb?

Door deze beveiligings vereisten worden gebruikers in een partner-Tenant verplicht om te verifiëren met behulp van MFA bij het openen van micro soft-commerciële Cloud Services. Oplossingen van derden kunnen worden gebruikt om aan deze vereisten te voldoen. Micro soft biedt geen validatie tests meer voor onafhankelijke ID-providers voor compatibiliteit met Azure Active Directory. Raadpleeg deze [richt lijnen](https://www.microsoft.com/download/details.aspx?id=56843)om uw product te testen op interoperabiliteit.

> [!IMPORTANT]
> Wanneer u een oplossing van derden gebruikt, is het belang rijk om te controleren of de oplossing de naam van de verificatie methode Reference (AMR), die de MFA-waarde bevat, afgeeft. Zie [de vereisten voor de beveiliging van partners testen](/powershell/partnercenter/test-partner-security-requirements) voor meer informatie over hoe het valideren van de oplossing van derden de verwachte claim afgeeft.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Ik gebruik meerdere partner-tenants voor Transact. Moet ik MFA allemaal implementeren?

Ja, u moet MFA afdwingen voor elke Azure Active Directory Tenant die is gekoppeld aan het CSP-programma of het Advisor-programma. Als u een Azure Active Directory Premium licentie wilt aanschaffen, moet u een Azure Active Directory licentie voor de gebruikers in elke Azure Active Directory Tenant aanschaffen. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Moet voor elk gebruikers account in mijn partner-Tenant MFA worden afgedwongen?

Ja, voor elke gebruiker moet MFA worden afgedwongen. Als u echter de standaard instellingen van Azure AD gebruikt, is er geen aanvullende actie vereist omdat deze functie MFA afdwingt voor alle gebruikers accounts. Het inschakelen van standaard instellingen voor beveiliging is een gratis en eenvoudige manier om ervoor te zorgen dat uw gebruikers accounts MFA-compatibel zijn en niet worden beïnvloed als MFA wordt afgedwongen.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Ik ben een directe factuur partner met micro soft. Wat moet ik doen?

Partners van de partner oplossing voor direct factureren moeten MFA afdwingen voor elke gebruiker in de Tenant.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Ik ben een indirecte wederverkoper en alleen met Transact als distributeur. Moet ik MFA nog steeds inschakelen?

Alle indirecte wederverkopers zijn vereist voor het afdwingen van MFA voor elke gebruiker in hun partner Tenant. De indirecte wederverkoper moet MFA inschakelen.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Ik gebruik de partner centrum-API niet. Moet ik MFA nog steeds implementeren?

Ja, deze beveiligings vereiste geldt voor alle gebruikers, waaronder gebruikers van de partner beheerder en eind gebruikers in een partner Tenant.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Welke leveranciers van derden bieden MFA-oplossingen die compatibel zijn met Azure Active Directory?

Bij het controleren van de leveranciers en oplossingen van MFA, moeten partners ervoor zorgen dat de door hen gekozen oplossing compatibel is met Azure Active Directory.

Micro soft biedt geen validatie tests meer voor onafhankelijke ID-providers voor compatibiliteit met Azure Active Directory. Als u uw product wilt testen op interoperabiliteit, raadpleegt u deze [richt lijnen](https://www.microsoft.com/download/details.aspx?id=56843).

Zie de [Azure AD Federation-compatibiliteits lijst](/azure/active-directory/hybrid/how-to-connect-fed-compatibility)voor meer informatie.

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Hoe kan ik MFA testen in onze integratie sandbox?

De functie voor het standaard beveiligingsniveau van Azure AD moet worden ingeschakeld of u kunt ook gebruikmaken van een oplossing van derden die gebruikmaakt van Federatie.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Schakelt MFA in op de manier waarop ik met de Tenant van mijn klant Communiceer?

Nee. Het afhandelen van deze beveiligings vereisten heeft geen invloed op hoe u uw klanten beheert. De mogelijkheid om gedelegeerde beheer bewerkingen uit te voeren wordt niet onderbroken.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Zijn mijn klanten onderworpen aan de beveiligings vereisten van de partner?

Nee, het is niet vereist dat u MFA afdwingt voor elke gebruiker in de Azure AD-tenants van uw klant. Het is echter raadzaam om met elke klant te werken om te bepalen hoe de gebruikers het beste kunnen beveiligen.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Kan elke gebruiker worden uitgesloten van de MFA-vereiste?

Nee, elke gebruiker, inclusief service accounts, in uw partner Tenant is vereist voor verificatie met MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Zijn de beveiligings vereisten voor de partner van toepassing op de integratie sandbox?

Ja, de beveiligings vereisten voor de partner zijn van toepassing op de integratie sandbox. Dit betekent dat u de juiste MFA-oplossing moet implementeren voor gebruikers in de sandbox-Tenant van de integratie. Het is raadzaam om de standaard instellingen van Azure AD-beveiliging te implementeren om MFA te bieden.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Hoe kan ik een account voor nood toegang (afbreek glas) configureren?

Het wordt beschouwd als een best practice om een of twee accounts voor toegang tot een nood geval te maken om te voor komen dat uw Azure AD-Tenant per ongeluk wordt vergrendeld. Met betrekking tot de beveiligings vereisten van de partner moet elke gebruiker worden geverifieerd met MFA. Dit betekent dat u de definitie van een account voor nood toegang moet aanpassen. Dit kan een account zijn dat gebruikmaakt van een oplossing van derden voor MFA.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Is Active Directory Federation Service (ADFS) vereist als ik een oplossing van derden gebruik?

Nee, het is niet nodig om Active Directory Federation Service (ADFS) te hebben als u een oplossing van derden gebruikt. Het is raadzaam om te werken met de leverancier van de oplossing om te bepalen wat de vereisten zijn voor de oplossing.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Is het een vereiste om de standaard instellingen van Azure AD-beveiliging in te scha kelen?

Nee, het is niet vereist dat u de standaard instellingen voor Azure AD-beveiliging inschakelt.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Kan voorwaardelijke toegang worden gebruikt om te voldoen aan de MFA-vereiste?

Ja, u kunt voorwaardelijke toegang gebruiken om MFA af te dwingen voor elke gebruiker, inclusief service accounts, in uw partner Tenant. Gezien de zeer bevoegde aard van een partner moeten we er echter voor zorgen dat elke gebruiker een MFA-uitdaging voor elke afzonderlijke verificatie heeft. Dit betekent dat u geen gebruik kunt maken van de functie van voorwaardelijke toegang die de vereiste voor MFA omzeilt.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Wordt het service account dat wordt gebruikt door Azure AD Connect van invloed op de beveiligings vereisten van de partner?

Nee, het service account dat door Azure AD Connect wordt gebruikt, heeft geen invloed op de beveiligings vereisten van de partner. Als u een probleem ondervindt met Azure AD Connect als gevolg van het afdwingen van MFA, opent u een aanvraag voor technische ondersteuning met micro soft ondersteuning.

## <a name="secure-application-model"></a>Model voor beveiligde toepassing

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Wie moet het beveiligde toepassings model aannemen om te voldoen aan de vereisten?

Micro soft introduceert een veilig, schaalbaar Framework voor het verifiëren van de CSP-partners (Cloud Solution Provider) en leveranciers (CPV) van het configuratie scherm die gebruikmaken van Multi-Factor Authentication. Raadpleeg de [hand leiding voor het beveiligde toepassings model](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) voor meer informatie. Alle partners die aangepaste integratie hebben ontwikkeld met behulp van Api's (zoals Azure Resource Manager, Microsoft Graph, Partner Center-API enzovoort) of aangepaste automatisering met hulpprogram ma's van Power shell, moeten het [beveiligde Application model-Framework](/partner-center/develop/enable-secure-app-model) aannemen om te integreren met micro soft-Cloud Services.

### <a name="what-is-the-secure-application-model"></a>Wat is het beveiligde toepassings model?

Micro soft introduceert een veilig, schaalbaar Framework voor het verifiëren van de CSP-partners (Cloud Solution Provider) en leveranciers (CPV) van het configuratie scherm die gebruikmaken van Multi-Factor Authentication. Raadpleeg de [hand leiding voor het beveiligde toepassings model](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) voor meer informatie.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Hoe kan ik het beveiligde toepassings model implementeren?

Alle partners die aangepaste integratie hebben ontwikkeld met behulp van Api's (zoals Azure Resource Manager, Microsoft Graph, Partner Center-API enzovoort) of aangepaste automatisering met hulpprogram ma's van Power shell, moeten het [beveiligde Application model-Framework](/partner-center/develop/enable-secure-app-model) aannemen om te integreren met micro soft-Cloud Services. Als u dit niet doet, kan dit leiden tot een onderbreking vanwege een MFA-implementatie. De volgende bronnen bevatten een overzicht en richt lijnen voor het aannemen van het model.

- [Overzicht van veilig toepassings model](/partner-center/develop/enable-secure-app-model)
- [Partner centrum: hand leiding voor beveiligde toepassings modellen](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partners in het CSP-programma: .NET-voorbeeld code voor het inschakelen van een veilig toepassings model](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partners in het CSP-programma: Java-voorbeeld code voor het inschakelen van een veilig toepassings model](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Verificatie document van partner centrum](/partner-center/develop/partner-center-authentication)
- [Document Power shell Multi-Factor Authentication (MFA) van partner Center](/powershell/partnercenter/multi-factor-auth)

Als u een configuratie scherm gebruikt, moet u contact opnemen met de leverancier over de acceptatie van het Framework van het veilige toepassings model.

Leveranciers van het configuratie scherm zijn vereist voor de [onboarding](enroll-as-cpv.md) van het partner centrum als leverancier van het configuratie scherm en beginnen de implementatie van deze vereiste onmiddellijk te starten. Raadpleeg het [partner centrum: Secure Application model-Framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Leveranciers van het configuratie scherm moeten de toestemming van de CSP-partners accepteren en beheren in plaats van referenties en alle bestaande referenties van de CSP-partners opschonen.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Moet het beveiligde toepassings model alleen worden geïmplementeerd voor de Partner Center API/SDK?

Door multi-factor Authentication af te dwingen voor alle gebruikers accounts, worden alle automatisering of integratie die is bedoeld om niet-interactief te worden uitgevoerd, beïnvloed. Hoewel de vereisten voor de beveiliging van de partner vereisen dat u het beveiligde toepassings model voor de Partner Center-API inschakelt, kan dit worden gebruikt om te voldoen aan de behoefte aan een tweede factor van verificatie met automatisering en integratie.

>[!Note] 
>Bronnen die worden geopend, moeten authenticatie op basis van toegangs tokens ondersteunen.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Ik gebruik automatiserings Programma's zoals Power shell. Hoe kan ik het beveiligde toepassings model implementeren?

U moet het beveiligde toepassings model implementeren als uw automatisering is bedoeld om niet-interactief te worden uitgevoerd en afhankelijk van de gebruikers referenties voor authenticatie. Zie [veilig toepassings model | Partner Center Power shell](/powershell/partnercenter/multi-factor-auth) voor hulp bij het implementeren van dit framework.  

>[!Note] 
>Niet alle Automation-hulpprogram ma's bieden de mogelijkheid om te verifiëren met behulp van toegangs tokens. Plaats een bericht in de groep met [beveiligings richtlijnen van partner centrum](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) als u hulp nodig hebt bij het weten welke wijzigingen moeten worden aangebracht. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Welke gebruikers referenties moet de toepassings beheerder geven bij het uitvoeren van het toestemming proces?

Het is raadzaam een service account te gebruiken waaraan de minimale privileged permissions zijn toegewezen. Met betrekking tot de Partner Center-API moet u een account gebruiken dat is toegewezen aan de rol verkoop agent of beheerder agent.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Waarom moet de toepassings beheerder geen globale referenties voor beheerders gebruikers opgeven wanneer zij het toestemming proces uitvoeren?

Het is een best practice om de identiteit met een minst privilege te gebruiken.  Dit vermindert het risico. Het is niet raadzaam een account te gebruiken dat globale beheerders bevoegdheden heeft, omdat dat meer machtigingen zou bieden dan nodig is.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Ik ben een CSP-partner. Hoe kan ik weet of de leverancier van het configuratie scherm (CPV) werkt voor het implementeren van de oplossing of niet?

Voor partners die gebruikmaken van een CPV-oplossing (configuratie scherm) naar Transact in het programma Cloud Solution Provider (CSP), is het uw verantwoordelijkheid om met uw CPV te raadplegen.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Wie is een leverancier van het configuratie scherm (CPV)?

Een leverancier van het configuratie scherm is een onafhankelijke software leverancier die apps ontwikkelt voor gebruik door CSP-partners om te integreren met partner Center-Api's. Een leverancier van het configuratie scherm is geen CSP-partner met directe toegang tot het dash board of Api's van de Partner Center. In het partner centrum is een gedetailleerde beschrijving beschikbaar [: Secure Applications model Guide (Engelstalig](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Ik ben een CPV. Hoe kan ik inschrijven?

Als u zich wilt inschrijven als leverancier van het configuratie scherm (CPV), volgt u de richt lijnen die [hier](enroll-as-cpv.md)worden beschreven.

CPVs moet contact opnemen met [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) om de inschrijvings koppeling te ontvangen en een mede werker van micro soft-werk nemers te bieden die een zakelijke relatie met de CPV heeft of hun bedrijf kent. Bijvoorbeeld een partner Development Manager (PDM).

Zodra u zich hebt Inge schreven bij partner centrum en uw toepassingen hebt geregistreerd, hebt u toegang tot partner Center-Api's. Als u een nieuwe CPV bent, ontvangt u uw sandbox-informatie via een partner centrum-melding. Zodra u de inschrijving als een micro soft CPV hebt voltooid en de CPV-overeenkomst hebt geaccepteerd, kunt u het volgende doen:

1. Multi tenant-toepassing beheren (toepassingen toevoegen aan Azure Portal, toepassingen registreren en registreren in het partner centrum).

   >[!Note]
   >CPVs moet hun toepassingen registreren in het partner centrum om toestemming te krijgen voor Partner Center-Api's. Door toepassingen toe te voegen aan de Azure Portal alleen worden CPV-toepassingen voor partner centrum-Api's geautoriseerd.

1. Uw CPV-profiel weer geven en beheren.

1. Bekijk en beheer uw gebruikers die toegang tot de CPV-mogelijkheden nodig hebben. Een CPV kan alleen de rol globale beheerder hebben.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Ik gebruik de Partner Center-SDK. Wordt het veilige toepassings model automatisch door SDK toegepast?

Nee, u moet de richt lijnen volgen die worden beschreven in de [hand leiding voor het beveiligde toepassings model](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Kan ik een vernieuwings token genereren voor het beveiligde toepassings model met accounts waarvoor MFA niet is ingeschakeld?

Ja, er kan een vernieuwings token worden gegenereerd met een account zonder MFA-afdwinging. Dit moet echter worden vermeden. Tokens die zijn gegenereerd met een account waarvoor MFA niet is ingeschakeld, hebben geen toegang tot bronnen vanwege de vereiste voor MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Hoe moet mijn toepassing een toegangs token verkrijgen als we MFA inschakelen?

U moet de [hand leiding voor het beveiligde toepassings model](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) volgen voor meer informatie over hoe u dit doet, en die voldoet aan de nieuwe beveiligings vereisten. Hier vindt u hier informatie over .NET-voorbeeld [code en Java](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) -voorbeeld [code.](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Als CPV moet ik een Azure AD-toepassing maken in onze CPV-Tenant of de Tenant van de CSP-partner?

De CPV moet de Azure Active Directory-toepassing maken in de Tenant die is gekoppeld aan hun inschrijving als CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Ik ben een CSP die alleen app-verificatie gebruikt. Moet ik wijzigingen aanbrengen?

Alleen app-verificatie wordt niet beïnvloed omdat er geen gebruikers referenties worden gebruikt om een toegangs token aan te vragen. Als er gebruikers referenties worden gedeeld, moeten de leveranciers van het configuratie scherm (CPVs) het Framework voor het [beveiligde toepassings model](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) aannemen en alle bestaande partner referenties die ze hebben opschonen.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Als CPV kan ik gebruikmaken van de verificatie stijl alleen voor apps om toegangs tokens op te halen?

Nee, leverancier-partners van het configuratie scherm kunnen de verificatie stijl alleen voor apps gebruiken om toegangs tokens namens de partner aan te vragen. Ze moeten het beveiligde toepassings model implementeren, waarbij gebruik wordt gemaakt van de stijl app + gebruiker-verificatie.

## <a name="technical-enforcement"></a>Technische afdwinging

### <a name="what-is-the-activation-of-security-safeguards"></a>Wat is de activering van beveiligings maatregelen?

Alle partners die deel nemen aan het programma Cloud Solution Provider (CSP), leveranciers van het configuratie scherm (CPVs) en Advisor moeten de verplichte beveiligings vereisten implementeren om te blijven voldoen aan het beleid.

Om extra beveiliging te bieden, begon micro soft met de activering van beveiligings maatregelen waarmee partners hun tenants en hun klanten kunnen beveiligen door eisen multi-factor Authentication (MFA) verificatie om onbevoegde toegang te voor komen.  

De activering van de beheer-en ADMINISTRATE-mogelijkheden voor alle partner tenants is voltooid. Om partners en klanten verder te beschermen en te richten op Q2 CY2020, beginnen we met de activering van partner Center-trans acties in CSP, waardoor partners hun bedrijven en klanten kunnen beschermen tegen incidenten met betrekking tot identiteits diefstal.

Ga voor meer informatie naar [eisen multi-factor Authentication (MFA) voor uw partner-Tenant](partner-security-requirements-mandating-mfa.md) pagina.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Ik gebruik een MFA-oplossing van derden en ik ben geblokkeerd; wat moet ik doen?

Als u wilt controleren of het account dat toegang heeft tot bronnen is aangevraagd voor multi-factor Authentication, zullen we de referentie claim van de [verificatie methode](https://tools.ietf.org/html/rfc8176) controleren om te zien of MFA wordt weer gegeven. Sommige oplossingen van derden geven deze claim niet af of bevatten de MFA-waarde niet. Als de claim ontbreekt of als de MFA-waarde niet wordt weer gegeven, is er geen manier om te bepalen of het geverifieerde account is gecontroleerd op multi-factor Authentication. U moet samen werken met de leverancier voor uw oplossing van derden om te bepalen welke acties moeten worden uitgevoerd, zodat de oplossing de referentie claim van de verificatie methode uitgeeft.

Zie [de vereisten voor de beveiliging van de partner testen](/powershell/partnercenter/test-partner-security-requirements) als u niet zeker weet of uw oplossing van derden de verwachte claim geeft.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>Er wordt door MFA geblokkeerd voor de ondersteuning van mijn klant met ADMINISTRATE, wat moet ik doen?

De technische afdwinging voor de beveiligings vereisten van de partner wordt gecontroleerd als het geverifieerde account is aangevraagd voor multi-factor Authentication. Als het account niet is ingesteld, wordt u omgeleid naar de aanmeldings pagina en wordt u gevraagd om opnieuw te verifiëren. Lees extra ervaring en richt lijnen in deze [eisen multi-factor Authentication (MFA) voor uw partner-Tenant](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) documentatie. In het scenario waarbij uw domein niet federatief is, wordt u gevraagd om multi-factor Authentication in te stellen na de verificatie. Zodra dit is voltooid, kunt u uw klanten beheren met behulp van ADMINISTRATE. In het scenario waarin uw domein federatief is, moet u ervoor zorgen dat het account wordt bevraagd voor multi-factor Authentication.

## <a name="security-defaults-transition"></a>Overgang van beveiligings standaard waarden

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Hoe kan ik overstappen van basislijn beleidsregels naar beveiligings standaards of andere MFA-oplossingen?

Azure Active Directory (Azure AD) ["baseline"-beleids regels worden verwijderd en vervangen](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) door "standaard instellingen voor beveiliging", een uitgebreidere reeks beveiligings beleidsregels voor u en uw klanten. Met [standaard instellingen voor beveiliging](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kunt u uw organisatie beschermen tegen beveiligings aanvallen met betrekking tot identiteits diefstal.

Uw MFA-implementatie (multi-factor Authentication) wordt verwijderd als gevolg van het buiten gebruik stellen van basislijn beleid als u niet hebt overgeschakeld van basislijn beleidsregels naar het beleid voor beveiligings standaarden of [andere opties voor MFA-implementatie](partner-security-requirements.md#implementing-multi-factor-authentication). Gebruikers in uw partner-tenants die MFA beveiligde bewerkingen uitvoeren, worden gevraagd MFA-verificatie te volt ooien. Bekijk [hier](partner-security-requirements-mandating-mfa.md)meer gedetailleerde richt lijnen.
Voer een van de volgende acties uit om te blijven voldoen en onderbrekingen tot een minimum te beperken:

- Overgang naar standaard instellingen voor beveiliging
    - Beleid voor standaard instellingen van beveiliging is een van de opties die partners kunnen kiezen voor het implementeren van MFA. Het biedt een basis niveau van beveiliging zonder extra kosten.
    - Meer informatie over het inschakelen van MFA voor uw organisatie met Azure AD en de [belangrijkste aandachtspunten voor de beveiligings standaards](partner-security-requirements.md#security-defaults).
    - Schakel de beleids regels voor standaard beveiliging in als deze voldoen aan uw bedrijfs behoeften.
- Overgang naar voorwaardelijke toegang
    - Als beleids regels voor de beveiliging niet voldoen aan uw behoeften, schakelt u voorwaardelijke toegang in. Raadpleeg de documentatie voor voorwaardelijke toegang van Azure AD voor meer informatie.

## <a name="key-resources"></a>Belangrijkste bronnen

### <a name="how-to-get-started"></a>Hoe gaat u aan de slag

- [Beveiligings vereisten voor partners: stapsgewijze hand leiding](partner-security-requirements.md).
- Stuur uw vragen en feedback naar deze [partner centrum-beveiligings richtlijnen groep](https://aka.ms/MPCSecurityGuidance).
- Kom naar aanstaande partners kantoor uren en webinars. Controleer [hier het gedetailleerde schema en de resources](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Bronnen voor het aannemen van een veilig toepassings model

- [Overzicht van veilig toepassings model](/partner-center/develop/enable-secure-app-model)
- [Partner centrum: hand leiding voor beveiligde toepassings modellen](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partners in het CSP-programma: .NET-voorbeeld code voor het inschakelen van een veilig toepassings model](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partners in het CSP-programma: Java-voorbeeld code voor het inschakelen van een veilig toepassings model](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Verificatie document van partner centrum](/partner-center/develop/partner-center-authentication)
- [Document Power shell Multi-Factor Authentication (MFA) van partner Center](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Ondersteuning

### <a name="where-can-i-get-support"></a>Waar kan ik ondersteuning krijgen?

Voor ondersteunings bronnen om te voldoen aan de beveiligings vereisten, als u geavanceerde ondersteuning voor partners (ASfP) hebt, neemt u contact op met uw service account manager. Neem contact op met uw service account manager en Technical Account Manager voor Premier Support voor partner overeenkomst (PSfP).

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Hoe kan ik technische informatie en ondersteuning verkrijgen om me te helpen bij het aannemen van een veilig toepassings model-Framework?

Technische ondersteunings opties voor Azure Active Directory zijn beschikbaar via uw MPN-voor delen. Partners met toegang tot een actief ASfP-of PSfP-abonnement kunnen samen werken met hun bijbehorende account manager (SAM/TAM) om de beschik bare opties voor hen goed te begrijpen.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Hoe kan ik contact opnemen met ondersteuning als ik de toegang tot het partner centrum kwijt ben?

Als u geen toegang meer hebt vanwege een MFA-probleem, neemt u contact op met de globale beheerder voor uw Tenant. Uw interne IT-afdeling kan u vertellen wie uw globale beheerder is. 

Als u uw wacht woord bent verg eten, kunt [u zich niet aanmelden](unable-to-sign-in.md) voor hulp.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Waar vind ik meer informatie over algemene technische problemen?

Informatie met betrekking tot de algemene technische problemen vindt u in de [beveiligings vereisten van de partner voor partners die partner Center of partner Center-api's gebruiken](partner-security-requirements.md)