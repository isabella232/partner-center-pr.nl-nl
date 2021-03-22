---
title: Hoe BTW-beleid invloed heeft op de uitbetaling voor Azure Marketplace
description: Meer informatie over hoe BTW-beleid invloed heeft op de uitbetaling voor Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 817cdb895efab553b6f0131cdcdcf9b24bc6db3e
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768819"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Hoe BTW-beleid invloed heeft op de uitbetaling voor Azure Marketplace

**Juiste rollen**
-    Globale beheerder
-    Beheerder van gebruikers beheer
-    Beheer agent

## <a name="introduction"></a>Introductie

Micro soft Commercial Marketplace heeft wereld wijde bereik. Trans acties vinden plaats in de grenzen en afhankelijk van waar de ISV en de klant zich bevinden, kunnen de gevolgen voor de belasting verschillen. Microsoft AppSource en Azure Marketplace gebruiken de gegevens van het Partner Center-BTW-profiel om het land van de ISV te bepalen. Om het land van de klant te bepalen, kunt u de facturerings gegevens van de klant gebruiken of, als de klant zich in de EU bevindt, twee verschillende gegevens gebruiken.

Raadpleeg de tabel [Tax Details voor meer](tax-details-marketplace.md) informatie over de volgende scenario's, waarin wordt weer gegeven of micro soft belasting namens de uitgever verzamelt en betaalt, of dat de verantwoordelijkheid bij de uitgever hoort.

> [!NOTE]
> Alle voor beelden van verkoop waarden en BTW-percentages in dit onderwerp zijn alleen ter illustratie, niet van de exacte cijfers.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Publisher transacties in het land van door micro soft beheerde belasting

**Scenario A** : trans acties die plaatsvinden tussen een uitgever en een klant in een door [micro soft beheerd fiscaal land](tax-details-marketplace.md#microsoft-managed-countries). Deze trans acties zijn van toepassing op de belasting die op het moment van de verkoop geldt, en micro soft stuurt deze belasting naar het betreffende land. Er worden geen BTW-afbetalingen afgehouden van de toekenning en de uitbetalings berekeningen zijn exclusief BTW.

Zie [Scenario D](#foreign-publisher-transacts-with-us-customer) voor trans acties tussen een niet-Amerikaanse uitgever en een klant van de VS.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Geeft werk stroom weer voor het uitbetalings proces scenario A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Publisher transvindt zich in het land van micro soft Managed Tax waarbij de kosten voor Marketplace de belastde service zijn

**Scenario B** : trans acties die plaatsvinden tussen een US-gebaseerde Uitgever (zoals gedefinieerd door de informatie over het BTW-Profiel van de Partner Center) naar een klant in een door micro soft beheerd fiscaal land waar het land een belasting oplegt van de kosten voor Marketplace (een belaste dienst). In dit scenario wordt de belasting van de winkel service-kosten afgetrokken van de uitbetaling van de uitgever.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Geeft werk stroom voor het uitbetalings proces scenario B weer.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Publisher communiceert in een door Publisher beheerd land van belasting

**Scenario C** : trans acties die worden uitgevoerd tussen een uitgever en een klant in een door de uitgever beheerd fiscaal land dat geen bron belasting voor klanten oplegt. Klanten betalen geen BTW op het verkoop punt en het is de verplichting van de uitgever om alle toepasselijke belastingen te betalen.

Zie [Abonnementen en prijzen voor commerciële Marketplace-aanbiedingen](/azure/marketplace/plans-pricing#custom-prices)voor meer informatie over landspecifieke prijzen (bijvoorbeeld om toekomstige belasting te verrekenen).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Geeft werk stroom weer voor het uitbetalings proces scenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Afwijkende Uitgever communiceert met de klanten van de VS

**Scenario D** : alle externe uitgevers (zoals gedefinieerd door de informatie over het BTW-Profiel van het partner centrum) in landen zonder een Amerikaanse Verdrag (Zie [scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) een verkoop aan een klant in de VS (zoals gedefinieerd door het adres van de klant account). Voor de Amerikaanse overheid moet de belasting van micro soft worden geheven namens de uitgever. De BTW van de betaling aan de uitgever wordt berekend op basis van de prijs van de aanbieding.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Geeft werk stroom weer voor het uitbetalings proces scenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Afwijkende uitgever met een Verdrag draagt bij aan de klant

**Scenario E** : alle externe uitgevers (zoals gedefinieerd door de informatie over het BTW-Profiel van de Partner Center) in landen met een Amerikaanse Verdrag, waarbij een verkoop wordt gedaan aan een klant die is gebaseerd op de klant (zoals gedefinieerd in het adres van hun klanten account). Voor Amerikaanse overheid is micro soft niet verplicht om de belasting namens de uitgever te inhouden.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Geeft werk stroom weer voor het uitbetalings proces scenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Afwijkende Uitgever verkoopt aan een BTW-geregistreerde klant in een door micro soft beheerd land (buiten Ierland)

**Scenario F** : alle trans acties tussen externe uitgevers en de BTW-geregistreerde klanten van de EU (buiten Ierland) in een Microsoft-Managed land. De klant betaalt geen belasting op de verkoop.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Geeft werk stroom weer voor het uitbetalings proces scenario F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Afwijkende Uitgever verkoopt aan een BTW-geregistreerde klant in een door micro soft beheerd land (in Ierland)

**Scenario G** : alle trans acties tussen externe uitgevers en de BTW-geregistreerde klanten van de EU (in Ierland) in een Microsoft-Managed land. De klant betaalt Ierse BTW en micro soft betaalt deze belasting aan de Ierse overheid.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Geeft werk stroom weer voor het uitbetalings proces scenario G.":::

## <a name="next-steps"></a>Volgende stappen

- [Veelgestelde vragen over Uitgever](/azure/marketplace/marketplace-faq-publisher-guide)
- [Instructies voor het maken van betalings-en belasting profielen](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)