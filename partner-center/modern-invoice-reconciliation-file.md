---
title: Bestandsvelden opnieuw configureren voor een een time-aankoop van CSP
ms.topic: conceptual
ms.date: 01/29/2021
description: Meer informatie over alle items in uw CSP-afstemmingsbestand voor een een time-aankoop in Partner Center, inclusief voorbeeldwaarden.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: d5d404519c107a3e1f0e926451eef4935c993fbd
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957502"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP-bestandsvelden voor een een time-aankoopafstemming

**Juiste rollen:** Accountbeheerder | Factureringsagent

## <a name="using-the-recon-file"></a>Het recon-bestand gebruiken
In de onderstaande tabel vindt u beschrijvingen en voorbeeldwaarden voor de velden in het afstemmingsbestand voor een een time-purchases van CSP.

Zie De afstemmingsbestanden gebruiken voor meer informatie [over afstemmingsbestanden.](use-the-reconciliation-files.md)

| Kolom | Beschrijving | Voorbeeldwaarde |
| ------ | ----------- | ------------ |
| PartnerId | Unieke id in GUID-indeling voor een specifieke factureringsentiteit. Niet vereist voor afstemming. Hetzelfde in alle rijen. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Unieke Microsoft-id voor de klant in GUID-indeling. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | De organisatienaam van de klant, zoals gerapporteerd in Partner Center. Deze kolom is belangrijk voor het afstemmen van de factuur met uw systeemgegevens. | *Johnny Modern Cust DE2* |
| CustomerDomainName | Domeinnaam van de klant. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | Het land waar uw klant zich bevindt. Bekijk de volledige [lijst met landen voor](./regional-authorization-overview.md) uw regio.  | *DE* |
| InvoiceNumber | Het factuurnummer dat is gekoppeld aan het afstemmingsbestand.  | *G002297372* |
| MpnId | MPN-id van de CSP-partner. Zie itemeren per partner voor [meer informatie.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | MPN-id van de wederverkoper van de record voor het abonnement. | *6048879* |
| OrderId | Unieke id voor een order in het Microsoft-factureringsplatform. Kan handig zijn om de volgorde te identificeren wanneer u contact opstelt met de ondersteuning. Niet gebruikt voor afstemming. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | De datum in UTC waarop de order is geplaatst. | *10/3/2020* |
| ProductId | De unieke id van het product. | *DZH318Z0BNZ5* |
| SkuId | De unieke SKU-id. | *006G* |
| AvailabilityId | De unieke beschikbaarheids-id. | *DZH318Z08B80* |
| SkuName | De SKU-naam. | *Tabellen - LRS* |
| ProductName | De productnaam. | *Tabellen* |
| ChargeType | Het [type kosten of](./recon-file-charge-types.md) correctie. | *Nieuw* |
| UnitPrice | Prijs per licentie, zoals gepubliceerd in de prijslijst op het moment van aankoop. Zorg ervoor dat dit overeenkomt met de informatie die tijdens de afstemming in uw factureringssysteem is opgeslagen. | *0.045* |
| Aantal | Het aantal licenties. Zorg ervoor dat dit overeenkomt met de informatie die tijdens de afstemming in uw factureringssysteem is opgeslagen. | *1* |
| Subtotaal | Totaal vóór belasting. Het subtotaal moet gelijk zijn aan de factureerbare hoeveelheid vermenigvuldigd met de effectieve eenheidsprijs. | *0* |
| TaxTotal | Btw-bedrag. Op basis van de belastingregels en specifieke omstandigheden van uw markt. | *0* |
| Totaal | Het totale bedrag is gelijk aan het subtotaal plus het belastingbedrag. | *0* |
| Valuta | Uw factuur wordt gegenereerd in de context van de valuta van de klant. Dit betekent dat als u een partner bent die met klanten van verschillende factureerbare valuta's omteert, u een factuur ontvangt voor elk type klantvaluta.  | *EUR* |
| PriceAdjustmentDescription | De redenen voor de aanpassingen in de eenheidsprijs. Dit zijn de belangrijkste redenen, maar niet beperkt tot het bepalen van de effectieve eenheidsprijs. | *["15,0% partnertegoed voor beheerde services"]* |
| PublisherName | Publisher van het product.  | *Microsoft* |
| PublisherId | Een unieke id die de Partner Center gebruikt om de uitgever te identificeren. | *NA* |
| SubscriptionDescription | De naam van de serviceaanbieding die door de klant is gekocht, zoals gedefinieerd in de prijslijst. Deze kolom is een identiek veld als OfferName. | *Azure-abonnement* |
| SubscriptionId | Unieke id voor een abonnement in het Microsoft-factureringsplatform. Niet gebruikt voor afstemming. Houd er rekening mee dat deze id niet hetzelfde is als de abonnements-id in de beheerconsole van de partner. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | De datum waarop de factureringsperiode van een abonnement begint. | *9/1/2020* |
| ChargeEndDate | De datum waarop de factureringsperiode van een abonnement eindigt. | *9/30/2020* |
| TermAndBillingCycle | De duur van de toezegging om door te gaan met het abonnement op het moment van aankoop. | *Opgeslagen gegevens (GB/maand)* |
| EffectiveUnitPrice | De prorated unit price om de kosten voor de factureringscyclus te berekenen. Kortingen, aanpassingen in factureringsdagen en andere factoren bepalen de effectieve eenheidsprijs. Zie Effectieve berekening van [eenheidsprijs voor meer informatie.](./effective-unit-price-calculation.md)  | *0.03825* |
| UnitType | Het type eenheid waarin de meter in rekening wordt gebracht. | *1 GB/maand* |
| AlternateId | De alternatieve id van het orderregelitem waarnaar wordt verwezen. | *6dc5c039750a* |
| BillableQuantity | De totale hoeveelheid die wordt gefactureerd.  | *0.005001* |
| BillingFrequency | Het factureringsplan dat is geselecteerd op het moment van aankoop. | *NA*  |
| PricingCurrency | De valuta in de prijslijst. | *USD* |
| PCToBCExchangeRate | De wisselkoers die wordt toegepast op de prijsvaluta op de factureringsvaluta. | *0.846202666* |
| PCToBCExchangeRateDate | De datum waarop de prijsvaluta voor de factureringsvaluta wordt bepaald. | *9/30/2020* |
| MeterDescription | Meterbeschrijving.  | *Tabellen - LRS Data Stored (GB/maand)* |
| ReservationOrderId | De reserveringsorder-id. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | De beschrijving van het tegoed. | *Azure-verbruikstegoed* |
| SubscriptionStartDate | De datum waarop een abonnement wordt aangeschaft. | *5/1/2021* |
| SubscriptionEndDate | De datum waarop een abonnement verloopt. | *4/30/2022* |
| ReferenceID | De koppeling naar alle transacties die plaatsvinden tijdens upgrades. | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | De id voor invoeg- of proefversieaankopen. | *["Invoeg-on"]* |
| PromotionID | De id die moet worden gebruikt om de gegevens van de promotie op te halen. | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>U kunt uw Azure-verbruik afstemmen in uw een-keer-aankoop recon-bestand. Ga hiervoor naar uw dagelijks beoordeelde gebruiks reconbestand en zoek naar uw SubscriptionID. Hiermee worden alle kosten weergegeven die zijn gekoppeld aan uw Azure-plan-id. Uw Azure SubscriptionID wordt weergegeven als de EntitlementID.
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>Het basisabonnement verbinden met het bijgewerkte abonnement

Gebruik de abonnements-id van het basisproduct om de bijbehorende referentie-id's te vinden en deze te gebruiken om alle gekoppelde transacties op te halen. In combinatie met de abonnements-id en referentie-id kunt u verbinding maken met alle upgrades die in één gebeurtenis zijn opgetreden.

## <a name="next-steps"></a>Volgende stappen

- [Facturering en belastingen](billing.md)
