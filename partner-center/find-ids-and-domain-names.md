---
title: Tenant-ID, domein naam, gebruikers object-ID zoeken
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: "Meer informatie over het zoeken naar Id's in de Azure Portal: de Azure AD-Tenant-ID, domein naam of specifieke gebruikers object-ID van een organisatie. Sommige taken hebben deze informatie nodig."
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/17/2020
ms.locfileid: "92528397"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="2bfc3-104">Belang rijke Id's voor een gebruiker zoeken</span><span class="sxs-lookup"><span data-stu-id="2bfc3-104">Locate important IDs for a user</span></span>

<span data-ttu-id="2bfc3-105">In dit artikel wordt beschreven hoe u de [Azure Portal](https://portal.azure.com/) kunt gebruiken om de volgende informatie te vinden voor een gebruiker:</span><span class="sxs-lookup"><span data-stu-id="2bfc3-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="2bfc3-106">De Tenant-ID van het Microsoft Azure Active Directory (Azure AD) van de organisatie of het bedrijf van de gebruiker</span><span class="sxs-lookup"><span data-stu-id="2bfc3-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="2bfc3-107">De primaire domein naam van de organisatie of het bedrijf dat is gekoppeld aan de Azure AD-Tenant</span><span class="sxs-lookup"><span data-stu-id="2bfc3-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="2bfc3-108">De gebruikers object-ID</span><span class="sxs-lookup"><span data-stu-id="2bfc3-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="2bfc3-109">De Microsoft Azure AD Tenant-ID en primaire domein naam zoeken</span><span class="sxs-lookup"><span data-stu-id="2bfc3-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="2bfc3-110">Volg deze stappen om de Tenant-ID van Azure AD of de primaire domein naam binnen de Azure Portal te vinden.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span>

> [!NOTE]
> <span data-ttu-id="2bfc3-111">De Tenant-ID kan verschillende namen in verschillende toepassingen of bronnen worden genoemd.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-111">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="2bfc3-112">De Tenant-ID kan bijvoorbeeld worden aangeduid als de Directory-ID, de Azure Active Directory (Azure AD)-Tenant, micro soft-ID of voor bepaalde rapporten, zelfs het *tenantguid* .</span><span class="sxs-lookup"><span data-stu-id="2bfc3-112">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid* .</span></span>

1. <span data-ttu-id="2bfc3-113">Meld u aan bij [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2bfc3-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="2bfc3-114">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-114">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

3. <span data-ttu-id="2bfc3-116">Er wordt een Azure Active Directory **overzichts** pagina weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-116">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="2bfc3-117">Als u de Tenant-ID van Azure AD of de naam van het primaire domein wilt zoeken, zoekt u naar het veld **Tenant-id** en het veld **primair domein** .</span><span class="sxs-lookup"><span data-stu-id="2bfc3-117">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="2bfc3-118">Deze velden worden weer gegeven in de sectie informatie over tenants.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-118">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Geeft overzichts pagina weer met twee gemarkeerde velden, Tenant-ID en primaire domein naam.":::

4. <span data-ttu-id="2bfc3-120">U kunt de Tenant-ID in de Azure Portal op een paar andere manieren vinden.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-120">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="2bfc3-121">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-121">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="2bfc3-122">Zoek vervolgens de sectie **beheren** in het menu en selecteer **Eigenschappen** .</span><span class="sxs-lookup"><span data-stu-id="2bfc3-122">Then, locate the **Manage** section on the menu and select **Properties** .</span></span>

   <span data-ttu-id="2bfc3-123">Op de pagina eigenschappen wordt ook de bijbehorende Tenant-ID van de gebruiker weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-123">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Eigenschappen pagina met gemarkeerd Tenant-ID-veld weer geven.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="2bfc3-125">De gebruikers object-ID zoeken</span><span class="sxs-lookup"><span data-stu-id="2bfc3-125">Find the user object ID</span></span>

<span data-ttu-id="2bfc3-126">Het is niet altijd voldoende om de domein naam en Tenant-ID te zoeken.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-126">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="2bfc3-127">Mogelijk moet u ook de specifieke object-ID vinden die aan een gebruiker is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-127">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="2bfc3-128">Volg deze stappen om de object-ID van een gebruiker te zoeken in de Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="2bfc3-128">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="2bfc3-129">Meld u aan bij [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="2bfc3-129">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="2bfc3-130">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-130">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="2bfc3-131">Ga naar de sectie **beheren** in het menu en selecteer vervolgens **gebruikers** .</span><span class="sxs-lookup"><span data-stu-id="2bfc3-131">Locate the **Manage** section on the menu, then select **Users** .</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Toont Azure Active Directory menu met gemarkeerde gebruikers opties.":::

4. <span data-ttu-id="2bfc3-133">Typ op de pagina gebruikers de naam van de gebruiker in het zoekvak.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-133">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Toont de pagina gebruikers met het zoekvak om te zoeken naar een specifieke gebruiker.":::

5. <span data-ttu-id="2bfc3-135">Selecteer de naam van de gebruiker die wordt weer gegeven in de lijst.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-135">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Gebruikers pagina weer geven waarin een rij voor de gezochte gebruiker wordt weer gegeven.":::

6. <span data-ttu-id="2bfc3-137">Zoek de sectie identiteit op de profiel pagina van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-137">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="2bfc3-138">Het veld object-ID wordt hier weer gegeven met de unieke object-ID van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="2bfc3-138">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Hiermee wordt de gebruikers profiel pagina met de identiteits sectie en één gemarkeerd veld voor de object-ID weer gegeven.":::

## <a name="next-steps"></a><span data-ttu-id="2bfc3-140">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="2bfc3-140">Next steps</span></span>

- [<span data-ttu-id="2bfc3-141">Meer informatie over gebruikers profielen in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="2bfc3-141">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="2bfc3-142">Ontdek hoe partners klant gegevens kunnen zien of exporteren in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="2bfc3-142">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)