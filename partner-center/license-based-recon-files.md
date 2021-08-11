---
title: Afstemmingsbestanden op basis van licentie
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Meer informatie over het lezen van op licenties gebaseerde afstemmingsbestanden in Partner Center. In dit artikel wordt de betekenis van elk veld in uw op licenties gebaseerde reconbestand uitgelegd.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7bb6900ba34c99d497d8273e56e6385aa3bf55690c8729526a5e4c6a1e60ba28
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694129"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Inzicht in de velden in Partner Center op licenties gebaseerde afstemmingsbestanden

**Van toepassing op**: Partner Center | Partner Center voor Microsoft Cloud for US Government

**Juiste rollen:** Globale | Gebruikersbeheerbeheer | Factureringsbeheerders | Beheeragent

Als u uw wijzigingen wilt afstemmen  op de orders van een klant, vergelijkt u de Syndication_Partner_Subscription_Number uit het afstemmingsbestand met de abonnements-id van Partner Center. 

## <a name="fields-in-license-based-reconciliation-files"></a>Velden in op licenties gebaseerde afstemmingsbestanden

| Kolom | Beschrijving | Voorbeeldwaarde |
| ------ | ----------- | ------------ |
| PartnerId | Unieke id in GUID-indeling voor een specifieke factureringsentiteit. Niet vereist voor afstemming. Hetzelfde in alle rijen. | *8ddd03642-test-test-46b58d356b4e* |
| CustomerId | Unieke Microsoft-id voor de klant in GUID-indeling. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | De organisatienaam van de klant, zoals vermeld in Partner Center. *Zeer belangrijk veld voor het afstemmen van de factuur met uw systeemgegevens.* | *Test klant A* |
| MpnId | MPN-id van de CSP-partner. Zie [hoe u kunt itemeren op partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMpnId | MPN-id van de wederverkoper van record voor het abonnement.  |
| OrderId | Unieke id voor een bestelling in het Microsoft-factureringsplatform. Kan handig zijn om de volgorde te identificeren wanneer u contact opstelt met de ondersteuning. Niet gebruikt voor afstemming. | *566890604832738111* |
| SubscriptionId | Unieke id voor een abonnement in het Microsoft-factureringsplatform. Kan handig zijn om het abonnement te identificeren wanneer u contact op met de ondersteuning opzegt. Niet gebruikt voor afstemming. *Deze waarde is niet hetzelfde als de **abonnements-id** in de beheerconsole van de partner. Zie in **plaats daarvan SyndicationPartnerSubscriptionNumber.*** | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Unieke id voor abonnementen. Een klant kan meerdere abonnementen voor hetzelfde abonnement hebben. Deze kolom is belangrijk voor afstemmingsbestandsanalyse. Dit veld wordt toe te staan **aan de abonnements-id** in de beheerconsole van de partner. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Unieke aanbiedings-id. Standaardaanbiedings-id, zoals gedefinieerd in de prijslijst. *Deze waarde komt niet overeen met **de aanbiedings-id** uit de prijslijst. Zie **in plaats daarvan DurableOfferID.*** | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | Unieke duurzame aanbiedings-id, zoals gedefinieerd in de prijslijst. *Deze waarde komt overeen met **de aanbiedings-id** uit de prijslijst.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | De naam van de serviceaanbieding die door de klant is gekocht, zoals gedefinieerd in de prijslijst. | *Microsoft Office 365 (Abonnement E3)* |
| SubscriptionStartDate | De begindatum van het abonnement in UTC. De tijd is altijd het begin van de dag, 0:00. Dit veld wordt ingesteld op de dag nadat de order is verzonden. Wordt gebruikt met **de SubscriptionEndDate** om te bepalen of de klant zich nog steeds binnen het eerste jaar van het abonnement of voor het volgende jaar heeft verlengd. | *2/1/2019 0:00* |
| SubscriptionEndDate | De einddatum van het abonnement in UTC. De tijd is altijd het begin van de dag, 0:00. *12 maanden plus x **dagen*** na de begindatum om af te stemmen met de factureringsdatum van de partner of 12 maanden vanaf *de verlengingsdatum.* Bij verlenging worden de prijzen bijgewerkt naar de huidige prijslijst. Communicatie van de klant is mogelijk vereist voor automatische verlenging. | *2/1/2019 0:00* |
| ChargeStartDate | Begindag van de kosten. De tijd is altijd het begin van de dag, 0:00. Wordt gebruikt om de dagelijkse kosten *(pro rata kosten) te* berekenen wanneer een klant de licentienummers wijzigt. | *2/1/2019 0:00* |
| ChargeEndDate | Einddag van de kosten. De tijd is altijd het einde van de dag, 23:59. Wordt gebruikt om de dagelijkse kosten *(pro rata kosten) te* berekenen wanneer een klant de licentienummers wijzigt. | *2/28/2019 23:59* |
| ChargeType | Het [type kosten of](recon-file-charge-types.md) correctie. | Zie [Kostentypen.](recon-file-charge-types.md) |
| UnitPrice | Prijs per licentie, zoals gepubliceerd in de prijslijst op het moment van aankoop. Zorg ervoor dat deze overeenkomt met de gegevens die tijdens de afstemming zijn opgeslagen in uw factureringssysteem. | *6.82* |
| Aantal | Aantal licenties. Zorg ervoor dat deze overeenkomt met de gegevens die tijdens de afstemming zijn opgeslagen in uw factureringssysteem. | *2* |
| Bedrag | Totaal van prijs voor hoeveelheid. Wordt gebruikt om te controleren of de berekening van het bedrag overeenkomt met de manier waarop u deze waarde voor uw klanten berekent. | *13.32* |
| TotalOtherDiscount | De hoeveelheid korting die op deze kosten wordt toegepast. Productlicenties die zijn opgenomen in een competentie of MAPS, of nieuwe abonnementen die in aanmerking komen voor een incentive, bevatten ook een kortingsbedrag in deze kolom. | *2.32* |
| Subtotaal | Totaal vóór belasting. Controleert of uw subtotaal overeenkomt met het verwachte totaal, in het geval van korting. | *11* |
| Btw | Btw-bedrag. Op basis van de belastingregels en specifieke omstandigheden van uw markt. | *0* |
| TotalForCustomer | Totaal na belasting. Controleert of er belasting in rekening wordt gebracht op de factuur. | *11* |
| Valuta | Valutatype. Elke factureringsentiteit heeft slechts één valuta. Controleer of deze overeenkomt met uw eerste factuur. Controleer het opnieuw na belangrijke updates voor het factureringsplatform. | *EUR* |
| DomainName | Domeinnaam van de klant. Dit veld kan leeg zijn tot de tweede factureringscyclus. *Gebruik dit veld niet als een unieke id voor de klant. De klant/partner kan het vanity- of standaarddomein bijwerken via Office 365 portal.* | *example.onmicrosoft.com* |
| SubscriptionName | Bijnaam van abonnement. Als er geen bijnaam is opgegeven, Partner Center de **OfferName gebruikt.** | *PROJECT ONLINE* |
| SubscriptionDescription | De naam van de serviceaanbieding die door de klant is gekocht, zoals gedefinieerd in de prijslijst. (Dit is een identiek veld als **OfferName.)** | *PROJECT ONLINE PREMIUM ZONDER PROJECTCLIENT* |
| BillingCycleType | Een frequentie voor een facturering.| *Maandelijks* |
