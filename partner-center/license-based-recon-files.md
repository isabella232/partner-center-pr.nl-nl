---
title: Afstemmings bestanden op basis van licentie
ms.topic: article
ms.date: 05/18/2020
description: Meer informatie over het lezen van op licenties gebaseerde afstemmings bestanden in Partner Center. In dit artikel wordt uitgelegd wat de betekenis is van elk veld in het afstemmings bestand op basis van licentie.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 86581db73f1bf2b6660af45aca4747a5db779bbe
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/30/2020
ms.locfileid: "92527566"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Informatie over de velden in het Partner Center-afstemmings bestand op basis van licentie

**Van toepassing op**

- Partnercentrum
- Partner centrum voor Microsoft Cloud voor de Amerikaanse overheid

**Juiste rollen**
- Globale beheerder
- Gebruikersbeheerder
- Factureringsbeheerder
- Beheer agent

Als u uw wijzigingen wilt afstemmen op de orders van een klant, vergelijkt u de **Syndication_Partner_Subscription_Number** van het afstemmings bestand met de **abonnements-id** van het partner centrum.

## <a name="fields-in-license-based-reconciliation-files"></a>Velden in op licentie gebaseerde afstemmings bestanden

| Kolom | Beschrijving | Voorbeeldwaarde |
| ------ | ----------- | ------------ |
| Partner | De unieke id in de GUID-indeling voor een specifieke facturerings entiteit. Niet vereist voor afstemming. Hetzelfde in alle rijen. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Unieke micro soft-id voor de klant in GUID-indeling. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | De organisatie naam van de klant, zoals gerapporteerd in het partner centrum. *Zeer belang rijk veld voor het afstemmen van de factuur met de systeem gegevens.* | *Klant A testen* |
| MpnId | De MPN-id van de CSP-partner. Zie [hoe u kunt specificeren op partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | De MPN-id van de dealer van de record voor het abonnement.  |
| OrderId | De unieke id voor een order in het micro soft-factuur platform. Kan handig zijn om de volg orde te identificeren wanneer u contact opneemt met ondersteuning. Niet gebruikt voor afstemming. | *566890604832738111* |
| SubscriptionId | De unieke id voor een abonnement in het micro soft-factuur platform. Kan nuttig zijn bij het identificeren van het abonnement bij het maken van contact met ondersteuning. Niet gebruikt voor afstemming. *Deze waarde is niet hetzelfde als de **abonnements-id** in de partner beheer console. Zie **SyndicationPartnerSubscriptionNumber** in plaats daarvan.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | De unieke id voor abonnementen. Een klant kan meerdere abonnementen hebben voor hetzelfde abonnement. Deze kolom is belang rijk voor het afstemmen van de analyse van bestanden. Dit veld is gekoppeld aan de **abonnements-id** in de partner beheer console. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Unieke aanbiedings-id. Id van standaard aanbieding, zoals gedefinieerd in de prijs lijst. *Deze waarde komt niet overeen met de **aanbiedings-id** uit de prijs lijst. Zie **DurableOfferID** in plaats daarvan.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Unieke id van de duurzame aanbieding, zoals gedefinieerd in de prijs lijst. *Deze waarde komt overeen met de **aanbiedings-id** uit de prijs lijst.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | De naam van het service aanbod dat door de klant is aangeschaft, zoals gedefinieerd in de prijs lijst. | *Microsoft Office 365 (abonnement E3)* |
| Subscription | De begin datum van het abonnement. De tijd is altijd het begin van de dag, 0:00. Dit veld wordt ingesteld op de dag nadat de order is verzonden. Wordt gebruikt in combi natie met de **SubscriptionEndDate** om te bepalen: als de klant zich nog in het eerste jaar van het abonnement bevindt, of als het abonnement voor het volgende jaar is verlengd. | *2/1/2019 0:00* |
| SubscriptionEndDate | De eind datum van het abonnement. De tijd is altijd het begin van de dag, 0:00. *12 maanden plus **x** dagen na de begin datum* om te worden uitgelijnd met de factuur datum van de partner of *12 maanden na de vernieuwings datum* . Bij de verlenging worden de prijzen bijgewerkt naar de huidige prijs lijst. De communicatie van de klant is mogelijk vereist voordat de geautomatiseerde verlenging wordt verlengd. | *2/1/2019 0:00* |
| ChargeStartDate | Start dag van de kosten. De tijd is altijd het begin van de dag, 0:00. Wordt gebruikt voor het berekenen van dagelijkse kosten ( *pro rata* kosten) wanneer een klant licentie nummers wijzigt. | *2/1/2019 0:00* |
| ChargeEndDate | De einddag van de kosten. De tijd is altijd het einde van de dag, 23:59. Wordt gebruikt voor het berekenen van dagelijkse kosten ( *pro rata* kosten) wanneer een klant licentie nummers wijzigt. | *2/28/2019 23:59* |
| ChargeType | Het [type kosten](recon-file-charge-types.md) of correctie. | Zie [kosten typen](recon-file-charge-types.md). |
| UnitPrice | Prijs per licentie, zoals gepubliceerd in de pricelist op het moment van aankoop. Zorg ervoor dat dit overeenkomt met de informatie die is opgeslagen in uw facturerings systeem tijdens het afstemmen. | *6,82* |
| Aantal | Aantal licenties. Zorg ervoor dat dit overeenkomt met de informatie die is opgeslagen in uw facturerings systeem tijdens het afstemmen. | *2* |
| Aantal | Totaal van de prijs voor de hoeveelheid. Wordt gebruikt om te controleren of de berekenings hoeveelheid overeenkomt met de manier waarop u deze waarde voor uw klanten berekent. | *13,32* |
| TotalOtherDiscount | De kortings hoeveelheid die op deze kosten wordt toegepast. Product licenties die zijn opgenomen in een competentie of kaarten of nieuwe abonnementen die in aanmerking komen voor een stimulans, bevatten ook een kortings bedrag in deze kolom. | *2,32* |
| Subtotaal | Totaal voor belasting. Hiermee wordt gecontroleerd of uw subtotaal overeenkomt met het verwachte totaal, in het geval van een korting. | *11* |
| Btw | Kosten belasting bedrag. Op basis van de belasting regels van uw markt en specifieke omstandigheden. | *0* |
| TotalForCustomer | Totaal na belasting. Hiermee wordt gecontroleerd of BTW in rekening wordt gebracht op de factuur. | *11* |
| Valuta | Valuta type. Elke facturerings entiteit heeft slechts één valuta. Controleer of deze overeenkomt met uw eerste factuur. Controleer opnieuw op de belangrijkste updates van het facturerings platform. | *EUR* |
| DomainName | Domein naam van de klant. Dit veld kan leeg zijn tot de tweede facturerings cyclus. *Gebruik dit veld niet als een unieke id voor de klant. De klant/partner kan de Vanity of het standaard domein bijwerken via de Office 365-Portal.* | *example.onmicrosoft.com* |
| SubscriptionName | Bijnaam van abonnement. Als er geen bijnaam is opgegeven, maakt partner centrum gebruik van de **aanbieding** . | *PROJECT ONLINE* |
| SubscriptionDescription | De naam van het service aanbod dat door de klant is aangeschaft, zoals gedefinieerd in de prijs lijst. (Dit is een identiek veld voor de **aanbieding** .) | *PROJECT ONLINE PREMIUM ZONDER PROJECT-CLIENT* |
| BillingCycleType | Eenmalige facturerings frequentie.| *Maandelijks* |