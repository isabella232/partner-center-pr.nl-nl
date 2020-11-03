---
title: Extra tenants toevoegen aan uw partner centrum-account
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen, consolideren en beheren van meerdere Azure AD-tenants in uw partner centrum-account. Lees ook over een aantal van de redenen waarom u dit zou willen doen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92528752"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="3f4de-104">Meerdere tenants toevoegen en beheren in uw partner centrum-account</span><span class="sxs-lookup"><span data-stu-id="3f4de-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="3f4de-105">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="3f4de-105">**Applies to**</span></span>

- <span data-ttu-id="3f4de-106">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="3f4de-106">Partner Center</span></span>

<span data-ttu-id="3f4de-107">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="3f4de-107">**Appropriate roles**</span></span>

- <span data-ttu-id="3f4de-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="3f4de-108">Global admin</span></span>

<span data-ttu-id="3f4de-109">Met deze functie kunt u meerdere tenants voor uw bedrijf beheren en deze consolideren in uw account van het Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="3f4de-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="3f4de-110">Er zijn verschillende redenen waarom u meerdere Azure AD-tenants in uw partner centrum-account moet beheren.</span><span class="sxs-lookup"><span data-stu-id="3f4de-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="3f4de-111">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="3f4de-111">For example:</span></span>

- <span data-ttu-id="3f4de-112">Uw bedrijf kan een ander bedrijf kopen en u wilt dat de werk nemers in het nieuwe bedrijf partner Center kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="3f4de-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="3f4de-113">U wilt echter dat de twee bedrijven gescheiden blijven.</span><span class="sxs-lookup"><span data-stu-id="3f4de-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="3f4de-114">In dit geval koppelt u de Azure AD-Tenant van het nieuwe bedrijf aan uw wereld wijde partner account (PGA).</span><span class="sxs-lookup"><span data-stu-id="3f4de-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="3f4de-115">Met deze koppeling kunnen gebruikers in beide bedrijven werken in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="3f4de-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="3f4de-116">Als u meer dan één Tenant hebt voor het uitvoeren van uw bedrijf (bijvoorbeeld contoso.com, contoso.uk, contoso.in), kunt u multitenancy gebruiken om ze te koppelen aan hetzelfde PC-account.</span><span class="sxs-lookup"><span data-stu-id="3f4de-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="3f4de-117">Voor fusies en acquisities moet u met meer dan één Tenant werken (bijvoorbeeld als contoso fabrikam aanschaft, moet u zowel Constoso.com als Fabrikam.com respectieve tenants gebruiken).</span><span class="sxs-lookup"><span data-stu-id="3f4de-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="3f4de-118">Gebruikers van een van de tenants moeten het volgende kunnen doen:</span><span class="sxs-lookup"><span data-stu-id="3f4de-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="3f4de-119">Access Partner Center voor training, digitale down loads, MCP-koppeling</span><span class="sxs-lookup"><span data-stu-id="3f4de-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="3f4de-120">Er zijn partner Center-rollen, zoals MPN-beheer, prikkel beheer enz.</span><span class="sxs-lookup"><span data-stu-id="3f4de-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="3f4de-121">Nog een Azure AD-Tenant aan uw account toevoegen</span><span class="sxs-lookup"><span data-stu-id="3f4de-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="3f4de-122">Meld u als globale beheerder aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="3f4de-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="3f4de-123">Selecteer op het pictogram **instellingen** **account instellingen** en selecteer vervolgens **tenants** .</span><span class="sxs-lookup"><span data-stu-id="3f4de-123">From the **Settings** icon, select **Account settings** and then select **Tenants** .</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="tenants koppelen"::: 

3. <span data-ttu-id="3f4de-125">Selecteer **een andere AD-Tenant koppelen** en geef aan welke Tenant u wilt koppelen.</span><span class="sxs-lookup"><span data-stu-id="3f4de-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="3f4de-126">Meld u als globale beheerder aan bij de Tenant die u wilt koppelen en bevestig de koppeling.</span><span class="sxs-lookup"><span data-stu-id="3f4de-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="koppelen van tenants bevestigen"::: 

5. <span data-ttu-id="3f4de-128">Nadat u hebt bevestigd, ziet u de melding **alle instellingen** .</span><span class="sxs-lookup"><span data-stu-id="3f4de-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="3f4de-129">Selecteer **terug naar Tenant beheer** en de zojuist toegevoegde Tenant wordt weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="3f4de-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="3f4de-130">U kunt een Tenant niet koppelen aan een account als het al is gekoppeld aan een ander partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="3f4de-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="3f4de-131">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="3f4de-131">Next steps</span></span>

- [<span data-ttu-id="3f4de-132">Gebruikers toevoegen</span><span class="sxs-lookup"><span data-stu-id="3f4de-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
