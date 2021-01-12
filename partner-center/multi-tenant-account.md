---
title: Extra tenants toevoegen aan uw partner centrum-account
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen, consolideren en beheren van meerdere Azure AD-tenants in uw partner centrum-account. Lees ook over een aantal van de redenen waarom u dit zou willen doen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105546"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="19e13-104">Meerdere tenants toevoegen en beheren in uw partner centrum-account</span><span class="sxs-lookup"><span data-stu-id="19e13-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="19e13-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="19e13-105">**Appropriate roles**</span></span>

- <span data-ttu-id="19e13-106">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="19e13-106">Global admin</span></span>

<span data-ttu-id="19e13-107">Met deze functie kunt u meerdere tenants voor uw bedrijf beheren en deze consolideren in uw account van het Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="19e13-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="19e13-108">Er zijn verschillende redenen waarom u meerdere Azure AD-tenants in uw partner centrum-account moet beheren.</span><span class="sxs-lookup"><span data-stu-id="19e13-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="19e13-109">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="19e13-109">For example:</span></span>

- <span data-ttu-id="19e13-110">Uw bedrijf kan een ander bedrijf kopen en u wilt dat de werk nemers in het nieuwe bedrijf partner Center kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="19e13-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="19e13-111">U wilt echter dat de twee bedrijven gescheiden blijven.</span><span class="sxs-lookup"><span data-stu-id="19e13-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="19e13-112">In dit geval koppelt u de Azure AD-Tenant van het nieuwe bedrijf aan uw wereld wijde partner account (PGA).</span><span class="sxs-lookup"><span data-stu-id="19e13-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="19e13-113">Met deze koppeling kunnen gebruikers in beide bedrijven werken in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="19e13-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="19e13-114">Als u meer dan één Tenant hebt voor het uitvoeren van uw bedrijf (bijvoorbeeld contoso.com, contoso.uk, contoso.in), kunt u multitenancy gebruiken om ze te koppelen aan hetzelfde PC-account.</span><span class="sxs-lookup"><span data-stu-id="19e13-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="19e13-115">Voor fusies en acquisities moet u met meer dan één Tenant werken (bijvoorbeeld als contoso fabrikam aanschaft, moet u zowel Constoso.com als Fabrikam.com respectieve tenants gebruiken).</span><span class="sxs-lookup"><span data-stu-id="19e13-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="19e13-116">Gebruikers van een van de tenants moeten het volgende kunnen doen:</span><span class="sxs-lookup"><span data-stu-id="19e13-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="19e13-117">Access Partner Center voor training, digitale down loads, MCP-koppeling</span><span class="sxs-lookup"><span data-stu-id="19e13-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="19e13-118">Er zijn partner Center-rollen, zoals MPN-beheer, prikkel beheer enz.</span><span class="sxs-lookup"><span data-stu-id="19e13-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="19e13-119">Nog een Azure AD-Tenant aan uw account toevoegen</span><span class="sxs-lookup"><span data-stu-id="19e13-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="19e13-120">Meld u als globale beheerder aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="19e13-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="19e13-121">Selecteer op het pictogram **instellingen** **account instellingen** en selecteer vervolgens **tenants**.</span><span class="sxs-lookup"><span data-stu-id="19e13-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="tenants koppelen"::: 

3. <span data-ttu-id="19e13-123">Selecteer **een andere AD-Tenant koppelen** en geef aan welke Tenant u wilt koppelen.</span><span class="sxs-lookup"><span data-stu-id="19e13-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="19e13-124">Meld u als globale beheerder aan bij de Tenant die u wilt koppelen en bevestig de koppeling.</span><span class="sxs-lookup"><span data-stu-id="19e13-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="koppelen van tenants bevestigen"::: 

5. <span data-ttu-id="19e13-126">Nadat u hebt bevestigd, ziet u de melding **alle instellingen** .</span><span class="sxs-lookup"><span data-stu-id="19e13-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="19e13-127">Selecteer **terug naar Tenant beheer om** de zojuist toegevoegde Tenant weer te geven.</span><span class="sxs-lookup"><span data-stu-id="19e13-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="19e13-128">U kunt een Tenant niet koppelen aan een account als het al is gekoppeld aan een ander partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="19e13-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="19e13-129">Een Tenant verwijderen uit uw account</span><span class="sxs-lookup"><span data-stu-id="19e13-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="19e13-130">Meld u als globale beheerder aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="19e13-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="19e13-131">Selecteer op het pictogram **instellingen** **Account instellingen** -> tenants en klik op het tabblad **partner** .</span><span class="sxs-lookup"><span data-stu-id="19e13-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="19e13-132">Klik op **verwijderen** voor de Tenant die u wilt ontkoppelen.</span><span class="sxs-lookup"><span data-stu-id="19e13-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="19e13-133">Het ontkoppelen van een Tenant betekent dat de gebruikers van die Tenant niet langer toegang hebben tot het partner centrum-account en dat dit gevolgen kan hebben voor uw vaardig heden.</span><span class="sxs-lookup"><span data-stu-id="19e13-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="19e13-134">De knop **verwijderen** is ingeschakeld voor alle gekoppelde tenants, met uitzonde ring van de primaire Tenant en de Tenant waarmee u momenteel bent aangemeld.</span><span class="sxs-lookup"><span data-stu-id="19e13-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="tenants met de knop verwijderen":::
 

## <a name="next-steps"></a><span data-ttu-id="19e13-136">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="19e13-136">Next steps</span></span>

- [<span data-ttu-id="19e13-137">Gebruikers toevoegen</span><span class="sxs-lookup"><span data-stu-id="19e13-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






