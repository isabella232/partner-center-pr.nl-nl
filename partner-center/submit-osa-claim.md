---
title: Een klantkoppeling maken
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Maak klantbindingen met het Claiming Partner of Record (CPOR)-model. Helpt bij het beheren van verkoop, gebruik en incentives Microsoft 365 & Dynamics 365-klanten.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489948"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="8869e-104">Klant verbanden via het model Geclaimde Partner of Record (CPOR) voor Microsoft 365 en Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="8869e-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="8869e-105">**Juiste rollen:** Incentives-beheerder</span><span class="sxs-lookup"><span data-stu-id="8869e-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="8869e-106">Op 1 oktober 2019 is Microsoft begonnen met het Claiming Partner of Record-model (CPOR) voor het beheren van de verbanden die u hebt met uw Microsoft 365- en Dynamics 365-klanten met betrekking tot het Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 en OSU-Business Application incentives.</span><span class="sxs-lookup"><span data-stu-id="8869e-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="8869e-107">CPOR-claims (Customer Association) zijn alleen van toepassing op de Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 en OSU-Business Application incentive-programma's.</span><span class="sxs-lookup"><span data-stu-id="8869e-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="8869e-108">Als u een claim voor samenwerking indient voor een ander programma, zoals Cloud Solution Provider (CSP), Managed Reseller, Hosting of Surface, raadpleegt u het proces voor samenwerkingsclaims dat hier wordt beschreven.</span><span class="sxs-lookup"><span data-stu-id="8869e-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider (CSP), Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="8869e-109">Wanneer u uw claim indient, valideert Microsoft deze.</span><span class="sxs-lookup"><span data-stu-id="8869e-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="8869e-110">We kunnen u op dit moment om meer informatie vragen.</span><span class="sxs-lookup"><span data-stu-id="8869e-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="8869e-111">We stellen de klant ook op de hoogte van uw associatieaanvraag.</span><span class="sxs-lookup"><span data-stu-id="8869e-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="8869e-112">Klanten hebben vijf werkdagen om af te zien. Als ze zich niet uiten, is uw associatie met deze specifieke tenant en workload officieel.</span><span class="sxs-lookup"><span data-stu-id="8869e-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="8869e-113">Op dit moment hebt u toegang tot de gebruiksgegevens van de klant.</span><span class="sxs-lookup"><span data-stu-id="8869e-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="8869e-114">U hebt de volgende informatie nodig om een claim te voltooien:</span><span class="sxs-lookup"><span data-stu-id="8869e-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="8869e-115">De **MPN-id** (Microsoft Partner Network-id) voor uw entiteit die de claim maakt</span><span class="sxs-lookup"><span data-stu-id="8869e-115">The **MPN ID** (Microsoft Partner Network ID) for your entity that makes the claim</span></span>

- <span data-ttu-id="8869e-116">Domeinnaam van **de klant** (zie Tenant-id, domeinnaam, gebruikersobject-id zoeken) voor meer [informatie.](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="8869e-116">Customer's **domain name** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="8869e-117">Directory-id  of **tenant-id van** de klant (zie Tenant-id, [domeinnaam, gebruikersobject-id](find-ids-and-domain-names.md)zoeken) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="8869e-117">Customer's **Directory ID** or **Tenant ID** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="8869e-118">Het **gebied Oplossing,** zoals Business Applications of Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8869e-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="8869e-119">De **activiteit** die u hebt uitgevoerd en het type claim dat u wilt maken, zoals de associatie Pre-sales, Usage of Revenue</span><span class="sxs-lookup"><span data-stu-id="8869e-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="8869e-120">De naam, titel en **het** e-mailadres van uw klant</span><span class="sxs-lookup"><span data-stu-id="8869e-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="8869e-121">Voor Dynamics 365 moet u ook de  technische contactnaam, titel en e-mailadres van uw klant verstrekken</span><span class="sxs-lookup"><span data-stu-id="8869e-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="8869e-122">De naam en het **e-mailadres van uw** eigen bedrijf</span><span class="sxs-lookup"><span data-stu-id="8869e-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="8869e-123">U maakt een naam **voor** deze claim</span><span class="sxs-lookup"><span data-stu-id="8869e-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="8869e-124">De **producten of** workloads die u claimt</span><span class="sxs-lookup"><span data-stu-id="8869e-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="8869e-125">**Proof of execution (PoE)**, zoals een werkverklaring die is ondertekend door de klant.</span><span class="sxs-lookup"><span data-stu-id="8869e-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="8869e-126">U kunt ook een PoE-sjabloon downloaden om te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="8869e-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="8869e-127">Alleen voor partners die een omzetbinding claimen: verkopernaam van **Dynamics-oplossing,** **Klantnaam** en **Naam van ISV-product/-oplossing.**</span><span class="sxs-lookup"><span data-stu-id="8869e-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="8869e-128">U moet ook de volgende punten begrijpen:</span><span class="sxs-lookup"><span data-stu-id="8869e-128">You should also understand the following points:</span></span>

- <span data-ttu-id="8869e-129">Als u bestaande Microsoft 365 hebt, moet u zich opnieuw koppelen aan de klanten die u osu-incentives wilt blijven verdienen met behulp van dit proces.</span><span class="sxs-lookup"><span data-stu-id="8869e-129">If you have existing Microsoft 365 customers, you'll need to reassociate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="8869e-130">Als u bestaande verbanden hebt met Dynamics 365- of Power BI-klanten, blijven deze associaties geldig tot de vervaldatum van hun abonnementen.</span><span class="sxs-lookup"><span data-stu-id="8869e-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="8869e-131">Een klant kan meerdere partners hebben, maar elke workload (voor OSU-Microsoft 365) of abonnementen (voor OSA-Sell en OSU-Business Applications) kan slechts aan één partner worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="8869e-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="8869e-132">Een klantkoppeling maken</span><span class="sxs-lookup"><span data-stu-id="8869e-132">Create a customer association</span></span>

1. <span data-ttu-id="8869e-133">Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8869e-133">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="8869e-134">Selecteer het **tabblad Incentives,** selecteer **Overzicht** en selecteer vervolgens **Klant associations.**</span><span class="sxs-lookup"><span data-stu-id="8869e-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="8869e-135">Selecteer boven aan de pagina Klant associations de optie **+ Customer association.**</span><span class="sxs-lookup"><span data-stu-id="8869e-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="8869e-136">Selecteer de **MPN-ID** van de partnerlocatie die aan de klant moet worden gekoppeld en voeg vervolgens de domeinnaam en directory-id van de klant toe.</span><span class="sxs-lookup"><span data-stu-id="8869e-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="8869e-137">Zoek deze</span><span class="sxs-lookup"><span data-stu-id="8869e-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="8869e-138">Selecteer **Doorgaan**.</span><span class="sxs-lookup"><span data-stu-id="8869e-138">Select **Continue**.</span></span>

6. <span data-ttu-id="8869e-139">Selecteer het **gebied Oplossing en** **Activiteit**.</span><span class="sxs-lookup"><span data-stu-id="8869e-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="8869e-140">Als u Business Applications selecteert, selecteert u **Usage and/or Pre-sales** of **Revenue association** en selecteert u **vervolgens Continue.**</span><span class="sxs-lookup"><span data-stu-id="8869e-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="8869e-141">Als u Revenue association selecteert, wordt u gevraagd om iets andere informatie dan hieronder wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="8869e-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="8869e-142">Voer de juiste informatie in op **de pagina Klant** koppelen en selecteer vervolgens Claim **maken.**</span><span class="sxs-lookup"><span data-stu-id="8869e-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="8869e-143">Selecteer de producten die zijn gekoppeld aan deze klantbinding en selecteer vervolgens **Doorgaan.**</span><span class="sxs-lookup"><span data-stu-id="8869e-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="8869e-144">Vul de contactgegevens van de klant en van uw bedrijf in.</span><span class="sxs-lookup"><span data-stu-id="8869e-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="8869e-145">Alle velden zijn verplicht.</span><span class="sxs-lookup"><span data-stu-id="8869e-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="8869e-146">Als uw product Dynamics 365 is en het product dat u kiest meerdere abonnementen heeft voor deze specifieke klant, moet u ook de abonnements-id invoeren.</span><span class="sxs-lookup"><span data-stu-id="8869e-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="8869e-147">Uw PoE leveren.</span><span class="sxs-lookup"><span data-stu-id="8869e-147">Supply your PoE.</span></span> <span data-ttu-id="8869e-148">U kunt deze naar het vak slepen, naar uw eigen ondersteunende documentatie bladeren of een sjabloon gebruiken door **Download template** te selecteren.</span><span class="sxs-lookup"><span data-stu-id="8869e-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="8869e-149">Voeg desgewenst opmerkingen toe en sla deze op voordat u **Submit claim** selecteert.</span><span class="sxs-lookup"><span data-stu-id="8869e-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="8869e-150">Er wordt een e-mail verzonden naar de klant met het verzoek om goedkeuring voor de klantkoppeling.</span><span class="sxs-lookup"><span data-stu-id="8869e-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="8869e-151">Zodra u uw klantbinding hebt indienen, kunt u deze niet meer bewerken.</span><span class="sxs-lookup"><span data-stu-id="8869e-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="8869e-152">De status van de klantkoppeling wordt weergegeven in het veld **Status**.</span><span class="sxs-lookup"><span data-stu-id="8869e-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="8869e-153">Selecteer **History** om de geschiedenis van een klantkoppeling te bekijken.</span><span class="sxs-lookup"><span data-stu-id="8869e-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8869e-154">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="8869e-154">Next steps</span></span>

- [<span data-ttu-id="8869e-155">Klantkoppelingen beheren</span><span class="sxs-lookup"><span data-stu-id="8869e-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)