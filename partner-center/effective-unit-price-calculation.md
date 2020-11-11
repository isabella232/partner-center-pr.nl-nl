---
title: Prijs berekening effectief eenheid
ms.topic: how-to
ms.date: 11/10/2020
description: Meer informatie over de werkelijke prijs eenheid en hoe deze worden berekend. Bevat een voor beeld van een berekening.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/11/2020
ms.locfileid: "94499138"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Efficiënte eenheid prijs berekening voor het verbruik van het Azure-abonnement

## <a name="the-effective-unit-price"></a>De werkelijke eenheids prijs

De werkelijke eenheids prijs wordt berekend op het niveau van de meter (in plaats van het resource niveau) en wordt dagelijks aangepast op basis van het gebruik van metingen.

De werkelijke eenheids prijs wordt berekend aan de hand van de volgende drie factoren:

- Verbruik, dat dagelijks wordt bewaakt tijdens de facturerings cyclus
- Factureer bare kosten voor de meter
- Trapsgewijs scha kelen (indien van toepassing)

Omdat we dagelijks het verbruik in de facturerings cyclus controleren, schommelt de werkelijke eenheids prijs. De uiteindelijke prijs voor een bepaalde facturerings cyclus is beschikbaar nadat de verbruiks berekening is gestopt en de facturerings periode is gesloten. U ziet de meeste wijzigingen in het verbruik na de vierde of vijfde decimaal positie.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Nagaan of uw meter gelaagde prijzen gebruikt

Als u niet weet of uw meter gelaagde prijzen gebruikt, gebruikt u de onderstaande procedure om erachter te komen. 

1. Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).
2. Selecteer **verkopen** , selecteer **prijzen en aanbiedingen** en selecteer vervolgens de **prijs** van het Azure-abonnement.
3. Zoek uw meter op ID en down load de prijs gegevens. 

## <a name="sample-calculation"></a>Voorbeeld berekening

De onderstaande tabel geeft een voor beeld van hoe we de werkelijke eenheids prijs berekenen tijdens de open periode.

De volgende waarden zijn van toepassing in de tabel: 

- **Up** = eenheids prijs van resource/uur = 0,868

- **BCU** = factureer bare verbruiks eenheid voor de meter

- **BC** = factureer bare kosten voor de meter = BCU * UP * 0,85. Dit weerspiegelt een aanpassing voor de PEC-korting van 15%. Vervolgens gebruiken we de ondergrens van de functie om de waarde te beperken tot twee cijfers na het decimaal teken, zodat de minimum hoeveelheid kan worden gefactureerd. 

- **Werkelijke eenheids prijs** = BCU/BC

>[!NOTE]
>Opmerking: de meter in dit voor beeld heeft geen lagen voor de prijzen.

| Datum | BCU (factureer bare verbruiks eenheid) | BC (factureer bare kosten) | Werkelijke eenheids prijs |
| ------ | ----------- | ----------- | ----------- |  
| 3-aug | 29 | 21,39 | 0.737586206896552 |
| 10-aug | 210,950039 | 155,63 | 0.737757626107858 |
| 25-aug | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Volgende stappen

- [Facturering en belastingen](billing.md)
