---
title: Veelvoorkomende maandelijkse factureringsscenario's
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: "Algemene scenario's Partner Center wanneer u maandelijkse facturering gebruikt: omvat het toevoegen van nieuwe abonnementen, het wijzigen van de licentiehoeveelheid en het opschorten van abonnementen."
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66c9ec09f707d87248fdef31e4cf66f4ca927ce1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148649"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Voorbeeld van maandelijkse factureringsscenario's voor nieuwe abonnementen, wijzigen van licentiebedragen of opzegging

**Juiste rollen:** beheeragent | Factureringsbeheerder | Helpdeskagent | Verkoopagent

Deze [veelvoorkomende factureringsscenario's](common-billing-scenarios.md) zijn van toepassing als u maandelijkse facturering gebruikt in Partner Center.

## <a name="new-monthly-subscription"></a>Nieuw maandelijks abonnement

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u maandelijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringslijnen:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cycluskosten   |4,00       |1        |4,00 |

Het afstemmingsbestand op basis van een licentie van 15 februari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Cycluskosten   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Licentieaantal wijzigen

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u maandelijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringslijnen:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cycluskosten   |4,00       |1        |4,00    |

Op 1 februari verhoogt u het aantal licenties van één naar twee. Het afstemmingsbestand op basis van een licentie van 15 februari bevat de volgende factureringsregels:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |Prorate van cyclus-exemplaar   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | Prorate van cyclus-exemplaar   |2.45       |1        |2.45    |
|1-2-2018         |2/12/2018    | Prorate van cyclus-exemplaar   |1,55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Prorate van cyclus-exemplaar   |4,00       |2        |8,00    |

De maandelijkse prijs is 4,00 en er zijn 31 dagen in de serviceperiode 13-01-2018 – 2/12/2018. Dit komt overeen met een dagelijkse prijs van 0,129 (4/31).

Er zijn 19 dagen in de prorationperiode van 13-1-2018 – 31-1-2018.

Prijs proration unit = 2,451 = 19 x 0,129

Er zijn 12 dagen in de prorationperiode van 1-2-2018 – 12-2-2018.

Prijs proration unit = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Opschorten vóór 30 dagen

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u maandelijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringslijnen:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |Cycluskosten   |4,00       |1        |4,00    |

Op 1 februari schort u een abonnement op. Het afstemmingsbestand op basis van licenties van 15 februari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Kosten annuleren|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Opschorten na 30 dagen

Uw factureringsdatum is de 15e van elke maand. Op 13 januari koopt u een nieuw abonnement met één licentie voor $ 4/maand en selecteert u maandelijkse facturering. Het afstemmingsbestand op basis van licenties van 15 januari bevat de volgende factureringsregels:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|Cycluskosten|4,00|1|4,00

Het afstemmingsbestand op basis van licenties van 15 februari bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Cycluskosten|4,00|1|4,00

Op 1 maart schort u het abonnement op. Het afstemmingsbestand van 15 maart op basis van licenties bevat de volgende factureringsregel:

|Begindatum van kosten |Einddatum van kosten |Kostentype |Prijs per eenheid |Aantal |Bedrag |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Kosten annuleren|-1.72|1|-1.72

De maandelijkse prijs is 4,00 en er zijn 28 dagen in de serviceperiode van 13-02-2018– 3/12/2018. Dit komt overeen met een dagelijkse prijs van 0,143 (4/28).

Eenheidsprijs = dagen in serviceperiode x dagelijkse prijs x aantal licenties.

De annuleringsperiode is 12 dagen 3/1/2018 – 12-3-2018.

Daarom is de eenheidsprijs = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Volgende stappen

- [Factureringsscenario's voor eenmalige en geselecteerde terugkerende aankopen](common-billing-scenarios-onetime-recurring.md)