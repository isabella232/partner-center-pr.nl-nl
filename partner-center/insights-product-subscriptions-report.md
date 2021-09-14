---
title: Partner Center Insights abonnementsrapport
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Bekijk wat u goed doet en waar u de cloudabonnementen kunt verbeteren die u voor uw klanten verkoopt of beheert.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eefb4f4ee6657acf583ad0b5d4149e662c320184
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244897"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Het rapport Productabonnementen is beschikbaar via Partner Center Insights dashboard

**Juiste rollen:** Globale | Beheeragent | Rapportviewer | Rapportviewer voor leidinggevenden

Het rapport Productabonnementen bevat analyses van cloudabonnementen die u hebt verkocht of die u voor uw klanten beheert. Dit is een product-specifiek rapport met de prestaties van abonnementen die zijn gekoppeld aan cloudproducten zoals Office 365, Azure, Dynamics en andere.

U kunt de volgende secties bekijken in het rapport Productabonnementen.

- Samenvatting
- Geografische spreiding van abonnementen
- Trend in toevoegen/verloop van abonnementen
- Abonnementsdistributie per partnerlocaties, verkoopkanaal, SKU's, type partner koppelen, segment
- Trend op abonnements states
- Trend in producten

 > [!NOTE]
 > Dit rapport is beschikbaar via het Insights dashboard. Als u dit rapport wilt weergeven, moet aan u een specifieke rol zijn toegewezen in Partner Center, zoals globale beheerder, accountbeheerder, rapportviewer of executive rapportviewer. Zie de globale beheerder van uw bedrijf voor meer informatie. Specifieke typen gegevens in dit rapport zijn mogelijk ook alleen beschikbaar voor gebruikers met beheerdersbevoegdheden voor rapportviewers.

## <a name="summary"></a>Samenvatting

De samenvattingssectie bevat een momentopnameweergave van de Key Performance Indicators (KPI's) die betrekking hebben op abonnementen die door u zijn verkocht of beheerd voor uw klanten.  

:::image type="content" source="images/insights/sub-report-summary.png" alt-text="rapportoverzicht abonnementen.":::

Zie hieronder voor meer informatie over elke sectie van de samenvatting:

- Abonnementen:
  - Het huidige aantal cloudproductabonnementen dat door u is verkocht of beheerd.
  - Percentagegroei of afname van abonnementen tijdens het geselecteerde datumbereik.
  - In de Micro-grafiek wordt een trend voor het aantal abonnementen gedurende het geselecteerde datumbereik weergegeven.

- Actieve abonnementen:
  - Huidig aantal cloudproductabonnementen met actief gebruik gemeten op basis van product-telemetrie. Hiermee worden alle proefabonnementen voor Azure-abonnementen uitgesloten.
  - Percentagegroei of afname van actieve abonnementen gedurende de geselecteerde periode.
  - De Micro-grafiek geeft een trend van de maand-over-maand weer van actieve abonnementen tijdens het geselecteerde datumbereik.

- Abonnementen toegevoegd:
  - Het totale aantal klantabonnementen dat door u is toegevoegd (verkocht of beheerd) tijdens het geselecteerde datumbereik. Nieuwe abonnementen met de **status Actief** **of** Vernieuwd worden geteld als Toegevoegde abonnementen.
  - Percentage groei of afname van abonnementen toegevoegd in de afgelopen volledige maand vergeleken met de eerste volledige maand.
  - De Micro-grafiek geeft een maandelijkse trend weer van abonnementen die zijn toegevoegd tijdens het geselecteerde datumbereik.

- Abonnementen die zijn verloop:
  - Het totale aantal klantabonnementen dat is verloop tijdens het geselecteerde datumbereik. Abonnementen met de status **Deprovisioned** of **Suspended** in die maand worden geteld als een verloop van abonnement.  
  - Percentage abonnementen dat is verloop tijdens het geselecteerde datumbereik.
  - De Micro-grafiek geeft een maandelijkse trend weer van abonnementen die over het geselecteerde datumbereik zijn verloop.

- Abonnementen op producten: Uitsplitsing van het huidige aantal abonnementen per cloudproducten.

## <a name="geographical-spread-of-subscriptions"></a>Geografische spreiding van abonnementen

In **de weergave Abonnementen op geografie** wordt de geografische verdeling van het totale aantal abonnementen per klantmarkt weergeven. Het totale abonnementsbedrag omvat zowel verkochte abonnementen als actieve abonnementen.

De **tabel Aantal landen/regio's** bevat het totale aantal landen/regio's waar u abonnementen hebt en het bedrag per land van het totale en actieve abonnement.

U kunt een land in het raster zoeken en selecteren om in te zoomen op de locatie op de kaart. Druk op **de optie** Start op de kaart om terug te keren naar de oorspronkelijke weergave. Beweeg de muisaanwijzer over de kaart om alle abonnementen en actieve abonnementen per land weer te zien. Beide velden in het raster kunnen worden gesorteerd.

:::image type="content" source="images/insights/sub-report-sub-by-geography.png" alt-text="abonnementen per geografie.":::

## <a name="subscription-addschurns"></a>Abonnements-adds/churns

Deze weergave toont een trend van abonnementen. Deze zijn onderverdeeld in verschillende categorieën (Nieuw, Bestaand, Verloop) voor het geselecteerde datumbereik. De x-as vertegenwoordigt maanden van het geselecteerde datumbereik. De Y-as vertegenwoordigt het aantal abonnementen. Verloopabonnementen worden weergegeven op de negatieve schaal van de Y-as. 

In het gestapelde kolomdiagram wordt een uitsplitsing weergegeven van nieuwe, bestaande en verloopde abonnementen voor de maand. U kunt het kolomdiagram opnieuw opbouwen, opgesplitst met specifieke stack-items. Selecteer de specifieke items in de legenda om dit te doen. U kunt ook de schuifregelaar boven op het diagram gebruiken om in te zoomen op een specifieke periode.

:::image type="content" source="images/insights/sub-report-sub-adds-churns.png" alt-text="abonnements toegevoegd en verloop.":::

## <a name="subscription-distribution"></a>Abonnementsdistributie

Deze weergave geeft een uitsplitsing van uw huidige abonnementen op uw Microsoft Partner Network-locaties (MPN), klantsegmenten, verkoopkanaal/Azure-prijsmodel en het toeschrijvingstype. Selecteer de respectieve tabbladen om de uitsplitsing te bekijken op basis van deze categorieën. Als u het cirkeldiagram wilt maken met een uitsplitsing van specifieke itemcategorieën, selecteert u die itemcategorieën in de legenda.

:::image type="content" source="images/insights/sub-report-distribution.png" alt-text="abonnementsdistributie.":::

## <a name="subscription-state-distribution"></a>Distributie van abonnementstoestand

Deze weergave toont de distributie van uw huidige klantabonnementen op abonnementsstatus of -status. Dit omvat de volgende abonnementsindelingen: **Actief,** **Uitgeschakeld,** **Deprovisioned,** **Openen,** **InGracePeriod,** **Gesloten** en **Overige**.

:::image type="content" source="images/insights/sub-report-sub-states.png" alt-text="distributie van abonnementstoestand.":::

## <a name="products-trend"></a>Trend in producten

In deze weergave ziet u een staafdiagram en twee cirkeldiagrammen. Het staafdiagram toont een maandelijkse trend van abonnementen, onderverdeeld naar commerciële producten, zoals Azure, Office en Dynamics.

De twee cirkeldiagrammen geven een uitsplitsing van uw huidige klantabonnementen weer. In het eerste cirkeldiagram worden abonnementen op producten weergegeven. In het tweede cirkeldiagram worden abonnementen op sku's of abonnementen opgebreed. Wanneer u een product  selecteert in de uitsplitsing op het cirkeldiagram Producten, toont het aangrenzende cirkeldiagram een uitsplitsing van de abonnementen van dat product op SKU's.

:::image type="content" source="images/insights/sub-report-prods-trend.png" alt-text="trend in producten.":::

> [!NOTE]
 > Het aantal abonnementen, onderverdeeld naar SKU's, komt mogelijk niet altijd overeen met het totale aantal abonnementen voor dat product. Dit kan gebeuren als een klant meerdere SKU's heeft aangeschaft onder hetzelfde productabonnement.

## <a name="next-steps"></a>Volgende stappen

- Zie voor meer rapporten [Partner Center Insights](partner-center-insights.md).

>[!NOTE] 
> U kunt de onbewerkte gegevens voor dit rapport downloaden via de sectie Rapporten downloaden in het Insights dashboard. [Meer informatie](insights-download-reports.md) 
