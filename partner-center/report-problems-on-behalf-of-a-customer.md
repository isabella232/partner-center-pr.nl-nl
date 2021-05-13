---
title: Problemen rapporteren namens een klant
ms.topic: how-to
ms.date: 02/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informatie over het escaleren van een klantenserviceprobleem naar Microsoft en het indienen van een ondersteuningsticket voor verschillende typen Microsoft-services.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ba25d0bfc4796ca43d36bb34bf6d9e82889881c
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855706"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Een serviceprobleem melden namens een klant, inclusief wanneer en hoe dit te doen

**Van toepassing op**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Juiste rollen:** globale beheerder

Als uw klant een serviceprobleem ondervindt dat u niet kunt oplossen en voldoet aan de criteria die worden beschreven in Problemen escaleren naar [Microsoft,](escalate-problems-to-microsoft.md)kan uw indirecte provider een ondersteuningsticket voor hen indienen. Dit proces is ook nuttig voor het escaleren van factureringsproblemen of geschillen en voor fraudeproblemen.

## <a name="submit-a-service-request-for-a-customer"></a>Een serviceaanvraag indienen voor een klant

1. Selecteer in Partner Center menu onder CSP de optie **Klanten**

2. Selecteer of zoek op de pagina Klanten naar de klant die u wilt
    
3. Selecteer Serviceaanvragen in het menu **van de klant**

4. Selecteer in **het vervolgkeuzemenu** Nieuwe aanvraag de optie **Azure** of **Office 365, Dynamics 365, Enterprise Mobility Suite.** U wordt omgeleid naar het Microsoft Azure-portal of het Office 365-beheercentrum.

>[!NOTE]
>Support Operations-partners die Dynamics 365 in CSP uitvoeren, moeten een ondersteuningsovereenkomst van het ASfP-plan (Advanced Support for Partner) of hoger onderhouden. Deze ondersteuningsovereenkomst is vereist voor het indienen van Dynamics 365-incidenten namens een CSP-klant. [Meer informatie over](https://partner.microsoft.com/support/partnersupport) de opties voor ondersteuningsovereenkomst.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Wanneer u een serviceaanvraag voor uw klant in Azure moet maken, moet u rekening houden met het volgende:
>
>- Als u, als indirecte reseller, serviceaanvragen wilt maken voor uw klant in Azure, moet uw indirecte provider u toegang verlenen tot het Azure-account van de klant. Dit verschilt van het beheer namens klanten voor Office 365.
>
>- Hoewel de helpdeskbeheerder in Partner Center geen serviceaanvragen kan maken in de Azure-serviceportal, kunnen ze een ondersteuningsgroep maken in de Azure-serviceportal en die groep machtigingen geven om ondersteuningsaanvragen te registreren.

1. Selecteer **Nieuwe ondersteuningsaanvraag**.

2. Vul de ondersteuningsaanvraag in met de juiste informatie en selecteer vervolgens **Maken:**

   - Selecteer in **de** sectie Basisbeginselen van de ondersteuningsaanvraag de optie **Cloud Solution Provider** in het **veld Ondersteuningsplan.**

   - Voer in **de sectie** Contactgegevens van de ondersteuningsaanvraag uw gegevens in, niet de gegevens van uw klant.

3. Controleer later de serviceaanvragen van uw klant binnen de Microsoft Azure-portal door **Ondersteuningsaanvragen beheren te selecteren.**

Mogelijk moet u een ondersteuningsaanvraag maken voor een klant wanneer u geen beheerdersmachtigingen voor die klant hebt. Dit kan gebeuren in een van de volgende twee scenario's:

- U hebt geen beheerdersbevoegdheden gevraagd toen u de relatie voor het eerst tot stand hebt gebracht.
- U beheert alleen de Azure-abonnementen van een klant, dus u hebt geen beheerdersmachtigingen.
 
In beide gevallen kunt u de volgende procedure gebruiken om een ondersteuningsaanvraag te maken. 

1. Kopieer de domeinnaam van de klant van de accountpagina in Partner Center.

2. Ga naar https://portal.azure.com/ [customerdomainname]. 

3. Selecteer het Azure-abonnement dat ondersteuning vereist.

4. Selecteer **Nieuwe ondersteuningsaanvraag** en volg de aanwijzingen om de aanvraag te maken. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. Kies in **de sectie Een serviceaanvraag** maken de juiste ondersteuningscategorie. Mogelijk moet u **Meer... selecteren om** aanvullende artikelen te bekijken.

2. Vul het formulier voor de serviceaanvraag in en selecteer **Verzenden.**

   > [!TIP]
   > Zorg ervoor dat u uw contactgegevens op neem, niet die van uw klant.

3. Bekijk later de serviceaanvragen van uw klant door naar het Office 365-beheercentrum te gaan en **Alle ondersteuningstickets bekijken te selecteren.**

### <a name="support-for-commercial-marketplace-products"></a>Ondersteuning voor commerciële marketplace-producten

Microsoft biedt geen productondersteuning voor producten op de commerciële marketplace. Neem contact op met de onafhankelijke softwareleverancier (ISV) die het product heeft gepubliceerd om ondersteuning te krijgen.

Ga als volgt te werk om de contactgegevens van de ISV te vinden:

1.  Selecteer op **de pagina** Marketplace het product waar u hulp bij nodig hebt.

2.  Op de pagina van het product vindt u contactgegevens voor ondersteuning. Dit kan een of meer van de volgende opties zijn:

    - Een koppeling naar een ondersteuningsinvoerpunt op de website van de ISV
    - Een e-mail met ondersteuning
    - Een telefoonnummer van een contactpersoon voor ondersteuning

## <a name="faq"></a>Veelgestelde vragen

Zie de volgende veelgestelde vragen over serviceaanvragen die u namens een klant kunt indienen. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>Wat is opgenomen als onderdeel van het ondersteuningsrechten?

Serviceaanvragen moeten worden ingediend via Partner Center. Ze zijn beschikbaar voor Azure, Microsoft Office 365, Microsoft Dynamics CRM Online en Enterprise Mobility Suite. Als partner die deelneemt aan het Cloud Solution Provider programma, kunt u de reactietijd van prioriteit op uw belangrijkste problemen verwachten.

Ondersteuning voor uw eigen partner-tenant is niet opgenomen als onderdeel van het CSP-ondersteuningsvoordeel. Office 365, Microsoft Dynamics CRM Online en Enterprise Mobility Suite brengen echter geen afzonderlijke ondersteuningsabonnementskosten in rekening voor partners of klanten. Er worden wel kosten in rekening gebracht in Azure, maar als u recht hebt op Signature Cloud Support- of andere MPN-voordelen (Microsoft Partner Network), kunt u deze voordelen gebruiken om die kosten te betalen.

Dit voordeel geldt voor alle partners die deelnemen aan het Cloud Solution Provider programma, ongeacht of het betaald is of een proefperiode heeft. Ondersteuning voor facturerings- en abonnementsbeheer is ook opgenomen als een gratis onderdeel van dit pakket.

### <a name="how-quickly-will-i-get-an-initial-response"></a>Hoe snel krijg ik een eerste reactie?

De initiële reactietijden zijn afhankelijk van de ernst van het verzonden incident. De ernst van een probleem wordt bepaald door uw indicatie van de bedrijfsimpact wanneer u een serviceaanvraag indient.

Initiële reactietijden voor **technische onderbrekingsincidenten:**

- Kritieke impact (ernst A): twee uur (aanzienlijk verlies of degradatie van services. Productieservices zijn uit.)
- Gemiddelde impact (ernst B): vier uur (gemiddeld verlies of degradatie van services. Productieservices die gedeeltelijk worden beïnvloed.)
- Minimale impact (ernst C): acht uur (minimaal verlies of degradatie van services. Services die nog steeds beschikbaar zijn of niet-productieservices zijn beïnvloed.)

De initiële reactietijden zijn alleen voor Engelstalige ondersteuning. Ondersteuning voor lokale taal wordt geboden tijdens de werkuren.
Voor incidenten die binnen de grenzen van het ondersteuningsrecht vallen, maar die niet worden beschouwd als onderbrekingsincidenten, kan de initiële reactietijd maximaal één werkdag zijn.

### <a name="can-i-submit-a-service-request-by-phone"></a>Kan ik een serviceaanvraag per telefoon indienen?

Nee, telefonische ondersteuning wordt niet aangeboden voor dit programma.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Wat gebeurt er als ik me bij de Azure Portal en mijn Partner Center?

Als u zich rechtstreeks Microsoft Azure-portal, bekijkt u het centrum in uw eigen context, niet in de context van een klant. Daarom moet u zich alleen rechtstreeks aanmelden bij de Microsoft Azure-portal bij het maken van een serviceaanvraag voor uw eigen abonnementen.

Het ondersteuningsrechten voor uw CSP-programma biedt geen ondersteuning voor uw eigen Partner-abonnement. Daarom moet u uw geldige ondersteuningsplanrechten verstrekken wanneer u een serviceaanvraag maakt die betrekking heeft op uw eigen Partner-abonnement. Voorbeelden zijn MPN-contract-id, Premier of ondersteuning voor Azure abonnement. Zie de veelgestelde vragen over de [Ondersteuning voor Azure voor meer informatie.](https://go.microsoft.com/fwlink/?LinkId=717532)

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Wat gebeurt er als ik me meld bij de portal van het Office 365-beheercentrum en mijn Partner Center?

Als u zich rechtstreeks bij het Office 365-beheercentrum meldt, bekijkt u het centrum in uw eigen context, niet in de context van een klant. Daarom moet u zich alleen rechtstreeks aanmelden bij het Office 365-beheercentrum wanneer u een serviceaanvraag voor uw eigen abonnementen maakt.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>Hoe kan ik ondersteuning voor Dynamics 365?

Als u problemen ondervindt met betrekking tot: Dynamics 365-abonnementsabonnementen, licentieverlening, facturering, Finance & Operations, Dynamics 365-productlicenties of als u verdere technische ondersteuning nodig hebt:
 
Neem contact [op met dynamics-ondersteuning](/dynamics365/customer-engagement/admin/contact-technical-support)

## <a name="next-steps"></a>Volgende stappen

- [Uw klanten ondersteuning bieden](customer-support.md)
- [Servicestatus controleren](check-service-health.md)
