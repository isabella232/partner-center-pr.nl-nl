---
title: Prijs lijst van Azure plan voor CSP-partners
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe CSP-programma partners partner centrum kunnen gebruiken om de prijs lijst voor abonnementen te bekijken onder het Azure-abonnement.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f11031c6071dadb427d2d5b93edd90af1a844131
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/28/2021
ms.locfileid: "98924953"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Prijslijst voor de nieuwe Commerce-ervaring in CSP voor Azure

**Juiste rollen**

- Beheer agent
- Factureringsbeheerder
- Globale beheerder
- Helpdesk medewerker
- Verkoop agent
- Beheerder van gebruikers beheer

De prijs lijst voor de nieuwe Azure commerce-ervaring in CSP wordt in partner centrum geplaatst. De prijs lijst wordt dynamisch geleverd in real-time nauw keurig bestand en de prijzen worden alleen in USD weer gegeven. Vanaf januari 28 2021 worden partners in de regio EU/EVA en UK die nieuwe klanten hebben en bestaande CSP-klanten nieuwe Commerce aanbiedingen kopen voor de eerste keer waarvan de tenants zijn gemaakt vóór 11 mei 2020, in rekening gebracht voor deze aankopen in de valuta van de partner locatie.  Partners die zich buiten de EU/EVA-en UK-regio bevinden, blijven in rekening gebracht voor de valuta van de partner locatie, de [facturering van het Azure-abonnement](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Prijzen voor abonnementen bekijken onder de prijzen van het Azure-abonnement

1. Selecteer in het menu partner centrum aan de linkerkant de optie **verkopen** en selecteer vervolgens **Marketplace**.

2. Selecteer onder prijzen van Azure-abonnement het land waarvoor u de prijzen wilt bepalen.

3. Selecteer in het veld **Export type** de **prijs stelling voor Azure plan verbruik**, de **prijzen voor Azure plan reserveringen** of de **FX-tarieven**. 

>[!NOTE] 
>De **FX-tarieven** zijn niet van het specifieke land.

4. Selecteer naast **prijs voor datum** de gewenste datum, bijvoorbeeld **actueel**.

   :::image type="content" source="images/azure/pricingnew.png" alt-text="land specifiek":::

>[!NOTE] 
>U kunt twee verschillende prijs lijsten exporteren: Azure-Plan prijzen en Marketplace-prijs van derden.

## <a name="azure-price-list-specifics"></a>Details van de prijzen lijst van Azure

- Prijzen voor Azure-abonnementen zijn beschikbaar via de Marketplace-pagina in Partner Center, onder **verkopen**.

- Exports zijn beschikbaar voor de verbruiks Services, Azure Reservations en FX-tarieven van Azure plan.

- De opties voor exporteren zijn onder andere:

  - **Prijzen vandaag**: Dit omvat alle meters en prijzen van de 1e van de maand tot de huidige datum van de huidige maand. Dit omvat nieuwe prijzen, gewijzigde prijzen of verwijderde prijzen. Alle prijzen hebben een geldige begin-en eind datum om uit te leggen of ze nieuw of verwijderd zijn.

  - **Prijs van vorige maand**: Down loads van elk type resource zijn per maand. Voor prijs bestanden bevat dit alle meters die beschikbaar waren tijdens die maand. Als er een nieuwe meter in het midden van de maand wordt weer gegeven, ziet u als een meter met een ingangs datum die de beschik baarheid weerspiegelt. Vergelijkbaar met prijzen die niet meer worden uitgevoerd, met een geldige eind datum die beschrijft wanneer deze niet meer beschikbaar zijn.

  - **FX-tarieven**: de FX-tarieven zijn beschikbaar voor het downloaden van de dag voor de 1e van de maand, 18:00 uur PST. Als u bijvoorbeeld de tarieven voor november wilt, downloadt u de tarieven op 31 oktober. De voor gaande FX-tarieven voor de maand zijn ook beschikbaar.

- Prijzen in de prijs lijsten zijn directe prijzen. Sommige partners komen mogelijk in aanmerking voor het tegoed van de partner. Lees hoe het tegoed van de partner wordt berekend [en betaald](partner-earned-credit-explanation.md)voor meer informatie over de manier waarop het tegoed voor de leverancier wordt bepaald.

- **In aanmerking komende Services**: het tegoed van de partner is van toepassing op Services die worden vermeld in de Azure-prijs informatie over het **plannen van prijzen** , kunnen worden geëxporteerd op de pagina met prijs informatie voor [Azure](https://partner.microsoft.com/commerce/sales) Houd er rekening mee dat er uitzonde ringen zijn, waaronder, maar niet beperkt tot, producten van derden die zijn geïdentificeerd als ' derde partij ' in de kolom Tags van de prijs lijst voor verbruik van Azure plan en Azure plan-reserve ringen.

## <a name="price-list-data"></a>Prijs lijst gegevens

|**Veld**   |**Beschrijving**   |
|--------------------------|:---------------------------|
|ProductTitle  |Titel of naam van het product|
|ProductID   |ID van het product|
|SKuId|ID van SKU|
|SkuTitle|Titel of naam van SKU|
|Publisher|eerste partij is altijd micro soft|
|SkuDescription|Beschrijving van de SKU|
|UnitOfMeasure|De eenheden die worden in rekening gebracht of gefactureerd|
|TermDuration|Voor producten op basis van een term, de duur van de periode, die van toepassing is op reserve ringen|
|Markt|Prijzen markt|
|Valuta|Valuta van de prijzen|
|UnitPrice|Prijs per eenheid|
|PricingTierRangeMin|Voor gelaagde prijzen geldt de minimum prijs|
|PricingTierRangeMax|Voor gelaagde prijzen geldt de maximum prijs|
|EffectiveStartDate|Start datum van prijzen|
|EffectiveEndDate|Eind datum van de prijs|
|MeterIds|Meter-ID van de product-SKU|
|MeterType|Type meter|
|Tags|Eigenschappen voor het item, zoals prijzen voor Azure-abonnementen, is Azure of Azure en reserve ringen (voor reserve ringen specifiek)|

Prijs lijsten voor Azure-abonnementen kunnen worden geëxporteerd op de [pagina prijzen en aanbiedingen](https://partner.microsoft.com/dashboard/sell/pricingandoffers) van het partner centrum.

## <a name="tiered-pricing"></a>Gelaagde prijzen

Sommige prijzen voor verbruikte Azure-Services ondersteunen laag. Partners kunnen deze producten en sku's vinden in de prijs lijst van het Azure-abonnement. Items met waarden in de kolommen prijs categorie bereik kunnen partners de prijs op basis van gebruik begrijpen. In het onderstaande voor beeld gebruikt u voorbeeld gegevens met één product-SKU met drie prijs categorieën.

|**ProductId**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|.50|100001|9223372036854780000|
|DDD123456ABC|01AB|.80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Als in dit voor beeld 101 eenheden worden gebruikt, zijn de kosten 100,80. De eerste 100 eenheden zijn één en de volgende eenheid wordt in rekening gebracht op. 80.

## <a name="pricing-api-for-azure-plan"></a>Prijs-API voor Azure-abonnement

U kunt de [prijs-API](/partner/develop/pricing) gebruiken voor het ophalen van de prijs van Azure-abonnementen voor verbruik en reserve ringen via een programma. U kunt ook wisselkoers tarieven ophalen.

De prijs-API bevindt zich op een ander eind punt dan de andere Api's van het partner centrum. De prijs informatie omvat de prijs van de meter in USD voor Azure-Plan resources en reserve ringen prijzen die worden toegepast op abonnementen van Azure plan.

Met deze API kunnen partners ook maandelijkse wissel koersen ophalen omdat de prijs van een Azure-abonnement slechts USD is. U kunt de Api's gebruiken voor het ophalen van prijzen en wissel koersen voor de huidige maand of vorige maanden.

>[!NOTE]
> De prijs-API is specifiek voor de prijzen van Azure-abonnementen. U moet nog steeds de bestaande RateCard-API en prijs lijsten gebruiken die zijn gepost op de pagina prijzen en aanbiedingen van het partner centrum voor Azure-resources of-reserve ringen die zijn geïmplementeerd op abonnementen die niet van het Azure-abonnement zijn. De prijs-API van het Azure-abonnement biedt geen ondersteuning voor software, Marketplace of prijzen op basis van licenties, zoals Microsoft 365 of Dynamics 365.

Zie de volledige [API-documentatie voor prijzen](/partner/develop/pricing)voor meer informatie over de prijzen van Azure-abonnementen en api's voor wisselkoersen.

## <a name="next-steps"></a>Volgende stappen

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
