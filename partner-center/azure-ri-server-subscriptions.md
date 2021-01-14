---
title: Azure-reserve ringen & server-abonnementen
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over de mogelijkheden van Cloud solution providers voor het verkrijgen, inrichten en beheren van Azure-reserve ringen en server abonnementen voor klanten.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d5386dd4b2b19e641cc9d731d4a3d0f44ab5ad6
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182491"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="401cd-103">Azure reserved VM instances (RI) + server-abonnementen voor klanten verkrijgen, inrichten, & beheren</span><span class="sxs-lookup"><span data-stu-id="401cd-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="401cd-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="401cd-104">**Appropriate roles**</span></span>

- <span data-ttu-id="401cd-105">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="401cd-105">Admin agent</span></span>
- <span data-ttu-id="401cd-106">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="401cd-106">Global admin</span></span>
- <span data-ttu-id="401cd-107">Helpdesk medewerker</span><span class="sxs-lookup"><span data-stu-id="401cd-107">Helpdesk agent</span></span>
- <span data-ttu-id="401cd-108">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="401cd-108">Sales agent</span></span>
- <span data-ttu-id="401cd-109">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="401cd-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="401cd-110">Wat zijn Azure-reserveringen?</span><span class="sxs-lookup"><span data-stu-id="401cd-110">What are Azure Reservations?</span></span>

<span data-ttu-id="401cd-111">Azure Reservations helpt u geld te besparen door vooraf te betalen voor een virtuele machine van één of drie jaar, SQL Database reken capaciteit, Azure Cosmos DB door Voer of andere Azure-resources.</span><span class="sxs-lookup"><span data-stu-id="401cd-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="401cd-112">Als u vooraf betaalt, kunt u een korting krijgen op de resources die u gebruikt.</span><span class="sxs-lookup"><span data-stu-id="401cd-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="401cd-113">Met reserve ringen kunt u uw virtuele machine aanzienlijk reduceren, SQL database reken-, Azure Cosmos DB-en andere resource kosten tot 72% in vergelijking met de prijzen voor betalen per gebruik.</span><span class="sxs-lookup"><span data-stu-id="401cd-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="401cd-114">Reserveringen voorzien in een korting op de factuur en zijn niet van invloed op de runtime-status van uw resources.</span><span class="sxs-lookup"><span data-stu-id="401cd-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="401cd-115">Zie [Wat is Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="401cd-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="401cd-116">Waarom moeten klanten een reserve ring aanschaffen?</span><span class="sxs-lookup"><span data-stu-id="401cd-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="401cd-117">Als klanten virtuele machines, Azure Cosmos DB-of SQL-data bases hebben die gedurende lange tijd worden uitgevoerd, biedt de aanschaf van een reserve ring de meest rendabele optie.</span><span class="sxs-lookup"><span data-stu-id="401cd-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="401cd-118">Als een klant bijvoorbeeld voortdurend vier exemplaren van een service uitvoert zonder een reserve ring, worden de kosten berekend op basis van betalen naar gebruik-tarieven.</span><span class="sxs-lookup"><span data-stu-id="401cd-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="401cd-119">Als ze een reserve ring voor deze resources kopen, krijgen ze onmiddellijk de reserverings korting.</span><span class="sxs-lookup"><span data-stu-id="401cd-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="401cd-120">De resources worden niet langer gefactureerd met de tarieven voor betalen per gebruik.</span><span class="sxs-lookup"><span data-stu-id="401cd-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="401cd-121">Fascinerende nieuwe Azure-aanbieding in CSP</span><span class="sxs-lookup"><span data-stu-id="401cd-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="401cd-122">Door Azure Reservations-en server abonnementen in te stellen op het CSP-programma, kan micro soft de partners beter helpen snel groeiende klant vragen te adresseren voor rendabele oplossingen ter ondersteuning van zeer voorspel bare, blijvende Cloud werkbelastingen.</span><span class="sxs-lookup"><span data-stu-id="401cd-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="401cd-123">Met het CSP-programma kunnen partners Azure Reservations-en server abonnementen verkrijgen, inrichten en beheren namens commerciële klanten via het micro soft partner centrum en Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="401cd-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="401cd-124">We bieden ook de mogelijkheden van onze CSP-Program ma's aan hoe Azure-reserve ringen kunnen worden aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="401cd-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="401cd-125">CSP-partners kunnen [Azure-reserve ringen namens een klant kopen](azure-reservations-buying.md) of ze kunnen [toestaan dat de klant hun eigen reserve ringen kan kopen](give-customers-permission.md) vanuit een eerder Azure-abonnement dat de partner hiervoor heeft gekocht.</span><span class="sxs-lookup"><span data-stu-id="401cd-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="401cd-126">Azure Reservations bieden klanten de flexibiliteit van virtualisatie voor een breed scala aan computer oplossingen, zoals ontwikkelen en testen, uitvoeren van toepassingen en uitbreiden van het Data Center.</span><span class="sxs-lookup"><span data-stu-id="401cd-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="401cd-127">Met [Azure reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) bijvoorbeeld kunnen commerciële klanten nu tot 72% besparen op prijzen van een Azure VM met betalen per gebruik, eenvoudigweg door de virtuele machine voor een periode van één of drie jaar aan te schaffen.</span><span class="sxs-lookup"><span data-stu-id="401cd-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="401cd-128">Windows Server-klanten met Azure Hybrid Benefit, die deel uitmaken van Software Assurance, kunnen Maxi maal 80% besparen op prijzen voor betalen per gebruik.</span><span class="sxs-lookup"><span data-stu-id="401cd-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="401cd-129">Met een niet-overeenkomende combi natie van aantrekkelijke prijzen en ongeëvenaarde implementatie flexibiliteit krijgen klanten de beste algemene waarde wanneer ze Azure Reservations kiezen.</span><span class="sxs-lookup"><span data-stu-id="401cd-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="401cd-130">Zie [reserve ringen kopen](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) in azure Portal.</span><span class="sxs-lookup"><span data-stu-id="401cd-130">See [Purchase Reservations](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="401cd-131">Zie de **commerciële prijs lijst van Azure RI CSP** onder de categorie **Microsoft Azure gereserveerde instanties** op de pagina [prijzen en aanbiedingen](https://partner.microsoft.com/dashboard/sell/pricingandoffers) van het partner centrum voor software abonnementen en Linux-ISV-abonnementen.</span><span class="sxs-lookup"><span data-stu-id="401cd-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="401cd-132">**Jaarlijks ISV-abonnementen voor Linux**</span><span class="sxs-lookup"><span data-stu-id="401cd-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="401cd-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="401cd-133">SUSE Linux</span></span>
- <span data-ttu-id="401cd-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="401cd-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="401cd-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="401cd-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="401cd-136">**ISV'S, jaar abonnementen**</span><span class="sxs-lookup"><span data-stu-id="401cd-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="401cd-137">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="401cd-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="401cd-138">Aan de slag</span><span class="sxs-lookup"><span data-stu-id="401cd-138">Getting started</span></span>

<span data-ttu-id="401cd-139">Als u wilt weten hoe u Azure Reservations kunt positioneren met uw klanten en zo snel mogelijk aan de slag gaat, wordt u aangeraden de volgende aanpak te volgen om de gereedheids materialen te controleren:</span><span class="sxs-lookup"><span data-stu-id="401cd-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="401cd-140">Bekijk en begrijp de [nieuwe Commerce Operations Guide van het partner centrum](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span><span class="sxs-lookup"><span data-stu-id="401cd-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="401cd-141">Informatie over updates voor Azure Reservations en server abonnementen in de [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span><span class="sxs-lookup"><span data-stu-id="401cd-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="401cd-142">Verkoop voorbereiding</span><span class="sxs-lookup"><span data-stu-id="401cd-142">Sales readiness</span></span>

- [<span data-ttu-id="401cd-143">Extern bureaublad-services (RDS) Client Access License (mede deling)</span><span class="sxs-lookup"><span data-stu-id="401cd-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="401cd-144">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="401cd-144">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="401cd-145">Server abonnementen</span><span class="sxs-lookup"><span data-stu-id="401cd-145">Server Subscriptions</span></span>](./csp-software-subscriptions.md)

- [<span data-ttu-id="401cd-146">SQL DB-reserve ringen (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="401cd-146">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="401cd-147">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="401cd-147">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="401cd-148">SQL Managed instance (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="401cd-148">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="401cd-149">SUSE en Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="401cd-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="401cd-150">Red Hat Linux op Azure</span><span class="sxs-lookup"><span data-stu-id="401cd-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="401cd-151">SUSE Linux op Azure</span><span class="sxs-lookup"><span data-stu-id="401cd-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="401cd-152">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="401cd-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="401cd-153">Azure-prijs overzicht</span><span class="sxs-lookup"><span data-stu-id="401cd-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="401cd-154">Azure prijscalculator</span><span class="sxs-lookup"><span data-stu-id="401cd-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="401cd-155">Reserve ringen van Azure Databricks eenheid</span><span class="sxs-lookup"><span data-stu-id="401cd-155">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="401cd-156">Training</span><span class="sxs-lookup"><span data-stu-id="401cd-156">Training</span></span>

<span data-ttu-id="401cd-157">Meld u aan om de webinars-en on-demand-gebeurtenissen van [commerciële licentie verlening](https://commercial-licensing.eventbuilder.com/FY2019_ALL) te bekijken.</span><span class="sxs-lookup"><span data-stu-id="401cd-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="401cd-158">Eerder vastgelegde licenties op aanvraag voor de licentie controle zijn onder meer onderwerpen als:</span><span class="sxs-lookup"><span data-stu-id="401cd-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="401cd-159">Online Services voor CSP'S, CSP Azure en algemene licentie-updates, waaronder Azure (november 2018)</span><span class="sxs-lookup"><span data-stu-id="401cd-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="401cd-160">Data base gereserveerde capaciteit & flexibiliteit van de instantie grootte (2018 augustus)</span><span class="sxs-lookup"><span data-stu-id="401cd-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="401cd-161">Server abonnementen in CSP (juli 2018)</span><span class="sxs-lookup"><span data-stu-id="401cd-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="401cd-162">Azure Reservations overzicht in CSP (mei 2018)</span><span class="sxs-lookup"><span data-stu-id="401cd-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="401cd-163">Bewerkingen</span><span class="sxs-lookup"><span data-stu-id="401cd-163">Operations</span></span>

<span data-ttu-id="401cd-164">[Partner centrum nieuwe Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): uitgebreide hand leiding met betrekking tot het sleutel beleid en operationele aspecten, zoals overeenkomsten, best Ellen via partner centrum, factuur, prijs lijst Details, prikkels, afstemmings bestanden, API/SDK, sandbox en gedeelde Azure partner-services.</span><span class="sxs-lookup"><span data-stu-id="401cd-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="401cd-165">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="401cd-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="401cd-166">De [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is een prijs voordelen voor klanten die licenties hebben met Software Assurance, waarmee u de waarde van bestaande on-premises Windows Server-en/of SQL Server-licentie investeringen kunt maximaliseren wanneer u naar Azure migreert.</span><span class="sxs-lookup"><span data-stu-id="401cd-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="401cd-167">In aanmerking komende klanten kunnen Maxi maal 40% \* besparen op Azure Virtual Machines (infra structuur als een service of IaaS), en tot 55% besparen op Azure SQL Database (platform as a service of PaaS) en SQL Server op Azure Virtual Machines (IaaS) met Azure Hybrid Benefit, wat in combi natie met gereserveerde instanties van Azure wordt verhoogd tot 80%.</span><span class="sxs-lookup"><span data-stu-id="401cd-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="401cd-168">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="401cd-168">Next steps</span></span>

- [<span data-ttu-id="401cd-169">Veelgestelde vragen over Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="401cd-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="401cd-170">\* De werkelijke besparingen kunnen variëren, afhankelijk van de regio, het type instantie of het gebruik.</span><span class="sxs-lookup"><span data-stu-id="401cd-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>