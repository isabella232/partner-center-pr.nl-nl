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
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534893"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="12576-104">Microsoft Azure reserve ringen verkopen aan klanten met behulp van partner centrum, de Azure Portal of Api's</span><span class="sxs-lookup"><span data-stu-id="12576-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="12576-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="12576-105">**Appropriate roles**</span></span>

- <span data-ttu-id="12576-106">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="12576-106">Admin agent</span></span>
- <span data-ttu-id="12576-107">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="12576-107">Global admin</span></span>
- <span data-ttu-id="12576-108">Helpdesk medewerker</span><span class="sxs-lookup"><span data-stu-id="12576-108">Helpdesk agent</span></span>
- <span data-ttu-id="12576-109">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="12576-109">Sales agent</span></span>
- <span data-ttu-id="12576-110">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="12576-110">User management admin</span></span>

<span data-ttu-id="12576-111">Als partner in het Cloud Solution Provider-programma (CSP) kunt u Azure-reserve ringen voor klanten kopen, verkopen of beheren.</span><span class="sxs-lookup"><span data-stu-id="12576-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="12576-112">Gebruik partner centrum, de Azure Portal of de partner centrum-API.</span><span class="sxs-lookup"><span data-stu-id="12576-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="12576-113">Dit artikel is alleen van toepassing op partners in CSP.</span><span class="sxs-lookup"><span data-stu-id="12576-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="12576-114">Klanten die andere soorten abonnementen gebruiken (zoals betalen per gebruik, individuele, micro soft-klant overeenkomst of Enterprise Agreement-abonnementen), moeten in plaats daarvan [deze Azure rehanden documentatie](/azure/cost-management-billing/reservations)lezen.</span><span class="sxs-lookup"><span data-stu-id="12576-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="12576-115">Partners in het CSP-programma kunnen hun klanten een Microsoft Azure reserve ringen aanbieden.</span><span class="sxs-lookup"><span data-stu-id="12576-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="12576-116">Klanten kunnen aanzienlijke besparingen krijgen wanneer ze vooraf worden gereserveerd.</span><span class="sxs-lookup"><span data-stu-id="12576-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="12576-117">Azure-reserve ringen bieden klanten eenvoud en flexibiliteit op de volgende manieren:</span><span class="sxs-lookup"><span data-stu-id="12576-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="12576-118">Reserverings voorwaarden voor één of drie jaar</span><span class="sxs-lookup"><span data-stu-id="12576-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="12576-119">Gemakkelijk aan de slag te gaan. Setup is in enkele seconden voltooid</span><span class="sxs-lookup"><span data-stu-id="12576-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="12576-120">Gereserveerde instanties voor annuleren of uitwisselen op elk gewenst moment voor een gecorrigeerde restitutie</span><span class="sxs-lookup"><span data-stu-id="12576-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="12576-121">Gebruik van gereserveerde instanties beheren op het niveau van de organisatie of het individuele afdeling</span><span class="sxs-lookup"><span data-stu-id="12576-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="12576-122">Azure-reserve ringen kunnen aan klanten worden bezwaard op de volgende manieren:</span><span class="sxs-lookup"><span data-stu-id="12576-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="12576-123">Reserve ringen kunnen aanzienlijke besparingen opleveren dan prijzen voor betalen per gebruik (PAYG)</span><span class="sxs-lookup"><span data-stu-id="12576-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="12576-124">Betere budget tering en prognoses met een vooraf betaalde betaling voor een termijn van één jaar of drie jaar</span><span class="sxs-lookup"><span data-stu-id="12576-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="12576-125">Computer capaciteit met prioriteit in de Azure-regio die het dichtst bij hun kant is</span><span class="sxs-lookup"><span data-stu-id="12576-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="12576-126">Azure-reserve ringen bieden de basis voor end-to-end infrastructuur oplossingen in combi natie met software zoals micro soft Windows Server en Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="12576-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="12576-127">U kunt Azure-reserve ringen in het partner centrum en de Azure Portal kopen, verkopen en beheren en de Partner Center-API gebruiken.</span><span class="sxs-lookup"><span data-stu-id="12576-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="12576-128">U kunt uw klanten ook toestemming geven om hun eigen Azure-reserve ringen te kopen vanuit een Azure-abonnement dat u hebt aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="12576-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="12576-129">Volg de onderstaande koppelingen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="12576-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="12576-130">Resources voor Azure-reserve ringen</span><span class="sxs-lookup"><span data-stu-id="12576-130">Azure reservations resources</span></span>

|<span data-ttu-id="12576-131">**Voor informatie over**</span><span class="sxs-lookup"><span data-stu-id="12576-131">**For information about**</span></span>   |<span data-ttu-id="12576-132">**Leest u**</span><span class="sxs-lookup"><span data-stu-id="12576-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="12576-133">Documentatie voor Azure-reserve ringen voor uw klanten</span><span class="sxs-lookup"><span data-stu-id="12576-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="12576-134">Wat zijn Azure-reserveringen?</span><span class="sxs-lookup"><span data-stu-id="12576-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="12576-135">Azure-reserve ringen voor uw klanten kopen in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="12576-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="12576-136">Azure-reserve ringen kopen</span><span class="sxs-lookup"><span data-stu-id="12576-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="12576-137">Azure-reserve ringen beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="12576-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="12576-138">Azure-reserve ringen beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="12576-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="12576-139">De juiste VM-grootte bepalen en het gebruik van de virtuele machine van de klant controleren</span><span class="sxs-lookup"><span data-stu-id="12576-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="12576-140">VM-grootte voor maximum gebruik van Azure-reserve ring</span><span class="sxs-lookup"><span data-stu-id="12576-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="12576-141">Azure-reserve ringen aanschaffen met de Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="12576-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="12576-142">[Azure reserved VM instances kopen](/partner-center/develop/purchase-azure-reservations) in de ontwikkelaars documentatie van partner Center</span><span class="sxs-lookup"><span data-stu-id="12576-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="12576-143">Klanten toestemming geven om hun eigen Azure-reserve ringen te kopen vanuit uw CSP-abonnement.</span><span class="sxs-lookup"><span data-stu-id="12576-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="12576-144">Geef klanten toestemming om hun eigen Azure-reserve ringen te kopen</span><span class="sxs-lookup"><span data-stu-id="12576-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |