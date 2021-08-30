---
title: Prijswijzigingen in Marketplace-producten na publicatie
description: In dit artikel worden veelvoorkomende vragen beschreven over het wijzigen van de prijzen voor abonnementen na publicatie.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 08/27/2021
ms.openlocfilehash: bfb99986483d0aaaa5d685c266c8118c1345517c
ms.sourcegitcommit: 09d251409c2070fdb8ae5f9caa79152665fb2ddb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/30/2021
ms.locfileid: "123164870"
---
# <a name="price-changes-to-marketplace-products"></a>Prijswijzigingen in Marketplace-producten

Onafhankelijke softwareleveranciers (ISV's) die hun producten verkopen via Azure Marketplace mogen de abonnementsprijzen (of SKU's) van tijd tot tijd bijwerken. De nieuwe prijs van de SKU kan hoger of lager zijn dan de vorige prijs. De prijswijziging wordt bijgewerkt op product-/SKU-/marktniveau. Er kunnen dus prijsupdates zijn die relevant zijn voor sommige markten, maar niet voor alle.

In bepaalde gevallen (zie hieronder) kan de prijswijziging invloed hebben op producten die in het verleden zijn gekocht en ziet de klant een prijswijziging op de maandelijkse factuur. Azure Marketplace klanten die deze producten gebruiken ten minste 90 dagen voordat de nieuwe prijs van kracht wordt, op de hoogte.

## <a name="which-offer-types-can-be-affected-from-price-change"></a>Welke aanbiedingstypen kunnen worden beïnvloed door prijswijziging?

Alle veractieve producten die worden verkocht via Azure Marketplace en AppSource, bijvoorbeeld producten met een of meer abonnementen.

## <a name="can-a-free-sku-turn-one-day-into-a-paid-one"></a>Kan een gratis SKU één dag veranderen in een betaalde SKU?

Nee. De ISV kan een gratis SKU niet veranderen in een betaalde SKU. Een ISV die een product factureerbaar wil maken, moet een nieuwe betaalde SKU publiceren.

## <a name="price-increase-awareness-in-the-marketplace-product-pages"></a>Prijsverhogingsbewustheid op de marketplace-productpagina's

Zoals vermeld, moeten ISV's die een prijsverhoging willen publiceren, ten minste 90 dagen een waarschuwing geven voordat de nieuwe prijs van kracht wordt. Dit is om klanten te laten weten dat ze een product willen kopen. Marketplace-productpagina's worden ten minste 90 dagen van tevoren bijgewerkt bij de komende wijziging. De pagina's worden bijgewerkt met een bericht met gedetailleerde informatie over de aanstaande datum van de prijswijziging en het nieuwe tarief

:::image type="content" source="media/price-change/plan-pricing.png" alt-text="Illustreert de pagina met prijzen van het abonnement":::

> [!NOTE]
> De prijzen in de bovenstaande afbeelding zijn alleen bedoeld als voorbeeld. De werkelijke prijzen kunnen variëren.

Een dergelijke melding wordt alleen als de prijs omhoog gaat en niet als de prijs omlaag gaat.

## <a name="when-is-the-new-price-taking-effect"></a>Wanneer wordt de nieuwe prijs van kracht?

 De nieuwe ingangsdatum van de prijs is altijd aan het begin van een kalendermaand. Met de kennisgevingsperiode van 90 dagen ziet een typische tijdlijn voor prijsupdates er als volgende uit:

Jan-15: ISV werkt een toekomstige prijsupdate bij naar een SKU in de catalogus

Jan-16-18: productpagina wordt bijgewerkt met een waarschuwingsbericht over aanstaande prijsverhoging die van 1 mei (eind januari + 90 dagen) zal duren.

1 mei: de nieuwe prijs wordt van kracht

## <a name="customers-affected-from-a-price-change-post-purchase"></a>Klanten die worden beïnvloed door een prijswijziging (na aankoop)

De aankoop van een product vóór de ingangsdatum van de prijsverhoging biedt *geen* garantie voor de aankoopprijs voor de levensduur van de productimplementatie. Verschillende aanbiedingstypen die worden beïnvloed, zijn:

- Producten op basis van verbruik (bijvoorbeeld VM's die worden gefactureerd op basis van het uur of de prijs van het gebruik naar gebruik van SaaS of beheerde apps), zodra de nieuwe prijs van kracht is, zullen de kosten per verbruikseenheid toenemen. In het geval van klanten die midden in de maand worden gefactureerd, worden er twee regels in het maandelijkse gebruiksrapport vermeld: één voor verbruik tot de nieuwe ingangsdatum van de prijs (in het bovenstaande voorbeeld: 1 mei) en één voor het verbruik na de ingangsdatum
- Producten op basis van verbruik met maandelijkse kosten (zoals SaaS met aangepaste meters), verbruikseenheden worden beïnvloed als de nieuwe prijs van kracht wordt in de marketplace. De maandelijkse kosten blijven ongewijzigd tot het einde van de rechtenperiode.
- Producten op basis van een seat (zoals SaaS-services op basis van licenties) als de ingangsdatum van de prijswijziging na aankoop plaatsvindt, wordt de aankoopprijs gegarandeerd tot de volgende verlengingsdatum, of het nu gaat om maandelijkse verlenging of jaarlijkse verlengingsdatum.
    - Plaatsen toevoegen of verwijderen na de ingangsdatum van de prijswijziging, maar vóór de verlengingsdatum van het contract wordt bewaard tegen de oorspronkelijke aankoopprijs. Na verlenging wordt de nieuwe prijs van kracht.
    - Het wijzigen van de SKU, het wijzigen van de SKU na de ingangsdatum van de prijswijziging, wordt beschouwd als nieuwe aankoop en is onderhevig aan de nieuwe prijs. Deze wijziging geldt ook voor scenario's waarin het wijzigen van het aantal seats vereist dat de SKU van de klant wordt gewijzigd. Bijvoorbeeld een overstap van 400 seats naar 500 seats, waarvoor de klant mogelijk een nieuwe laag/SKU van het product moet aanschaffen.

## <a name="customer-notifications"></a>Klantmeldingen

Klanten die het product/de SKU al gebruiken op een markt die wordt beïnvloed door de aanstaande prijsverhoging, worden via e-mail op de hoogte gesteld van de aanstaande wijziging. Dit is zodat ze er actie op kunnen ondernemen als ze hiervoor kiezen. De e-mailmelding wordt 90 dagen vóór de nieuwe prijs van kracht verzonden en een tweede bericht wordt 30 dagen vóór de ingangsdatum van de prijswijziging verzonden. Het bericht wordt verzonden naar de eigenaar van de factuursectie (project), eigenaren van factureringsgroep en factureringsaccounteigenaren van het abonnement.

## <a name="next-steps"></a>Volgende stappen

- [Wat is Azure Marketplace?](azure-marketplace-overview.md)
- [Azure Marketplace kopen](azure-purchasing-invoicing.md)