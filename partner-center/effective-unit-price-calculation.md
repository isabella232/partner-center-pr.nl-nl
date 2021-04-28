---
title: Effectieve berekening van eenheidsprijs
ms.topic: how-to
ms.date: 04/02/2021
description: Meer informatie over de effectieve eenheidsprijs en hoe deze wordt berekend. Dit artikel bevat ook een voorbeeldberekening.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172214"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Berekening van de effectieve eenheidsprijs voor azure-planverbruik

**Juiste rollen**

- Factureringsbeheerder

## <a name="the-effective-unit-price"></a>De effectieve eenheidsprijs

De effectieve eenheidsprijs wordt berekend op meterniveau (in tegenstelling tot het resourceniveau) en wordt dagelijks aangepast op basis van het metergebruik.

We berekenen de effectieve eenheidsprijs aan de hand van de volgende drie factoren:

- Verbruik, dat dagelijks wordt bewaakt gedurende de factureringscyclus
- Factureerbare kosten voor de meter
- Lagen (indien van toepassing)

Omdat we het verbruik dagelijks bewaken gedurende de factureringscyclus, zal de effectieve eenheidsprijs fluctueren. De uiteindelijke prijs voor een bepaalde factureringscyclus is beschikbaar nadat we de verbruiksberekening hebben gestopt en de factureringsperiode hebben gesloten. U ziet de meeste wijzigingen in het verbruik na de vierde of vijfde decimale plaats.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Uitzoeken of voor uw meter gelaagde prijzen worden gebruikt

Als u niet weet of uw meter gelaagde prijzen gebruikt, gebruikt u de onderstaande procedure om erachter te komen. 

1. Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).
2. Selecteer **Verkopen,** selecteer **Prijzen en aanbiedingen** en selecteer vervolgens Prijzen voor **Azure-abonnement.**
3. Zoek uw meter op id en download vervolgens uw prijsgegevens. 

## <a name="sample-calculation"></a>Voorbeeldberekening

De onderstaande tabel geeft een voorbeeld van hoe we de effectieve eenheidsprijs berekenen tijdens de open periode.

In de tabel zijn de volgende waarden van toepassing: 

- **UP** = Eenheidsprijs van de resource/uur = 0,868

- **BCU** = Factureerbare verbruikseenheid voor de meter

- **BC** = Factureerbare kosten voor de meter = BCU * UP * 0,85. Dit weerspiegelt een aanpassing voor de PEC-korting van 15%. Vervolgens gebruiken we de onderste limiet van de functie om de waarde te beperken tot twee cijfers achter het decimaalteken om het minimumbedrag in rekening te brengen. 

- **Effectieve eenheidsprijs** = BCU/BC

>[!NOTE]

>Opmerking: De meter in dit voorbeeld heeft geen prijscategorie of andere kortingen: de effectieve eenheidsprijs houdt rekening met kortingspercentages en andere aanpassingen.


| Datum | BCU (factureerbare verbruikseenheid) | BC (factureerbare kosten) | Effectieve eenheidsprijs |
| ------ | ----------- | ----------- | ----------- |  
| 3 aug | 29 | 21.39 | 0.737586206896552 |
| 10 aug | 210.950039 | 155.63 | 0.737757626107858 |
| 25 aug | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Volgende stappen

- [Facturering en belastingen](billing.md)
