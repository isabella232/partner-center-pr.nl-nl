---
title: Het formaat van Azure-VM's wijzigen voor een maximaal reserveringsgebruik
description: Leer hoe u een virtuele machine (VM) kunt afmeten aan de computerbehoeften van uw klanten wanneer u Microsoft Azure voor hen koopt.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510190"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="d1f2c-103">Het formaat van Microsoft Azure-VM’s wijzigen voor een maximaal reserveringsgebruik</span><span class="sxs-lookup"><span data-stu-id="d1f2c-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="d1f2c-104">**Juiste rollen:** beheeragent | Verkoopagent</span><span class="sxs-lookup"><span data-stu-id="d1f2c-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="d1f2c-105">In dit artikel wordt uitgelegd hoe u de grootte van een virtuele machine (VM) kunt afmeten aan de computerbehoeften van uw klanten wanneer u Microsoft Azure voor hen koopt.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="d1f2c-106">Dit artikel is alleen van toepassing op partners in het Cloud Solution Provider (CSP)-programma.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="d1f2c-107">Klanten die gebruikmaken van andere typen abonnementen (zoals betalen per gebruik, individueel, Microsoft-klantovereenkomst- of Enterprise Agreement-abonnementen), moeten in plaats daarvan deze documentatie voor [Azure-reserveringen lezen.](/azure/cost-management-billing/reservations)</span><span class="sxs-lookup"><span data-stu-id="d1f2c-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="d1f2c-108">De VM-grootte voor de Azure-reservering van een klant bepalen</span><span class="sxs-lookup"><span data-stu-id="d1f2c-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="d1f2c-109">Wanneer u Microsoft Azure namens uw klanten reserveringen koopt, moet u een virtuele machine (VM) kiezen die is geformatteerd om te voldoen aan de computerbehoeften van de klant.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="d1f2c-110">U vindt deze informatie op een van de volgende manieren:</span><span class="sxs-lookup"><span data-stu-id="d1f2c-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="d1f2c-111">Azure-gebruiks-API</span><span class="sxs-lookup"><span data-stu-id="d1f2c-111">Azure utilization API</span></span>
- <span data-ttu-id="d1f2c-112">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="d1f2c-112">The Azure portal</span></span>
- <span data-ttu-id="d1f2c-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="d1f2c-113">Azure PowerShell</span></span>
- <span data-ttu-id="d1f2c-114">De AZURE RESOURCE MANAGER API (ARM)</span><span class="sxs-lookup"><span data-stu-id="d1f2c-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="d1f2c-115">Instructies voor het gebruik van elk van deze methoden vindt u hieronder.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="d1f2c-116">Nadat u een reservering hebt gekocht, wordt de reserveringskorting automatisch toegepast op virtuele machines die overeenkomen met de kenmerken en hoeveelheid van de reservering.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="d1f2c-117">U hoeft de reservering niet toe te wijzen aan een VM.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="d1f2c-118">Reserveringskortingen zijn niet van toepassing op klassieke of aanbiedings-VM's.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="d1f2c-119">Als u het type en de grootte van de VM die u namens uw klant wilt kopen correct wilt identificeren, moet u een van de onderstaande methoden gebruiken, omdat het type VM-serie niet correct wordt weergegeven in Partner Center-afstemmingsbestanden.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="d1f2c-120">VM-formaatgegevens verkrijgen met behulp van de Azure-gebruiks-API</span><span class="sxs-lookup"><span data-stu-id="d1f2c-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="d1f2c-121">Gebruik de waarde voor het kenmerk ServiceType uit additionalInfo in het API-antwoord om de te kopen VM-grootte te identificeren.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="d1f2c-122">Zie Get [a customer's utilization records for Azure (Gebruiksrecords](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) van een klant voor Azure verkrijgen) in Partner Center [API voor meer informatie.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="d1f2c-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="d1f2c-123">VM-formaatgegevens verkrijgen met behulp van de Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="d1f2c-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="d1f2c-124">Ga Partner Center naar de **pagina** Klanten.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="d1f2c-125">Zoek de klant die Azure VM-reserveringen wil kopen en selecteer vervolgens de pijl-omlaag om de gegevens van de klant uit te vouwen.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="d1f2c-126">Selecteer **Microsoft Azure Beheerportal** om de record van de klant in de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="d1f2c-127">Selecteer **Virtuele machines** in het portalmenu en selecteer vervolgens de VM waarvoor u een reservering wilt kopen.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="d1f2c-128">Zoek op de detailpagina van de VM de grootte en regiogegevens, zoals hieronder wordt weergegeven, en gebruik deze informatie om de reservering in de lijst Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Grootte- en regiogegevens op de detailpagina.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="d1f2c-130">VM-formaatgegevens op halen met behulp van Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="d1f2c-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="d1f2c-131">Gebruik de informatie in de onderstaande afbeelding om de locatie en grootte op te halen van de VM waarvoor u een reservering wilt kopen.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM-locatie en -grootte.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="d1f2c-133">VM-formaatgegevens verkrijgen met behulp van de AZURE RESOURCE MANAGER API (ARM)</span><span class="sxs-lookup"><span data-stu-id="d1f2c-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="d1f2c-134">Gebruik de ARMClient of de ARM-API's om de ARM-client aan te roepen voor de VM waarvoor u een reservering wilt kopen.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. <span data-ttu-id="d1f2c-135">De aanroep retourneert de waarden voor **vmSize** en **location**, zoals hieronder wordt geïllustreerd.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-135">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize-waarde.":::
    :::image type="content" source="images/usage4.png" alt-text="locatiewaarde.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="d1f2c-138">Gebruik en reserveringskorting voor Azure-VM's controleren</span><span class="sxs-lookup"><span data-stu-id="d1f2c-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="d1f2c-139">Nadat u namens een klant een gereserveerde VM-instantie van Azure hebt aangeschaft, wordt de korting voor het vooraf betalen van VM-ruimte automatisch toegepast op de virtuele machines die overeenkomen met de kenmerken en hoeveelheid van de reservering van de klant.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="d1f2c-140">U kunt het reserveringsgebruik van de klant controleren en met een van de volgende methoden zien op welke virtuele machines de reserveringskortingen worden toegepast:</span><span class="sxs-lookup"><span data-stu-id="d1f2c-140">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="d1f2c-141">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="d1f2c-141">The Azure portal</span></span>
- <span data-ttu-id="d1f2c-142">Azure-gebruiks-API</span><span class="sxs-lookup"><span data-stu-id="d1f2c-142">Azure utilization API</span></span>

<span data-ttu-id="d1f2c-143">Instructies voor het gebruik van elk van deze methoden vindt u hieronder.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="d1f2c-144">Alleen de AZURE-gebruiks-API geeft aan op welke virtuele machine de korting wordt toegepast.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="d1f2c-145">Het reserveringsgebruik van de klant controleren in de Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="d1f2c-145">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="d1f2c-146">Ga Partner Center naar de **pagina** Klanten.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-146">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="d1f2c-147">Zoek de klant van wie u de reserveringskorting en het gebruik wilt controleren en selecteer vervolgens de pijl-omlaag om de gegevens van de klant uit te vouwen.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="d1f2c-148">Selecteer **Microsoft Azure Beheerportal** om de record van de klant in de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-148">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="d1f2c-149">Selecteer **Reserveringen in** het portalmenu en selecteer vervolgens de reservering voor wie u het gebruik wilt controleren.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="d1f2c-150">Controleer op **de** pagina Overzicht de gebruiksgrafiek van de reservering, die laat zien hoeveel van de reservering is toegepast op virtuele machines.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-150">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="d1f2c-151">Gebruiksgegevens kunnen maximaal acht uur worden vertraagd.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-151">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="d1f2c-152">a.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-152">a.</span></span> <span data-ttu-id="d1f2c-153">Als het gebruik van de reservering 100% is, krijgt uw klant alle mogelijke besparingen die de reserveringsaankoop kan bieden.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-153">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="d1f2c-154">b.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-154">b.</span></span> <span data-ttu-id="d1f2c-155">Als het gebruik van de reservering 0% is, wordt de korting niet toegepast op een virtuele machine.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-155">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="d1f2c-156">c.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-156">c.</span></span> <span data-ttu-id="d1f2c-157">Als het gebruik van de reservering tussen 1% en 99% ligt, zijn er ongebruikte voordelen.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-157">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="d1f2c-158">Om deze situatie te voorkomen, moet u de juiste grootte van de VM bepalen om de computerbehoeften van de klant te ondersteunen voordat u de aankoop doet.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-158">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="d1f2c-159">Het reserveringsgebruik van de klant controleren met de Azure-gebruiks-API</span><span class="sxs-lookup"><span data-stu-id="d1f2c-159">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="d1f2c-160">Alleen de AZURE-gebruiks-API geeft aan op welke virtuele machine de korting wordt toegepast.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="d1f2c-161">U kunt reserveringsgebruiksgegevens verkrijgen met de Azure-gebruiks-API om te controleren of de klant de reserveringskorting krijgt en om te zien op welke VM's (virtuele machines) de korting wordt toegepast.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="d1f2c-162">Vergelijk voorbeeld A met voorbeeld B om te zien hoe u het reserveringsgebruik van een klant verifieert.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-162">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Voorbeelden van reserveringsgebruik.":::

- <span data-ttu-id="d1f2c-164">De reservationId identificeert de Azure-reservering die is gebruikt om de korting op de VM toe te passen.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="d1f2c-165">consumptionMeter is de MeterId voor de VM waar de reserveringskorting op is toegepast.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="d1f2c-166">De Reserveringsmeter toont $0-kosten sinds de reserveringskorting is toegepast.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="d1f2c-167">Zie Get [a customer's utilization records for Azure (Gebruiksrecords](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) van een klant voor Azure verkrijgen) in Partner Center [API voor meer informatie.](/partner-center/develop/)</span><span class="sxs-lookup"><span data-stu-id="d1f2c-167">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="d1f2c-168">Softwarekosten, zoals Microsoft Windows Server, zijn momenteel niet opgenomen in de prijs van een VM-reservering en worden weergegeven als afzonderlijke regelitems in de orderrecord en op uw factuur.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="d1f2c-169">Als een klant echter azure Hybrid Use Benefit heeft, worden de softwarekosten niet toegepast.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="d1f2c-170">Zie voor meer informatie Windows [softwarekosten die niet zijn opgenomen in gereserveerde instanties.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="d1f2c-170">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="d1f2c-171">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="d1f2c-171">Next steps</span></span>

|<span data-ttu-id="d1f2c-172">**Voor informatie over**</span><span class="sxs-lookup"><span data-stu-id="d1f2c-172">**For information about**</span></span>   |<span data-ttu-id="d1f2c-173">**Leest u**</span><span class="sxs-lookup"><span data-stu-id="d1f2c-173">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="d1f2c-174">Overzicht van Azure-reserveringen in CSP</span><span class="sxs-lookup"><span data-stu-id="d1f2c-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="d1f2c-175">Verkopen Microsoft Azure gereserveerde VM-instanties</span><span class="sxs-lookup"><span data-stu-id="d1f2c-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="d1f2c-176">Azure-reserveringen kopen voor uw klanten in Partner Center</span><span class="sxs-lookup"><span data-stu-id="d1f2c-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="d1f2c-177">Azure-reserveringen kopen</span><span class="sxs-lookup"><span data-stu-id="d1f2c-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="d1f2c-178">Azure-reserveringen beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="d1f2c-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="d1f2c-179">Azure-reserveringen beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="d1f2c-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="d1f2c-180">Azure-reserveringen kopen in de Azure Portal</span><span class="sxs-lookup"><span data-stu-id="d1f2c-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="d1f2c-181">[Vooruitbetalen voor virtuele machines met Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in de Help van Azure</span><span class="sxs-lookup"><span data-stu-id="d1f2c-181">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="d1f2c-182">Azure-reserveringen beheren in de Azure Portal</span><span class="sxs-lookup"><span data-stu-id="d1f2c-182">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="d1f2c-183">[Gereserveerde VM-instanties beheren](/azure/billing/billing-manage-reserved-vm-instance) in de Help van Azure</span><span class="sxs-lookup"><span data-stu-id="d1f2c-183">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="d1f2c-184">Azure-reserveringen kopen met behulp van Partner Center API</span><span class="sxs-lookup"><span data-stu-id="d1f2c-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="d1f2c-185">[Aankoop van Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in de documentatie Partner Center ontwikkelaars</span><span class="sxs-lookup"><span data-stu-id="d1f2c-185">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="d1f2c-186">Klanten toestemming geven om hun eigen Azure-reserveringen te kopen bij een abonnement dat u voor hen hebt aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="d1f2c-186">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="d1f2c-187">Klanten toestemming geven om hun eigen Azure-reserveringen te kopen</span><span class="sxs-lookup"><span data-stu-id="d1f2c-187">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |