---
title: Jaarlijkse facturering - algemene scenario's
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: 'Partner Center- en jaarlijkse facturering: wanneer u nieuwe abonnementen toevoegt, licenties toevoegt vóór de factureringsdatum, het aantal licenties wijzigt of abonnementen ondernieuwt/opnieuw activeren.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f97c36c821955570965fcebb006610f4c5c0c79
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089484"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Algemene jaarlijkse factureringsscenario's in Partner Center

**Juiste rollen:** beheeragent | Factureringsbeheerders | Helpdeskagent | Verkoopagent

Deze algemene [factureringsscenario's zijn](common-billing-scenarios.md) van toepassing als u jaarlijkse facturering gebruikt in Partner Center.

## <a name="new-annual-subscription"></a>Nieuw jaarlijks abonnement

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4 per maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 januari 2018|12 januari 2019|Prorate kosten bij aankoop|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Licentie toevoegen na de inschrijvingsdatum van het abonnement, maar vóór de factureringsdatum

U koopt een nieuw abonnement op 11 februari 2017 met één licentie voor $ 211,20 per jaar. Uw abonnementsjubileum is ingesteld op de 11e van elke maand. Het Microsoft-factureringssysteem maakt de volgende factureringsregels:

- Kosten van $ 211,20 voor de periode 11 februari 2017 – 10 februari 2018.

Op 12 februari 2017 koopt u een tweede licentie. Uw factureringsdatum is 14 februari 2017. Er worden een factuur- en afstemmingsbestand gegenereerd. Het afstemmingsbestand bevat de volgende factureringsregels:

|Begindatum van kosten  |Einddatum van kosten  |Kostentype  |Prijs per eenheid |Aantal | Bedrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11 februari 2017 |10 februari 2018 |Prorate Kosten bij aankoop |211.20 |1 | 211.20 |

Op de inschrijvingsdatum van uw abonnement, 11 maart 2017, maakt het Microsoft-factureringssysteem de volgende factureringslijnen voor de licentieverhoging op 12 februari 2017:

- Tegoed van $ 211,20 voor de periode van 11 februari 2017 tot 10 februari 2018.
- Pro 0,58 dollar per licentie voor één licentie voor de periode van 11 februari 2017 tot 11 februari 2017.
- Pro 15,62 dollar per licentie voor twee licenties voor de periode van 12 februari 2017 tot en met 10 maart.
- Pro 195,00 dollar per licentie voor twee licenties voor de periode van 11 maart 2017 tot 10 februari 2018.

Op 11 februari 2017 koopt u een abonnement. Op 12 februari 2017 voegt u een licentie toe. Uw factureringsdatum is 14 februari 2017. Op 11 februari 2018 wordt uw abonnement verlengd.

De volgende factureringsdatum is 14 maart 2017 en er wordt een factuur- en afstemmingsbestand gegenereerd. Het afstemmingsbestand bevat de volgende factureringsregels:

|Begindatum van kosten  |Einddatum van kosten  |Kostentype  |Prijs per eenheid |Aantal | Bedrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11 februari 2017 |10 februari 2018 |Prorate van cyclus-exemplaar |-211.20 |1 |-211.20 |
|11 februari 2017 |11 februari 2017 |Prorate van cyclus-exemplaar |0.58 |1 |0.58 |
|12 februari 2017 |10 maart 2017 |Prorate van cyclus-exemplaar |15.62 |2 |31.25 |
|11 maart 2017 |10 februari 2018 |Prorate van cyclus-exemplaar |195.00 |2 |390.00 |

Op 11 februari 2018 wordt het abonnement verlengd met nog een termijn van 12 maanden.

## <a name="change-license-quantity"></a>Licentieaantal wijzigen

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4 per maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 januari 2018|12 januari 2019|Prorate fees when buy (Prorate-kosten bij aankoop)|48.00|1|48.00

Op 1 februari verhoogt u het aantal licenties van één naar twee. Het afstemmingsbestand op basis van licenties van 15 februari bevat de volgende factureringsregels:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 januari 2018|12 januari 2019|Prorate van cyclus-exemplaar|-48.00|1|-48.00
13 januari 2018|31 januari 2018|Prorate van cyclus-exemplaar|2.47|1|2.47
1 februari 2018|12 januari 2019|Prorate van cyclus-exemplaar|44.98|2|89.96

De jaarlijkse prijs is $ 48,00, wat gelijk is aan de dagelijkse prijs van $ 0,13 ($ 48,00 / 365).

Eenheidsprijs = dagen in de serviceperiode x dagelijkse prijs x aantal licenties.

Er zijn 19 dagen in de serviceperiode van 13 januari 2018 tot 31 januari 2018.

De eenheidsprijs is dus $ 2,47 (19 x 0,13 x 1)

De serviceperiode van 1 februari 2018 tot 12 januari 2019 is 346 dagen.

De eenheidsprijs is dus $ 44,98 (346 x 0,13 x 2)

## <a name="suspend-before-30-days"></a>Vóór 30 dagen opschorten

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4 per maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 januari 2018|12 januari 2019|Prorate kosten bij aankoop|48.00|1|48.00

Op 1 februari schort u uw abonnement op. Het afstemmingsbestand op basis van licenties van 15 februari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 januari 2018|12 januari 2019|Kosten annuleren|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Opschorten na 30 dagen

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 januari 2018|12 januari 2019|Prorate fees when buy (Prorate-kosten bij aankoop)|48.00|1|48.00

Het afstemmingsbestand op basis van licenties van 15 februari bevat geen factureringslijnen voor dit abonnement.
Op 1 maart schort u uw abonnement op. Het afstemmingsbestand van 15 maart op basis van licenties bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 maart 2018|12 januari 2019|Kosten annuleren|-41.34|1|-41.34

De jaarlijkse prijs is $ 48,00, wat gelijk is aan de dagelijkse prijs van 0,13 (48,00 / 365).

Eenheidsprijs = dagen in serviceperiode x dagelijkse prijs x aantal licenties.

Er zijn 318 dagen in de serviceperiode van 1 maart 2018 tot 12 januari 2019.

De eenheidsprijs is dus $ 41,34 (318 x 0,13 x 1). Omdat dit een tegoed is, is de eenheidsprijs -$41,34.

## <a name="suspend-and-reactivate"></a>Suspend and reactivate (Opnieuw activeren)

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4 per maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 januari 2018|12 januari 2019|Prorate kosten bij aankoop|48.00|1|48.00

Op 1 februari schort u uw abonnement op. Het afstemmingsbestand op basis van een licentie van 15 februari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13 januari 2018|12 januari 2019|Kosten annuleren|-48.00|1|-48.00

Op 1 maart kunt u uw abonnement opnieuw activeren. Het afstemmingsbestand op basis van een licentie van 15 maart bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1 maart 2018|12 januari 2019|Prorate kosten bij aankoop|41.34|1|41.34

De jaarlijkse prijs is 48,00, wat gelijk is aan de dagelijkse prijs van 0,13 (48,00/365).

Eenheidsprijs = dagen in serviceperiode x dagelijkse prijs x aantal licenties.

Er zijn 318 dagen in de serviceperiode van 1 maart 2018 – 12 januari 2019.

De eenheidsprijs is dus $ 41,34 (318 x 0,13 x 1).

## <a name="multiyear-offers-with-annual-billing"></a>Aanbiedingen voor meerdere jaren met jaarlijkse facturering

Voor aanbiedingen van meerdere jaren met jaarlijkse facturering beginnen de kosten op de aankoopdatum en worden ze één jaar voortgezet.

(In het [volgende](#example-of-multiyear-billing) voorbeeld van facturering voor meerdere jaren beginnen de kosten voor het eerste jaar op 20 maart 2020 en eindigen ze een jaar later op 19 maart 2021.)

Kosten voor het tweede jaar beginnen één maand eerder dan de einddatum van het eerste jaar.

(In het voorbeeld beginnen kosten voor het tweede jaar op 20 februari 2021, één maand vóór de einddatum van de kosten van het eerste jaar van 19 maart 2021.)

Dit jaarlijkse factureringsproces heeft een maandverschil tussen de einddatum van het abonnement en de einddatum van de kosten voor het derde jaar. Het abonnement blijft echter actief tot de einddatum van het abonnement.

(In het voorbeeld is de einddatum van het abonnement van 19 maart 2023 in het derde jaar één maand na de einddatum van de kosten van 19 februari 2023.)

### <a name="example-of-multiyear-billing"></a>Voorbeeld van facturering voor meerdere jaren

Voor een aanbieding van 36 maanden die is aangeschaft op 20 maart 2020, zoals weergegeven in de volgende tabellen, is het afstemmingsbestand:

#### <a name="first-year"></a>Eerste jaar

|Begindatum van abonnement  |Einddatum van abonnement  |Begindatum van kosten  |Einddatum van kosten  |Kostentype  |
|:-:|:-:|:-:|:-:|:-:|
|20 maart 2020|19 maart 2023|20 maart 2020|19 maart 2021|Prorate fees when purchased (Prorate kosten bij aankoop)|

#### <a name="second-year"></a>Tweede jaar

|Begindatum van abonnement  |Einddatum van abonnement  |Begindatum van kosten  |Einddatum van kosten  |Kostentype  |
|:-:|:-:|:-:|:-:|:-:|
|20 maart 2020|19 maart 2023|20 februari 2021|19 februari 2022|Cycluskosten|

#### <a name="third-year"></a>Derde jaar

|Begindatum van abonnement  |Einddatum van abonnement  |Begindatum van kosten  |Einddatum van kosten  |Kostentype  |
|:-:|:-:|:-:|:-:|:-:|
|20 maart 2020|19 maart 2023|20 februari 2022|19 februari 2023|Cycluskosten|
