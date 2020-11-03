---
title: Facturering voor eenmalige & terugkerende aankopen
ms.topic: article
ms.date: 05/05/2020
description: 'Partner centrum facturerings voorbeelden voor eenmalige en selecteer terugkerende aankopen: wanneer u abonnementen aanschaft, kunt u meer abonnementen toevoegen, licenties toevoegen of verwijderen.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 720e3c4f97e374b0137db2302988a0fbd2db9432
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92528684"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Facturerings scenario's van partner centrum voor eenmalige en geselecteerde terugkerende aankopen

**Juiste rollen**

- Beheer agent
- Factureringsbeheerder
- Helpdesk medewerker
- Verkoop agent

Dit zijn [veelvoorkomende facturerings scenario's](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Een abonnement kopen en op dezelfde dag een licentie toevoegen

In scenario 1 koopt u een abonnement op 11 juni tegen een eenheids prijs van $4. Later diezelfde dag hebt u een ander abonnement op dezelfde prijs aangeschaft.

Het afstemmings bestand bevat het volgende:

- $4 factuur voor service periode van 10 juni: 9 juli.
- $-4,00 gefactureerd herfactureren voor service periode van 11 juni. Dit is de periode waarin 1 licentie is geweest. Berekening = (maand-prijs/totaal aantal dagen in service periode) x dagen in gefactureerde service periode x aantal licenties = (4/30) x 30 x 1 = 4,00.
- $8,00 gefactureerd herfactureren voor service periode van 10 juli: 9 juni. Dit is de periode waarin u 2 licenties hebt. Calculation = (4/30) x 30 x 2 = 8,00.

|**Aankoop datum**   |**Start kosten** |**Einde van kosten**  |**Eenheids prijs**  |**Aantal**  |**Aantal** |**Kostentype** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Nieuw         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Een abonnement aanschaffen en later meer abonnementen toevoegen

In scenario 2 koopt u een abonnement op 11 juni tegen een eenheids prijs van $4, en op 12 juni hebt u een ander abonnement voor hetzelfde product gekocht tegen dezelfde prijs.

Het afstemmings bestand bevat het volgende:

- $4 factuur voor service periode van 10 juni: 9 juli.
- $-3,87 gefactureerd herfactureren voor service periode van 11 juni. Dit is de periode waarin 1 licentie is geweest. Berekening = (maand-prijs/totaal aantal dagen in service periode) x dagen in gefactureerde service periode x aantal licenties = (4/30) x 29 x 1 = 3,87.
- $7,74 gefactureerd op basis van de herwaardering voor service periode van 12 juli. Dit is de periode waarin u 2 licenties hebt. Calculation = (4/30) x 29 x 2 = 7,74.

|**Aankoop datum**   |**Start kosten** |**Einde van kosten**  |**Eenheids prijs**  |**Aantal**  |**Aantal** |**Kostentype** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (u hebt één licentie)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Nieuw         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3,87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7,74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Een abonnement kopen en een licentie op dezelfde dag verwijderen

In scenario 3 koopt u twee abonnementen voor hetzelfde product op 11 juni tegen een eenheids prijs van $4. Later diezelfde dag u een van de licenties verwijdert.  

Het afstemmings bestand bevat het volgende:

- $8 factuur voor twee licenties voor service periode van 10 juli: 9 juni.
- $-8,00 gefactureerd herfactureren voor service periode van 11 juni. Dit is de periode waarin u 2 licenties hebt. Berekening = (maand-prijs/totaal aantal dagen in service periode) x dagen in service periode van profactoris x aantal licenties = (4/30) x 30 x 2 = 8,00.
- $4,00 gefactureerd op basis van de herwaardering voor service periode van 11 juni: 9 juli. Dit is de periode waarin 1 licentie is geweest. Calculation = (4/30) x 30 x 1 = 4,00.

|**Aankoop datum**   |**Start kosten** |**Einde van kosten**  |**Eenheids prijs**  |**Aantal**  |**Aantal** |**Kostentype** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Nieuw         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Later een abonnement kopen en licenties verwijderen

In scenario 4 koopt u 2 abonnementen op 11 juni tegen een eenheids prijs van $4 en op 12 juni verwijdert u een van de licenties.

Het afstemmings bestand bevat het volgende:

- $8 factuur voor service periode van 10 juni: 9 juli.
- $-7,74 gefactureerd herfactureren voor service periode van 11 juni. Dit is de periode waarin u 2 licenties hebt. Berekening = (maand-prijs/totaal aantal dagen in service periode) x dagen in gefactureerde service periode x aantal licenties = (4/30) x 29 x 2 = 7,74.
- $3,87 gefactureerd op basis van de herwaardering voor service periode van 12 juli. Dit is de periode waarin 1 licentie is geweest. Calculation = (4/30) x 29 x 1 = 3,87.

|**Aankoop datum**   |**Start kosten** |**Einde van kosten**  |**Eenheids prijs**  |**Aantal**  |**Aantal** |**Kostentype** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (u hebt 2 licenties)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Nieuw       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7,74       |removeQuantity           |
|6/12/2019 (u hebt 1 licentie)    | 6/10/2019    |7/09/2019   |$4    |1      |$3,87    |removeQuantity |
