---
title: Prijslijst met Azure-plannen voor CSP-partners
ms.topic: how-to
ms.date: 07/21/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over hoe CSP-programmapartners Partner Center de prijslijst voor abonnementen onder het Azure-plan te bekijken.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: e4adc04f0d8b27f9cd53bbd678d1264b29b86b54
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/04/2021
ms.locfileid: "115101296"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Prijslijst voor de nieuwe Commerce-ervaring in CSP voor Azure

**Juiste rollen:** beheeragent | Factureringsbeheerders | Globale beheerders | Helpdeskagent | Verkoopagent | Beheerder van gebruikersbeheer

De realtime prijzen voor de nieuwe Azure Commerce-ervaring in CSP worden dynamisch in realtime geleverd op Partner Center. Prijzen worden alleen weergegeven in USD. Vanaf 28 januari 2021 wordt elke partner in de regio EU/EFTA en het VK die nieuwe of bestaande CSP-klanten heeft, voor het eerst nieuwe commerceaanbiedingen gekocht en die tenants zijn gemaakt vóór 11 mei 2020, gefactureerd voor deze aankopen in de locatievaluta van de partner. Partners die zich buiten de regio EU/EFTA en het VK bevinden, worden nog steeds gefactureerd in partnerlocatievaluta. Zie Azure-abonnement - facturering [voor meer informatie.](azure-plan-billing.md)

Als onderdeel van de nieuwe commerce-ervaring voor Azure in CSP hebben we een [nieuwe Azure-aanbieding geïntroduceerd.](./azure-plan-lp.md) Raadpleeg het aanbiedingsdocument voor belangrijke datums met betrekking tot de vorige [Azure-aanbieding](https://go.microsoft.com/fwlink/p/?linkid=2164140)(MS-AZR-0145p).

Als u zich hebt *geregistreerd vóór* 21 juli 2021
- U blijft de vorige Azure-aanbieding in de prijslijst zien.

Als u zich hebt *geregistreerd op of na* 21 juli 2021
- U ziet *de* vorige Azure-aanbieding niet in de prijslijst.

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Bekijk de prijzen voor abonnementen onder de prijzen van het Azure-abonnement

1.  Selecteer in Partner Center menu Verkopen **en** vervolgens Prijzen en **aanbiedingen.**
2.  Selecteer **onder Prijzen voor Azure-abonnementsverbruik** en prijzen voor **Azure-planreserveringen** het land en vervolgens de downloadkoppeling.
   - Selecteer **voor Wisselkoersen de** downloadkoppeling onder de sectie .

   > [!NOTE] 
   > **FX-tarieven** zijn niet specifiek voor landen.

   :::image type="content" source="images/azure/pricing-new.png" alt-text="Schermopname van prijzen en aanbiedingen met de nieuwe commerce-ervaring.":::

   > [!NOTE] 
   > U kunt twee verschillende prijslijsten exporteren: Prijzen van Azure-plannen en prijzen van derden voor Marketplace.

## <a name="azure-price-list-specifics"></a>Details van azure-prijslijst

- Prijzen voor Azure-plannen zijn beschikbaar op **de pagina Prijzen en** aanbiedingen in Partner Center, onder **Verkopen.**

- Exports zijn beschikbaar voor verbruiksservices voor Azure-plannen, Azure-reserveringen en FX-tarieven.

- Opties voor exporteren zijn onder andere:

  - **Huidige prijzen:** deze optie omvat alle meters en prijzen van de eerste van de maand tot de huidige datum van de maand, zoals nieuwe prijzen, gewijzigde prijzen of verwijderde prijzen. Alle prijzen hebben effectieve begin- en einddatums om uit te leggen of ze nieuw of verwijderd zijn.

  - **Prijzen van vorige maand:** Downloads van elk type resource zijn per maand. Voor prijsbestanden bevat dit alle meters die beschikbaar waren tijdens die maand. Als er midden in de maand een nieuwe meter wordt geopend, wordt deze als een meter met een effectieve datum als beschikbaarheidsdatum weer geven. Vergelijkbaar met prijzen die niet meer beschikbaar zijn, met een effectieve einddatum die beschrijft wanneer ze niet meer beschikbaar zijn.

  - **FX-tarieven:** FX-tarieven kunnen worden gedownload op de dag vóór de 1e van de maand, 18:00 pst. Als u bijvoorbeeld de tarieven voor november wilt, downloadt u de tarieven op 31 oktober. Fx-tarieven van de vorige maand zijn ook beschikbaar.

- Prijzen in de prijslijsten zijn directe prijzen. Sommige partners komen mogelijk in aanmerking voor partnertegoeden. Lees How the partner earned credit is calculated and paid (Hoe het partnertegoed wordt berekend en betaald) voor meer informatie over hoe het [partnertegoed wordt berekend.](partner-earned-credit-explanation.md)

- **In aanmerking komende services:** partnertegoeden zijn van toepassing op services die worden vermeld in de **azure-abonnementsprijzen** die partners met prijzen kunnen exporteren op de [pagina Met Azure-planprijzen.](https://partner.microsoft.com/commerce/sales)
   > [!NOTE]
   > Er zijn uitzonderingen, waaronder, maar niet beperkt tot, producten van derden die worden geïdentificeerd als 'Derde partij' in de kolom **Tags** van de lijst met prijzen voor Azure-planverbruik en Azure-planreserveringen.

## <a name="price-list-data"></a>Prijslijstgegevens

|**Veld**   |**Beschrijving**   |
|--------------------------|:---------------------------|
|ProductTitle  |Titel of naam van het product|
|ProductID   |Id van het product|
|SKuId|Id van SKU|
|SkuTitle|Titel of naam van SKU|
|Publisher|Eerste partij is altijd Microsoft|
|SkuDescription|Beschrijving van de SKU|
|UnitOfMeasure|De eenheden die in rekening worden gebracht of gefactureerd|
|TermDuration|Voor producten op basis van een term, de lengte van de term die van toepassing is op reserveringen|
|Markt|Markt van de prijzen|
|Valuta|Valuta van de prijzen|
|UnitPrice|Prijs per eenheid|
|PricingTierRangeMin|Voor gelaagde prijzen is de minimumprijs van toepassing|
|PricingTierRangeMax|Voor gelaagde prijzen is de maximumprijs van toepassing|
|EffectiveStartDate|Begindatum van prijzen|
|EffectiveEndDate|Einddatum van de prijzen|
|MeterIds|Meter-id van de product-SKU|
|MeterType|Type of Meter|
|Tags|Eigenschappen voor het item. Voor azure-abonnementsprijzen zijn dit Azure of Azure en reserveringen (met name voor reserveringen)|

Prijslijsten voor het Azure-abonnement kunnen worden geëxporteerd op de [pagina Prijzen en aanbiedingen](https://partner.microsoft.com/dashboard/sell/pricingandoffers) in Partner Center.

## <a name="tiered-pricing"></a>Gelaagde prijzen

Sommige azure-abonnementsverbruiksservices ondersteunen gelaagde prijzen. Partners kunnen deze producten en SKU's vinden in de prijslijst van het Azure-abonnement. Met items met waarden in de kolommen in het prijscategoriebereik kunnen partners inzicht krijgen in de prijs op basis van gebruik. In het onderstaande voorbeeld met voorbeeldgegevens hebben we één product-SKU met drie prijslagen.

|**Productid**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|0,50|100001|9223372036854780000|
|DDD123456ABC|01AB|0,80|101|100000|
|DDD123456ABC|01AB|1|1|100|

Als in dit voorbeeld 101 eenheden worden gebruikt, zijn de kosten 100,80. De eerste 100 eenheden zijn één per eenheid en voor de volgende eenheid wordt 0,80 in rekening gebracht.

## <a name="pricing-api-for-azure-plan"></a>Prijs-API voor Azure-abonnement

U kunt de [prijs-API gebruiken om](/partner/develop/pricing) programmatisch prijzen voor Azure-plannen voor verbruik en reserveringen op te halen. U kunt ook wisselkoersen ophalen.

De prijs-API heeft een ander eindpunt dan de Partner Center API's. De prijsinformatie omvat meterprijzen in USD voor Azure-abonnementsbronnen en reserveringsprijzen die zijn toegepast op Azure-abonnementsabonnementen.

Met deze API kunnen partners ook maandelijkse wisselkoersen ophalen, omdat de prijzen van het Azure-plan alleen in USD zijn. U kunt de API's gebruiken om prijzen en wisselkoersen voor de huidige maand of vorige maanden op te halen.

> [!NOTE]
> De prijs-API is specifiek voor azure-abonnementsprijzen. U moet nog steeds de bestaande RateCard-API en prijslijsten gebruiken die op de pagina Prijzen en aanbiedingen van de Partner Center worden geplaatst voor Azure-resources of -reserveringen die zijn geïmplementeerd in niet-Azure-abonnementsabonnementen. De API voor prijzen voor Azure-plannen biedt geen ondersteuning voor software, Marketplace of prijzen op basis van licenties, zoals Microsoft 365 of Dynamics 365.

Zie de volledige api-documentatie over prijzen voor meer informatie over azure-planprijzen en API's voor [wisselkoersen.](/partner/develop/pricing)

## <a name="next-steps"></a>Volgende stappen

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
