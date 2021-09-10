---
title: Jaarlijkse facturering - veelvoorkomende scenario's
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: 'Partner Center-facturering: wanneer u nieuwe abonnementen toevoegt, licenties toevoegt vóór de factureringsdatum, de licentiehoeveelheid wijzigt of abonnementen onder actief of opnieuw activeren.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cf6ddd8ed73fcd9a7ee20a180072ad51cc5b7c4
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123956902"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Algemene jaarlijkse factureringsscenario's in Partner Center

**Juiste rollen:** beheeragent | Factureringsbeheerder | Helpdeskagent | Verkoopagent

Deze algemene [scenario's voor facturering zijn](common-billing-scenarios.md) van toepassing als u jaarlijkse facturering in Partner Center.

## <a name="new-annual-subscription"></a>Nieuw jaarlijks abonnement

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate kosten bij aankoop|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Licentie toevoegen na de jubileumdatum van het abonnement, maar vóór de factureringsdatum

U koopt een nieuw abonnement op 11-2-2017 met één licentie voor $ 211,20/jaar. De inschrijvingsdag van uw abonnement is ingesteld op de 11e van elke maand. Het Microsoft-factureringssysteem maakt de volgende factureringslijnen:

- $ 211,20 in rekening brengen voor de periode 11-2-2017 – 10-2-2018.

Op 12-02-2017 koopt u een tweede licentie. Uw factureringsdatum is 14-2-2017. Er wordt een factuur- en afstemmingsbestand gegenereerd. Het afstemmingsbestand bevat de volgende factureringsregels:

|Begindatum van kosten  |Einddatum van kosten  |Kostentype  |Prijs per eenheid |Aantal | Bedrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Prorate Fees When Purchase |211.20 |1 | 211.20 |

Op de inschrijvingsdatum van uw abonnement, 11-3-2017, maakt het Microsoft-factureringssysteem de volgende factureringslijnen voor de licentieverhoging op 12-2-2017:

- Tegoed van $ 211,20 voor de periode 2/11/17 – 2/10/18.
- Pro 0,58 dollar per licentie voor één licentie voor de periode 11-2-2017 - 11-2017.
- Pro 15,62 dollar per licentie voor twee licenties voor de periode van 12-02-2017- 3-10-2017.
- Pro 195,00 dollar per licentie voor twee licenties voor de periode 11-3-2017 – 10-2-2018.

Op 11-2-2017 koopt u een abonnement. Op 12-2-2017 voegt u een licentie toe. Uw factureringsdatum is 14-2-2017. Op 11-2-2018 wordt uw abonnement verlengd.

De volgende factureringsdatum is 3/14/17 en er wordt een factuur- en afstemmingsbestand gegenereerd. Het afstemmingsbestand bevat de volgende factureringsregels:

|Begindatum van kosten  |Einddatum van kosten  |Kostentype  |Prijs per eenheid |Aantal | Bedrag |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Prorate cyclus-exemplaar |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Prorate cyclus-exemplaar |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Prorate cyclus-exemplaar |15.62 |2 |31.25 |
|3/11/2017 |2/10/2018 |Prorate cyclus-exemplaar |195.00 |2 |390.00 |

Op 11-2-2018 wordt het abonnement met nog een periode van 12 maanden verlengd.

## <a name="change-license-quantity"></a>Licentieaantal wijzigen

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate kosten bij aankoop|48.00|1|48.00

Op 1 februari verhoogt u het aantal licenties van één naar twee. Het afstemmingsbestand op basis van licenties van 15 februari bevat de volgende factureringsregels:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate van cyclus-exemplaar|-48.00|1|-48.00
1/13/2018|1/31/2018|Prorate van cyclus-exemplaar|2.47|1|2.47
1-2-2018|1/12/2019|Prorate van cyclus-exemplaar|44.98|2|89.96

De jaarlijkse prijs is 48,00, wat gelijk is aan de dagelijkse prijs van 0,13 (48,00/365).

Eenheidsprijs = dagen in serviceperiode x dagelijkse prijs x aantal licenties.

De serviceperiode is 13-13-2018 13-2018 31-2018 19 dagen.

Daarom is eenheidsprijs = 2,47 (19x0,13x1)

Er zijn 346 dagen in serviceperiode 1-2-2018 – 12-1-2019.

Daarom is eenheidsprijs = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>Vóór 30 dagen opschorten

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate kosten bij aankoop|48.00|1|48.00

Op 1 februari schort u uw abonnement op. Het afstemmingsbestand op basis van licenties van 15 februari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Kosten annuleren|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Opschorten na 30 dagen

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate kosten bij aankoop|48.00|1|48.00

Het afstemmingsbestand op basis van licenties van 15 februari bevat geen factureringslijnen voor dit abonnement.
Op 1 maart schort u uw abonnement op. Het afstemmingsbestand van 15 maart op basis van licenties bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Kosten annuleren|-41.34|1|-41.34

De jaarlijkse prijs is 48,00, wat gelijk is aan de dagelijkse prijs van 0,13 (48,00/365).

Eenheidsprijs = dagen in serviceperiode x dagelijkse prijs x aantal licenties.

Er zijn 318 dagen in serviceperiode 3/1/2018 – 12-1-2019.

Daarom is eenheidsprijs = 41,34 (318x0,13x1). Omdat dit een tegoed is, is de eenheidsprijs -41,34.

## <a name="suspend-and-reactivate"></a>Suspend and reactivate (Opnieuw activeren)

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u jaarlijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorate kosten bij aankoop|48.00|1|48.00

Op 1 februari schort u uw abonnement op. Het afstemmingsbestand op basis van een licentie van 15 februari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Kosten annuleren|-48.00|1|-48.00

Op 1 maart kunt u uw abonnement opnieuw activeren. Het afstemmingsbestand op basis van een licentie van 15 maart bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Prorate kosten bij aankoop|41.34|1|41.34

De jaarlijkse prijs is 48,00, wat gelijk is aan de dagelijkse prijs van 0,13 (48,00/365).

Eenheidsprijs = dagen in serviceperiode x dagelijkse prijs x aantal licenties.

Er zijn 318 dagen in serviceperiode 3/1/2018 – 12-01-2019.

Daarom is eenheidsprijs = 41,34 (318x0.13x1).
