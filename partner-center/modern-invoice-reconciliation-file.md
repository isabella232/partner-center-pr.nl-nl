---
title: Bestands velden afstemmen voor eenmalige inkopen CSP
ms.topic: conceptual
ms.date: 01/29/2021
description: Meer informatie over alle artikelen op uw CSP-afstemmings bestand voor eenmalige aankopen in het partner centrum, inclusief voorbeeld waarden.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: f1606cceaf9dec1f04850fd85b3924ef75bbfda0
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098802"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Eenmalige CSP-velden voor het afstemmen van inkopen

## <a name="using-the-recon-file"></a>Het afstemmings bestand gebruiken
De onderstaande tabel bevat beschrijvingen en voorbeeld waarden voor de velden in het afstemmings bestand voor eenmalige inkopen van CSP.

Zie [reconciliatie bestanden gebruiken](use-the-reconciliation-files.md)voor meer informatie over het afstemmen van bestanden.

| Kolom | Beschrijving | Voorbeeldwaarde |
| ------ | ----------- | ------------ |
| Partner | De unieke id in de GUID-indeling voor een specifieke facturerings entiteit. Niet vereist voor afstemming. Hetzelfde in alle rijen. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Unieke micro soft-id voor de klant in GUID-indeling. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Organisatie naam van de klant zoals gerapporteerd in het partner centrum. Deze kolom is belang rijk voor het afstemmen van de factuur met uw systeem gegevens. | *Modern verkoop DE2 in Johnny* |
| CustomerDomainName | Domein naam van de klant. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Het land waar de klant zich bevindt. Bekijk de volledige [lijst met landen](./regional-authorization-overview.md) voor uw regio.  | *NORMALIS* |
| InvoiceNumber | Het factuur nummer dat is gekoppeld aan het afstemmings bestand.  | *G002297372* |
| MpnId | De MPN-id van de CSP-partner. Zie [How to specificeren op partner](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)voor meer informatie. | *6034453* |
| ResellerMpnId | De MPN-id van de dealer van de record voor het abonnement. | *6048879* |
| OrderId | De unieke id voor een order in het micro soft-factuur platform. Kan handig zijn om de volg orde te identificeren wanneer u contact opneemt met ondersteuning. Niet gebruikt voor afstemming. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | De datum waarop de bestelling is geplaatst. | *10/3/2020* |
| ProductId | De unieke id van het product. | *DZH318Z0BNZ5* |
| SkuId | De unieke id van de SKU. | *006G* |
| AvailabilityId | De unieke id van de beschik baarheid. | *DZH318Z08B80* |
| SkuName | De naam van de SKU. | *Tables-LRS* |
| ProductName | De product naam. | *Tabellen* |
| ChargeType | Het [type kosten](./recon-file-charge-types.md) of correctie. | *Nieuw* |
| UnitPrice | Prijs per licentie, zoals gepubliceerd in de prijs lijst, op het moment van aankoop. Zorg ervoor dat dit overeenkomt met de informatie die is opgeslagen in uw facturerings systeem tijdens het afstemmen. | *0,045* |
| Aantal | Het aantal licenties. Zorg ervoor dat dit overeenkomt met de informatie die is opgeslagen in uw facturerings systeem tijdens het afstemmen. | *1* |
| Subtotaal | Totaal voor belasting. Het subtotaal moet gelijk zijn aan het factureer bare aantal vermenigvuldigd met de werkelijke eenheids prijs. | *0* |
| TaxTotal | Kosten belasting bedrag. Op basis van de belasting regels van uw markt en specifieke omstandigheden. | *0* |
| Totaal | De totale hoeveelheid is gelijk aan het subtotaal plus het BTW-bedrag. | *0* |
| Valuta | Uw factuur wordt gegenereerd in de context van de valuta van de klant. Dit betekent dat als u een partner bent die gebruikmaakt van klanten uit verschillende factureer bare valuta's, een factuur ontvangt voor elk type valuta van de klant.  | *EUR* |
| PriceAdjustmentDescription | De redenen voor de aanpassingen van de eenheids prijs. Dit zijn de belangrijkste redenen, maar niet beperkt tot het bepalen van de werkelijke eenheids prijs. | *["15,0% de partner heeft creditering voor services beheerd"]* |
| PublisherName | Uitgever van het product.  | *Microsoft* |
| PublisherId | Een unieke id die het partner centrum gebruikt om de uitgever te identificeren. | *NA* |
| SubscriptionDescription | De naam van het service aanbod dat door de klant is aangeschaft, zoals gedefinieerd in de prijs lijst. Deze kolom is een identiek veld voor de naam van de aanbieding. | *Azure-abonnement* |
| SubscriptionId | De unieke id voor een abonnement in het micro soft-factuur platform. Niet gebruikt voor afstemming. Houd er rekening mee dat deze id niet hetzelfde is als de abonnements-ID in de partner beheer console. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | De datum waarop het partner centrum de abonnements kosten in rekening brengt. Als het abonnement is gekocht met een jaarlijkse facturerings periode en een maandelijks facturerings abonnement, is dit de dag waarop het abonnement is gekocht. Met ingang van het volgende afstemmings bestand wordt het aantal 30 dagen verhoogd. | *9/1/2020* |
| ChargeEndDate | De einddag van de kosten voor de facturerings cyclus van het abonnement. Als het abonnement is gekocht met een jaarlijkse facturerings periode en een maandelijks facturerings plan, is dit de 30e dag nadat het abonnement is gekocht. Met ingang van het volgende afstemmings bestand wordt het aantal 30 dagen verhoogd. | *9/30/2020* |
| TermAndBillingCycle | De duur van de toezeg ging om het abonnement te blijven op het moment van aankoop. | *Opgeslagen gegevens (GB/maand)* |
| EffectiveUnitPrice | De eenheids prijs in rekening gebracht voor het berekenen van de kosten voor de facturerings cyclus. Kortingen, aanpassingen in facturerings dagen en andere factoren bepalen de werkelijke eenheids prijs. Zie [effectief eenheids prijs berekenen](./effective-unit-price-calculation.md)voor meer informatie.  | *0,03825* |
| Unit type | Het type eenheid waarin de meter wordt gefactureerd. | *1 GB/maand* |
| AlternateId | De alternatieve ID van het order regel item waarnaar wordt verwezen. | *6dc5c039750a* |
| BillableQuantity | De totale hoeveelheid die wordt gefactureerd.  | *0,005001* |
| BillingFrequency | Het facturerings abonnement dat is geselecteerd op het moment van aankoop. | *NA*  |
| PricingCurrency | De valuta in de prijslijst. | *USD* |
| PCToBCExchangeRate | De wissel koers die wordt toegepast voor prijs valuta voor facturerings valuta. | *0,846202666* |
| PCToBCExchangeRateDate | De datum waarop de prijs valuta naar de facturerings valuta wordt bepaald. | *9/30/2020* |
| MeterDescription | Beschrijving van meter.  | *Tabellen-LRS opgeslagen gegevens (GB/maand)* |
| ReservationOrderId | De reserverings order-id. | *E21A6344E398FFC1C4D7...* |

>[!NOTE]
>U kunt uw Azure-verbruik in uw eenmalige aankoop afstemmings bestand afstemmen. Ga hiervoor naar het afstemmings bestand van het dagelijks geclassificeerde gebruik en zoek naar uw abonnement op. Hiermee worden alle kosten weer gegeven die zijn gekoppeld aan uw Azure plan-ID. Uw Azure SubscriptionID wordt weer gegeven als de EntitlementID.

## <a name="next-steps"></a>Volgende stappen

- [Facturering en belastingen](billing.md)