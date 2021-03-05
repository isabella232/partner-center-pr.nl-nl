---
title: Tenants toevoegen aan uw partner centrum-account
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen, consolideren of beheren van meerdere Azure AD-tenants in uw partner centrum-account en waarom u dit mogelijk wilt maken.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124802"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="1889e-103">Meerdere tenants toevoegen en beheren in uw partner centrum-account</span><span class="sxs-lookup"><span data-stu-id="1889e-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="1889e-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="1889e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1889e-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="1889e-105">Global admin</span></span>
- <span data-ttu-id="1889e-106">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="1889e-106">Account admin</span></span>

<span data-ttu-id="1889e-107">In dit artikel wordt beschreven hoe u meerdere Azure Active Directory-tenants (Azure AD) consolideert voor uw bedrijf en deze vervolgens kunt toevoegen en beheren in uw partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="1889e-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="1889e-108">Er zijn veel redenen om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="1889e-108">There are many reasons to do so.</span></span> <span data-ttu-id="1889e-109">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="1889e-109">For example:</span></span>

- <span data-ttu-id="1889e-110">Stel dat uw bedrijf, contoso, een ander bedrijf, Fabrikam heeft aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="1889e-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="1889e-111">U wilt dat de twee bedrijven gescheiden blijven, maar u wilt dat de nieuwe werk nemers partner centrum kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="1889e-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="1889e-112">In dit geval koppelt u de Azure AD-Tenant van het nieuwe bedrijf aan uw wereld wijde partner account (PGA).</span><span class="sxs-lookup"><span data-stu-id="1889e-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="1889e-113">Met deze koppeling kunnen gebruikers in beide bedrijven werken in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="1889e-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="1889e-114">Als u uw bedrijf met meer dan één Tenant uitvoert (bijvoorbeeld *contoso.com*, *contoso.uk* en *contoso.in*), kunt u multitenancy gebruiken om ze te groeperen in hetzelfde PC-account.</span><span class="sxs-lookup"><span data-stu-id="1889e-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="1889e-115">Als er richt lijnen voor samen voegen en acquisities nodig zijn om te werken met tenants van beide bedrijven, gebruikt u zowel de *constoso.com* -als *fabrikam.com* -tenants.</span><span class="sxs-lookup"><span data-stu-id="1889e-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="1889e-116">Gebruikers van de tenants moeten het volgende kunnen doen:</span><span class="sxs-lookup"><span data-stu-id="1889e-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="1889e-117">Access Partner Center voor training, digitale down loads of de micro soft Certified Professional (MCP)-koppeling.</span><span class="sxs-lookup"><span data-stu-id="1889e-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="1889e-118">U hebt Partner Center-rollen zoals Microsoft Partner Network (MPN) beheerder of prikkel beheerder toegewezen.</span><span class="sxs-lookup"><span data-stu-id="1889e-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="1889e-119">Een Azure AD-Tenant toevoegen aan uw account</span><span class="sxs-lookup"><span data-stu-id="1889e-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="1889e-120">Meld u aan als globale beheerder bij het [micro soft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="1889e-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="1889e-121">Selecteer in de rechter bovenhoek **instellingen**, selecteer **account instellingen** en selecteer vervolgens **tenants**.</span><span class="sxs-lookup"><span data-stu-id="1889e-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Scherm afbeelding van de knop koppelen in het deel venster Azure AD-profiel."::: 

1. <span data-ttu-id="1889e-123">Selecteer **koppelen** en geef vervolgens de Tenant op die u wilt koppelen.</span><span class="sxs-lookup"><span data-stu-id="1889e-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="1889e-124">Meld u aan bij de prompt als globale beheerder voor de Tenant die u wilt koppelen en selecteer vervolgens **bevestigen**.</span><span class="sxs-lookup"><span data-stu-id="1889e-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Scherm afbeelding van de knop bevestigen in het deel venster nieuwe Azure AD-koppeling bevestigen."::: 

   <span data-ttu-id="1889e-126">Nadat u de koppeling hebt bevestigd, wordt een **set** -bericht weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="1889e-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="1889e-127">Als u de zojuist toegevoegde Tenant wilt weer geven, selecteert **u terug naar Tenant beheer**.</span><span class="sxs-lookup"><span data-stu-id="1889e-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="1889e-128">U kunt een Tenant niet koppelen aan een account als het al is gekoppeld aan een ander partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="1889e-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="1889e-129">Een Tenant verwijderen uit uw account</span><span class="sxs-lookup"><span data-stu-id="1889e-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="1889e-130">Meld u aan als globale beheerder bij het [micro soft Partner Center](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="1889e-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="1889e-131">Selecteer in de rechter bovenhoek het pictogram **instellingen** en selecteer vervolgens **account instellingen**.</span><span class="sxs-lookup"><span data-stu-id="1889e-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="1889e-132">Selecteer in het linkerdeel venster **tenants**.</span><span class="sxs-lookup"><span data-stu-id="1889e-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="1889e-133">Onder **Azure AD-tenants beheren** selecteert u het tabblad **partner** .</span><span class="sxs-lookup"><span data-stu-id="1889e-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="1889e-134">Selecteer **verwijderen** naast de Tenant waarvan u de koppeling wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="1889e-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Scherm opname van de huidige Tenant koppelingen en hun koppelingen verwijderen.":::

   <span data-ttu-id="1889e-136">Zoals u in de vorige scherm afbeelding ziet, worden de koppelingen **verwijderen** ingeschakeld voor alle gekoppelde tenants, met uitzonde ring van de primaire Tenant en de Tenant waarbij u momenteel bent aangemeld.</span><span class="sxs-lookup"><span data-stu-id="1889e-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="1889e-137">Wanneer u een Tenant verwijdert, hebben de gebruikers van die Tenant geen toegang meer tot het partner centrum-account en kan het verwijderen van invloed zijn op uw vaardig heden.</span><span class="sxs-lookup"><span data-stu-id="1889e-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="1889e-138">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="1889e-138">Next steps</span></span>

- [<span data-ttu-id="1889e-139">Gebruikersaccounts maken</span><span class="sxs-lookup"><span data-stu-id="1889e-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






