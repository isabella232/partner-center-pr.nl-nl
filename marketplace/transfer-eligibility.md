---
title: Geschiktheid voor overdragen – richt lijnen voor het overdragen van een abonnement tussen facturerings accounts, Azure Marketplace
description: Richt lijnen voor commerciële controles voorafgaand aan het overdragen van een abonnement tussen facturerings accounts in de Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412553"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="777b9-103">Geschiktheid voor een abonnement overdragen tussen facturerings accounts</span><span class="sxs-lookup"><span data-stu-id="777b9-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="777b9-104">U kunt [een abonnement overzetten](/azure/cost-management-billing/understand/subscription-transfer) van het ene facturerings account naar het andere in het gedeelte Facturering van de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="777b9-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="777b9-105">Vóór een overdracht wordt het abonnement gescand op producten van derden.</span><span class="sxs-lookup"><span data-stu-id="777b9-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="777b9-106">De overdracht is alleen toegestaan als *alle* producten zijn gewist voor overdracht (Zie de onderstaande [criteria](#criteria-for-transfer-approval-or-denial) ).</span><span class="sxs-lookup"><span data-stu-id="777b9-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="777b9-107">Het systeem genereert relevante fout berichten voor de apps die niet kunnen worden gewist om de volgende stappen te bepalen.</span><span class="sxs-lookup"><span data-stu-id="777b9-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="777b9-108">Dit artikel is niet van toepassing op SaaS-aanbiedingen omdat SaaS-resources zijn gekoppeld aan een Tenant, niet op een abonnement.</span><span class="sxs-lookup"><span data-stu-id="777b9-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="777b9-109">SaaS-resources zijn overdraagbaar van het ene facturerings account naar het andere, maar dit gebeurt per resource en Azure-ondersteuning als ondersteunings aanvraag.</span><span class="sxs-lookup"><span data-stu-id="777b9-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="777b9-110">Criteria voor het goed keuren van de overdracht of weigering</span><span class="sxs-lookup"><span data-stu-id="777b9-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="777b9-111">U kunt een abonnement niet overdragen als een van de apps van derden aan een van de volgende criteria voldoet:</span><span class="sxs-lookup"><span data-stu-id="777b9-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="777b9-112">Het doel account is commercieel en de app is opt-out voor de verkoop via partners.</span><span class="sxs-lookup"><span data-stu-id="777b9-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="777b9-113">De app is opt-in voor geselecteerde partners en het doel account bevindt zich niet in de acceptatie lijst.</span><span class="sxs-lookup"><span data-stu-id="777b9-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="777b9-114">De aanbieding is in het verleden een preview-aanbieding voor geselecteerde abonnementen of het is een privé-aanbieding en het abonnement is niet langer beschikbaar in de acceptatie lijst.</span><span class="sxs-lookup"><span data-stu-id="777b9-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="777b9-115">Het nieuwe facturerings account bevindt zich in een andere regio dan waar de aanbieding wordt verkocht en de aanbieding wordt niet in die regio verkocht.</span><span class="sxs-lookup"><span data-stu-id="777b9-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="777b9-116">Een geblokkeerde overdracht blijft van kracht totdat u de resource uit het abonnement verwijdert, waarna u de overdracht opnieuw kunt proberen.</span><span class="sxs-lookup"><span data-stu-id="777b9-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="777b9-117">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="777b9-117">Next steps</span></span>

[<span data-ttu-id="777b9-118">Ontvang ondersteuning voor Microsoft AppSource en Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="777b9-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

