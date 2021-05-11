---
title: Tenant-id, domeinnaam, gebruikersobject-id zoeken
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Informatie over het vinden van id's in de Azure Portal- de Azure AD-tenant-id, domeinnaam of specifieke gebruikersobject-id van een organisatie. Sommige taken hebben deze informatie nodig.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740281"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="1c9d4-104">Belangrijke ID's voor een gebruiker zoeken</span><span class="sxs-lookup"><span data-stu-id="1c9d4-104">Locate important IDs for a user</span></span>

<span data-ttu-id="1c9d4-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="1c9d4-105">**Appropriate roles**</span></span>

- <span data-ttu-id="1c9d4-106">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="1c9d4-106">Global admin</span></span>

<span data-ttu-id="1c9d4-107">In dit artikel wordt beschreven hoe u de [Azure Portal](https://portal.azure.com/) zoeken naar de volgende informatie voor een gebruiker:</span><span class="sxs-lookup"><span data-stu-id="1c9d4-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="1c9d4-108">De Microsoft Azure Active Directory tenant-id (Azure AD) van de organisatie of het bedrijf van de gebruiker</span><span class="sxs-lookup"><span data-stu-id="1c9d4-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="1c9d4-109">De primaire domeinnaam van de organisatie of het bedrijf dat is gekoppeld aan de Azure AD-tenant</span><span class="sxs-lookup"><span data-stu-id="1c9d4-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="1c9d4-110">De object-id van de gebruiker</span><span class="sxs-lookup"><span data-stu-id="1c9d4-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="1c9d4-111">De tenant Microsoft Azure AD-id en primaire domeinnaam zoeken</span><span class="sxs-lookup"><span data-stu-id="1c9d4-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="1c9d4-112">Volg deze stappen om de Azure AD-tenant-id of primaire domeinnaam in de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="1c9d4-113">(Zie Tenant-id zoeken met [PowerShell](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)of CLI als u programmatisch een tenant-id wilt zoeken.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="1c9d4-114">De tenant-id kan verschillende namen worden genoemd in verschillende toepassingen of resources.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="1c9d4-115">De tenant-id kan bijvoorbeeld worden aangeduid als de directory-id, de Azure Active Directory-tenant (Azure AD), Microsoft ID of voor bepaalde rapporten, zelfs de *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="1c9d4-116">Meld u aan bij de [Azure-portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="1c9d4-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="1c9d4-117">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Toont Azure Portal de optie Azure Active Directory selecteren in het menu.":::

3. <span data-ttu-id="1c9d4-119">Er Azure Active Directory **pagina Overzicht** weergegeven.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="1c9d4-120">Als u de Azure AD-tenant-id of primaire domeinnaam wilt zoeken, gaat u naar het **veld Tenant-id** en **het veld Primair** domein.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="1c9d4-121">Deze velden worden weergegeven in de sectie Tenantgegevens.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Toont de pagina Overzicht met twee gemarkeerde velden, tenant-id en primaire domeinnaam.":::

4. <span data-ttu-id="1c9d4-123">U kunt de tenant-id op een Azure Portal andere manieren vinden.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="1c9d4-124">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="1c9d4-125">Zoek vervolgens de sectie **Beheren** in het menu en selecteer **Eigenschappen.**</span><span class="sxs-lookup"><span data-stu-id="1c9d4-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="1c9d4-126">Op de pagina Eigenschappen wordt ook de gekoppelde tenant-id van de gebruiker weergegeven.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Toont de pagina Eigenschappen met het gemarkeerde veld Tenant-id.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="1c9d4-128">De object-id van de gebruiker zoeken</span><span class="sxs-lookup"><span data-stu-id="1c9d4-128">Find the user object ID</span></span>

<span data-ttu-id="1c9d4-129">Het vinden van de domeinnaam en tenant-id is mogelijk niet altijd voldoende.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="1c9d4-130">Mogelijk moet u ook de specifieke object-id vinden die aan een gebruiker is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="1c9d4-131">Volg deze stappen om de object-id van een gebruiker te vinden in de Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="1c9d4-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="1c9d4-132">Meld u aan bij de [Azure-portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="1c9d4-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="1c9d4-133">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="1c9d4-134">Zoek de **sectie** Beheren in het menu en selecteer vervolgens **Gebruikers.**</span><span class="sxs-lookup"><span data-stu-id="1c9d4-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Geeft Azure Active Directory menu weer met gemarkeerde optie Gebruikers.":::

4. <span data-ttu-id="1c9d4-136">Typ op de pagina Gebruikers de naam van de gebruiker in het zoekvak.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Toont de pagina Gebruikers met een zoekvak om te zoeken naar een specifieke gebruiker.":::

5. <span data-ttu-id="1c9d4-138">Selecteer de naam van de gebruiker waar deze wordt weergegeven in de lijst.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Toont de pagina Gebruiker met een rij voor de gezochte gebruiker.":::

6. <span data-ttu-id="1c9d4-140">Zoek de sectie Identiteit op de pagina Profiel van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="1c9d4-141">Het veld Object-id wordt hier weergegeven met de unieke object-id van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="1c9d4-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Toont de pagina Gebruikersprofiel met de sectie Identiteit en één gemarkeerd veld voor Object-id.":::

## <a name="next-steps"></a><span data-ttu-id="1c9d4-143">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="1c9d4-143">Next steps</span></span>

- [<span data-ttu-id="1c9d4-144">Uw tenant-id programmatisch zoeken met PowerShell of CLI</span><span class="sxs-lookup"><span data-stu-id="1c9d4-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="1c9d4-145">Meer informatie over gebruikersprofielen in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1c9d4-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="1c9d4-146">Ontdek hoe partners klantgegevens kunnen zien of exporteren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="1c9d4-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

