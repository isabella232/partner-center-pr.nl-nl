---
title: Beheerders bevoegdheden voor Azure CSP opnieuw invoeren
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe u klanten helpt om de beheerders bevoegdheden van een partner te herstellen, zodat de partner de Azure CSP-abonnementen van een klant kan beheren.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315844"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="a2c0d-103">Beheerders bevoegdheden voor de Azure CSP-abonnementen van een klant opnieuw invoeren</span><span class="sxs-lookup"><span data-stu-id="a2c0d-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="a2c0d-104">**Toepasselijke rollen**</span><span class="sxs-lookup"><span data-stu-id="a2c0d-104">**Applicable roles**</span></span>

- <span data-ttu-id="a2c0d-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="a2c0d-105">Global admin</span></span>
- <span data-ttu-id="a2c0d-106">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="a2c0d-106">Admin agent</span></span>

<span data-ttu-id="a2c0d-107">Als CSP-partner verwachten uw klanten vaak dat u hun Azure-gebruik en hun systemen hiervoor gaat beheren.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="a2c0d-108">Hiervoor moet u beheerders bevoegdheden hebben.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="a2c0d-109">Sommige bevoegdheden worden verleend wanneer uw reseller-relatie met de klant tot stand is gebracht.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="a2c0d-110">Anderen worden aan u verleend door uw klant.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="a2c0d-111">Beheerders bevoegdheden voor Azure in CSP</span><span class="sxs-lookup"><span data-stu-id="a2c0d-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="a2c0d-112">Er zijn twee niveaus van beheerders bevoegdheden voor Azure in CSP.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="a2c0d-113">**Beheerders bevoegdheden op Tenant niveau** (**gedelegeerde beheerders bevoegdheden**): CSP-partners krijgen deze bevoegdheden bij het tot stand brengen van de leverancier van de CSP-dealer met klanten.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="a2c0d-114">Gedelegeerde beheerders bevoegdheden bieden CSP-partners toegang tot de tenants van hun klanten, waardoor ze beheer functies kunnen uitvoeren zoals gebruikers toevoegen/beheren, wacht woorden opnieuw instellen en gebruikers licenties beheren.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-114">Delegated admin privileges gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="a2c0d-115">**Beheerders bevoegdheden op abonnements niveau** : CSP-partners krijgen deze bevoegdheden tijdens het maken van Azure CSP-abonnementen voor hun klanten.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="a2c0d-116">Met deze bevoegdheden hebben CSP-partners volledige toegang tot deze abonnementen, waardoor ze Azure-bronnen kunnen inrichten en beheren.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="a2c0d-117">Beheerders bevoegdheden voor de CSP-partners herstellen</span><span class="sxs-lookup"><span data-stu-id="a2c0d-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="a2c0d-118">Uw klant kan de toewijzing van de cryptografie functie opnieuw maken zolang u de object-ID van de AdminAgents-groep aan uw klant verstrekt.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-118">Your customer is able to re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="a2c0d-119">Als u gedelegeerde beheerders bevoegdheden wilt herstellen, moet u samen werken met uw klant.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="a2c0d-120">Meld u aan bij het dash board van de partner centrum en selecteer **klanten** in het menu partner centrum.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="a2c0d-121">Selecteer de klant waarmee u werkt en **vraag een reseller-relatie aan.**</span><span class="sxs-lookup"><span data-stu-id="a2c0d-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="a2c0d-122">Hiermee genereert u een koppeling naar de klant die Tenant beheerders rechten heeft.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-122">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="a2c0d-123">Die klant moet de koppeling selecteren en de wederverkoper-relatie aanvraag goed keuren.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Voor beeld van een reseller-relatie voor het maken van e-mail":::

4. <span data-ttu-id="a2c0d-125">U moet, de partner, verbinding maken met de partner-Tenant om de object-ID van de AdminAgents-groep op te halen.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="a2c0d-126">Uw klant die de rol van **eigenaar of beheerder voor gebruikers toegang** heeft en gemachtigd is om roltoewijzing op het abonnements niveau te maken, doet het volgende:</span><span class="sxs-lookup"><span data-stu-id="a2c0d-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="a2c0d-127">Hiermee maakt u verbinding met de Tenant waar het CSP-abonnement bestaat.</span><span class="sxs-lookup"><span data-stu-id="a2c0d-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="a2c0d-128">Maakt verbinding met het abonnement (alleen van toepassing als de gebruiker machtigingen voor roltoewijzingen heeft via meerdere abonnementen in de Tenant).</span><span class="sxs-lookup"><span data-stu-id="a2c0d-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="a2c0d-129">PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "CSP-abonnements-ID" '</span><span class="sxs-lookup"><span data-stu-id="a2c0d-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="a2c0d-130">Hiermee wordt de roltoewijzing gemaakt</span><span class="sxs-lookup"><span data-stu-id="a2c0d-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="a2c0d-131">Als u wilt dat de machtiging rol van eigenaar wordt verleend op resource groeps niveau of op resource niveau in plaats van het abonnements bereik, kunnen de volgende opdrachten werken:</span><span class="sxs-lookup"><span data-stu-id="a2c0d-131">If the desire is to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="a2c0d-132">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="a2c0d-132">Next steps</span></span>

- [<span data-ttu-id="a2c0d-133">Abonnementen en resources beheren onder het Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="a2c0d-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
