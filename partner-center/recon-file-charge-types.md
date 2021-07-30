---
title: Kostentypen voor afstemmingsbestanden
ms.topic: article
ms.date: 06/05/2020
description: Ontdek de typen kosten (zoals op licentie gebaseerd, op gebruik gebaseerd en een keer), tegoeden en kortingen in Partner Center afstemmingsbestanden.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fe37a7cdc6ac8e60b9cc5672f4b53813e1f194f8
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114844238"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Inzicht in de verschillende kostentypen in Partner Center afstemmingsbestanden

**Van toepassing op**: Partner Center | Partner Center voor Microsoft Cloud for US Government

**Juiste rollen:** beheeragent | Factureringsbeheerder | Globale beheerder

In dit artikel worden de toewijzingen beschreven tussen een factuursectie en de bijbehorende kostentypen die mogelijk in uw afstemmingsbestand staan. Uw factuur bevat een overzicht van de kosten. Uw afstemmingsbestand biedt een gedetailleerde uitsplitsing van line-itemtransacties, inclusief kostentypen. Zie afstemmingsbestanden gebruiken voor meer informatie [over afstemmingsbestanden.](use-the-reconciliation-files.md)

Beide [afstemmingsbestanden](usage-based-recon-files.md) [](license-based-recon-files.md) op basis van gebruik en afstemmingsbestanden op basis van licenties tonen alleen gebruiksgerelateerde transacties en kosten (verbruikte eenheden en gerelateerde kosten).

> [!NOTE]
> Eenmalige tegoeden, kortingen of restituties die op de factuur worden weergegeven als **Aanpassingen** worden niet weergegeven in het afstemmingsbestand.

## <a name="map-charge-types-to-invoice-charges"></a>Kostentypen aan factuurkosten toe te rekenen

Als u wilt verwijzen naar kostenbedragen tussen uw factuur- en afstemmingsbestand, gebruikt u de filteropties in Microsoft Excel. Filter op kostentypen in uw afstemmingsbestand om de factuurkosten toe te rekenen aan een set kosteninsplitsingen op het afstemmingsbestand.

## <a name="license-based-charges"></a>Kosten op basis van licenties

Als u deze op licenties gebaseerde kosten wilt toevoegen aan uw factuur, somt u de kolom **Amount** uit het op licenties gebaseerde bestand op.

| Beschrijving van kosten (kolom ChargeType in afstemmingsbestand) | Uitleg over kosten |
| ------------------------------------------------------------- | ------------------ |
| Activeringskosten | Het bedrag dat aan de klant wordt in rekening gebracht wanneer deze het abonnement na aankoop gebruikt. |
| Kosten annuleren | Prorated charges refunded to the customer when associated licenses are changed. |
| Prorate instantie annuleren | Pro rated charges canceled when customer with monthly subscription has suspended and associated licenses changed within the same month. |
| Cycluskosten | Periodieke kosten voor een abonnement. |
| Prorate van cyclus-exemplaar | Pro rated charges assessed from the customer when associated licenses are changed. |
| Prorate fees when cancel (Prorate kosten bij annuleren) | Prorated refund for unused portion of service upon cancellation(Prorated refund for unused portion of service bij annulering). |
| Prorate fees when convert away from current offering (Prorate-kosten bij het omzetten van de huidige aanbieding) | Prorated charges after converting away from the current monthly subscription to an annual subscription( Prorated charges after converting away from the current monthly subscription to an annual subscription. |
| Prorate fees when convert to a new offering (Prorate-kosten bij conversie naar een nieuwe aanbieding) | Naar pro prognoses na het converteren van een maandelijks abonnement naar een nieuw jaarlijks abonnement. |
| Prorate kosten bij aankoop | Het kostentype voor een abonnement wanneer u maandelijkse of jaarlijkse facturering gebruikt. |
| Prorate fee when renew (Prorate fee bij verlenging) | Pro rated kosten bij abonnementsvernieuwing. |
| Kosten vernieuwen | Kosten voor het verlengen van een abonnement |
| Prorate fees when activate (Prorate kosten bij activeren) | Pro factureringskosten vanaf activering tot het einde van de factureringsperiode. |

## <a name="one-time-charges"></a>Eenkosten voor één keer

Als u deze een time-kosten wilt toevoegen aan uw factuur, somt u de kolom **Amount** uit het op licenties gebaseerde bestand op.

| Beschrijving van kosten (kolom ChargeType in afstemmingsbestand) | Uitleg over kosten |
| ------------------------------------------------------------- | ------------------ |
| nieuw | Wordt gebruikt wanneer een nieuwe aankoop wordt gemaakt. |
| vernieuwen | Wordt gebruikt wanneer een abonnement na het einde van de termijn wordt verlengd. |
| addQuantity | Wordt gebruikt in zowel de restitutie van de oorspronkelijke aankoop als de nieuwe hoeveelheid na een verhoging. |
| removeQuantity | Wordt gebruikt in zowel de restitutie van de oorspronkelijke aankoop als de nieuwe hoeveelheid na een afname. |
| cancelImmediate | Wordt gebruikt wanneer een abonnement wordt geannuleerd. |
| converteren | Wordt gebruikt wanneer een licentie wordt bijgewerkt. |
| customerCredit | Wordt gebruikt wanneer tegoeden (bijvoorbeeld Azure, SLA, enzovoort) worden gegeven voor een transactie. |

## <a name="usage-charges"></a>Gebruikskosten

Als u deze gebruikskosten wilt toevoegen aan uw factuur, somt u de kolom **PretaxCharges** op uit het bestand op basis van gebruik.

| Beschrijving van kosten (kolom ChargeType in afstemmingsbestand) | Uitleg over kosten |
| ------------------------------------------------------------- | ------------------ |
| Gebruikskosten beoordelen wanneer u annuleert | Toegang tot gebruikskosten na annulering van onbetaald gebruik tijdens de huidige factureringsperiode. |
| Gebruikskosten voor de huidige cyclus beoordelen | Toegangskosten voor de huidige factureringsperiode. |

### <a name="credits"></a>Tegoeden

Deze tegoeden aan uw factuur toe te wijsen:

- Som de **TotalForCustomer op** uit het op licenties gebaseerde bestand.
- Som de **kolom PostTaxTotal op** uit het bestand op basis van gebruik.

| Beschrijving van kosten (kolom ChargeType in afstemmingsbestand) | Uitleg over kosten |
| ------------------------------------------------------------- | ------------------ |
| Een regelitem verschoven | Gedeeltelijke of volledige restitutie voor een regelitem, inclusief belastingen. |

### <a name="usage-based-discounts"></a>Kortingen op basis van gebruik

Als u deze kortingen op basis van gebruik wilt toevoegen aan uw factuur, somt u de **kolom PretaxCharges** op uit het bestand op basis van gebruik.

| Beschrijving van kosten (kolom ChargeType in afstemmingsbestand) | Uitleg over kosten |
| ------------------------------------------------------------- | ------------------ |
| Activeringskorting | Korting die wordt toegepast wanneer het abonnement is geactiveerd. |
| Cycluskorting | Korting die wordt toegepast op periodieke kosten. |
| Korting vernieuwen | Korting die wordt toegepast wanneer het abonnement wordt verlengd. |
| Korting annuleren | Kosten die worden toegepast wanneer kortingen worden geannuleerd. |

### <a name="license-based-discounts"></a>Kortingen op basis van licenties

Als u op licenties gebaseerde kortingen wilt toevoegen aan uw factuur, somt u de **kolom TotalOtherDiscount** op uit het op licenties gebaseerde bestand.

*Op licenties gebaseerde kortingen kunnen worden toegepast op meerdere kostentypen.*
