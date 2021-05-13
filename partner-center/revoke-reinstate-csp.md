---
title: Beheerdersbevoegdheden voor Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe u klanten kunt helpen de beheerdersbevoegdheden van een partner te herstellen, zodat de partner kan helpen bij het beheren van de Azure CSP van een klant.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855417"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="1aa27-103">Beheerdersbevoegdheden voor de Azure CSP van een klant herstellen</span><span class="sxs-lookup"><span data-stu-id="1aa27-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="1aa27-104">**Juiste rollen:** Globale | Beheeragent</span><span class="sxs-lookup"><span data-stu-id="1aa27-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="1aa27-105">Als CSP-partner verwachten uw klanten vaak dat u hun Azure-gebruik en hun systemen voor hen beheert.</span><span class="sxs-lookup"><span data-stu-id="1aa27-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="1aa27-106">Hiervoor moet u beheerdersbevoegdheden hebben.</span><span class="sxs-lookup"><span data-stu-id="1aa27-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="1aa27-107">Sommige bevoegdheden worden verleend wanneer uw resellerrelatie met de klant tot stand is gebracht.</span><span class="sxs-lookup"><span data-stu-id="1aa27-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="1aa27-108">Andere worden aan u verleend door uw klant.</span><span class="sxs-lookup"><span data-stu-id="1aa27-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="1aa27-109">Beheerdersbevoegdheden voor Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="1aa27-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="1aa27-110">Er zijn twee niveaus van beheerdersbevoegdheden voor Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="1aa27-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="1aa27-111">**Beheerdersbevoegdheden op tenantniveau** **(gedelegeerde beheerdersbevoegdheden)**- CSP-partners krijgen deze bevoegdheden tijdens het tot stand brengen van een CSP-resellerrelatie met klanten.</span><span class="sxs-lookup"><span data-stu-id="1aa27-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="1aa27-112">Gedelegeerde beheerdersbevoegdheden geven CSP-partners toegang tot de tenants van hun klanten, zodat ze beheerfuncties kunnen uitvoeren, zoals gebruikers toevoegen/beheren, wachtwoorden opnieuw instellen en gebruikerslicenties beheren.</span><span class="sxs-lookup"><span data-stu-id="1aa27-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="1aa27-113">**Beheerdersbevoegdheden op abonnementsniveau:** CSP-partners krijgen deze bevoegdheden tijdens het maken van Azure CSP-abonnementen voor hun klanten.</span><span class="sxs-lookup"><span data-stu-id="1aa27-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="1aa27-114">Deze bevoegdheden geven CSP-partners volledige toegang tot deze abonnementen, zodat ze Azure-resources kunnen inrichten en beheren.</span><span class="sxs-lookup"><span data-stu-id="1aa27-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="1aa27-115">Beheerdersbevoegdheden van CSP-partners herstellen</span><span class="sxs-lookup"><span data-stu-id="1aa27-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="1aa27-116">Uw klant kan de CSP-roltoewijzing opnieuw maken zolang u de object-id van de groep AdminAgents aan uw klant hebt verstrekt.</span><span class="sxs-lookup"><span data-stu-id="1aa27-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="1aa27-117">Als u weer gedelegeerde beheerdersbevoegdheden wilt krijgen, moet u samenwerken met uw klant.</span><span class="sxs-lookup"><span data-stu-id="1aa27-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="1aa27-118">Meld u aan Partner Center dashboard en selecteer in Partner Center menu **Klanten.**</span><span class="sxs-lookup"><span data-stu-id="1aa27-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="1aa27-119">Selecteer de klant met wie u werkt en vraag **een resellerrelatie aan.**</span><span class="sxs-lookup"><span data-stu-id="1aa27-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="1aa27-120">Met deze actie wordt een koppeling gegenereerd naar de klant met tenantbeheerdersrechten.</span><span class="sxs-lookup"><span data-stu-id="1aa27-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="1aa27-121">Die klant moet de koppeling selecteren en de aanvraag voor de resellerrelatie goedkeuren.</span><span class="sxs-lookup"><span data-stu-id="1aa27-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-mailvoorbeeld van een resellerrelatie maken":::

4. <span data-ttu-id="1aa27-123">U, de partner, moet verbinding maken met de partnerten tenant om de object-id van de groep AdminAgents op te halen.</span><span class="sxs-lookup"><span data-stu-id="1aa27-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="1aa27-124">Uw klant die de rol van eigenaar **of** beheerder van gebruikerstoegang heeft en machtigingen heeft om roltoewijzing op abonnementsniveau te maken, doet het volgende:</span><span class="sxs-lookup"><span data-stu-id="1aa27-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="1aa27-125">Maakt verbinding met de tenant waar het CSP-abonnement zich bevindt.</span><span class="sxs-lookup"><span data-stu-id="1aa27-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="1aa27-126">Maakt verbinding met het abonnement (alleen van toepassing als de gebruiker roltoewijzingsmachtigingen heeft voor meerdere abonnementen in de tenant).</span><span class="sxs-lookup"><span data-stu-id="1aa27-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="1aa27-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"'</span><span class="sxs-lookup"><span data-stu-id="1aa27-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="1aa27-128">Hiermee maakt u de roltoewijzing</span><span class="sxs-lookup"><span data-stu-id="1aa27-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="1aa27-129">Als u machtigingen voor de rol eigenaar wilt verlenen op het niveau van de resourcegroep of op resourceniveau in plaats van het abonnementsbereik, kunnen de volgende opdrachten worden gebruikt:</span><span class="sxs-lookup"><span data-stu-id="1aa27-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="1aa27-130">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="1aa27-130">Next steps</span></span>

- [<span data-ttu-id="1aa27-131">Abonnementen en resources beheren onder het Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="1aa27-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
