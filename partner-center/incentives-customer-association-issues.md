---
title: Problemen met klantkoppeling Incentives
description: Meer informatie over het oplossen van problemen die zich voordoen bij het werken met CPOR-klant koppelingen (partner of record).
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 30639725c0a852046251e83c3791f56d788931c1
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179207"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemen met klant koppelingen met geclaimde partner of record (CPOR)

**Juiste rollen**

- Factureringsbeheerder
- Globale beheerder
- Prikkel beheerder

De onderstaande inhoud helpt u bij het oplossen van problemen die kunnen optreden wanneer u met klant koppelingen werkt.

## <a name="domain-tenant-mismatch"></a>Domein-Tenant komt niet overeen

U wordt gevraagd om de Tenant-ID en het subdomein van de klant op te geven in de claimed partner of record (CPOR)-koppelings stroom. Als er een fout bericht wordt weer gegeven dat ze niet overeenkomen, neemt u contact op met uw klant om te controleren of u de juiste gegevens hebt.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Abonnements fouten in de CPOR Association-koppelings stroom

In de claim stroom van de CPOR-koppeling wordt u mogelijk gevraagd om een abonnement te geven voor een product dat u wilt claimen via Business Applications (Dynamics 365). Er wordt om het abonnement gevraagd omdat er dynamisch wordt gecontroleerd of het product en het abonnement behoren tot de Tenant waarvoor wordt geclaimd. Er wordt ook gecontroleerd of het abonnement actief/in de respijt status is.

Als het fout bericht wordt weer gegeven, kan dit verschillende oorzaken hebben:

- Het geselecteerde product bestaat niet in de tenant van de klant
- Het gegeven abonnement is niet voor Dynamics
- Het opgegeven abonnement is niet voor CSP
- De klant heeft de producten voor dat abonnement nog niet geactiveerd/ingericht
- Het abonnement is al geclaimd
- De door gegeven id is geen abonnements-ID

Als u een vraag hebt over de nauw keurigheid van uw abonnement, werkt u samen met uw klant om te controleren of het abonnement juist is en of u de juiste Tenant-ID gebruikt.

Neem contact op met de [ondersteuning](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)als deze route het probleem nog niet heeft opgelost.

## <a name="when-subscriptions-will-be-available-to-claim"></a>Wanneer abonnementen kunnen worden claimd

Wanneer u een abonnement claimt, ontvangt u een fout melding als het abonnement nog niet is ingericht. Er zijn verschillende stappen die de klant nodig heeft om het abonnement beschikbaar te maken voor het CPOR-platform, zodat het kan worden opgehaald en beschikbaar wordt gemaakt om te worden claimen. Als er een fout optreedt bij het claimen van een abonnement, neemt u contact op met uw klant om te controleren of deze is ingericht en of het abonnement dat u claimt juist is. Als u deze route al hebt gemaakt, neemt u contact op met de [ondersteuning](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Welke activiteit moet ik kiezen?

Het CPOR-claim platform biedt CPOR-koppelings claims met betrekking tot Business Applications en Microsoft 365 oplossings gebieden. De activiteiten die van toepassing zijn op elk oplossings gebied staan hieronder. Selecteer de juiste activiteit op basis van de beschrijvingen om te voor komen dat u in de toekomst vrijmaakt. Claimen met een onjuiste activiteit kan leiden tot gemiste geschiktheid en winst van het prestatie verlies.


| Gebied waarvoor de oplossing geldt | Activiteit | Van toepassing voor |
| ------ | ----------- | ----------- |
| Zakelijke toepassingen      | Presale   | Selecteer deze optie als u de aankoop van een in aanmerking komend product hebt beïnvloed en u wilt Toep assen op prikkels voor de verkoop. Deze optie is alleen van toepassing als de klant deze producten heeft aangeschaft via een volume licentieovereenkomst of via web-direct. |
|    |  Gebruik  | Selecteer deze optie als u de acceptatie en het gebruik van een in aanmerking komende werk belasting aanstuurt en wilt Toep assen op gebruiks prikkels. Deze optie is alleen van toepassing als de klant deze producten heeft aangeschaft via een volume licentieovereenkomst of via web-direct. |
|    | Opbrengst koppeling   | Selecteer deze optie als u de selectie van een in aanmerking komend product hebt beïnvloed als een bedrijfs impact. Deze optie is alleen voor opbrengst koppeling, niet voor het stimuleren van betalingen. Deze optie is alleen van toepassing als de klant deze producten heeft aangeschaft via een volume licentieovereenkomst of via web-direct.   |
| Microsoft 365   | Gebruik   | Selecteer deze optie als u de acceptatie en het gebruik van een in aanmerking komende werk belasting aanstuurt en wilt Toep assen op gebruiks prikkels. |

## <a name="which-mpn-do-i-choose"></a>Welke MPN moet ik kiezen?

In de claim stroom van de CPOR-koppeling wordt u gevraagd om een MPN te kiezen die moet worden gekoppeld aan het werk dat u aanvraagt voor de eind klant. Uw bedrijf heeft mogelijk veel MPNs, waarvan sommige zijn Inge schreven in prikkel Programma's en anderen die zijn gekoppeld aan een partner type zoals FRP FastTrack. De CPOR Association-claim stroom identificeert welke MPNs zijn geregistreerd in een prestatie programma, maar laat u niet weten of het een specifiek partner type MPN is. Het is belang rijk om de juiste MPN te selecteren om te voor komen dat u in de toekomst vrijmaakt. Claimen met een onjuiste MPN kan leiden tot gemiste geschiktheid en winst van het prestatie verlies.

Als u niet weet welke MPN u moet gebruiken, neemt u contact op met uw globale beheerder.

Als de MPN die u wilt gebruiken, niet is inge schreven, kunt u deze beheren op het [tabblad Overzicht van prikkels](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (aanmelden vereist).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Een product kiezen versus een abonnement invoeren

Wanneer een Dynamics-product wordt geclaimd en goedgekeurd, kan de partner de abonnements-ID weer geven in de CPOR-koppelings claim zelf. Wanneer dit abonnement wordt geclaimd, bevindt het zich in een actief of in respijt status, maar er is mogelijk een tijd waarop het abonnement eindigt en de nieuwe abonnementen moeten worden geclaimd in een afzonderlijke CPOR-koppeling.

## <a name="competing-claims"></a>Concurrerende claims

Als u een claim voor een CPOR maakt voor een klant en hun product (en) die al aan een andere partner is gekoppeld, gaat u door naar arbitrage:

1. Nadat u een nieuwe klantkoppeling hebt gemaakt, verifieert Microsoft de details van de koppeling en de aangeleverde PoE om de nauwkeurigheid van de informatie te garanderen.

2. Als u en een andere partner claimen voor dezelfde klant en product/werk belasting, zal micro soft de documentatie voor de uitvoering van elke partner door nemen om te bepalen welke partner moet worden goedgekeurd.

3. Er kan meer informatie worden gevraagd van beide partners, wat kan leiden tot vertragingen bij het verwerken van uw koppelings aanvraag.

4. Uw CPOR-koppelings claim wordt binnen vijf werk dagen nog steeds gecontroleerd, hoewel de status ervan gedurende een langere periode in de _beoordeling_ kan blijven. Dit scenario kan zich voordoen wanneer micro soft werkt met de partner die momenteel eigenaar is van het product/de werk belasting. Als dat het geval is, ontvangt u een melding in het gedeelte met opmerkingen van uw claim. 

>[!IMPORTANT]
>Als we aanvullende informatie nodig hebben om uw CPOR Association-koppelings bewijs (PoE) te verifiëren, nemen we contact met u op via de sectie CPOR Association claim opmerkingen.

## <a name="next-steps"></a>Volgende stappen

- [Aan de slag gaan met Incentives](incentives-get-started-intro.md)
