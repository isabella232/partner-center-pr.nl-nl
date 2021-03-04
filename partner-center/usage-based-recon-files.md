---
title: Afstemmings bestanden op basis van gebruik
ms.topic: article
ms.date: 06/08/2020
description: Meer informatie over alle items in uw op gebruik gebaseerd afstemmings bestand in partner centrum. Bevat enkele voor beelden.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d3941d09d6ec808f3d188521c4f0c51c9a6d0222
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755761"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Informatie over het afstemmen van op gebruik gebaseerde bestanden en hun specifieke velden in partner centrum

Van toepassing op:

- Partnercentrum
- Partnercentrum voor Microsoft Cloud for US Government

**Juiste rollen**

- Accountbeheerder
- Factureringsbeheerder

Als u uw kosten wilt afstemmen op het gebruik van de klant, vergelijkt u de **ResellerID**, de naam van de **verkoper** en **ResellerBillableAccount** uit het afstemmings bestand met de **klant** **-en abonnements-id** van het partner centrum.

## <a name="fields-in-usage-based-reconciliation-files"></a>Velden in afstemmings bestanden op basis van gebruik

In de volgende velden wordt uitgelegd welke services zijn gebruikt en wat het aantal is.

| Kolom | Beschrijving | Voorbeeld waarde (n) |
| ------ | ----------- | ------------ |
| Partner | Partner-id, in GUID-indeling. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Naam van de partner. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Partner account-id. | *1010578050* |
| CustomerCompanyName | De organisatie naam van de klant, zoals gerapporteerd in het partner centrum. *Zeer belang rijk voor het afstemmen van de factuur met uw systeem gegevens.* | *Test klant* |
| MpnId | De MPN-id van de CSP-partner. | *4390934* |
| ResellerMpnId | De MPN-id van de dealer van de record voor het abonnement.  |
| InvoiceNumber | Factuur nummer waar de opgegeven trans actie wordt weer gegeven. | *D020001IVK* |
| ChargeStartDate | De begin datum van de facturerings cyclus, behalve bij het presen teren van eerder niet-gefactureerde geposte gebruiks gegevens (van de vorige factuur cyclus). De tijd is altijd het begin van de dag, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | De eind datum van de facturerings cyclus, behalve wanneer de datums van eerder niet-gefactureerde onkosten worden weer gegeven (vanaf de vorige factuur cyclus). De tijd is altijd het einde van de dag, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | De unieke id voor een abonnement in het micro soft-factuur platform. Kan nuttig zijn bij het identificeren van het abonnement bij het maken van contact met ondersteuning. Niet gebruikt voor afstemming. *Dit is niet hetzelfde als de **abonnements-id** in de partner beheer console.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Bijnaam voor de service aanbieding. | *Microsoft Azure* |
| SubscriptionDescription | Line-of-Business van de service aanbieding. | *Microsoft Azure* |
| OrderID | De unieke id voor een order in het micro soft-factuur platform. Kan nuttig zijn bij het identificeren van het abonnement bij het maken van contact met ondersteuning. Niet gebruikt voor afstemming. | *566890604832738111* |
| ServiceName | De naam van de betreffende Azure-service. | *VIRTUELE MACHINES* |
| ServiceType | Het specifieke type van de Azure-service. | *Service Bus: persoonlijk of pakket*, *SQL Azure Data Base – Business of Web Edition* |
| ResourceGuid | Specifieke unieke id voor alle service gegevens en prijs structuur. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | De naam van de Azure-resource. | *Gegevensoverdracht in (GB)*, *gegevensoverdracht uit (GB)* |
| Region | De regio waarop het gebruik van toepassing is. Wordt hoofd zakelijk gebruikt voor het toewijzen van tarieven aan gegevens overdrachten, omdat tarieven per regio verschillen. | *Azië en Stille Oceaan*, *Europa*, *Latijns-Amerika*, *Noord-Amerika* |
| Sku | De unieke micro soft-id voor een aanbieding. | *7UD-00001* |
| DetailLineItemId | Een id en hoeveelheid voor het specificeren van verschillende tarieven voor een service of resource in een bepaalde facturerings periode. Voor Azure-gelaagde prijzen kan er één tarief zijn voor Maxi maal een bepaald aantal factureer bare eenheden, en daarna een ander tarief na dat aantal. | *1* |
| ConsumedQuantity | De hoeveelheid verbruikte Services (zoals uren of GB) tijdens de rapportage periode. Omvat ook niet-gefactureerd gebruik uit eerdere rapportage perioden. | *11* |
| IncludedQuantity | Eenheden die deel uitmaken van de aanbieding. Doorgaans niet aanwezig in CSP. | *0* |
| OverageQuantity | Eenheden die niet zijn opgenomen als onderdeel van de aanbieding. Deze moeten worden betaald door de partner. Gelijk aan **ConsumedQuantity** min **IncludedQuantity**. | *11* |
| ListPrice | De aanbiedings prijs van kracht op de begin datum van het abonnement. | *$0,0808* |
| PretaxCharges | Gelijk aan **ListPrist** vermenigvuldigd met **OverageQuantity**, afgerond op het dichtstbijzijnde cent. | *$0,085* |
| TaxAmount | Kosten belasting bedrag. Op basis van de belasting regels van uw markt en specifieke omstandigheden. | *$0,08* |
| PostTaxTotal | Totaal na belasting, wanneer belasting van toepassing is. | *$0,93* |
| Valuta | Valuta type. Elke facturerings entiteit heeft slechts één valuta. Controleer of deze overeenkomt met uw eerste factuur en vervolgens na belang rijke updates van het facturerings platform. | *EUR* |
| PretaxEffectiveRate | Pretax prijs per eenheid. Gelijk aan **PretaxCharges** gedeeld door **OverageQuantity**, afgerond op het dichtstbijzijnde cent. | *$0,08* |
| PostTaxEffectiveRate | De BTW-prijs per eenheid. Gelijk aan **PostTaxTotal** gedeeld door **OverageQuantity**, afgerond op het dichtstbijzijnde cent. Of, gelijk aan **PretaxEffectiveRate** plus het BTW-tarief per eenheids bedrag, afgerond op het dichtstbijzijnde cent. | *$0,08* |
| ChargeType | Het [type kosten](recon-file-charge-types.md) of correctie. | Zie [kosten typen](recon-file-charge-types.md). |
| CustomerId | De unieke micro soft-id voor de klant, in GUID-indeling. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Domein naam van de klant. Dit veld kan leeg zijn tot de tweede facturerings cyclus. | *example.onmicrosoft.com* |
| BillingCycleType | Facturerings frequentie van tijd.| **Maandelijks**  |
| Eenheid | De eenheid van de resource **naam**. | *GB* of *uren* |
| CustomerBillableAccount | Unieke account-id in het micro soft-factuur platform. | *1280018095* |
| UsageDate | De datum van de service-implementatie. | *2/1/2019 0:00* |
| MeteredRegion | Hiermee wordt de locatie van een Data Center binnen de regio aangegeven (voor services waar deze waarde van toepassing is en ingevuld). | *Azië-Oost*, *zuid Azië-Oost*, *Europa-Noord*, *Europa-West*, *Noord-Centraal VS*, *Zuid-Centraal VS* |
| MeteredService | Identificeert het afzonderlijke Azure-service gebruik als het niet specifiek wordt aangegeven in de kolom **service** naam. Gegevens overdrachten worden bijvoorbeeld gerapporteerd als *Microsoft Azure-alle services* in de kolom **service** naam. | *AccessControl*, *CDN*, *Compute*, *Data Base*, *ServiceBus*, *Storage* |
| MeteredServiceType | Subkoppen voor het veld **MeteredService** die een extra uitleg bieden over het gebruik van Azure-service. | *BUITEN* |
| Project | Door de klant gedefinieerde naam voor het service-exemplaar. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Het aantal Azure Service Bus verbindingen dat op een bepaalde dag is ingericht en gebruikt. | *1,000000 verbindingen/30 dagen* (als u een afzonderlijk ingerichte verbinding hebt tijdens een maand van 30 dagen), *25 verbindingen/30 dagen – gebruikt: 1,000000* (als er een 25 pack van service bus verbindingen is ingericht en u 1 tijdens die dag hebt gebruikt) |

## <a name="next-steps"></a>Volgende stappen

- [Informatie over de velden in het Partner Center-afstemmings bestand op basis van licentie](license-based-recon-files.md)