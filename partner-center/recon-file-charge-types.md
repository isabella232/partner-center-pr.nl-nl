---
title: Kosten typen van het afstemmings bestand
ms.topic: article
ms.date: 06/05/2020
description: Ontdek de typen kosten (zoals, op gebruik gebaseerde en eenmalige), tegoeden en kortingen in Partner Center-afstemmings bestanden.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/31/2020
ms.locfileid: "92527572"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Meer informatie over de verschillende kosten typen in Partner Center reconciliatie bestanden

**Van toepassing op**

- Partnercentrum
- Partner centrum voor Microsoft Cloud voor de Amerikaanse overheid

**Juiste rollen**

- Beheer agent
- Factureringsbeheerder
- Globale beheerder

In dit onderwerp vindt u een beschrijving van de toewijzingen tussen een factuur gedeelte en gekoppelde kosten typen die mogelijk in uw afstemmings bestand staan. Uw factuur bevat een samen vatting van de kosten. Uw afstemmings bestand bevat een gedetailleerde verdeling van trans acties met regel items, inclusief kosten typen. Zie [reconciliatie bestanden gebruiken](use-the-reconciliation-files.md)voor meer informatie over het afstemmen van bestanden.

Zowel [afstemmings bestanden op basis van gebruik](usage-based-recon-files.md) en [afstemmings bestanden op basis van een licentie](license-based-recon-files.md) geven alleen gebruiks gerelateerde trans acties en kosten (verbruikte eenheden en gerelateerde kosten) weer.

> [!NOTE]
> Eenmalige kredieten, kortingen of terugstortingen die worden weer gegeven op de factuur als **aanpassingen** , worden niet weer gegeven in het afstemmings bestand.

## <a name="map-charge-types-to-invoice-charges"></a>Kosten typen toewijzen aan facturerings kosten

Gebruik de filter opties in micro soft Excel om de bedragen te verdelen tussen uw factuur-en afstemmings bestand. Filter op kosten typen in het afstemmings bestand om de kosten van de factuur toe te wijzen aan een set toeslag uitsplitsingen in het afstemmings bestand.

## <a name="license-based-charges"></a>Kosten op basis van licenties

Als u deze kosten op basis van licenties aan uw factuur wilt toewijzen, moet u de kolom **bedrag** in het bestand op basis van licentie optellen.

| Beschrijving van kosten (kolom ChargeType in afstemmings bestand) | Uitleg bij kosten |
| ------------------------------------------------------------- | ------------------ |
| Activerings kosten | De hoeveelheid die bij de klant in rekening wordt gebracht wanneer deze na de aankoop gebruikmaakt van het abonnement. |
| Annulerings kosten | Gefactureerde kosten worden aan de klant gerestitueerd wanneer de gekoppelde licenties worden gewijzigd. |
| Exemplaar van prorente annuleren | Gefactureerde kosten worden geannuleerd wanneer de klant met een maandelijks abonnement abonnementen heeft opgeschort en de bijbehorende licenties zijn gewijzigd binnen dezelfde maand. |
| Cyclus kosten | Periodieke kosten voor een abonnement. |
| Cyclus exemplaar prorente | De geraamde kosten die van de klant worden berekend wanneer de gekoppelde licenties worden gewijzigd. |
| Tarief vergoedingen wanneer annuleren | Gefactureerde restitutie voor ongebruikt servicef onderdeel na annulering. |
| Kosten evenredigheid bij het converteren van de huidige aanbieding | Gefactureerde kosten na de conversie van het huidige maandelijkse abonnement op een jaar abonnement. |
| Kosten per tarief bij conversie naar een nieuwe aanbieding | Gefactureerde kosten nadat een maandelijks abonnement is geconverteerd naar een nieuw jaarlijks abonnement. |
| Tarief vergoedingen bij aankoop | Het type kosten voor een abonnement bij het gebruik van zowel maandelijkse als jaarlijkse facturering. |
| Tarief vergoeding bij verlenging | Gefactureerde kosten bij het verlengen van het abonnement. |
| Kosten verlengen | Kosten voor het vernieuwen van een abonnement |
| Tarief vergoedingen bij activeren | Gefactureerde kosten van de Activering tot het einde van de facturerings periode. |

## <a name="one-time-charges"></a>Eenmalige kosten

Als u deze eenmalige kosten aan uw factuur wilt toewijzen, moet u de kolom **bedrag** in het bestand op basis van licentie optellen.

| Beschrijving van kosten (kolom ChargeType in afstemmings bestand) | Uitleg bij kosten |
| ------------------------------------------------------------- | ------------------ |
| Nieuw | Wordt gebruikt wanneer een nieuwe aankoop wordt gemaakt. |
| addQuantity | Wordt gebruikt in de restitutie van de oorspronkelijke aankoop en de nieuwe hoeveelheid na een verhoging. |
| removeQuantity | Wordt gebruikt in de restitutie van de oorspronkelijke aankoop en de nieuwe hoeveelheid na een afname. |
| Annuleren | Wordt gebruikt wanneer een abonnement wordt geannuleerd. |
| Converteren | Wordt gebruikt wanneer een licentie wordt bijgewerkt, maar het aantal licenties blijft ongewijzigd. |

## <a name="usage-charges"></a>Gebruikskosten

Als u deze gebruiks kosten aan uw factuur wilt toewijzen, moet u de kolom **PretaxCharges** in het op gebruik gebaseerde bestand opsommen.

| Beschrijving van kosten (kolom ChargeType in afstemmings bestand) | Uitleg bij kosten |
| ------------------------------------------------------------- | ------------------ |
| Gebruiks kosten evalueren bij annuleren | Toegang tot gebruiks kosten na annulering voor onbetaald gebruik tijdens de huidige facturerings periode. |
| Gebruiks kosten evalueren voor de huidige cyclus | Gebruiks kosten voor de huidige facturerings periode. |

### <a name="credits"></a>Tegoeden

Deze tegoeden toewijzen aan uw factuur:

- Som van de **TotalForCustomer** van het bestand op basis van licentie.
- Som van de kolom **PostTaxTotal** van het bestand op basis van gebruik.

| Beschrijving van kosten (kolom ChargeType in afstemmings bestand) | Uitleg bij kosten |
| ------------------------------------------------------------- | ------------------ |
| Verschuiving van een regel item | Gedeeltelijke of volledige restitutie voor een regel item, inclusief BTW. |

### <a name="usage-based-discounts"></a>Kortingen op basis van gebruik

Als u deze op gebruik gebaseerde kortingen wilt toewijzen aan uw factuur, kunt u de kolom **PretaxCharges** van het bestand op basis van gebruik opsommen.

| Beschrijving van kosten (kolom ChargeType in afstemmings bestand) | Uitleg bij kosten |
| ------------------------------------------------------------- | ------------------ |
| Activerings korting | Korting toegepast wanneer het abonnement wordt geactiveerd. |
| Cyclus korting | Korting toegepast op periodieke kosten. |
| Korting vernieuwen | Korting toegepast wanneer het abonnement wordt verlengd. |
| Korting annuleren | Kosten worden toegepast wanneer kortingen worden geannuleerd. |

### <a name="license-based-discounts"></a>Kortingen op basis van licenties

Als u kortingen op basis van licenties aan uw factuur wilt toewijzen, moet u de kolom **TotalOtherDiscount** in het bestand op basis van licentie opsommen.

*Kortingen op basis van licenties kunnen worden toegepast op meerdere kosten typen.*
