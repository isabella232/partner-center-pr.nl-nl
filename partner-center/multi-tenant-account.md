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
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182427"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="3ce40-104">Meerdere tenants toevoegen en beheren in uw partner centrum-account</span><span class="sxs-lookup"><span data-stu-id="3ce40-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="3ce40-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="3ce40-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3ce40-106">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="3ce40-106">Global admin</span></span>
- <span data-ttu-id="3ce40-107">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="3ce40-107">Account admin</span></span>

<span data-ttu-id="3ce40-108">Met deze functie kunt u meerdere tenants voor uw bedrijf beheren en deze consolideren in uw account van het Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="3ce40-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="3ce40-109">Er zijn verschillende redenen waarom u meerdere Azure AD-tenants in uw partner centrum-account moet beheren.</span><span class="sxs-lookup"><span data-stu-id="3ce40-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="3ce40-110">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="3ce40-110">For example:</span></span>

- <span data-ttu-id="3ce40-111">Uw bedrijf kan een ander bedrijf kopen en u wilt dat de werk nemers in het nieuwe bedrijf partner Center kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="3ce40-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="3ce40-112">U wilt echter dat de twee bedrijven gescheiden blijven.</span><span class="sxs-lookup"><span data-stu-id="3ce40-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="3ce40-113">In dit geval koppelt u de Azure AD-Tenant van het nieuwe bedrijf aan uw wereld wijde partner account (PGA).</span><span class="sxs-lookup"><span data-stu-id="3ce40-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="3ce40-114">Met deze koppeling kunnen gebruikers in beide bedrijven werken in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="3ce40-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="3ce40-115">Als u meer dan één Tenant hebt voor het uitvoeren van uw bedrijf (bijvoorbeeld contoso.com, contoso.uk, contoso.in), kunt u multitenancy gebruiken om ze te koppelen aan hetzelfde PC-account.</span><span class="sxs-lookup"><span data-stu-id="3ce40-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="3ce40-116">Voor fusies en acquisities moet u met meer dan één Tenant werken (bijvoorbeeld als contoso fabrikam aanschaft, moet u zowel Constoso.com als Fabrikam.com respectieve tenants gebruiken).</span><span class="sxs-lookup"><span data-stu-id="3ce40-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="3ce40-117">Gebruikers van een van de tenants moeten het volgende kunnen doen:</span><span class="sxs-lookup"><span data-stu-id="3ce40-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="3ce40-118">Access Partner Center voor training, digitale down loads, MCP-koppeling</span><span class="sxs-lookup"><span data-stu-id="3ce40-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="3ce40-119">Er zijn partner Center-rollen, zoals MPN-beheer, prikkel beheer enz.</span><span class="sxs-lookup"><span data-stu-id="3ce40-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="3ce40-120">Nog een Azure AD-Tenant aan uw account toevoegen</span><span class="sxs-lookup"><span data-stu-id="3ce40-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="3ce40-121">Meld u als globale beheerder aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="3ce40-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="3ce40-122">Selecteer op het pictogram **instellingen** **account instellingen** en selecteer vervolgens **tenants**.</span><span class="sxs-lookup"><span data-stu-id="3ce40-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="tenants koppelen"::: 

3. <span data-ttu-id="3ce40-124">Selecteer **een andere AD-Tenant koppelen** en geef aan welke Tenant u wilt koppelen.</span><span class="sxs-lookup"><span data-stu-id="3ce40-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="3ce40-125">Meld u als globale beheerder aan bij de Tenant die u wilt koppelen en bevestig de koppeling.</span><span class="sxs-lookup"><span data-stu-id="3ce40-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="koppelen van tenants bevestigen"::: 

5. <span data-ttu-id="3ce40-127">Nadat u hebt bevestigd, ziet u de melding **alle instellingen** .</span><span class="sxs-lookup"><span data-stu-id="3ce40-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="3ce40-128">Selecteer **terug naar Tenant beheer om** de zojuist toegevoegde Tenant weer te geven.</span><span class="sxs-lookup"><span data-stu-id="3ce40-128">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="3ce40-129">U kunt een Tenant niet koppelen aan een account als het al is gekoppeld aan een ander partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="3ce40-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="3ce40-130">Een Tenant verwijderen uit uw account</span><span class="sxs-lookup"><span data-stu-id="3ce40-130">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="3ce40-131">Meld u als globale beheerder aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="3ce40-131">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="3ce40-132">Selecteer op het pictogram **instellingen** **Account instellingen** -> tenants en klik op het tabblad **partner** .</span><span class="sxs-lookup"><span data-stu-id="3ce40-132">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="3ce40-133">Klik op **verwijderen** voor de Tenant die u wilt ontkoppelen.</span><span class="sxs-lookup"><span data-stu-id="3ce40-133">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="3ce40-134">Het ontkoppelen van een Tenant betekent dat de gebruikers van die Tenant niet langer toegang hebben tot het partner centrum-account en dat dit gevolgen kan hebben voor uw vaardig heden.</span><span class="sxs-lookup"><span data-stu-id="3ce40-134">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="3ce40-135">De knop **verwijderen** is ingeschakeld voor alle gekoppelde tenants, met uitzonde ring van de primaire Tenant en de Tenant waarmee u momenteel bent aangemeld.</span><span class="sxs-lookup"><span data-stu-id="3ce40-135">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="tenants met de knop verwijderen":::
 

## <a name="next-steps"></a><span data-ttu-id="3ce40-137">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="3ce40-137">Next steps</span></span>

- [<span data-ttu-id="3ce40-138">Gebruikers toevoegen</span><span class="sxs-lookup"><span data-stu-id="3ce40-138">Add users</span></span>](create-user-accounts-and-set-permissions.md)






