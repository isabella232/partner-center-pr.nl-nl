---
title: Een klantkoppeling maken
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Maak klant koppelingen met het model van de claim partner van record (CPOR). Helpt bij het beheren van de verkoop, het gebruik en de stimulansen voor Microsoft 365 & Dynamics 365-klanten.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fec01e6c4554421593de4135ccd1af5c5e7ce13b
ms.sourcegitcommit: 1840767efa4c5de41889bc9245567cf286a084c8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2020
ms.locfileid: "92917247"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="07d2b-104">Klant koppelingen via het geclaimde partner of record (CPOR) model voor Microsoft 365 en Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="07d2b-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="07d2b-105">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="07d2b-105">**Applies to**</span></span>

- <span data-ttu-id="07d2b-106">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="07d2b-106">Partner Center</span></span>

<span data-ttu-id="07d2b-107">**Juiste rollen:**</span><span class="sxs-lookup"><span data-stu-id="07d2b-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="07d2b-108">Prikkel beheerder</span><span class="sxs-lookup"><span data-stu-id="07d2b-108">Incentives admin</span></span>

<span data-ttu-id="07d2b-109">Op 1 oktober 2019 begon micro soft het CPOR-model (partner of record) te gebruiken voor het beheren van de koppelingen die u hebt met uw Microsoft 365 en Dynamics 365-klanten met betrekking tot de verkoop van online services-advies (OSA), Online Services usage (OSU)-Microsoft 365 en OSU-Business toepassings stimulansen.</span><span class="sxs-lookup"><span data-stu-id="07d2b-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="07d2b-110">Claims voor klant koppeling (CPOR) zijn alleen van toepassing op de verkoop van online services-advies (OSA), Online Services usage (OSU)-Microsoft 365 en OSU-Business Application prikkel-Program ma's.</span><span class="sxs-lookup"><span data-stu-id="07d2b-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="07d2b-111">Als u een mede-op-aanvraag indient voor een ander programma, zoals een Cloud solution provider, een beheerde wederverkoper, hosting of Opper vlak, raadpleegt u dit proces dat hier wordt beschreven.</span><span class="sxs-lookup"><span data-stu-id="07d2b-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="07d2b-112">Wanneer u uw claim verzendt, valideert micro soft deze.</span><span class="sxs-lookup"><span data-stu-id="07d2b-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="07d2b-113">We kunnen u op dit punt vragen om meer informatie.</span><span class="sxs-lookup"><span data-stu-id="07d2b-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="07d2b-114">We melden ook de klant van uw koppelings aanvraag.</span><span class="sxs-lookup"><span data-stu-id="07d2b-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="07d2b-115">Klanten hebben vijf werk dagen nodig om u af te melden. Als ze niet worden afgemeld, zal uw koppeling met deze specifieke Tenant en werk belasting officieel zijn.</span><span class="sxs-lookup"><span data-stu-id="07d2b-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="07d2b-116">U hebt op dit moment toegang tot de gebruiks gegevens van de klant.</span><span class="sxs-lookup"><span data-stu-id="07d2b-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="07d2b-117">U hebt de volgende informatie nodig om een claim te volt ooien:</span><span class="sxs-lookup"><span data-stu-id="07d2b-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="07d2b-118">De **MPN-id** voor uw entiteit die de claim maakt</span><span class="sxs-lookup"><span data-stu-id="07d2b-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="07d2b-119">**Domein naam** van de klant [Dit zoeken](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="07d2b-119">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="07d2b-120">De **Directory-id** of **Tenant-id** van de klant [vindt u deze](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="07d2b-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="07d2b-121">Het **oplossings gebied** , zoals Business Applications of Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="07d2b-121">The **Solution area** , such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="07d2b-122">De **activiteit** die u hebt uitgevoerd en het type claim dat u wilt maken, zoals de koppeling vóór verkoop, gebruik of omzet</span><span class="sxs-lookup"><span data-stu-id="07d2b-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="07d2b-123">De **contact naam** , de titel en het e-mail adres van uw klant</span><span class="sxs-lookup"><span data-stu-id="07d2b-123">Your customer's **Contact name** , title, and email address</span></span>

- <span data-ttu-id="07d2b-124">Voor Dynamics 365 moet u ook de **technische contact** naam, de titel en het e-mail adres van uw klant opgeven</span><span class="sxs-lookup"><span data-stu-id="07d2b-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="07d2b-125">De **contact naam** en het e-mail adres van uw eigen bedrijf</span><span class="sxs-lookup"><span data-stu-id="07d2b-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="07d2b-126">U maakt een **naam** voor deze claim</span><span class="sxs-lookup"><span data-stu-id="07d2b-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="07d2b-127">De **product (en)** of workload ('s) die u aanspraakt</span><span class="sxs-lookup"><span data-stu-id="07d2b-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="07d2b-128">**Testen van de uitvoering (PoE)** , zoals een overzicht van werk dat door de klant is ondertekend.</span><span class="sxs-lookup"><span data-stu-id="07d2b-128">**Proof of execution (PoE)** , such as a statement of work signed by the customer.</span></span> <span data-ttu-id="07d2b-129">U kunt ook een PoE-sjabloon downloaden om te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="07d2b-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="07d2b-130">Voor partners die alleen een opbrengst koppeling claimen: de naam van de **verkoper** , de naam van de **klant** en de **naam van de ISV-product/-oplossing** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-130">For partners claiming revenue association only: **Dynamics solution seller name** , **Customer name** , and **Name of ISV product/solution** .</span></span> 

<span data-ttu-id="07d2b-131">U moet ook inzicht krijgen in de volgende punten:</span><span class="sxs-lookup"><span data-stu-id="07d2b-131">You should also understand the following points:</span></span>

- <span data-ttu-id="07d2b-132">Als u bestaande Microsoft 365 klanten hebt, moet u opnieuw koppelen aan de gebruikers die u wilt door gaan met het verdienen van OSUe prikkels met behulp van dit proces.</span><span class="sxs-lookup"><span data-stu-id="07d2b-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="07d2b-133">Als u bestaande koppelingen met Dynamics 365 of Power BI klanten hebt, blijven deze koppelingen geldig, totdat de abonnementen verlopen.</span><span class="sxs-lookup"><span data-stu-id="07d2b-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="07d2b-134">Een klant kan meerdere partners hebben, maar elke werk belasting (voor OSU-Microsoft 365) of-abonnement (voor OSA-Sell en OSU-Business toepassingen) kan slechts worden gekoppeld aan één partner.</span><span class="sxs-lookup"><span data-stu-id="07d2b-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="07d2b-135">Een klantkoppeling maken</span><span class="sxs-lookup"><span data-stu-id="07d2b-135">Create a customer association</span></span>

1. <span data-ttu-id="07d2b-136">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="07d2b-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="07d2b-137">Selecteer het tabblad **prikkels** , selecteer **overzicht** en selecteer vervolgens **klant koppelingen** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-137">Select the **Incentives** tab, select **Overview** , and then select **Customer associations** .</span></span>

3. <span data-ttu-id="07d2b-138">Selecteer boven aan de pagina klant koppelingen de optie **+ klant koppeling** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-138">At the top of the Customer associations page, select **+ Customer association** .</span></span>

4. <span data-ttu-id="07d2b-139">Selecteer de **MPN-ID** van de partnerlocatie die aan de klant moet worden gekoppeld en voeg vervolgens de domeinnaam en directory-id van de klant toe.</span><span class="sxs-lookup"><span data-stu-id="07d2b-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="07d2b-140">Dit zoeken</span><span class="sxs-lookup"><span data-stu-id="07d2b-140">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="07d2b-141">Selecteer **Doorgaan** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-141">Select **Continue** .</span></span>

6. <span data-ttu-id="07d2b-142">Selecteer het **oplossings gebied** en de **activiteit** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-142">Select the **Solution area** and **Activity** .</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="07d2b-143">Als u Business Applications selecteert, selecteert u **gebruik en/of** omzet, of **opbrengst koppeling** , en selecteert u vervolgens **door gaan** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-143">If you select Business Applications, select either **Usage and/or Pre-sales** , or **Revenue association** , and then select **Continue** .</span></span> 
   <br><br><span data-ttu-id="07d2b-144">Als u Revenue association selecteert, wordt u gevraagd om iets andere informatie dan hieronder wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="07d2b-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="07d2b-145">Voer de juiste informatie in op de pagina **klant koppelen** en selecteer vervolgens **claim maken** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim** .</span></span>

8. <span data-ttu-id="07d2b-146">Selecteer de producten die zijn gekoppeld aan deze klant koppeling en selecteer vervolgens **door gaan** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-146">Select the product(s) associated with this customer association, and then select **Continue** .</span></span>

9. <span data-ttu-id="07d2b-147">Vul de contactgegevens van de klant en van uw bedrijf in.</span><span class="sxs-lookup"><span data-stu-id="07d2b-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="07d2b-148">Alle velden zijn verplicht.</span><span class="sxs-lookup"><span data-stu-id="07d2b-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="07d2b-149">Als uw product Dynamics 365 is en het product dat u hebt gekozen meerdere abonnementen heeft voor deze bepaalde klant, moet u ook de abonnements-ID invoeren.</span><span class="sxs-lookup"><span data-stu-id="07d2b-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="07d2b-150">Geef uw bewijs van uitvoering op (PoE).</span><span class="sxs-lookup"><span data-stu-id="07d2b-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="07d2b-151">U kunt deze naar het vak slepen, naar uw eigen ondersteunende documentatie bladeren of een sjabloon gebruiken door **Download template** te selecteren.</span><span class="sxs-lookup"><span data-stu-id="07d2b-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template** .</span></span> 

11. <span data-ttu-id="07d2b-152">Voeg desgewenst opmerkingen toe en sla deze op voordat u **Submit claim** selecteert.</span><span class="sxs-lookup"><span data-stu-id="07d2b-152">Add and save comments if you like, and then select **Submit claim** .</span></span> <span data-ttu-id="07d2b-153">Er wordt een e-mail verzonden naar de klant met het verzoek om goedkeuring voor de klantkoppeling.</span><span class="sxs-lookup"><span data-stu-id="07d2b-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="07d2b-154">Wanneer u uw klant koppeling hebt ingediend, kunt u deze niet meer bewerken.</span><span class="sxs-lookup"><span data-stu-id="07d2b-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="07d2b-155">De status van de klantkoppeling wordt weergegeven in het veld **Status** .</span><span class="sxs-lookup"><span data-stu-id="07d2b-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="07d2b-156">Selecteer **History** om de geschiedenis van een klantkoppeling te bekijken.</span><span class="sxs-lookup"><span data-stu-id="07d2b-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="07d2b-157">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="07d2b-157">Next steps</span></span>

- [<span data-ttu-id="07d2b-158">Klantkoppelingen beheren</span><span class="sxs-lookup"><span data-stu-id="07d2b-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)