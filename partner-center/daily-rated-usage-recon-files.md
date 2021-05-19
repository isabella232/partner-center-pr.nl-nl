---
title: Bestanden voor afstemming van dagelijks beoordeeld gebruik
ms.topic: article
ms.date: 06/12/2020
description: Meer informatie over het lezen van bestanden voor dagelijkse afstemming van gebruik in Partner Center. Bevat beschrijvingen voor specifieke velden in het recon-bestand.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147272"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Meer informatie over het lezen van bestanden voor dagelijkse afstemming van gebruik in Partner Center

**Van toepassing op**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Juiste rollen:** beheeragent | Factureringsbeheerder | Verkoopagent | Helpdeskagent

In dit artikel wordt uitgelegd hoe u bestanden voor het afstemmen van dagelijks beoordeeld gebruik kunt lezen.

>[!NOTE]
>Normaal gesproken duurt het 24 uur om het dagelijks beoordeelde gebruik weer te geven in Partner Center te worden geopend via de API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Velden in bestanden voor afstemming van dagelijks beoordeeld gebruik

| Kolom | Beschrijving |
| ------ | ----------- |
| PartnerId | Partner-id in GUID-indeling. |
| PartnerName | Naam van de partner. |
| CustomerId | Unieke Microsoft-id voor de klant in GUID-indeling. |
| CustomerName | De organisatienaam van de klant, zoals gerapporteerd in Partner Center. *Deze kolom is belangrijk voor het afstemmen van de factuur met uw systeemgegevens.* |
| CustomerDomainName | De domeinnaam van de klant. |
| CustomerCountry | Het land waarin de klant zich bevindt. |
| MpnId | MPN-id van de CSP-partner. |
| Tier2MpnId | MPN-id van de wederverkoper van de record voor het abonnement. |
| InvoiceNumber | Factuurnummer waar de opgegeven transactie wordt weergegeven. |
| ProductId | De id voor het product. |
| SkuId | De id voor een bepaalde SKU. |
| AvailabilityId | De id voor de beschikbaarheid van een bepaalde SKU. In deze kolom ziet u of de SKU beschikbaar is voor aankoop in het opgegeven land, de valuta, het branchesegment, enzovoort. |
| SkuName | De titel voor een bepaalde SKU. |
| ProductName | De naam van het product. |
| PublisherName | De naam van de uitgever. |
| PublisherId | De id van de uitgever in GUID-indeling. |
| SubscriptionDescription | De naam van de serviceaanbieding die door de klant is gekocht, zoals gedefinieerd in de prijslijst. (Deze kolom is een identiek veld voor **OfferName).** |
| SubscriptionId | Unieke id voor een abonnement in het Microsoft-factureringsplatform. Niet gebruikt voor afstemming. *Deze id is niet hetzelfde  als de abonnements-id in de beheerconsole van de partner.* |
| ChargeStartDate | Begindatum van de factureringscyclus (behalve bij het presenteren van datums van eerder niet-in rekening gebrachte latente gebruiksgegevens uit de vorige factureringscyclus). De tijd is altijd het begin van de dag, 0:00. |
| ChargeEndDate | Einddatum van factureringscyclus (behalve bij het presenteren van datums van eerder niet-in rekening gebrachte latente gebruiksgegevens uit de vorige factureringscyclus). De tijd is altijd het einde van de dag, 23:59. |
| UsageDate | Datum van servicegebruik. |
| MeterType | Het type meter. |
| MeterCategory | De service op het hoogste niveau voor het gebruik. |
| MeterId | De id voor de meter die wordt gebruikt. |
| MeterSubCategory | Het type Azure-service, dat van invloed kan zijn op de snelheid. |
| MeterName | De maateenheid voor de meter die wordt verbruikt. |
| MeterRegion | In deze kolom wordt de locatie van een datacenter in de regio voor services aangegeven waar MeterRegion van toepassing is en wordt ingevuld. |
| Eenheid | De eenheid van de **resourcenaam**. |
| ResourceLocation | Het datacenter waar de meter wordt uitgevoerd. |
| ConsumedService | De Azure-platformservice die u hebt gebruikt. |
| ResourceGroup | Vertegenwoordigt een container met gerelateerde resources voor een Azure-oplossing. |
| ResourceURI | De URI van de resource die wordt gebruikt. |
| ChargeType | Het type kosten of correctie.  |
| UnitPrice | Prijs per licentie, zoals gepubliceerd in de prijslijst op het moment van aankoop. Zorg ervoor dat deze prijs overeenkomt met de gegevens die tijdens de afstemming zijn opgeslagen in uw factureringssysteem. |
| Aantal | Aantal licenties. Zorg ervoor dat deze prijs overeenkomt met de gegevens die tijdens de afstemming zijn opgeslagen in uw factureringssysteem. |
| UnitType | Het type eenheid waarin de meter wordt in rekening gebracht.  |
| BillingPreTaxTotal | Totaal factureringsbedrag vóór belastingen.<br/> _**BillingPreTaxTotal** = FLOOR([] @EffectiveUnitPrice *[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | De valuta in de geografische regio van de klant. |
| PricingPreTaxTotal | De prijzen, vóór belastingen worden toegevoegd. |
| PricingCurrency | De valuta in de prijslijst. |
| ServiceInfo1 | Het aantal Service Bus verbindingen dat op een bepaalde dag is ingericht en gebruikt. |
| ServiceInfo2 | Een verouderd veld met optionele servicespecifieke metagegevens. |
| Tags | Vertegenwoordigt een logische organisatie van Azure-resources die door de gebruiker zijn ingesteld. |
| AdditionalInfo | Aanvullende informatie die niet wordt behandeld in andere kolommen. |
| EffectiveUnitPrice | De werkelijke waarde die per eenheid in rekening wordt gebracht, inclusief eventuele kortingen, verdiend tegoed, en meer. |
| PCToBCExchangeRate | De wisselkoers die wordt toegepast op de prijsvaluta op factureringsvaluta. |
| PCToBCExchangeRateDate | De datum waarop de prijsvaluta voor de factureringsvaluta wordt bepaald. |
| EntitlementId | Vertegenwoordigt de Azure-abonnements-id. |
| EntitlementDescription | Vertegenwoordigt de naam van de Azure-abonnements-id. |
| PartnerEarnedCreditPercentage | Geeft de PartnerEarnedCredit weer voor het regelitem. Het tegoed is 0 of 15 procent |
| Tegoedpercentage | Geeft het Azure-verbruikstegoed weer. Het tegoed is 0 of 100 procent. |
| CreditType | Type tegoed. Bijvoorbeeld **Azure-tegoed toegepast.** |
>[!NOTE]
>Normaal gesproken duurt het 24 uur om het dagelijks beoordeelde gebruik weer te geven in Partner Center te worden geopend via de API.


