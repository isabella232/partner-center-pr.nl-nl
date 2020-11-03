---
title: Azure-reserve ringen & server-abonnementen
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over de mogelijkheden van Cloud solution providers voor het verkrijgen, inrichten en beheren van Azure-reserve ringen en server abonnementen voor klanten.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528551"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="b6076-103">Azure reserved VM instances (RI) + server-abonnementen voor klanten verkrijgen, inrichten, & beheren</span><span class="sxs-lookup"><span data-stu-id="b6076-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="b6076-104">Van toepassing op:</span><span class="sxs-lookup"><span data-stu-id="b6076-104">Applies to:</span></span>

- <span data-ttu-id="b6076-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="b6076-105">Partner Center</span></span>

<span data-ttu-id="b6076-106">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="b6076-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b6076-107">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="b6076-107">Admin agent</span></span>
- <span data-ttu-id="b6076-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="b6076-108">Global admin</span></span>
- <span data-ttu-id="b6076-109">Helpdesk medewerker</span><span class="sxs-lookup"><span data-stu-id="b6076-109">Helpdesk agent</span></span>
- <span data-ttu-id="b6076-110">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="b6076-110">Sales agent</span></span>
- <span data-ttu-id="b6076-111">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="b6076-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="b6076-112">Dit artikel is alleen van toepassing op partners in het Cloud Solution Provider-programma (CSP).</span><span class="sxs-lookup"><span data-stu-id="b6076-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="b6076-113">Klanten die andere soorten abonnementen gebruiken (zoals betalen per gebruik, individuele, micro soft-klant overeenkomst of Enterprise Agreement-abonnementen), moeten in plaats daarvan [deze Azure rehanden documentatie](/azure/cost-management-billing/reservations)lezen.</span><span class="sxs-lookup"><span data-stu-id="b6076-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="b6076-114">Wat zijn Azure-reserveringen?</span><span class="sxs-lookup"><span data-stu-id="b6076-114">What are Azure Reservations?</span></span>

<span data-ttu-id="b6076-115">Azure Reservations helpt u geld te besparen door vooraf te betalen voor een virtuele machine van één of drie jaar, SQL Database reken capaciteit, Azure Cosmos DB door Voer of andere Azure-resources.</span><span class="sxs-lookup"><span data-stu-id="b6076-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="b6076-116">Als u vooraf betaalt, kunt u een korting krijgen op de resources die u gebruikt.</span><span class="sxs-lookup"><span data-stu-id="b6076-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="b6076-117">Met reserve ringen kunt u uw virtuele machine aanzienlijk reduceren, SQL database reken-, Azure Cosmos DB-en andere resource kosten tot 72% in vergelijking met de prijzen voor betalen per gebruik.</span><span class="sxs-lookup"><span data-stu-id="b6076-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="b6076-118">Reserveringen voorzien in een korting op de factuur en zijn niet van invloed op de runtime-status van uw resources.</span><span class="sxs-lookup"><span data-stu-id="b6076-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="b6076-119">Zie [Wat is Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b6076-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="b6076-120">Waarom moeten klanten een reserve ring aanschaffen?</span><span class="sxs-lookup"><span data-stu-id="b6076-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="b6076-121">Als klanten virtuele machines, Azure Cosmos DB-of SQL-data bases hebben die gedurende lange tijd worden uitgevoerd, biedt de aanschaf van een reserve ring de meest rendabele optie.</span><span class="sxs-lookup"><span data-stu-id="b6076-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="b6076-122">Als een klant bijvoorbeeld voortdurend vier exemplaren van een service uitvoert zonder een reserve ring, worden de kosten berekend op basis van betalen naar gebruik-tarieven.</span><span class="sxs-lookup"><span data-stu-id="b6076-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="b6076-123">Als ze een reserve ring voor deze resources kopen, krijgen ze onmiddellijk de reserverings korting.</span><span class="sxs-lookup"><span data-stu-id="b6076-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="b6076-124">De resources worden niet langer gefactureerd met de tarieven voor betalen per gebruik.</span><span class="sxs-lookup"><span data-stu-id="b6076-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="b6076-125">Fascinerende nieuwe Azure-aanbieding in CSP</span><span class="sxs-lookup"><span data-stu-id="b6076-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="b6076-126">Door Azure Reservations-en server abonnementen in te stellen op het CSP-programma, kan micro soft de partners beter helpen snel groeiende klant vragen te adresseren voor rendabele oplossingen ter ondersteuning van zeer voorspel bare, blijvende Cloud werkbelastingen.</span><span class="sxs-lookup"><span data-stu-id="b6076-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="b6076-127">Met het CSP-programma kunnen partners Azure Reservations-en server abonnementen verkrijgen, inrichten en beheren namens commerciële klanten via het micro soft partner centrum en Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="b6076-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="b6076-128">We bieden ook de mogelijkheden van onze CSP-Program ma's aan hoe Azure-reserve ringen kunnen worden aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="b6076-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="b6076-129">CSP-partners kunnen [Azure-reserve ringen namens een klant kopen](azure-reservations-buying.md) of ze kunnen [toestaan dat de klant hun eigen reserve ringen kan kopen](give-customers-permission.md) vanuit een eerder Azure-abonnement dat de partner hiervoor heeft gekocht.</span><span class="sxs-lookup"><span data-stu-id="b6076-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="b6076-130">Azure Reservations bieden klanten de flexibiliteit van virtualisatie voor een breed scala aan computer oplossingen, zoals ontwikkelen en testen, uitvoeren van toepassingen en uitbreiden van het Data Center.</span><span class="sxs-lookup"><span data-stu-id="b6076-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="b6076-131">Met [Azure reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) bijvoorbeeld kunnen commerciële klanten nu tot 72% besparen op prijzen van een Azure VM met betalen per gebruik, eenvoudigweg door de virtuele machine voor een periode van één of drie jaar aan te schaffen.</span><span class="sxs-lookup"><span data-stu-id="b6076-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="b6076-132">Windows Server-klanten met Azure Hybrid Benefit, die deel uitmaken van Software Assurance, kunnen Maxi maal 80% besparen op prijzen voor betalen per gebruik.</span><span class="sxs-lookup"><span data-stu-id="b6076-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="b6076-133">Met een niet-overeenkomende combi natie van aantrekkelijke prijzen en ongeëvenaarde implementatie flexibiliteit krijgen klanten de beste algemene waarde wanneer ze Azure Reservations kiezen:</span><span class="sxs-lookup"><span data-stu-id="b6076-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="b6076-134">Azure-reserveringen</span><span class="sxs-lookup"><span data-stu-id="b6076-134">Azure reservations</span></span>

- <span data-ttu-id="b6076-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="b6076-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="b6076-136">SQL DB-reserve ringen</span><span class="sxs-lookup"><span data-stu-id="b6076-136">SQL DB Reservations</span></span>
- <span data-ttu-id="b6076-137">SQL Managed Instance</span><span class="sxs-lookup"><span data-stu-id="b6076-137">SQL Managed Instance</span></span>
- <span data-ttu-id="b6076-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b6076-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="b6076-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="b6076-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="b6076-140">App Services</span><span class="sxs-lookup"><span data-stu-id="b6076-140">App Services</span></span>
- <span data-ttu-id="b6076-141">Reserve ringen van Azure Databricks eenheid</span><span class="sxs-lookup"><span data-stu-id="b6076-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="b6076-142">Managed Disk</span><span class="sxs-lookup"><span data-stu-id="b6076-142">Managed Disk</span></span>
- <span data-ttu-id="b6076-143">Blok-blob</span><span class="sxs-lookup"><span data-stu-id="b6076-143">Block blob</span></span>
- <span data-ttu-id="b6076-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="b6076-144">MySQL</span></span>
- <span data-ttu-id="b6076-145">Azure Data Explorer</span><span class="sxs-lookup"><span data-stu-id="b6076-145">Azure Data explorer</span></span>
- <span data-ttu-id="b6076-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="b6076-146">MariaDB</span></span>
- <span data-ttu-id="b6076-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="b6076-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="b6076-148">Server abonnementen</span><span class="sxs-lookup"><span data-stu-id="b6076-148">Server subscriptions</span></span>

- <span data-ttu-id="b6076-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="b6076-149">Windows Server</span></span>
- <span data-ttu-id="b6076-150">Cal's voor Extern bureaublad-services (RDS)</span><span class="sxs-lookup"><span data-stu-id="b6076-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="b6076-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="b6076-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="b6076-152">Jaarlijks ISV-abonnementen voor Linux</span><span class="sxs-lookup"><span data-stu-id="b6076-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="b6076-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="b6076-153">SUSE Linux</span></span>
- <span data-ttu-id="b6076-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="b6076-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="b6076-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="b6076-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="b6076-156">ISV'S, jaar abonnementen</span><span class="sxs-lookup"><span data-stu-id="b6076-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="b6076-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="b6076-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="b6076-158">Aan de slag</span><span class="sxs-lookup"><span data-stu-id="b6076-158">Getting started</span></span>

<span data-ttu-id="b6076-159">Als u wilt weten hoe u Azure Reservations kunt positioneren met uw klanten en zo snel mogelijk aan de slag gaat, wordt u aangeraden de volgende aanpak te volgen om de gereedheids materialen te controleren:</span><span class="sxs-lookup"><span data-stu-id="b6076-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="b6076-160">Bekijk de overzichts presentaties en de bijbehorende webinars voor de toegevoegde en positionering van de klant waarde</span><span class="sxs-lookup"><span data-stu-id="b6076-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="b6076-161">Bekijk en begrijp de moderne commerce-bedienings handleiding</span><span class="sxs-lookup"><span data-stu-id="b6076-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="b6076-162">Raadpleeg de veelgestelde vragen over Azure RI en server abonnementen</span><span class="sxs-lookup"><span data-stu-id="b6076-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="b6076-163">Informatie over updates voor Azure Reservations en server abonnementen in de [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="b6076-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="b6076-164">Resources</span><span class="sxs-lookup"><span data-stu-id="b6076-164">Resources</span></span>

<span data-ttu-id="b6076-165">Hieronder vindt u een uitgebreide lijst met resources die u kunnen helpen om snel op de slag te gaan met het omhandelen van Azure Reservations via het partner centrum:</span><span class="sxs-lookup"><span data-stu-id="b6076-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="b6076-166">Verkoop voorbereiding</span><span class="sxs-lookup"><span data-stu-id="b6076-166">Sales readiness</span></span>

- [<span data-ttu-id="b6076-167">Azure Reservations-en server abonnementen met Azure Hybrid Benefit overzicht</span><span class="sxs-lookup"><span data-stu-id="b6076-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="b6076-168">Verkoop overzicht</span><span class="sxs-lookup"><span data-stu-id="b6076-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="b6076-169">Veelgestelde vragen over partners voor Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="b6076-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="b6076-170">Veelgestelde vragen over partners voor Azure Reservations en SQL DB</span><span class="sxs-lookup"><span data-stu-id="b6076-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="b6076-171">Extern bureaublad-services (RDS) Client Access License (mede deling)</span><span class="sxs-lookup"><span data-stu-id="b6076-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="b6076-172">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="b6076-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="b6076-173">Server abonnementen</span><span class="sxs-lookup"><span data-stu-id="b6076-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="b6076-174">Overzicht van SQL-data base in azure</span><span class="sxs-lookup"><span data-stu-id="b6076-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="b6076-175">SQL DB-reserve ringen (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="b6076-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="b6076-176">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="b6076-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="b6076-177">SQL Managed instance (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="b6076-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="b6076-178">SUSE en Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="b6076-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="b6076-179">Red Hat Linux op Azure</span><span class="sxs-lookup"><span data-stu-id="b6076-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="b6076-180">SUSE Linux op Azure</span><span class="sxs-lookup"><span data-stu-id="b6076-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="b6076-181">Linux in Azure</span><span class="sxs-lookup"><span data-stu-id="b6076-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="b6076-182">Azure-prijs overzicht</span><span class="sxs-lookup"><span data-stu-id="b6076-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="b6076-183">Azure prijscalculator</span><span class="sxs-lookup"><span data-stu-id="b6076-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="b6076-184">Reserve ringen van Azure Databricks eenheid</span><span class="sxs-lookup"><span data-stu-id="b6076-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="b6076-185">CSP-prijs lijsten: de prijs lijsten **Microsoft Azure gereserveerde instanties** en **Software abonnementen** bevinden zich op de pagina prijzen van partner centrum [& aanbiedingen](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="b6076-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="b6076-186">Training</span><span class="sxs-lookup"><span data-stu-id="b6076-186">Training</span></span>

<span data-ttu-id="b6076-187">Meld u aan om de webinars-en on-demand-gebeurtenissen van [commerciële licentie verlening](https://commercial-licensing.eventbuilder.com/FY2019_ALL) te bekijken.</span><span class="sxs-lookup"><span data-stu-id="b6076-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="b6076-188">In het geval van licentie voorbereiding op aanvraag gebeurtenissen zijn onder andere onderwerpen zoals:</span><span class="sxs-lookup"><span data-stu-id="b6076-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="b6076-189">Online Services voor CSP'S, CSP Azure en algemene licentie-updates, waaronder Azure (november 2018)</span><span class="sxs-lookup"><span data-stu-id="b6076-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="b6076-190">Data base gereserveerde capaciteit & flexibiliteit van de instantie grootte (2018 augustus)</span><span class="sxs-lookup"><span data-stu-id="b6076-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="b6076-191">Server abonnementen in CSP (juli 2018)</span><span class="sxs-lookup"><span data-stu-id="b6076-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="b6076-192">Azure Reservations overzicht in CSP (mei 2018)</span><span class="sxs-lookup"><span data-stu-id="b6076-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="b6076-193">Andere nuttige training omvat de [Azure-licentie module op partner University](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="b6076-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="b6076-194">Bewerkingen</span><span class="sxs-lookup"><span data-stu-id="b6076-194">Operations</span></span>

- <span data-ttu-id="b6076-195">[Moderne commerce-bedienings handleiding](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (bijgewerkt): een uitgebreide hand leiding met betrekking tot het sleutel beleid en operationele aspecten, zoals overeenkomsten, best Ellen via partner centrum, factuur, prijs lijst Details, prikkels, afstemmings bestanden, API/SDK, sandbox en gedeelde Azure partner-services.</span><span class="sxs-lookup"><span data-stu-id="b6076-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="b6076-196">Modern aanbod Beschik baarheid land en matrix van klant valuta</span><span class="sxs-lookup"><span data-stu-id="b6076-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="b6076-197">Gereserveerde instanties van Microsoft Azure verkopen</span><span class="sxs-lookup"><span data-stu-id="b6076-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="b6076-198">Microsoft Azure reserve ringen namens uw klanten kopen</span><span class="sxs-lookup"><span data-stu-id="b6076-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="b6076-199">Azure-reserve ringen namens uw klanten beheren</span><span class="sxs-lookup"><span data-stu-id="b6076-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="b6076-200">Facturering voor Azure-reserve ringen</span><span class="sxs-lookup"><span data-stu-id="b6076-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="b6076-201">VM-grootte voor het gebruik van maximale reserve ring</span><span class="sxs-lookup"><span data-stu-id="b6076-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="b6076-202">Partner Center-API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="b6076-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="b6076-203">Extern bureaublad-services</span><span class="sxs-lookup"><span data-stu-id="b6076-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="b6076-204">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="b6076-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="b6076-205">Met de [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) kunt u meer waarde krijgen van uw Windows Server-licenties en kunt u Maxi maal \* 47 procent besparen op virtuele machines.</span><span class="sxs-lookup"><span data-stu-id="b6076-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="b6076-206">U kunt gebruikmaken van het voor deel van licenties voor Windows Server Data Center en Standard Edition die worden gedekt door Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="b6076-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="b6076-207">Afhankelijk van de editie kunt u uw licenties converteren of hergebruiken voor het uitvoeren van virtuele Windows Server-machines in Azure en een lager basis reken tarief betalen (tarieven voor virtuele Linux-machines).</span><span class="sxs-lookup"><span data-stu-id="b6076-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="b6076-208">Zie ook [Azure Hybrid Benefit Veelgestelde vragen](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="b6076-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="b6076-209">\* De werkelijke besparingen kunnen variëren, afhankelijk van de regio, het type instantie of het gebruik.</span><span class="sxs-lookup"><span data-stu-id="b6076-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
