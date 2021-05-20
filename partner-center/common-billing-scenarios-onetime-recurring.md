---
title: Facturering voor eenmalige & terugkerende aankopen
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Partner Center voor eenmalige facturering en selecteer terugkerende aankopen: wanneer u abonnementen koopt, voegt u meer abonnementen toe, voegt u licenties toe of verwijdert u deze.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a26b6e5299c5186959612e622808161ca0f7f7c2
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148615"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Partner Center voor eenmalige factureringsscenario's en terugkerende aankopen selecteren

**Juiste rollen:** beheeragent | Factureringsbeheerders | Helpdeskagent | Verkoopagent

Dit zijn [veelvoorkomende factureringsscenario's.](common-billing-scenarios.md) 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Een abonnement kopen en op dezelfde dag een licentie toevoegen

In scenario 1 koopt u een abonnement op 11 juni tegen een eenheidsprijs van $ 4. Later op dezelfde dag koopt u een ander abonnement tegen dezelfde prijs.

Het reconbestand bevat het volgende:

- $4 factuur voor serviceperiode 10 juni – 9 juli.
- $-4,00 prorated rebill for service period 11 juni – 11 juni. Dit is de periode waarin u een licentie hebt. Berekening = (maandelijkse prijs/totaal aantal dagen in serviceperiode) x dagen in pro rated service period x number of licenses = (4/30) x 30 x 1 = 4,00.
- $ 8,00 prorated rebill for service period 10 juni – 9 juli. Dit is de periode waarin u twee licenties hebt. Berekening = (4/30) x 30 x 2 = 8,00.

|**Aankoopdatum**   |**Kosten starten** |**Einde van kosten**  |**Eenheidsprijs**  |**Aantal**  |**Bedrag** |**Kostentype** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$ 4                |1                 |$ 4            |Nieuw         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$ 4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$ 4        | 2      |$ 8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Een abonnement kopen en later meer abonnementen toevoegen

In scenario 2 koopt u een abonnement op 11 juni tegen een eenheidsprijs van $ 4 en op 12 juni koopt u een ander abonnement voor hetzelfde product tegen dezelfde prijs.

Het reconbestand bevat het volgende:

- $ 4 voor serviceperiode 10 juni – 9 juli.
- $-3,87 prorated rebill for service period 11 juni – 12 juni. Dit is de periode waarin u één licentie hebt. Berekening = (maandelijkse prijs/totaal aantal dagen in serviceperiode) x dagen in serviceperiode naar waarde x aantal licenties = (4/30) x 29 x 1 = 3,87.
- $ 7,74 probill voor serviceperiode 12 juni – 9 juli. Dit is de periode waarin u twee licenties hebt. Berekening = (4/30) x 29 x 2 = 7,74.

|**Aankoopdatum**   |**Kosten starten** |**Einde van de kosten**  |**Eenheidsprijs**  |**Aantal**  |**Bedrag** |**Kostentype** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11-6-2019 (u hebt één licentie)     |6/10/2019   |7/09/2019         |$ 4         |1        |$ 4            |Nieuw         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$ 4        |1        | -$3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$ 4        | 2      |$ 7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Een abonnement aanschaffen en een licentie op dezelfde dag verwijderen

In scenario 3 koopt u twee abonnementen voor hetzelfde product op 11 juni tegen een eenheidsprijs van $ 4. Later op dezelfde dag verwijdert u een van de licenties.  

Het reconbestand bevat het volgende:

- $ 8 factureert voor twee licenties voor de serviceperiode van 10 juni tot 9 juli.
- $-8,00 prorated rebill for service period 11 juni – 11 juni. Dit is de periode waarin u twee licenties hebt. Berekening = (maandelijkse prijs/totaal aantal dagen in serviceperiode) x dagen in pro rated service period x number of licenses = (4/30) x 30 x 2 = 8,00.
- $ 4,00 prorated rebill for service period 11 juni – 9 juli. Dit is de periode waarin u één licentie hebt. Berekening = (4/30) x 30 x 1 = 4,00.

|**Aankoopdatum**   |**Kosten starten** |**Einde van de kosten**  |**Eenheidsprijs**  |**Aantal**  |**Bedrag** |**Kostentype** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$ 4                |2                 |$ 8            |Nieuw         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$ 4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$ 4        | 1      |$ 4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Een abonnement kopen en licenties later verwijderen

In scenario 4 koopt u twee abonnementen op 11 juni tegen een eenheidsprijs van $ 4 en op 12 juni verwijdert u een van de licenties.

Het reconbestand bevat het volgende:

- $8 factuur voor serviceperiode 10 juni – 9 juli.
- $-7,74 prorated rebill for service period 11 juni – 12 juni. Dit is de periode waarin u twee licenties hebt. Berekening = (maandelijkse prijs/totaal aantal dagen in serviceperiode) x dagen in pro rated service period x number of licenses = (4/30) x 29 x 2 = 7,74.
- $ 3,87 prorated rebill for service period 12 juni – 9 juli. Dit is de periode waarin u één licentie hebt. Berekening = (4/30) x 29 x 1 = 3,87.

|**Aankoopdatum**   |**Kosten starten** |**Einde van kosten**  |**Eenheidsprijs**  |**Aantal**  |**Bedrag** |**Kostentype** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11-6-2019 (u hebt twee licenties)     |6/10/2019   |7/09/2019         |$ 4         |2        |$ 8       |Nieuw       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$ 4        |2        | -$7,74       |removeQuantity           |
|12-6-2019 (u hebt één licentie)    | 6/10/2019    |7/09/2019   |$ 4    |1      |$ 3,87    |removeQuantity |

## <a name="next-steps"></a>Volgende stappen

- [Voorbeeld van maandelijkse factureringsscenario's voor nieuwe abonnementen, wijzigen van licentiebedragen of opzegging](common-billing-scenarios-monthly.md)