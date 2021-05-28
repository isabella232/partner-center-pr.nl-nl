---
title: Beheerdersbevoegdheden voor Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe u klanten kunt helpen de beheerdersbevoegdheden van een partner te herstellen, zodat de partner kan helpen bij het beheren van de Azure CSP van een klant.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ca4c8323562e6c6f1d762465cad86e7ae113eb19
ms.sourcegitcommit: beba696954b62ab5396a893d050d0c2c211aeafc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/28/2021
ms.locfileid: "110601423"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="2965b-103">Beheerdersbevoegdheden voor de Azure CSP van een klant herstellen</span><span class="sxs-lookup"><span data-stu-id="2965b-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="2965b-104">**Juiste rollen:** Globale | Beheeragent</span><span class="sxs-lookup"><span data-stu-id="2965b-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="2965b-105">Als CSP-partner verwachten uw klanten vaak dat u hun Azure-gebruik en hun systemen voor hen beheert.</span><span class="sxs-lookup"><span data-stu-id="2965b-105">As a CSP partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="2965b-106">U moet beheerdersbevoegdheden hebben om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="2965b-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="2965b-107">Sommige bevoegdheden worden verleend wanneer uw resellerrelatie met de klant tot stand is gebracht.</span><span class="sxs-lookup"><span data-stu-id="2965b-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="2965b-108">Andere worden aan u verleend door uw klant.</span><span class="sxs-lookup"><span data-stu-id="2965b-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="2965b-109">Beheerdersbevoegdheden voor Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="2965b-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="2965b-110">Er zijn twee niveaus van beheerdersbevoegdheden voor Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="2965b-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="2965b-111">**Beheerdersbevoegdheden op tenantniveau (gedelegeerde beheerdersbevoegdheden)**: CSP-partners krijgen deze bevoegdheden tijdens het tot stand brengen van een CSP-resellerrelatie met klanten.</span><span class="sxs-lookup"><span data-stu-id="2965b-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="2965b-112">Gedelegeerde beheerdersbevoegdheden geven CSP-partners toegang tot de tenants van hun klanten.</span><span class="sxs-lookup"><span data-stu-id="2965b-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="2965b-113">Met deze toegang kunnen ze beheerfuncties uitvoeren, zoals gebruikers toevoegen/beheren, wachtwoorden opnieuw instellen en gebruikerslicenties beheren.</span><span class="sxs-lookup"><span data-stu-id="2965b-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="2965b-114">**Beheerdersbevoegdheden op abonnementsniveau:** CSP-partners krijgen deze bevoegdheden tijdens het maken van Azure CSP voor hun klanten.</span><span class="sxs-lookup"><span data-stu-id="2965b-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="2965b-115">Deze bevoegdheden geven CSP-partners volledige toegang tot deze abonnementen, zodat ze Azure-resources kunnen inrichten en beheren.</span><span class="sxs-lookup"><span data-stu-id="2965b-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="2965b-116">De beheerdersbevoegdheden van een partner opnieuw in CSP herstellen</span><span class="sxs-lookup"><span data-stu-id="2965b-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="2965b-117">Uw klant kan de CSP-roltoewijzing opnieuw maken als u de van de `object ID` groep AdminAgents aan uw klant verstrekt.</span><span class="sxs-lookup"><span data-stu-id="2965b-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="2965b-118">Als u weer gedelegeerde beheerdersbevoegdheden wilt krijgen, moet u met uw klant samenwerken door de volgende stappen uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="2965b-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="2965b-119">Meld u aan bij Partner Center dashboard.</span><span class="sxs-lookup"><span data-stu-id="2965b-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="2965b-120">Selecteer in Partner Center menu **Klanten.**</span><span class="sxs-lookup"><span data-stu-id="2965b-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="2965b-121">Selecteer de klant met wie u werkt en vraag **een resellerrelatie aan.**</span><span class="sxs-lookup"><span data-stu-id="2965b-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="2965b-122">Met deze actie wordt een koppeling gegenereerd naar de klant die tenantbeheerdersrechten heeft.</span><span class="sxs-lookup"><span data-stu-id="2965b-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="2965b-123">Uw klant moet de koppeling selecteren en de aanvraag voor de resellerrelatie goedkeuren.</span><span class="sxs-lookup"><span data-stu-id="2965b-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-mailvoorbeeld van een resellerrelatie maken":::

5. <span data-ttu-id="2965b-125">U, de partner, moet verbinding maken met de partnerten tenant om de object-id van de groep AdminAgents op te halen.</span><span class="sxs-lookup"><span data-stu-id="2965b-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="2965b-126">Uw klant moet vervolgens de volgende stappen uitvoeren met behulp van PowerShell of Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="2965b-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="2965b-127">Uw klant moet het volgende hebben:</span><span class="sxs-lookup"><span data-stu-id="2965b-127">Your customer must have:</span></span>

- <span data-ttu-id="2965b-128">De rol van **eigenaar** of **beheerder van gebruikerstoegang**</span><span class="sxs-lookup"><span data-stu-id="2965b-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="2965b-129">Machtigingen voor het maken van roltoewijzingen op abonnementsniveau</span><span class="sxs-lookup"><span data-stu-id="2965b-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="2965b-130">a.</span><span class="sxs-lookup"><span data-stu-id="2965b-130">a.</span></span> <span data-ttu-id="2965b-131">Alleen voor PowerShell moet de klant de `Az.Resources` module bijwerken.</span><span class="sxs-lookup"><span data-stu-id="2965b-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="2965b-132">b.</span><span class="sxs-lookup"><span data-stu-id="2965b-132">b.</span></span> <span data-ttu-id="2965b-133">De klant maakt verbinding met de tenant waar het CSP-abonnement zich bevindt.</span><span class="sxs-lookup"><span data-stu-id="2965b-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="2965b-134">c.</span><span class="sxs-lookup"><span data-stu-id="2965b-134">c.</span></span> <span data-ttu-id="2965b-135">De klant maakt verbinding met het abonnement.</span><span class="sxs-lookup"><span data-stu-id="2965b-135">The customer connects to the subscription.</span></span> <span data-ttu-id="2965b-136">Dit is *alleen* van toepassing als de gebruiker machtigingen voor roltoewijzing heeft voor meerdere abonnementen in de tenant.</span><span class="sxs-lookup"><span data-stu-id="2965b-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="2965b-137">d.</span><span class="sxs-lookup"><span data-stu-id="2965b-137">d.</span></span> <span data-ttu-id="2965b-138">De klant maakt vervolgens de roltoewijzing.</span><span class="sxs-lookup"><span data-stu-id="2965b-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="2965b-139">In plaats van eigenaarsmachtigingen te verlenen voor het abonnementsbereik, kunt u verlenen op het niveau van de resourcegroep of resource.</span><span class="sxs-lookup"><span data-stu-id="2965b-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="2965b-140">Op het niveau van de resourcegroep</span><span class="sxs-lookup"><span data-stu-id="2965b-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="2965b-141">Op resourceniveau</span><span class="sxs-lookup"><span data-stu-id="2965b-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

## <a name="next-steps"></a><span data-ttu-id="2965b-142">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="2965b-142">Next steps</span></span>

- [<span data-ttu-id="2965b-143">Abonnementen en resources beheren onder het Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="2965b-143">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
