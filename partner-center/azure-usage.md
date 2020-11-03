---
title: Het formaat van Azure-VM's wijzigen voor een maximaal reserveringsgebruik
description: Meer informatie over hoe u de grootte van een virtuele machine (VM) kunt aanpassen aan de computer vereisten van uw klanten wanneer u Microsoft Azure reserve ringen voor hen aanschaft.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: e6c4e3e7a68de720f586754703308a447d7d30c1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528549"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="306a2-103">Het formaat van Microsoft Azure-VM’s wijzigen voor een maximaal reserveringsgebruik</span><span class="sxs-lookup"><span data-stu-id="306a2-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="306a2-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="306a2-104">**Applies to**</span></span>

- <span data-ttu-id="306a2-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="306a2-105">Partner Center</span></span>
- <span data-ttu-id="306a2-106">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="306a2-106">Azure portal</span></span>
- <span data-ttu-id="306a2-107">Partners in het CSP-programma</span><span class="sxs-lookup"><span data-stu-id="306a2-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="306a2-108">Dit artikel is alleen van toepassing op partners in het Cloud Solution Provider-programma (CSP).</span><span class="sxs-lookup"><span data-stu-id="306a2-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="306a2-109">Klanten die andere soorten abonnementen gebruiken (zoals betalen per gebruik, individuele, micro soft-klant overeenkomst of Enterprise Agreement-abonnementen), moeten in plaats daarvan [deze Azure rehanden documentatie](/azure/cost-management-billing/reservations)lezen.</span><span class="sxs-lookup"><span data-stu-id="306a2-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="306a2-110">De VM-grootte voor de Azure-reserve ring van een klant bepalen</span><span class="sxs-lookup"><span data-stu-id="306a2-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="306a2-111">Wanneer u Microsoft Azure reserve ringen namens uw klanten koopt, moet u een grootte van een virtuele machine (VM) kiezen om te voldoen aan de computer behoeften van de klant.</span><span class="sxs-lookup"><span data-stu-id="306a2-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="306a2-112">U kunt deze informatie vinden met een van de volgende methoden:</span><span class="sxs-lookup"><span data-stu-id="306a2-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="306a2-113">Azure-gebruiks-API</span><span class="sxs-lookup"><span data-stu-id="306a2-113">Azure utilization API</span></span>
- <span data-ttu-id="306a2-114">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="306a2-114">The Azure portal</span></span>
- <span data-ttu-id="306a2-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="306a2-115">Azure PowerShell</span></span>
- <span data-ttu-id="306a2-116">De Azure Resource Manager-API (ARM)</span><span class="sxs-lookup"><span data-stu-id="306a2-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="306a2-117">Hieronder vindt u instructies voor het gebruik van deze methoden.</span><span class="sxs-lookup"><span data-stu-id="306a2-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="306a2-118">Nadat u een reserve ring hebt gekocht, wordt de reserverings korting automatisch toegepast op virtuele machines die overeenkomen met de kenmerken en hoeveelheid van de reserve ring.</span><span class="sxs-lookup"><span data-stu-id="306a2-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="306a2-119">U hoeft de reserve ring niet aan een virtuele machine toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="306a2-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="306a2-120">Reserverings kortingen zijn niet van toepassing op klassieke of promotie-Vm's.</span><span class="sxs-lookup"><span data-stu-id="306a2-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="306a2-121">Als u het type en de grootte van de virtuele machine die u wilt kopen namens uw klant correct wilt identificeren, moet u een van de volgende methoden gebruiken omdat het type VM-reeks niet correct wordt weer gegeven in de reconciliatie bestanden van partner Center.</span><span class="sxs-lookup"><span data-stu-id="306a2-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="306a2-122">Informatie over VM-grootte ophalen met behulp van de Azure-gebruiks-API</span><span class="sxs-lookup"><span data-stu-id="306a2-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="306a2-123">Gebruik het kenmerk waarde voor service type vanuit additionalInfo in de API-reactie om de te kopen VM-grootte te identificeren.</span><span class="sxs-lookup"><span data-stu-id="306a2-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="306a2-124">Zie voor meer informatie [klant gebruiks records voor Azure ophalen](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in de [partner centrum-API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="306a2-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="306a2-125">Informatie over VM-grootte ophalen met behulp van de Microsoft Azure-portal</span><span class="sxs-lookup"><span data-stu-id="306a2-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="306a2-126">Ga in Partner Center naar uw **klanten** pagina.</span><span class="sxs-lookup"><span data-stu-id="306a2-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="306a2-127">Zoek de klant die Azure-VM-reserve ringen wil kopen en selecteer vervolgens de pijl-omlaag om de gegevens van de klant uit te breiden.</span><span class="sxs-lookup"><span data-stu-id="306a2-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="306a2-128">Selecteer **Microsoft Azure Management Portal** om de record van de klant te openen in de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="306a2-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="306a2-129">Selecteer **virtuele machines** in het menu van de portal en selecteer vervolgens de virtuele machine waarvoor u een reserve ring wilt kopen.</span><span class="sxs-lookup"><span data-stu-id="306a2-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="306a2-130">Zoek op de detail pagina van de virtuele machine naar de informatie over de grootte en regio, zoals hieronder wordt weer gegeven, en gebruik deze informatie om de reserve ring te kopen in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="306a2-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Informatie over grootte en regio op de detail pagina":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="306a2-132">Informatie over VM-grootte ophalen met behulp van Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="306a2-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="306a2-133">Gebruik de informatie in de onderstaande afbeelding om de locatie en grootte van de virtuele machine op te halen waarvoor u een reserve ring wilt kopen.</span><span class="sxs-lookup"><span data-stu-id="306a2-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Locatie en grootte van virtuele machine":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="306a2-135">Informatie over VM-grootte ophalen met behulp van de API voor Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="306a2-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="306a2-136">Roep de ARM-client voor de virtuele machine waarvoor u een reserve ring wilt kopen met behulp van de ARMClient-of ARM-Api's.</span><span class="sxs-lookup"><span data-stu-id="306a2-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="306a2-137">/Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="306a2-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="306a2-138">De aanroep retourneert de waarden voor **vmSize** en **locatie** , zoals hieronder wordt weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="306a2-138">The call returns the values for **vmSize** and **location** , as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="waarde vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="locatie waarde":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="306a2-141">Azure VM-gebruik en-reserverings korting controleren</span><span class="sxs-lookup"><span data-stu-id="306a2-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="306a2-142">Nadat u een voor Azure gereserveerde VM-instantie hebt aangeschaft namens een klant, wordt de korting voor het vooraf betalen van VM-ruimte automatisch toegepast op de virtuele machines die overeenkomen met de kenmerken en hoeveelheid van de reserve ring van de klant.</span><span class="sxs-lookup"><span data-stu-id="306a2-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="306a2-143">U kunt het reserverings gebruik van de klant controleren en zien op welke virtuele machines de reserverings kortingen worden toegepast met behulp van een van de volgende methoden:</span><span class="sxs-lookup"><span data-stu-id="306a2-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="306a2-144">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="306a2-144">The Azure portal</span></span>
- <span data-ttu-id="306a2-145">Azure-gebruiks-API</span><span class="sxs-lookup"><span data-stu-id="306a2-145">Azure utilization API</span></span>

<span data-ttu-id="306a2-146">Hieronder vindt u instructies voor het gebruik van deze methoden.</span><span class="sxs-lookup"><span data-stu-id="306a2-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="306a2-147">Alleen de Azure-gebruiks-API laat zien op welke virtuele machine de korting wordt toegepast.</span><span class="sxs-lookup"><span data-stu-id="306a2-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="306a2-148">Controleer het reserverings gebruik van de klant in de Microsoft Azure-portal</span><span class="sxs-lookup"><span data-stu-id="306a2-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="306a2-149">Ga in Partner Center naar uw **klanten** pagina.</span><span class="sxs-lookup"><span data-stu-id="306a2-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="306a2-150">Zoek de klant waarvan u de reserverings korting en het gebruik wilt controleren en selecteer vervolgens de pijl-omlaag om de gegevens van de klant uit te breiden.</span><span class="sxs-lookup"><span data-stu-id="306a2-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="306a2-151">Selecteer **Microsoft Azure Management Portal** om de record van de klant te openen in de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="306a2-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="306a2-152">Selecteer **reserve ringen** in het menu van de portal en selecteer vervolgens de reserve ring waarvoor u het gebruik wilt controleren.</span><span class="sxs-lookup"><span data-stu-id="306a2-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="306a2-153">Controleer op de pagina **overzicht** de gebruiks grafiek van de reserve ring, waarin wordt weer gegeven hoeveel van de reserve ring is toegepast op virtuele machines.</span><span class="sxs-lookup"><span data-stu-id="306a2-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="306a2-154">Gebruiks gegevens kunnen Maxi maal acht uur worden vertraagd.</span><span class="sxs-lookup"><span data-stu-id="306a2-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="306a2-155">a.</span><span class="sxs-lookup"><span data-stu-id="306a2-155">a.</span></span> <span data-ttu-id="306a2-156">Als het gebruik van de reserve ring 100% is, krijgt uw klant alle mogelijke besparingen die de aankoop van de reserve ring kan bieden.</span><span class="sxs-lookup"><span data-stu-id="306a2-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="306a2-157">b.</span><span class="sxs-lookup"><span data-stu-id="306a2-157">b.</span></span> <span data-ttu-id="306a2-158">Als het gebruik van de reserve ring 0% is, wordt de korting niet toegepast op een virtuele machine.</span><span class="sxs-lookup"><span data-stu-id="306a2-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="306a2-159">c.</span><span class="sxs-lookup"><span data-stu-id="306a2-159">c.</span></span> <span data-ttu-id="306a2-160">Als het gebruik van de reserve ring tussen 1% en 99% ligt, zijn er ongebruikte voor delen.</span><span class="sxs-lookup"><span data-stu-id="306a2-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="306a2-161">Om deze situatie te voor komen, bepaalt u de juiste VM-grootte voor de ondersteuning van de computer behoeften van de klant voordat u de aanschaft.</span><span class="sxs-lookup"><span data-stu-id="306a2-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="306a2-162">Het reserverings gebruik van de klant controleren met de Azure-gebruiks-API</span><span class="sxs-lookup"><span data-stu-id="306a2-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="306a2-163">Alleen de Azure-gebruiks-API laat zien op welke virtuele machine de korting wordt toegepast.</span><span class="sxs-lookup"><span data-stu-id="306a2-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="306a2-164">U kunt gegevens over reserverings gebruik ophalen met de API voor Azure-gebruik om te controleren of de klant de reserverings korting krijgt en te zien op welke Vm's (virtuele machines) de korting wordt toegepast.</span><span class="sxs-lookup"><span data-stu-id="306a2-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="306a2-165">Vergelijk voor beeld A met voor beeld B om te zien hoe u het reserverings gebruik van een klant kunt controleren.</span><span class="sxs-lookup"><span data-stu-id="306a2-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Voor beelden van reserverings gebruik":::

- <span data-ttu-id="306a2-167">De reservationId identificeert de Azure-reserve ring die is gebruikt voor het Toep assen van de korting op de virtuele machine.</span><span class="sxs-lookup"><span data-stu-id="306a2-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="306a2-168">consumptionMeter is de MeterId voor de virtuele machine waarop de reserverings korting van toepassing is.</span><span class="sxs-lookup"><span data-stu-id="306a2-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="306a2-169">De ReservationMeter toont $0 kosten sinds de reserverings korting werd toegepast.</span><span class="sxs-lookup"><span data-stu-id="306a2-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="306a2-170">Zie voor meer informatie [klant gebruiks records voor Azure ophalen](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in de [partner centrum-API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="306a2-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="306a2-171">Software kosten, zoals micro soft Windows Server, zijn momenteel niet opgenomen in de prijs van een VM-reserve ring en worden weer gegeven als afzonderlijke regel items in de order record en op uw factuur.</span><span class="sxs-lookup"><span data-stu-id="306a2-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="306a2-172">Als een klant echter de Azure Hybrid Use Benefit heeft, worden de software kosten niet toegepast.</span><span class="sxs-lookup"><span data-stu-id="306a2-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="306a2-173">Zie [Windows-software kosten die niet zijn opgenomen in gereserveerde instanties](/azure/billing/billing-reserved-instance-windows-software-costs)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="306a2-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="306a2-174">Resources voor Azure-reserve ringen</span><span class="sxs-lookup"><span data-stu-id="306a2-174">Azure reservations resources</span></span>

|<span data-ttu-id="306a2-175">**Voor informatie over**</span><span class="sxs-lookup"><span data-stu-id="306a2-175">**For information about**</span></span>   |<span data-ttu-id="306a2-176">**Leest u**</span><span class="sxs-lookup"><span data-stu-id="306a2-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="306a2-177">Overzicht van Azure-reserve ringen in CSP</span><span class="sxs-lookup"><span data-stu-id="306a2-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="306a2-178">Microsoft Azure gereserveerde VM-instanties verkopen</span><span class="sxs-lookup"><span data-stu-id="306a2-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="306a2-179">Azure-reserve ringen voor uw klanten kopen in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="306a2-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="306a2-180">Azure-reserve ringen kopen</span><span class="sxs-lookup"><span data-stu-id="306a2-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="306a2-181">Azure-reserve ringen beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="306a2-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="306a2-182">Azure-reserve ringen beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="306a2-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="306a2-183">Azure-reserve ringen kopen in de Azure Portal</span><span class="sxs-lookup"><span data-stu-id="306a2-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="306a2-184">[Vooruitbetalen voor virtuele machines met Azure reserved VM instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in de Help van Azure</span><span class="sxs-lookup"><span data-stu-id="306a2-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="306a2-185">Azure-reserve ringen beheren in de Azure Portal</span><span class="sxs-lookup"><span data-stu-id="306a2-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="306a2-186">[Gereserveerde VM-instanties beheren](/azure/billing/billing-manage-reserved-vm-instance) in de Help van Azure</span><span class="sxs-lookup"><span data-stu-id="306a2-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="306a2-187">Azure-reserve ringen aanschaffen met de Partner Center-API</span><span class="sxs-lookup"><span data-stu-id="306a2-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="306a2-188">[Azure reserved VM instances kopen](/partner-center/develop/purchase-azure-reservations) in de ontwikkelaars documentatie van partner Center</span><span class="sxs-lookup"><span data-stu-id="306a2-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="306a2-189">Klanten toestemming geven om hun eigen Azure-reserve ringen te kopen vanuit een abonnement dat u hebt aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="306a2-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="306a2-190">Geef klanten toestemming om hun eigen Azure-reserve ringen te kopen</span><span class="sxs-lookup"><span data-stu-id="306a2-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |