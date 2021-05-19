---
title: Tenants toevoegen aan uw Partner Center account
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen, consolideren of beheren van meerdere Azure AD-tenants in uw Partner Center-account en ontdek waarom u dit zou willen doen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151199"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="453b1-103">Meerdere tenants toevoegen en beheren in uw Partner Center account</span><span class="sxs-lookup"><span data-stu-id="453b1-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="453b1-104">**Juiste rollen:** globale | Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="453b1-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="453b1-105">In dit artikel wordt beschreven hoe u meerdere Azure Active Directory (Azure AD)-tenants voor uw bedrijf samenvoegt en vervolgens toevoegt en beheert in uw Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="453b1-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="453b1-106">Er zijn veel redenen om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="453b1-106">There are many reasons to do so.</span></span> <span data-ttu-id="453b1-107">Bijvoorbeeld:</span><span class="sxs-lookup"><span data-stu-id="453b1-107">For example:</span></span>

- <span data-ttu-id="453b1-108">Stel dat uw bedrijf, Contoso, een ander bedrijf heeft overgenomen, Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="453b1-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="453b1-109">U wilt dat de twee bedrijven gescheiden blijven, maar u wilt dat de nieuwe werknemers deze kunnen Partner Center.</span><span class="sxs-lookup"><span data-stu-id="453b1-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="453b1-110">In dit geval koppelt u de Azure AD-tenant van het nieuwe bedrijf aan uw Partner Global Account (PGA).</span><span class="sxs-lookup"><span data-stu-id="453b1-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="453b1-111">Met deze associatie kunnen gebruikers in beide bedrijven in een Partner Center.</span><span class="sxs-lookup"><span data-stu-id="453b1-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="453b1-112">Als u uw bedrijf met meer dan één tenant hebt (bijvoorbeeld *contoso.com*, *contoso.uk* en *contoso.in*), kunt u multitenancy gebruiken om ze in hetzelfde pc-account te groepen.</span><span class="sxs-lookup"><span data-stu-id="453b1-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="453b1-113">Als voor fusies en overnamesrichtlijnen is vereist dat u met tenants van beide bedrijven werkt, gebruikt u zowel de constoso.com *als* *fabrikam.com* tenants.</span><span class="sxs-lookup"><span data-stu-id="453b1-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="453b1-114">Gebruikers van een van de tenants moeten het volgende kunnen doen:</span><span class="sxs-lookup"><span data-stu-id="453b1-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="453b1-115">Toegang Partner Center voor training, digitale downloads of MICROSOFT Certified Professional (MCP)-associatie.</span><span class="sxs-lookup"><span data-stu-id="453b1-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="453b1-116">Worden toegewezen Partner Center zoals Microsoft Partner Network (MPN)-beheerder of incentivesbeheerder.</span><span class="sxs-lookup"><span data-stu-id="453b1-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="453b1-117">Een Azure AD-tenant toevoegen aan uw account</span><span class="sxs-lookup"><span data-stu-id="453b1-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="453b1-118">Meld u als globale beheerder aan [bij Microsoft Partner Center.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="453b1-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="453b1-119">Selecteer in de rechterbovenhoek **Instellingen,** selecteer **Accountinstellingen** en selecteer vervolgens **Tenants.**</span><span class="sxs-lookup"><span data-stu-id="453b1-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Schermopname van de knop Koppelen in het deelvenster Azure AD-profiel."::: 

1. <span data-ttu-id="453b1-121">Selecteer **Koppelen** en geef vervolgens de tenant aan die u wilt koppelen.</span><span class="sxs-lookup"><span data-stu-id="453b1-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="453b1-122">Meld u bij de prompt aan als globale beheerder bij de tenant die u wilt koppelen en selecteer **vervolgens Bevestigen.**</span><span class="sxs-lookup"><span data-stu-id="453b1-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Schermopname van de knop Bevestigen in het deelvenster Nieuwe Azure AD-associatie bevestigen."::: 

   <span data-ttu-id="453b1-124">Nadat u de associatie hebt bevestigd, wordt het **bericht** Alle ingesteld weergegeven.</span><span class="sxs-lookup"><span data-stu-id="453b1-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="453b1-125">Als u de zojuist toegevoegde tenant wilt weergeven, selecteert **u Terugkeren naar tenantbeheer.**</span><span class="sxs-lookup"><span data-stu-id="453b1-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="453b1-126">U kunt een tenant niet koppelen aan een account als deze al is gekoppeld aan een Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="453b1-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="453b1-127">Een tenant uit uw account verwijderen</span><span class="sxs-lookup"><span data-stu-id="453b1-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="453b1-128">Meld u als globale beheerder aan [bij Microsoft Partner Center.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="453b1-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="453b1-129">Selecteer rechtsboven het pictogram **Instellingen** en selecteer vervolgens **Accountinstellingen.**</span><span class="sxs-lookup"><span data-stu-id="453b1-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="453b1-130">Selecteer tenants in het **linkerdeelvenster.**</span><span class="sxs-lookup"><span data-stu-id="453b1-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="453b1-131">Selecteer **onder Azure AD-tenants beheren** het tabblad **Partner.**</span><span class="sxs-lookup"><span data-stu-id="453b1-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="453b1-132">Selecteer **Verwijderen naast** de tenant waarvan u de associatie wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="453b1-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Schermopname van de huidige tenantkoppelingen en de koppelingen verwijderen.":::

   <span data-ttu-id="453b1-134">Zoals u in de vorige  schermopname ziet, zijn de koppelingen verwijderen ingeschakeld voor alle gekoppelde tenants, met uitzondering van de primaire tenant en de tenant waarmee u momenteel bent aangemeld.</span><span class="sxs-lookup"><span data-stu-id="453b1-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="453b1-135">Wanneer u een tenant verwijdert, hebben de gebruikers in die tenant niet langer toegang tot het Partner Center-account en heeft het verwijderen mogelijk invloed op uw competenties.</span><span class="sxs-lookup"><span data-stu-id="453b1-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="453b1-136">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="453b1-136">Next steps</span></span>

- [<span data-ttu-id="453b1-137">Gebruikersaccounts maken</span><span class="sxs-lookup"><span data-stu-id="453b1-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






