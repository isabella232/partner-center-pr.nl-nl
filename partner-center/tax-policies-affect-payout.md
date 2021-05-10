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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="f74c0-103">Hoe belastingbeleid van invloed is op uitbetaling voor Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f74c0-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="f74c0-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="f74c0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f74c0-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="f74c0-105">Global admin</span></span>
- <span data-ttu-id="f74c0-106">Beheerder van gebruikersbeheer</span><span class="sxs-lookup"><span data-stu-id="f74c0-106">User management admin</span></span>
- <span data-ttu-id="f74c0-107">Beheeragent</span><span class="sxs-lookup"><span data-stu-id="f74c0-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="f74c0-108">Introductie</span><span class="sxs-lookup"><span data-stu-id="f74c0-108">Introduction</span></span>

<span data-ttu-id="f74c0-109">De commerciële marketplace van Microsoft heeft een wereldwijd bereik.</span><span class="sxs-lookup"><span data-stu-id="f74c0-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="f74c0-110">Transacties vinden plaats buiten de grenzen en afhankelijk van waar de ISV en de klant zich bevinden, kunnen de gevolgen voor de belasting variëren.</span><span class="sxs-lookup"><span data-stu-id="f74c0-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="f74c0-111">Microsoft AppSource en Azure Marketplace de Partner Center belastingprofielgegevens gebruiken om het land van de ISV te bepalen.</span><span class="sxs-lookup"><span data-stu-id="f74c0-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="f74c0-112">Om het land van de klant te bepalen, gebruikt u de factureringsgegevens van de klant of, als de klant zich in de EU belandt, gebruiken we twee verschillende gegevens.</span><span class="sxs-lookup"><span data-stu-id="f74c0-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="f74c0-113">Voor een beter begrip van [](tax-details-marketplace.md) de volgende scenario's raadpleegt u de tabel Belastingdetails. Hier ziet u of Microsoft namens de uitgever belastingen int en betaalt of dat deze verantwoordelijkheid bij de uitgever hoort.</span><span class="sxs-lookup"><span data-stu-id="f74c0-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="f74c0-114">Alle voorbeelden van verkoopwaarden en belastingpercentages in dit onderwerp zijn alleen bedoeld ter illustratie, niet voor exacte cijfers.</span><span class="sxs-lookup"><span data-stu-id="f74c0-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="f74c0-115">Uitgeverstransacties in door Microsoft beheerd belastingland</span><span class="sxs-lookup"><span data-stu-id="f74c0-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="f74c0-116">**Scenario A:** transacties die plaatsvinden tussen een uitgever en een klant in een door [Microsoft beheerd belastingland.](tax-details-marketplace.md#microsoft-managed-countries)</span><span class="sxs-lookup"><span data-stu-id="f74c0-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="f74c0-117">Voor deze transacties wordt de toepasselijke belasting toegevoegd op het moment van verkoop en Microsoft verzendt die belasting naar het toepasselijke land.</span><span class="sxs-lookup"><span data-stu-id="f74c0-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="f74c0-118">Er worden geen belastingen ingehouden voor uitbetaling en uitbetalingsberekeningen zijn exclusief belasting.</span><span class="sxs-lookup"><span data-stu-id="f74c0-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="f74c0-119">Zie [Scenario D](#foreign-publisher-transacts-with-us-customer) voor transacties tussen een niet-Amerikaanse uitgever en een Amerikaanse klant.</span><span class="sxs-lookup"><span data-stu-id="f74c0-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="f74c0-121">Publisher Transacts in door Microsoft beheerd belastingland waar Marketplace-kosten een belastbare service zijn</span><span class="sxs-lookup"><span data-stu-id="f74c0-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="f74c0-122">**Scenario B:** transacties die plaatsvinden tussen een Amerikaanse uitgever (zoals gedefinieerd door hun Partner Center Tax Profile Information) naar een klant in een door Microsoft beheerd belastingland waar het land een belasting op de Marketplace-kosten (een belastbare service) oplegt.</span><span class="sxs-lookup"><span data-stu-id="f74c0-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="f74c0-123">In dit scenario wordt de belasting op de servicekosten van de winkel afgetrokken van de uitbetaling van de uitgever.</span><span class="sxs-lookup"><span data-stu-id="f74c0-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="f74c0-125">Uitgeverstransacties in door uitgever beheerd belastingland</span><span class="sxs-lookup"><span data-stu-id="f74c0-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="f74c0-126">**Scenario C:** transacties die plaatsvinden tussen een uitgever en een klant in een door de uitgever beheerd belastingland dat geen bronbelasting oplegt aan klanten.</span><span class="sxs-lookup"><span data-stu-id="f74c0-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="f74c0-127">Klanten betalen geen belasting op het verkooppunt en het is de verplichting van de uitgever om alle toepasselijke belastingen te betalen.</span><span class="sxs-lookup"><span data-stu-id="f74c0-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="f74c0-128">Zie Abonnementen en prijzen voor commerciële marketplace-aanbiedingen voor meer informatie over landspecifieke prijzen (bijvoorbeeld om toekomstige belastingen [te compenseren).](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="f74c0-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="f74c0-130">Foreign Publisher Transacts with US Customer</span><span class="sxs-lookup"><span data-stu-id="f74c0-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="f74c0-131">**Scenario D:** alle foreign publishers (zoals gedefinieerd door hun Partner Center Tax Profile Information) in landen zonder een Amerikaanse verantwoordelijke (zie [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) die een verkoop aan een Amerikaanse klant maakt (zoals gedefinieerd door het adres van hun klantaccount).</span><span class="sxs-lookup"><span data-stu-id="f74c0-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="f74c0-132">De Amerikaanse overheid vereist dat Microsoft bronbelasting int namens de uitgever.</span><span class="sxs-lookup"><span data-stu-id="f74c0-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="f74c0-133">De belasting die wordt ingehouden van uitbetaling aan de uitgever wordt berekend op basis van de prijs van de aanbieding.</span><span class="sxs-lookup"><span data-stu-id="f74c0-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="f74c0-135">Uitgever van het vreemde land met een Transacts-overeenkomst met een Amerikaanse klant</span><span class="sxs-lookup"><span data-stu-id="f74c0-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="f74c0-136">**Scenario E:** alle foreign publishers (zoals gedefinieerd door hun Partner Center Tax Profile Information) in landen waar een Amerikaanse klant een verkoop wil aanbieden aan een Amerikaanse klant (zoals gedefinieerd door het adres van hun klantaccount).</span><span class="sxs-lookup"><span data-stu-id="f74c0-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="f74c0-137">Voor de Amerikaanse overheid hoeft Microsoft geen belasting in te voeren namens de uitgever.</span><span class="sxs-lookup"><span data-stu-id="f74c0-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="f74c0-139">Een externe uitgever verkoopt aan een in de EU geregistreerde klant met btw in een door Microsoft beheerd land (buiten Ierland)</span><span class="sxs-lookup"><span data-stu-id="f74c0-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="f74c0-140">**Scenario F:** alle transacties tussen externe uitgevers en eu-klanten die zijn geregistreerd voor btw (buiten Ierland) in een Microsoft-Managed land.</span><span class="sxs-lookup"><span data-stu-id="f74c0-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="f74c0-141">De klant betaalt geen belasting over de verkoop.</span><span class="sxs-lookup"><span data-stu-id="f74c0-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="f74c0-143">Een vreemde uitgever verkoopt aan een in de EU geregistreerde klant in een door Microsoft beheerd land (in Ierland)</span><span class="sxs-lookup"><span data-stu-id="f74c0-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="f74c0-144">**Scenario G:** alle transacties tussen internationale uitgevers en eu-klanten met btw-registratie (binnen Ierland) in een Microsoft-Managed land.</span><span class="sxs-lookup"><span data-stu-id="f74c0-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="f74c0-145">De klant betaalt Btw en Microsoft betaalt deze belasting aan de Amerikaanse overheid.</span><span class="sxs-lookup"><span data-stu-id="f74c0-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Toont de werkstroom voor uitbetalingsprocesscenario G.":::

## <a name="next-steps"></a><span data-ttu-id="f74c0-147">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="f74c0-147">Next steps</span></span>

- [<span data-ttu-id="f74c0-148">Veelgestelde vragen over uitgevers</span><span class="sxs-lookup"><span data-stu-id="f74c0-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="f74c0-149">Instructies voor het maken van betalings- en belastingprofielen</span><span class="sxs-lookup"><span data-stu-id="f74c0-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)