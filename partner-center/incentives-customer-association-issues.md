---
title: Problemen met klantkoppeling Incentives
description: Meer informatie over het oplossen van problemen die zich kunnen voor doen bij het werken met geclaimde Partner of Record (CPOR) klantorganisaties.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: d23c95981c39bb9b9773e3b1e6f474146f41325546cc5f96408237e2213280d2
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681804"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemen met geclaimde Partner of Record (CPOR) klant verbanden

**Juiste rollen:** Factureringsbeheerder | Globale beheerder | Incentives-beheerder

De onderstaande inhoud helpt u bij het oplossen van problemen die kunnen komen wanneer u met klantorganisaties werkt.

## <a name="domain-tenant-mismatch"></a>Domein-tenant komt niet overeen

In de stroom Claimclaim geclaimde Partner of Record (CPOR) wordt u gevraagd om de tenant-id en het subdomein van de klant op te geven. Als er een foutbericht wordt weergegeven dat deze niet overeenkomen, neem dan contact op met uw klant om te controleren of u de juiste gegevens hebt.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Abonnementsfouten in de stroom van de CPOR-associatieclaim

In de stroom van de CPOR-associatieclaim wordt u mogelijk gevraagd een abonnement op te geven voor een product dat u probeert te claimen via Business Applications (Dynamics 365). We vragen om het abonnement omdat we dynamisch controleren of het product en het abonnement behoren tot de tenant die wordt geclaimd. We controleren ook of het abonnement actief is/de respijtstatus heeft.

Als u de foutmelding ontvangt, kan dit verschillende oorzaken hebben:

- Het geselecteerde product bestaat niet in de tenant van de klant
- Het opgegeven abonnement is niet voor Dynamics
- Het opgegeven abonnement is niet voor CSP
- De klant heeft de producten voor dat abonnement nog niet geactiveerd/ingericht
- Het abonnement is al geclaimd
- De opgegeven id is geen abonnements-id

Als u een vraag hebt over de juistheid van uw abonnement, moet u met uw klant samenwerken om ervoor te zorgen dat het abonnement juist is en of u de juiste tenant-id gebruikt.

Als het probleem met deze route niet is opgelost, neem dan contact op met [de ondersteuning](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Wanneer abonnementen beschikbaar zijn om te claimen

Wanneer u claimt voor een abonnement, ontvangt u een foutmelding als het abonnement nog niet is ingericht. Er zijn verschillende stappen die de klant moet nemen om het abonnement beschikbaar te maken voor het CPOR-platform om het op te halen en beschikbaar te maken om te claimen. Als u een foutmelding krijgt bij het claimen van een abonnement, neem dan contact op met uw klant om te controleren of het is ingericht en of het abonnement dat u claimt, juist is. Neem contact op met ondersteuning als u deze route al [hebt genomen.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="which-activity-do-i-choose"></a>Welke activiteit kies ik?

Het CPOR-claimplatform maakt CPOR-associatieclaims mogelijk die betrekking hebben op Business Applications en Microsoft 365 oplossingsgebieden. Hieronder vindt u de activiteiten die van toepassing zijn op elk oplossingsgebied. Selecteer de juiste activiteit op basis van de beschrijvingen om te voorkomen dat deze in de toekomst opnieuw moet worden vrijgevorderd. Claimen met een onjuiste activiteit kan leiden tot gemiste geschiktheid en beloningsverdiensten.


| Gebied waarvoor de oplossing geldt | Activiteit | Van toepassing op |
| ------ | ----------- | ----------- |
| Zakelijke toepassingen      | Voorverkoop   | Selecteer of u de aankoop van een in aanmerking komend product hebt beïnvloed en of u zich wilt aanmelden voor incentives voor pre-sale. Deze optie is alleen van toepassing als de klant deze producten heeft gekocht via een volumelicentieovereenkomst of Web-Direct. |
|    |  Gebruik  | Selecteer of u de acceptatie en het gebruik van een in aanmerking komende workload aand rijt en u wilt solliciteren op gebruikspriprisers. Deze optie is alleen van toepassing als de klant deze producten heeft gekocht via een volumelicentieovereenkomst of Web-Direct. |
|    | Revenue Association   | Selecteer of u de selectie van een in aanmerking komend product als zakelijke beïnvloeder hebt beïnvloed. Deze optie is alleen voor inkomstenorganisatie, niet voor incentive-betalingen. Deze optie is alleen van toepassing als de klant deze producten heeft gekocht via een volumelicentieovereenkomst of Web-Direct.   |
| Microsoft 365   | Gebruik   | Selecteer of u de acceptatie en het gebruik van een in aanmerking komende workload aand rijt en u wilt solliciteren op gebruikspriprisers. |

## <a name="which-mpn-do-i-choose"></a>Welke MPN kies ik?

In de stroom van de CPOR-associatieclaim wordt u gevraagd om een MPN van het bedrijf te kiezen die moet worden gekoppeld aan het werk dat u claimt bij de eindklant. Uw bedrijf heeft mogelijk veel MPN's, waarvan sommige zijn ingeschreven bij incentive-programma's en andere gekoppeld aan een partnertype zoals FRP FastTrack. De stroom van de CPOR-associatieclaim identificeert welke MPN's zijn ingeschreven in een incentive-programma, maar het laat u niet weten of het een specifiek partnertype MPN is. Het is belangrijk om de juiste MPN te selecteren, om te voorkomen dat u dit in de toekomst opnieuw moet claimen. Claimen met een onjuiste MPN kan leiden tot gemiste geschiktheid en incentive-inkomsten.

Als u niet weet welke MPN u moet gebruiken, neem dan contact op met uw globale beheerder.

Als de MPN die u wilt gebruiken niet is geregistreerd, kunt u dat beheren op het tabblad [Incentives-overzicht](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (aanmelden vereist).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Een product kiezen versus een abonnement invoeren

Wanneer een Dynamics-product wordt geclaimd en goedgekeurd, kan de partner de abonnements-id weergeven in de CPOR-associatieclaim zelf. Wanneer dit abonnement wordt geclaimd, is het actief of heeft deze de respijtstatus, maar het kan een tijd duren wanneer het abonnement wordt beëindigd en de nieuwe abonnementen moeten worden geclaimd in een afzonderlijke CPOR-claim.

## <a name="competing-claims"></a>Concurrerende claims

Als u een CPOR-associatieclaim maakt voor een klant en hun product(en) die al aan een andere partner zijn gekoppeld, wordt uw claim geseed tegen de arbiteratie:

1. Nadat u een nieuwe klantkoppeling hebt gemaakt, verifieert Microsoft de details van de koppeling en de aangeleverde PoE om de nauwkeurigheid van de informatie te garanderen.

2. Als u en een andere partner dezelfde klant en product/workload claimen, bekijkt Microsoft de documentatie over het bewijs van uitvoering van elke partner om te bepalen welke partner moet worden goedgekeurd.

3. Er kan aanvullende informatie worden aangevraagd bij beide partners, wat kan leiden tot vertragingen bij het verwerken van uw associatieaanvraag.

4. Uw CPOR-associatieclaim wordt nog steeds binnen vijf werkdagen  beoordeeld, hoewel de status ervan mogelijk langer wordt beoordeeld als Beoordeling. Dit scenario kan zich voor doen wanneer Microsoft werkt met de partner die momenteel eigenaar is van het product/de workload. Als dat het geval is, wordt u hiervan op de hoogte gesteld in de sectie met opmerkingen van uw claim. 

>[!IMPORTANT]
>Als we aanvullende informatie nodig hebben om te controleren of uw CPOR-association proof of execution (PoE) is uitgevoerd, nemen we contact met u op via de sectie Opmerkingen bij CPOR-associatieclaims.

## <a name="next-steps"></a>Volgende stappen

- [Aan de slag gaan met Incentives](incentives-get-started-intro.md)
