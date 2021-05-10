---
title: Hoe belastingbeleid van invloed is op uitbetaling voor Azure Marketplace
description: Meer informatie over hoe belastingbeleid van invloed is op uitbetaling Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686310"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Hoe belastingbeleid van invloed is op uitbetaling voor Azure Marketplace

**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikersbeheer
- Beheeragent

## <a name="introduction"></a>Introductie

De commerciële marketplace van Microsoft heeft een wereldwijd bereik. Transacties vinden plaats buiten de grenzen en afhankelijk van waar de ISV en de klant zich bevinden, kunnen de gevolgen voor de belasting variëren. Microsoft AppSource en Azure Marketplace de Partner Center belastingprofielgegevens gebruiken om het land van de ISV te bepalen. Om het land van de klant te bepalen, gebruikt u de factureringsgegevens van de klant of, als de klant zich in de EU belandt, gebruiken we twee verschillende gegevens.

Voor een beter begrip van [](tax-details-marketplace.md) de volgende scenario's raadpleegt u de tabel Belastingdetails. Hier ziet u of Microsoft namens de uitgever belastingen int en betaalt of dat deze verantwoordelijkheid bij de uitgever hoort.

> [!NOTE]
> Alle voorbeelden van verkoopwaarden en belastingpercentages in dit onderwerp zijn alleen bedoeld ter illustratie, niet voor exacte cijfers.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Uitgeverstransacties in door Microsoft beheerd belastingland

**Scenario A:** transacties die plaatsvinden tussen een uitgever en een klant in een door [Microsoft beheerd belastingland.](tax-details-marketplace.md#microsoft-managed-countries) Voor deze transacties wordt de toepasselijke belasting toegevoegd op het moment van verkoop en Microsoft verzendt die belasting naar het toepasselijke land. Er worden geen belastingen ingehouden voor uitbetaling en uitbetalingsberekeningen zijn exclusief belasting.

Zie [Scenario D](#foreign-publisher-transacts-with-us-customer) voor transacties tussen een niet-Amerikaanse uitgever en een Amerikaanse klant.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Publisher Transacts in door Microsoft beheerd belastingland waar Marketplace-kosten een belastbare service zijn

**Scenario B:** transacties die plaatsvinden tussen een Amerikaanse uitgever (zoals gedefinieerd door hun Partner Center Tax Profile Information) naar een klant in een door Microsoft beheerd belastingland waar het land een belasting op de Marketplace-kosten (een belastbare service) oplegt. In dit scenario wordt de belasting op de servicekosten van de winkel afgetrokken van de uitbetaling van de uitgever.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Uitgeverstransacties in door uitgever beheerd belastingland

**Scenario C:** transacties die plaatsvinden tussen een uitgever en een klant in een door de uitgever beheerd belastingland dat geen bronbelasting oplegt aan klanten. Klanten betalen geen belasting op het verkooppunt en het is de verplichting van de uitgever om alle toepasselijke belastingen te betalen.

Zie Abonnementen en prijzen voor commerciële marketplace-aanbiedingen voor meer informatie over landspecifieke prijzen (bijvoorbeeld om toekomstige belastingen [te compenseren).](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Foreign Publisher Transacts with US Customer

**Scenario D:** alle foreign publishers (zoals gedefinieerd door hun Partner Center Tax Profile Information) in landen zonder een Amerikaanse verantwoordelijke (zie [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) die een verkoop aan een Amerikaanse klant maakt (zoals gedefinieerd door het adres van hun klantaccount). De Amerikaanse overheid vereist dat Microsoft bronbelasting int namens de uitgever. De belasting die wordt ingehouden van uitbetaling aan de uitgever wordt berekend op basis van de prijs van de aanbieding.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Uitgever van het vreemde land met een Transacts-overeenkomst met een Amerikaanse klant

**Scenario E:** alle foreign publishers (zoals gedefinieerd door hun Partner Center Tax Profile Information) in landen waar een Amerikaanse klant een verkoop wil aanbieden aan een Amerikaanse klant (zoals gedefinieerd door het adres van hun klantaccount). Voor de Amerikaanse overheid hoeft Microsoft geen belasting in te voeren namens de uitgever.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Een externe uitgever verkoopt aan een in de EU geregistreerde klant met btw in een door Microsoft beheerd land (buiten Ierland)

**Scenario F:** alle transacties tussen externe uitgevers en eu-klanten die zijn geregistreerd voor btw (buiten Ierland) in een Microsoft-Managed land. De klant betaalt geen belasting over de verkoop.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>Een vreemde uitgever verkoopt aan een in de EU geregistreerde klant in een door Microsoft beheerd land (in Ierland)

**Scenario G:** alle transacties tussen internationale uitgevers en eu-klanten met btw-registratie (binnen Ierland) in een Microsoft-Managed land. De klant betaalt Btw en Microsoft betaalt deze belasting aan de Amerikaanse overheid.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario G.":::

## <a name="next-steps"></a>Volgende stappen

- [Veelgestelde vragen over uitgevers](/azure/marketplace/marketplace-faq-publisher-guide)
- [Instructies voor het maken van betalings- en belastingprofielen](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)