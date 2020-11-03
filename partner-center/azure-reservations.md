---
title: Klanten Microsoft Azure reserve ringen verkopen
description: Als Cloud Solution Provider kunt u Azure-reserve ringen voor klanten kopen, verkopen of beheren. Gebruik partner centrum, de Azure Portal of de partner centrum-API.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528552"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="64a07-104">Microsoft Azure reserve ringen verkopen aan klanten met behulp van partner centrum, de Azure Portal of Api's</span><span class="sxs-lookup"><span data-stu-id="64a07-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="64a07-105">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="64a07-105">**Applies to**</span></span>

- <span data-ttu-id="64a07-106">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="64a07-106">Partner Center</span></span>
- <span data-ttu-id="64a07-107">Microsoft Azure-portal</span><span class="sxs-lookup"><span data-stu-id="64a07-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="64a07-108">Partners in het CSP-programma</span><span class="sxs-lookup"><span data-stu-id="64a07-108">Partners in the CSP program</span></span>

<span data-ttu-id="64a07-109">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="64a07-109">**Appropriate roles**</span></span>

- <span data-ttu-id="64a07-110">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="64a07-110">Admin agent</span></span>
- <span data-ttu-id="64a07-111">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="64a07-111">Global admin</span></span>
- <span data-ttu-id="64a07-112">Helpdesk medewerker</span><span class="sxs-lookup"><span data-stu-id="64a07-112">Helpdesk agent</span></span>
- <span data-ttu-id="64a07-113">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="64a07-113">Sales agent</span></span>
- <span data-ttu-id="64a07-114">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="64a07-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="64a07-115">Dit artikel is alleen van toepassing op partners in het Cloud Solution Provider-programma (CSP).</span><span class="sxs-lookup"><span data-stu-id="64a07-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="64a07-116">Klanten die andere soorten abonnementen gebruiken (zoals betalen per gebruik, individuele, micro soft-klant overeenkomst of Enterprise Agreement-abonnementen), moeten in plaats daarvan [deze Azure rehanden documentatie](/azure/cost-management-billing/reservations)lezen.</span><span class="sxs-lookup"><span data-stu-id="64a07-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="64a07-117">Partners in het CSP-programma kunnen hun klanten een Microsoft Azure reserve ringen aanbieden.</span><span class="sxs-lookup"><span data-stu-id="64a07-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="64a07-118">Klanten kunnen aanzienlijke besparingen krijgen wanneer ze vooraf worden gereserveerd.</span><span class="sxs-lookup"><span data-stu-id="64a07-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="64a07-119">Azure-reserve ringen bieden klanten eenvoud en flexibiliteit op de volgende manieren:</span><span class="sxs-lookup"><span data-stu-id="64a07-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="64a07-120">Reserverings voorwaarden voor één of drie jaar</span><span class="sxs-lookup"><span data-stu-id="64a07-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="64a07-121">Gemakkelijk aan de slag te gaan. Setup is in enkele seconden voltooid</span><span class="sxs-lookup"><span data-stu-id="64a07-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="64a07-122">Gereserveerde instanties voor annuleren of uitwisselen op elk gewenst moment voor een gecorrigeerde restitutie</span><span class="sxs-lookup"><span data-stu-id="64a07-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="64a07-123">Gebruik van gereserveerde instanties beheren op het niveau van de organisatie of het individuele afdeling</span><span class="sxs-lookup"><span data-stu-id="64a07-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="64a07-124">Azure-reserve ringen kunnen aan klanten worden bezwaard op de volgende manieren:</span><span class="sxs-lookup"><span data-stu-id="64a07-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="64a07-125">Reserve ringen kunnen aanzienlijke besparingen opleveren dan prijzen voor betalen per gebruik (PAYG)</span><span class="sxs-lookup"><span data-stu-id="64a07-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="64a07-126">Betere budget tering en prognoses met een vooraf betaalde betaling voor een termijn van één jaar of drie jaar</span><span class="sxs-lookup"><span data-stu-id="64a07-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="64a07-127">Computer capaciteit met prioriteit in de Azure-regio die het dichtst bij hun kant is</span><span class="sxs-lookup"><span data-stu-id="64a07-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="64a07-128">Azure-reserve ringen bieden de basis voor end-to-end infrastructuur oplossingen in combi natie met software zoals micro soft Windows Server en Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="64a07-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="64a07-129">U kunt Azure-reserve ringen in het partner centrum en de Azure Portal kopen, verkopen en beheren en de Partner Center-API gebruiken.</span><span class="sxs-lookup"><span data-stu-id="64a07-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="64a07-130">U kunt uw klanten ook toestemming geven om hun eigen Azure-reserve ringen te kopen vanuit een Azure-abonnement dat u hebt aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="64a07-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="64a07-131">Volg de onderstaande koppelingen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="64a07-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="64a07-132">Resources voor Azure-reserve ringen</span><span class="sxs-lookup"><span data-stu-id="64a07-132">Azure reservations resources</span></span>

|<span data-ttu-id="64a07-133">**Voor informatie over**</span><span class="sxs-lookup"><span data-stu-id="64a07-133">**For information about**</span></span>   |<span data-ttu-id="64a07-134">**Leest u**</span><span class="sxs-lookup"><span data-stu-id="64a07-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="64a07-135">Documentatie voor Azure-reserve ringen voor uw klanten</span><span class="sxs-lookup"><span data-stu-id="64a07-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="64a07-136">Wat zijn Azure-reserveringen?</span><span class="sxs-lookup"><span data-stu-id="64a07-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="64a07-137">Azure-reserve ringen voor uw klanten kopen in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="64a07-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="64a07-138">Azure-reserve ringen kopen</span><span class="sxs-lookup"><span data-stu-id="64a07-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="64a07-139">Azure-reserve ringen beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="64a07-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="64a07-140">Azure-reserve ringen beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="64a07-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="64a07-141">De juiste VM-grootte bepalen en het gebruik van de virtuele machine van de klant controleren</span><span class="sxs-lookup"><span data-stu-id="64a07-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="64a07-142">VM-grootte voor maximum gebruik van Azure-reserve ring</span><span class="sxs-lookup"><span data-stu-id="64a07-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="64a07-143">Azure-reserve ringen aanschaffen met de Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="64a07-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="64a07-144">[Azure reserved VM instances kopen](/partner-center/develop/purchase-azure-reservations) in de ontwikkelaars documentatie van partner Center</span><span class="sxs-lookup"><span data-stu-id="64a07-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="64a07-145">Klanten toestemming geven om hun eigen Azure-reserve ringen te kopen vanuit uw CSP-abonnement.</span><span class="sxs-lookup"><span data-stu-id="64a07-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="64a07-146">Geef klanten toestemming om hun eigen Azure-reserve ringen te kopen</span><span class="sxs-lookup"><span data-stu-id="64a07-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |