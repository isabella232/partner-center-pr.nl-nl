---
title: Dagelijks geclassificeerde gebruiks afstemmings bestanden
ms.topic: article
ms.date: 06/12/2020
description: Meer informatie over het lezen van het gebruik van dagelijkse geclassificeerde gebruiks afstemmings bestanden in het partner centrum. Bevat beschrijvingen voor specifieke velden in het afstemmings bestand.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89080cb580d9b451454d108c6ef0ce0a08c1bf0c
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441894"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Meer informatie over het lezen van een gebruiks afstemmings bestand met dagelijkse waardering in het partner centrum

**Van toepassing op**

- Partnercentrum voor Microsoft Cloud for US Government

**Juiste rollen**

- Beheer agent
- Factureringsbeheerder
- Verkoop agent
- Helpdesk medewerker

In dit artikel wordt uitgelegd hoe u dagelijkse geclassificeerde gebruiks reconciliatie bestanden kunt lezen.

>[!NOTE]
>Het dagelijks geclassificeerde gebruik duurt doorgaans 24 uur in het partner centrum of voor toegang via de API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Velden in de gebruiks reconciliatie bestanden met dagelijkse waardering

| Kolom | Beschrijving |
| ------ | ----------- |
| Partner | Partner-id in GUID-indeling. |
| PartnerName | Naam van de partner. |
| CustomerId | Unieke micro soft-id voor de klant in GUID-indeling. |
| CustomerName | Organisatie naam van de klant zoals gerapporteerd in het partner centrum. *Deze kolom is belang rijk voor het afstemmen van de factuur met uw systeem gegevens.* |
| CustomerDomainName | De domein naam van de klant. |
| CustomerCountry | Het land waarin de klant zich bevindt. |
| MpnId | De MPN-id van de CSP-partner. |
| Tier2MpnId | De MPN-id van de dealer van de record voor het abonnement. |
| InvoiceNumber | Factuur nummer waar de opgegeven trans actie wordt weer gegeven. |
| ProductId | De id voor het product. |
| SkuId | De id voor een bepaalde SKU. |
| AvailabilityId | De id voor de beschik baarheid van een bepaalde SKU. In deze kolom wordt aangegeven of de SKU beschikbaar is voor aankoop in het opgegeven land, de valuta, het sector segment, enzovoort. |
| SkuName | De titel voor een bepaalde SKU. |
| ProductName | De naam van het product. |
| PublisherName | De naam van de uitgever. |
| PublisherId | De id van de uitgever in GUID-indeling. |
| SubscriptionDescription | De naam van het service aanbod dat door de klant is aangeschaft, zoals gedefinieerd in de prijs lijst. (Deze kolom is een identiek veld voor de naam van de **aanbieding**). |
| SubscriptionId | De unieke id voor een abonnement in het micro soft-factuur platform. Niet gebruikt voor afstemming. *Deze id is niet hetzelfde als de **abonnements-id** in de partner beheer console.* |
| ChargeStartDate | De begin datum van de facturerings cyclus (behalve bij het presen teren van eerder niet-gefactureerde geposte gebruiks gegevens van de vorige facturerings cyclus). De tijd is altijd het begin van de dag, 0:00. |
| ChargeEndDate | De eind datum van de facturerings cyclus (behalve bij het presen teren van eerder niet-gefactureerde geposte gebruiks gegevens van de vorige facturerings cyclus). De tijd is altijd het einde van de dag, 23:59. |
| UsageDate | De datum van het gebruik van de service. |
| MeterType | Het type meter. |
| MeterCategory | De service op het hoogste niveau voor het gebruik. |
| MeterId | De id voor de meter die wordt gebruikt. |
| MeterSubCategory | Het type van de Azure-service. Dit kan van invloed zijn op het aantal. |
| MeterName | De maat eenheid voor de meting die wordt verbruikt. |
| MeterRegion | Deze kolom bevat de locatie van een Data Center binnen de regio voor services waarbij MeterRegion van toepassing is en is ingevuld. |
| Eenheid | De eenheid van de resource **naam**. |
| ResourceLocation | Het Data Center waar de meter wordt uitgevoerd. |
| ConsumedService | De Azure-platform service die u hebt gebruikt. |
| ResourceGroup | Vertegenwoordigt een container met gerelateerde resources voor een Azure-oplossing. |
| ResourceURI | De URI van de resource die wordt gebruikt. |
| ChargeType | Het type kosten of correctie.  |
| UnitPrice | Prijs per licentie, zoals gepubliceerd in de prijs lijst, op het moment van aankoop. Zorg ervoor dat deze prijs overeenkomt met de informatie die is opgeslagen in uw facturerings systeem tijdens het afstemmen. |
| Aantal | Aantal licenties. Zorg ervoor dat deze prijs overeenkomt met de informatie die is opgeslagen in uw facturerings systeem tijdens het afstemmen. |
| Unit type | Het type eenheid waarop de meter wordt gefactureerd.  |
| BillingPreTaxTotal | Totaal factuur bedrag vóór belastingen.<br/> _**BillingPreTaxTotal** = Floor (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | De valuta in de geografische regio van de klant. |
| PricingPreTaxTotal | De prijzen voordat belastingen worden toegevoegd. |
| PricingCurrency | De valuta in de prijslijst. |
| ServiceInfo1 | Het aantal Service Bus verbindingen dat op een bepaalde dag is ingericht en gebruikt. |
| ServiceInfo2 | Een verouderd veld waarin optionele servicespecifieke meta gegevens worden vastgelegd. |
| Tags | Vertegenwoordigt een logische organisatie van Azure-resources die door de gebruiker zijn ingesteld. |
| AdditionalInfo | Aanvullende informatie die niet wordt behandeld in andere kolommen. |
| EffectiveUnitPrice | De werkelijke waarde in rekening gebracht per eenheid, inclusief eventuele kortingen, gefactureerd tegoed, enzovoort. |
| PCToBCExchangeRate | De wissel koers wordt toegepast op de prijs van de facturerings valuta. |
| PCToBCExchangeRateDate | De datum waarop de prijs valuta naar de facturerings valuta wordt bepaald. |
| EntitlementId | Vertegenwoordigt de ID van het Azure-abonnement. |
| EntitlementDescription | Vertegenwoordigt de naam van de ID van het Azure-abonnement. |
| PartnerEarnedCreditPercentage | Hiermee wordt de PartnerEarnedCredit voor het regel item weer gegeven. Het tegoed van de huidige marge is 0 of 15% |
| CreditPercentage | Hiermee wordt het verbruiks tegoed voor Azure weer gegeven. Het tegoed van de huidige marge is 0 of 100 procent. |
| CreditType | Het type van het tegoed. Bijvoorbeeld, **Azure-tegoed toegepast.** |
>[!NOTE]
>Het dagelijks geclassificeerde gebruik duurt normaal gesp roken 24 uur in het partner centrum of voor toegang via API.


