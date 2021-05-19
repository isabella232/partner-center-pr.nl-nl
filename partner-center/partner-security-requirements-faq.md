---
title: Veelgestelde vragen over beveiligingsvereisten van partners
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Veelgestelde vragen over de beveiligingsvereisten van partners: wat ze zijn, hoe partners deze moeten implementeren en hoe u weet of u aan deze vereisten hebt voldaan.'
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 174c56ce9bb5fb3d9d92c1ef18af73479619f4bb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145878"
---
# <a name="common-questions-about-partner-security-requirements"></a>Veelvoorkomende vragen over beveiligingsvereisten van partners

**Juiste rollen:** alle Partner Center gebruikers

In dit artikel vindt u antwoorden op enkele veelvoorkomende vragen over [de beveiligingsvereisten van partners.](partner-security-requirements.md)

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement-them"></a>Wat zijn de beveiligingsvereisten van partners en waarom moeten partners deze implementeren?

Betere en voortdurende veiligheidsmaatregelen op het gebied van beveiliging en privacy staan bij onze topprioriteiten en we blijven partners helpen hun klanten en tenants te beschermen. We blijven steeds meer geavanceerde, toenemende beveiligingsaanvallen zien, voornamelijk gerelateerd aan identiteitsincidenten. Aangezien preventieve maatregelen een belangrijke rol spelen in een algehele verdedigingsstrategie om beveiligingsaanvallen te voorkomen, hebben we [in](partner-security-requirements.md) 2019 verplichte beveiligingsvereisten geïntroduceerd. Alle partners die deelnemen aan het Cloud Solution Provider(CSP)-programma, Configuratiescherm Vendors en Advisors moeten de vereisten implementeren om compatibel te blijven.

### <a name="what-are-the-key-timelines-and-milestones"></a>Wat zijn de belangrijkste tijdlijnen en mijlpalen?

De voorwaarden die zijn gekoppeld aan deze beveiligingsvereisten, inclusief tijdlijnen en mijlpalen, zijn opgenomen in [de Microsoft Partner-overeenkomst.](microsoft-partner-agreement.md) U moet deze beveiligingsvereisten zo snel mogelijk implementeren om te blijven voldoen aan uw deelname aan het CSP-programma.

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>Wat gebeurt er als ik deze beveiligingsvereisten van partners niet implementeert?

De Microsoft Partner-overeenkomst vereist dat u meervoudige verificatie afdwingt voor gebruikersaccounts en het veilige toepassingsmodel gebruikt voor interactie met de Partner Center API. 

Partners die zich niet houden aan deze beveiligingsprocedures, verliezen mogelijk hun vermogen om te transacten in het CSP-programma of om tenants van klanten te beheren met beheerdersrechten delegeren.

### <a name="do-the-security-requirements-apply-to-all-geographies"></a>Zijn de beveiligingsvereisten van toepassing op alle geografische gebieden?

Ja, de beveiligingsvereisten gelden voor alle geografische gebieden. Het wordt ten zeerste aangeraden dat alle partners die via een soevereine cloud (Amerikaanse overheid en Duitsland) handelen, onmiddellijk aan deze nieuwe beveiligingsvereisten voldoen. Deze partners zijn momenteel echter niet vereist om te voldoen aan de beveiligingsvereisten. Microsoft geeft in de toekomst aanvullende informatie over het afdwingen van deze beveiligingsvereisten voor onafhankelijke clouds.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>Is het mogelijk om een uitsluiting voor een account te krijgen?

Nee, het is niet mogelijk om een gebruikersaccount uit te sluiten van de vereiste dat meervoudige verificatie (MFA) wordt afgedwongen. Gezien de zeer bevoorrechte aard van een partner, vereist de Microsoft Partner-overeenkomst dat meervoudige verificatie wordt afgedwongen voor elk gebruikersaccount in uw partnerten tenant.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>Hoe kan ik weten of ik heb voldaan aan de beveiligingsvereisten van de partner?

Voer de volgende stappen uit:

- U moet voldoen aan alle vereisten die worden beschreven in de [beveiligingsvereisten van de partner.](partner-security-requirements.md)
- U moet ervoor zorgen dat voor alle gebruikersaccounts in uw partner-tenant meervoudige verificatie wordt afgedwongen.

Om de belangrijkste gebieden te identificeren waar u acties kunt ondernemen, bieden we het [statusrapport](https://partner.microsoft.com/commerce/security/compliance) van de beveiligingsvereisten dat beschikbaar is via Partner Center.

Zie status van partnerbeveiligingsvereisten voor meer informatie [over het statusrapport.](partner-security-compliance.md)

## <a name="required-actions"></a>Vereiste acties

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>Wat zijn de belangrijkste acties die ik moet ondernemen om aan de vereisten te voldoen?

Alle partners in het CSP-programma (directe factuur, indirecte provider en indirecte reseller), advisors en Configuratiescherm leveranciers moeten voldoen aan de vereisten.

1. **MFA afdwingen voor alle gebruikers**

    Alle partners in het CSP-programma, adviseurs en Configuratiescherm leveranciers moeten MFA afdwingen voor alle gebruikers in hun partnerten tenant.

    Aanvullende overwegingen:

    - Indirecte providers moeten samenwerken met indirecte resellers om onboarding uit te Partner Center als ze dit nog niet hebben gedaan en hun resellers stimuleren om aan de vereisten te voldoen.
    - Azure MFA wordt gratis beschikbaar gesteld voor alle gebruikers in de partnertenant via standaardinstellingen voor Azure AD-beveiliging met de enige verificatiemethode van een ver authenticator-toepassing die ondersteuning biedt voor een time-based one time passwords (TOTP).
    - Aanvullende verificatiemethoden zijn beschikbaar via de [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU's, als andere methoden, zoals een telefoongesprek of sms-bericht, vereist zijn.
    - Partners kunnen ook een MFA-oplossing van derden voor elk account gebruiken bij toegang tot commerciële cloudservices van Microsoft.

2. **Het veilig toepassingsmodel framework**

    Alle partners die aangepaste integratie hebben ontwikkeld met behulp van API's (zoals Azure Resource Manager, Microsoft Graph, Partner Center-API, enzovoort) of aangepaste automatisering hebben geïmplementeerd met behulp van hulpprogramma's zoals PowerShell, moeten het [veilig toepassingsmodel-framework](/partner-center/develop/enable-secure-app-model) gebruiken om te integreren met Microsoft-cloudservices. Als u dit niet doet, kan dit leiden tot een onderbreking vanwege de MFA-implementatie. De volgende bronnen bieden een overzicht en richtlijnen met betrekking tot het gebruik van het model.

    - [veilig toepassingsmodel overzicht](/partner-center/develop/enable-secure-app-model)
    - [Partner Center: veilig toepassingsmodel handleiding](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partners in CSP-programma: .NET-voorbeeldcode voor het inschakelen van veilig toepassingsmodel](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partners in CSP-programma: Java-voorbeeldcode voor het inschakelen van veilig toepassingsmodel](/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Partner Center-verificatiedocument](/partner-center/develop/partner-center-authentication)
    - [Partner Center PowerShell Multi-Factor Authentication (MFA) document](/powershell/partnercenter/multi-factor-auth)

    Neem contact op met de leverancier als u een configuratiescherm gebruikt met betrekking tot de acceptatie van het veilig toepassingsmodel framework.

    Leveranciers van configuratiescherm moeten [onboarding](enroll-as-cpv.md) uitvoeren voor Partner Center als leverancier van het configuratiescherm en onmiddellijk beginnen met het implementeren van deze vereiste. Raadpleeg het [Partner Center: veilig toepassingsmodel framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Leveranciers van configuratiescherm moeten de toestemming van CSP-partners accepteren en beheren in plaats van referenties en de referenties van alle bestaande CSP-partners opsisten.

## <a name="multi-factor-authentication"></a>Meervoudige verificatie

### <a name="what-is-multi-factor-authentication-mfa"></a>Wat is Meervoudige verificatie (MFA)?

MFA is een beveiligingsmechanisme voor het verifiëren van personen via meer dan één vereiste beveiligings- en validatieprocedure. Dit werkt door twee of meer van de volgende verificatiemethoden te vereisen:

- Iets dat u weet (meestal een wachtwoord)
- Iets dat u hebt (een vertrouwd apparaat dat niet eenvoudig kan worden gedupliceerd, zoals een telefoon)
- Iets dat u bent (biometrie)

### <a name="what-is-the-cost-of-enabling-mfa"></a>Wat zijn de kosten voor het inschakelen van MFA?

Microsoft biedt MFA gratis aan via de implementatie van standaardinstellingen voor Azure AD-beveiliging. De enige verificatieoptie die beschikbaar is met behulp van deze versie van MFA is een verificatietoepassing. Als een telefoongesprek of sms-bericht is vereist, moet [Azure Active Directory Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium) licentie voor een licentie worden aangeschaft. U kunt ook een oplossing van derden gebruiken om MFA te bieden voor elke gebruiker in uw partner-tenant. In dit geval is het uw verantwoordelijkheid om ervoor te zorgen dat uw MFA-oplossing wordt afgedwongen en dat u aan het beleid voldoet.

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>Welke acties moet ik uitvoeren als ik al een MFA-oplossing heb?

Via deze beveiligingsvereisten moeten gebruikers in een partner-tenant zich verifiëren met MFA bij toegang tot commerciële cloudservices van Microsoft. Oplossingen van derden kunnen worden gebruikt om aan deze vereisten te voldoen. Microsoft biedt geen validatietests meer aan onafhankelijke id-providers voor compatibiliteit met Azure Active Directory. Raadpleeg deze richtlijnen om uw product te testen op [interoperabiliteit.](https://www.microsoft.com/download/details.aspx?id=56843)

> [!IMPORTANT]
> Wanneer u een oplossing van derden gebruikt, is het belangrijk om te controleren of de oplossing de AMR-claim (Authentication Method Reference) geeft die de MFA-waarde bevat. Zie [Testing the Partner Security Requirements (De](/powershell/partnercenter/test-partner-security-requirements) beveiligingsvereisten van de partner testen) voor meer informatie over het valideren van uw oplossing van derden die de verwachte claim uit geeft.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Ik gebruik meerdere partnerten tenants om te transacten. Moet ik MFA op al deze twee implementeren?

Ja, u moet MFA afdwingen voor elke Azure Active Directory tenant die is gekoppeld aan het CSP-programma of het Advisor-programma. Als u een Azure Active Directory Premium wilt kopen, moet u een Azure Active Directory aanschaffen voor de gebruikers in elke Azure Active Directory tenant. 

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>Moet voor elk gebruikersaccount in de tenant van mijn partner MFA worden afgedwongen?

Ja, voor elke gebruiker moet MFA worden afgedwongen. Als u echter de standaardinstellingen voor Azure AD-beveiliging gebruikt, is er geen extra actie vereist omdat met deze functie MFA wordt afgedwongen voor alle gebruikersaccounts. Het inschakelen van standaardinstellingen voor beveiliging is een gratis en eenvoudige manier om ervoor te zorgen dat uw gebruikersaccounts compatibel zijn met MFA en niet worden beïnvloed wanneer MFA wordt afgedwongen.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Ik ben een partner voor directe factuur bij Microsoft. Wat moet ik doen?

Directe factuur Cloud Solution Provider moeten MFA afdwingen voor elke gebruiker in hun partner-tenant.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-enable-mfa"></a>Ik ben een indirecte reseller en doe alleen iets als een distributeur. Moet ik MFA nog steeds inschakelen?

Alle indirecte resellers moeten MFA afdwingen voor elke gebruiker in hun partnerten tenant. De indirecte reseller moet MFA inschakelen.

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Ik gebruik de api Partner Center api. Moet ik MFA nog steeds implementeren?

Ja, deze beveiligingsvereiste geldt voor alle gebruikers, inclusief gebruikers met partnerbeheerders en eindgebruikers in een partner-tenant.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Welke externe leveranciers bieden MFA-oplossingen die compatibel zijn met Azure Active Directory?

Bij het beoordelen van MFA-leveranciers en -oplossingen moeten partners ervoor zorgen dat de oplossing die ze kiezen compatibel is met Azure Active Directory.

Microsoft biedt geen validatietests meer aan onafhankelijke id-providers voor compatibiliteit met Azure Active Directory. Als u uw product wilt testen op interoperabiliteit, raadpleegt u deze [richtlijnen.](https://www.microsoft.com/download/details.aspx?id=56843)

Zie de compatibiliteitslijst voor [Azure AD-federatie voor meer informatie.](/azure/active-directory/hybrid/how-to-connect-fed-compatibility)

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>Hoe kan ik MFA testen in onze integratie-sandbox?

De functie standaardinstellingen voor Azure AD-beveiliging moet zijn ingeschakeld of u kunt ook een oplossing van derden gebruiken die gebruikmaakt van federatie.

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>Heeft het inschakelen van MFA invloed op de interactie met de tenant van mijn klant?

Nee. De uitvoering van deze beveiligingsvereisten heeft geen invloed op de manier waarop u uw klanten beheert. De mogelijkheid om gedelegeerde beheerbewerkingen uit te voeren, wordt niet onderbroken.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>Gelden voor mijn klanten de beveiligingsvereisten van de partner?

Nee, het is niet vereist dat u MFA afdwingt voor elke gebruiker in de Azure AD-tenants van uw klant. Het wordt echter aanbevolen dat u met elke klant samenwerkt om te bepalen hoe de gebruikers het beste kunnen worden beschermd.

### <a name="can-any-user-be-excluded-from-the-mfa-requirement"></a>Kan een gebruiker worden uitgesloten van de MFA-vereiste?

Nee, elke gebruiker, inclusief serviceaccounts, in uw partner-tenant is vereist voor verificatie met behulp van MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>Zijn de beveiligingsvereisten van de partner van toepassing op de integratie-sandbox?

Ja, de beveiligingsvereisten van de partner zijn van toepassing op de integratie-sandbox. Dit betekent dat u de juiste MFA-oplossing moet implementeren voor gebruikers in de sandbox-tenant voor integratie. Het wordt aanbevolen om standaardinstellingen voor Azure AD-beveiliging te implementeren om MFA op te geven.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>Hoe kan ik account voor toegang in noodgevallen configureren?

Het wordt beschouwd als een best practice om een of twee accounts voor toegang in noodgevallen te maken om te voorkomen dat uw Azure AD-tenant per ongeluk wordt vergrendeld. Met betrekking tot de beveiligingsvereisten van de partner is het vereist dat elke gebruiker wordt geverifieerd met MFA. Deze vereiste betekent dat u de definitie van een account voor toegang in noodgevallen moet wijzigen. Dit kan een account zijn dat gebruik maakt van een oplossing van derden voor MFA.

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>Is Active Directory Federation Service (ADFS) vereist als ik een oplossing van derden gebruik?

Nee, het is niet vereist om Active Directory Federation Service (ADFS) te hebben als u een oplossing van derden gebruikt. Het is raadzaam om samen met de leverancier van de oplossing te bepalen wat de vereisten voor hun oplossing zijn.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Is het een vereiste om standaardinstellingen voor Azure AD-beveiliging in te kunnenschakelen?

Nee, het is niet vereist dat u standaardinstellingen voor Azure AD-beveiliging inschakelen.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>Kan voorwaardelijke toegang worden gebruikt om te voldoen aan de MFA-vereiste?

Ja, u kunt voorwaardelijke toegang gebruiken om MFA af te dwingen voor elke gebruiker, inclusief serviceaccounts, in uw partnerten tenant. Gezien de aard van een partner met hoge bevoegdheden moeten we er echter voor zorgen dat elke gebruiker een MFA-uitdaging heeft voor elke afzonderlijke verificatie. Dit betekent dat u de functie van voorwaardelijke toegang waarmee de vereiste voor MFA wordt omzeild, niet kunt gebruiken.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Wordt het serviceaccount dat wordt gebruikt door Azure AD Connect worden beïnvloed door de beveiligingsvereisten van de partner?

Nee, het serviceaccount dat wordt gebruikt door Azure AD Connect worden niet beïnvloed door de beveiligingsvereisten van de partner. Als u een probleem hebt met Azure AD Connect als gevolg van het afdwingen van MFA, opent u een aanvraag voor technische ondersteuning bij Microsoft Ondersteuning.

## <a name="secure-application-model"></a>veilig toepassingsmodel

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>Wie moet het model voor beveiligde toepassingen gebruiken om aan de vereisten te voldoen?

Microsoft introduceert een veilig, schaalbaar framework voor de verificatie van Cloud Solution Provider-partners (CSP) en Configuratiescherm Vendors (CPV) die multi-factor Authentication gebruiken. Zie de veilig toepassingsmodel [voor meer informatie.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) Alle partners die aangepaste integratie hebben ontwikkeld met behulp van API's (zoals Azure Resource Manager, Microsoft Graph, Partner Center API, enzovoort) of aangepaste automatisering hebben geïmplementeerd met behulp van hulpprogramma's zoals PowerShell, moeten het [veilig toepassingsmodel-framework](/partner-center/develop/enable-secure-app-model) implementeren om te integreren met Microsoft-cloudservices.

### <a name="what-is-the-secure-application-model"></a>Wat is de veilig toepassingsmodel?

Microsoft introduceert een veilig, schaalbaar framework voor de verificatie van Cloud Solution Provider-partners (CSP) en Configuratiescherm Vendors (CPV) die gebruikmaken van Multi-Factor Authentication. Zie de [veilig toepassingsmodel voor](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) meer informatie.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Hoe kan ik de veilig toepassingsmodel?

Alle partners die aangepaste integratie hebben ontwikkeld met behulp van API's (zoals Azure Resource Manager, Microsoft Graph, Partner Center API, enzovoort) of aangepaste automatisering hebben geïmplementeerd met behulp van hulpprogramma's zoals PowerShell, moeten het [veilig toepassingsmodel-framework](/partner-center/develop/enable-secure-app-model) implementeren om te integreren met Microsoft-cloudservices. Als u dit niet doet, kan dit leiden tot een onderbreking vanwege de MFA-implementatie. De volgende bronnen bieden een overzicht en richtlijnen met betrekking tot het gebruik van het model.

- [veilig toepassingsmodel overzicht](/partner-center/develop/enable-secure-app-model)
- [Partner Center: veilig toepassingsmodel handleiding](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partners in CSP-programma: .NET-voorbeeldcode voor het inschakelen van veilig toepassingsmodel](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partners in CSP-programma: Java-voorbeeldcode voor het inschakelen van veilig toepassingsmodel](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Partner Center-verificatiedocument](/partner-center/develop/partner-center-authentication)
- [Partner Center PowerShell Multi-Factor Authentication (MFA) document](/powershell/partnercenter/multi-factor-auth)

Als u een configuratiescherm gebruikt, moet u contact opnemen met de leverancier over de acceptatie van het veilig toepassingsmodel framework.

Leveranciers van configuratiescherm moeten onboarden [bij](enroll-as-cpv.md) Partner Center als leverancier van het configuratiescherm en onmiddellijk beginnen met het implementeren van deze vereiste. Raadpleeg het [Partner Center: veilig toepassingsmodel framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Leveranciers van configuratiescherm moeten de toestemming van CSP-partners accepteren en beheren in plaats van referenties, en de referenties van alle bestaande CSP-partners opsisten.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>Moet de veilig toepassingsmodel alleen worden geïmplementeerd voor Partner Center API/SDK?

Als u meervoudige verificatie afdwingt voor alle gebruikersaccounts, heeft dit gevolgen voor automatisering of integratie die is bedoeld om niet-interactief te worden uitgevoerd. Hoewel de beveiligingsvereisten van de partner vereisen dat u het veilige toepassingsmodel voor de Partner Center-API inschakelen, kan het worden gebruikt om te voldoen aan de noodzaak van een tweede verificatiefactor met automatisering en integratie.

>[!Note] 
>Resources die worden gebruikt, moeten ondersteuning bieden voor verificatie op basis van toegangs token.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Ik gebruik automatiseringshulpprogramma's zoals PowerShell. Hoe kan ik de veilig toepassingsmodel?

U moet de veilig toepassingsmodel implementeren als uw automatisering is bedoeld om niet-interactief te worden uitgevoerd en afhankelijk is van gebruikersreferenties voor verificatie. Zie [veilig toepassingsmodel | Partner Center PowerShell voor](/powershell/partnercenter/multi-factor-auth) hulp bij het implementeren van dit framework.  

>[!Note] 
>Niet alle automatiseringshulpprogramma's bieden de mogelijkheid om te verifiëren met behulp van toegangstokens. Plaats een bericht op de [Partner Center beveiligingshulpgroep](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) als u hulp nodig hebt bij het begrijpen welke wijzigingen moeten worden aangebracht. 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>Welke gebruikersreferenties moet de toepassingsbeheerder verstrekken bij het uitvoeren van het toestemmingsproces?

U wordt aangeraden een serviceaccount te gebruiken dat de machtigingen met de minste bevoegdheden heeft gekregen. Met betrekking tot Partner Center API moet u een account gebruiken dat is toegewezen aan de rol Verkoopagent of Beheerderagent.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>Waarom moet de toepassingsbeheerder geen gebruikersreferenties voor globale beheerders verstrekken bij het uitvoeren van het toestemmingsproces?

Het is een best practice minst bevoegde identiteit te gebruiken.  Dit vermindert het risico. Het wordt afgeraden om een account met globale beheerdersbevoegdheden te gebruiken, omdat dit meer machtigingen biedt dan is vereist.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Ik ben een CSP-partner. Hoe kan ik weten of mijn Configuratiescherm Vendor (CPV) al dan niet bezig is met het implementeren van de oplossing?

Voor partners die een CPV-oplossing (Configuratiescherm Vendor) gebruiken voor transact in het Cloud Solution Provider-programma (CSP), is het uw verantwoordelijkheid om contact op te nemen met uw CPV.

### <a name="who-is-a-control-panel-vendor-cpv"></a>Wie is een Configuratiescherm Vendor (CPV)?

Een Configuratiescherm is een onafhankelijke softwareleverancier die apps ontwikkelt die door CSP-partners kunnen worden gebruikt om te integreren met Partner Center API's. Een Configuratiescherm is geen CSP-partner met directe toegang tot Partner Center dashboard of API's. Een gedetailleerde beschrijving is beschikbaar in de [handleiding Partner Center: Secure Applications Model](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Ik ben een CPV. Hoe kan ik registreren?

Als u zich wilt registreren als een leverancier van het configuratiescherm (CPV), volgt u de richtlijnen die hier [worden gegeven.](enroll-as-cpv.md)

CPV's moeten contact opnemen om de inschrijvingskoppeling te ontvangen en een Microsoft-medewerkerssponsor te leveren die een zakelijke relatie heeft met de CPV of die [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) bekend is met hun bedrijf. Bijvoorbeeld een Partner Development Manager (PDM).

Nadat u zich hebt Partner Center en uw toepassingen hebt geregistreerd, hebt u toegang tot Partner Center API's. U ontvangt uw sandboxgegevens via een Partner Center als u een nieuwe CPV bent. Nadat u de inschrijving als Een Microsoft CPV hebt voltooid en de CPV-overeenkomst hebt geaccepteerd, kunt u het volgende doen:

1. Toepassingen met meerdere tenants beheren (toepassingen toevoegen aan Azure Portal en registratie van toepassingen in Partner Center).

   >[!Note]
   >CPV's moeten hun toepassingen registreren in Partner Center om te worden geautoriseerd voor Partner Center API's. Het toevoegen van toepassingen aan Azure Portal alleen biedt geen toestemming voor CPV-toepassingen voor Partner Center API's.

1. Uw CPV-profiel weergeven en beheren.

1. Bekijk en beheer uw gebruikers die toegang nodig hebben tot CPV-mogelijkheden. Een CPV kan alleen de rol Globale beheerder hebben.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Ik gebruik de Partnercentrum-SDK. Wordt de SDK automatisch veilig toepassingsmodel?

Nee, u moet de richtlijnen in de handleiding voor veilig toepassingsmodel [volgen.](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>Kan ik een vernieuwings token genereren voor het veilige toepassingsmodel met accounts die MFA niet hebben ingeschakeld?

Ja, een vernieuwings token kan worden gegenereerd met behulp van een account dat MFA niet heeft afgedwongen. Dit moet echter worden vermeden. Elk token dat wordt gegenereerd met een account dat MFA niet heeft ingeschakeld, heeft geen toegang tot resources vanwege de vereiste voor MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>Hoe moet mijn toepassing een toegangs token verkrijgen als we MFA inschakelen?

Volg de handleiding veilig toepassingsmodel [informatie](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) over hoe u dit doet terwijl u voldoet aan de nieuwe beveiligingsvereisten. U vindt hier .NET-voorbeeldcode [en](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) Java-voorbeeldcode [hier.](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Maak ik als CPV een Azure AD-toepassing in onze CPV-tenant of de tenant van de CSP-partner?

De CPV moet de toepassing Azure Active Directory maken in de tenant die is gekoppeld aan hun inschrijving als CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Ik ben een CSP die alleen app-verificatie gebruikt. Moet ik wijzigingen aanbrengen?

Verificatie alleen voor apps wordt niet beïnvloed omdat gebruikersreferenties niet worden gebruikt om een toegangs token aan te vragen. Als gebruikersreferenties worden gedeeld, moeten leveranciers van configuratiescherm (CPV's) het [veilig toepassingsmodel-framework gebruiken](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) en de bestaande partnerreferenties die ze hebben, opsisten.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Kan ik als CPV gebruikmaken van de verificatiestijl van de app om toegangstokens op te halen?

Nee, Configuratiescherm kunnen de verificatiestijl van de app alleen gebruiken om namens de partner toegangstokens aan te vragen. Ze moeten het veilige toepassingsmodel implementeren, dat gebruikmaakt van de stijl app + gebruikersverificatie.

## <a name="technical-enforcement"></a>Technische afdwinging

### <a name="what-is-the-activation-of-security-safeguards"></a>Wat is de activering van beveiligingsbeveiligingen?

Alle partners die deelnemen aan het Cloud Solution Provider(CSP)-programma, Configuratiescherm Vendors (CPV's) en advisors moeten de verplichte beveiligingsvereisten implementeren om compatibel te blijven.

Om extra beveiliging te bieden, is Microsoft begonnen met het activeren van beveiligingsbeveiligingen waarmee partners hun tenants en hun klanten kunnen beveiligen door meervoudige verificatie (MFA) te verplichten om onbevoegde toegang te voorkomen.  

De activering voor AOBO-mogelijkheden (admin-on-behalf-of) voor alle partnertenties is voltooid. Ter bescherming van partners en klanten, gericht op Q2 CY2020, beginnen we met de activering van Partner Center-transacties in CSP, waarbij partners hun bedrijf en klanten beschermen tegen identiteitsdiefstalgerelateerde incidenten.

Ga naar De [MFA (Multi-Factor Authentication) voor uw partner-tenantpagina](partner-security-requirements-mandating-mfa.md) voor meer informatie.

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Ik gebruik een MFA-oplossing van derden en ik wordt geblokkeerd. Wat moet ik doen?

Om te valideren dat het account dat toegang heeft tot [](https://tools.ietf.org/html/rfc8176) resources is om meervoudige verificatie is gesteld, controleren we de referentieclaim voor verificatiemethoden om te zien of MFA wordt vermeld. Sommige oplossingen van derden geven deze claim niet uit of bevatten niet de MFA-waarde. Als de claim ontbreekt of als de MFA-waarde niet wordt vermeld, is er geen manier om te bepalen of het geverifieerde account is om meervoudige verificatie is omgemiddeld. U moet samenwerken met de leverancier voor uw oplossing van derden om te bepalen welke acties moeten worden ondernomen, zodat de oplossing de referentieclaim voor de verificatiemethode zal uitgeven.

Zie [Testing the Partner Security Requirements](/powershell/partnercenter/test-partner-security-requirements) (De beveiligingsvereisten van de partner testen) als u niet zeker weet of uw oplossing van derden de verwachte claim indient.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA blokkeert de ondersteuning van mijn klant met AOBO. Wat moet ik doen?

De technische afdwinging voor de beveiligingsvereisten van de partner wordt gecontroleerd als het geverifieerde account is ingeschakeld voor meervoudige verificatie. Als het account niet is, wordt u omgeleid naar de aanmeldingspagina en wordt u gevraagd om opnieuw te verifiëren. Lees aanvullende ervaring en richtlijnen in [deze MFA (Mandating Multi-Factor Authentication) voor de tenantdocumentatie van uw](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) partner. In het scenario waarin uw domein niet is ge federeerd, wordt u na een verificatie gevraagd om meervoudige verificatie in te stellen. Zodra dit is voltooid, kunt u uw klanten beheren met AOBO. In het scenario waarin uw domein is ge federeerd, moet u ervoor zorgen dat het account wordt gebruikt voor meervoudige verificatie.

## <a name="security-defaults-transition"></a>Overgang naar standaardinstellingen voor beveiliging

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>Hoe kan ik overstappen van basislijnbeleid naar standaardinstellingen voor beveiliging of andere MFA-oplossingen?

Azure Active Directory (Azure [AD)](/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults) basislijnbeleid wordt verwijderd en vervangen door 'standaardinstellingen voor beveiliging', een uitgebreidere set beveiligingsbeleidsregels voor u en uw klanten. [Standaardinstellingen voor beveiliging](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) kunnen uw organisatie beschermen tegen beveiligingsaanvallen die te maken hebben met identiteitsdiefstal.

Uw MFA-implementatie (Multi-Factor Authentication) wordt verwijderd omdat het basislijnbeleid wordt afgeschaft als u niet bent overgeplaatst van basislijnbeleid naar het standaardbeleid voor beveiliging of andere [MFA-implementatieopties.](partner-security-requirements.md#implementing-multi-factor-authentication) Alle gebruikers in uw partnerten tenants die met MFA beveiligde bewerkingen uitvoeren, worden gevraagd om de MFA-verificatie te voltooien. Bekijk hier meer [gedetailleerde richtlijnen.](partner-security-requirements-mandating-mfa.md)
Als u compatibel wilt blijven en onderbrekingen wilt minimaliseren, moet u een van de volgende acties uitvoeren:

- Overgang naar standaardinstellingen voor beveiliging
    - Standaardbeleid voor beveiliging is een van de opties die partners kunnen kiezen om MFA te implementeren. Het biedt een basisbeveiligingsniveau dat zonder extra kosten is ingeschakeld.
    - Meer informatie over het inschakelen van MFA voor uw organisatie met Azure AD en het bekijken van de belangrijkste overwegingen voor [de standaardinstellingen voor beveiliging.](partner-security-requirements.md#security-defaults)
    - Schakel standaardbeleid voor beveiliging in als dit voldoet aan de behoeften van uw bedrijf.
- Overgang naar voorwaardelijke toegang
    - Als het standaardbeleid voor beveiliging niet aan uw behoeften voldoen, kunt u voorwaardelijke toegang inschakelen. Lees de documentatie voor voorwaardelijke toegang van Azure AD voor meer informatie.

## <a name="key-resources"></a>Belangrijkste resources

### <a name="how-to-get-started"></a>Hoe gaat u aan de slag

- [Beveiligingsvereisten van partners: stapsgewijs.](partner-security-requirements.md)
- Stuurt uw vragen en feedback naar deze [Partner Center security guidance group](https://aka.ms/MPCSecurityGuidance).
- Neem deel aan kantooruren en webinars van partners. Controleer hier [de gedetailleerde planning en resources.](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)

### <a name="resources-for-adopting-secure-application-model"></a>Resources voor het over aannemen van een veilig toepassingsmodel

- [veilig toepassingsmodel overzicht](/partner-center/develop/enable-secure-app-model)
- [Partner Center: veilig toepassingsmodel handleiding](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partners in CSP-programma: .NET-voorbeeldcode voor het inschakelen van veilig toepassingsmodel](/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partners in CSP-programma: Java-voorbeeldcode voor het inschakelen van veilig toepassingsmodel](/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Partner Center-verificatiedocument](/partner-center/develop/partner-center-authentication)
- [Partner Center PowerShell Multi-Factor Authentication (MFA) document](/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Ondersteuning

### <a name="where-can-i-get-support"></a>Waar kan ik ondersteuning krijgen?

Neem contact op met uw serviceaccountmanager als u geavanceerde ondersteuning voor partners (ASfP) hebt om te voldoen aan de beveiligingsvereisten; voor Premier Support partnerovereenkomst (PSfP) kunt u contact opnemen met uw serviceaccountmanager en technische accountmanager.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>Hoe kan ik technische informatie en ondersteuning om mij te helpen het framework voor een veilig toepassingsmodel te gebruiken?

Technische productondersteuningsopties voor Azure Active Directory zijn beschikbaar via uw MPN-voordelen. Partners met toegang tot een actief ASfP- of PSfP-abonnement kunnen samenwerken met hun gekoppelde account manager (SAM/TAM) om zo goed mogelijk inzicht te krijgen in de beschikbare opties.

### <a name="how-do-i-contact-support-if-ive-lost-access-to-partner-center"></a>Hoe kan ik contact opnemen met de ondersteuning als ik geen toegang meer heb Partner Center?

Als u geen toegang meer hebt vanwege een probleem met MFA, neem dan contact op met de globale beheerder voor uw tenant. Uw interne IT-afdeling kan u vertellen wie uw globale beheerder is. 

Als u uw wachtwoord bent vergeten, leest [u Kan u niet aanmelden](unable-to-sign-in.md) voor hulp.

### <a name="where-can-i-find-more-information-about-common-technical-issues"></a>Waar vind ik meer informatie over veelvoorkomende technische problemen?

Informatie over de veelvoorkomende technische problemen vindt u in [Partner security requirements for partners using Partner Center or Partner Center APIs (Beveiligingsvereisten](partner-security-requirements.md) van partners voor partners die gebruikmaken Partner Center of Partner Center API's)