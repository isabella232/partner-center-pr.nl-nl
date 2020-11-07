---
title: Tenant-ID, domein naam, gebruikers object-ID zoeken
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: "Meer informatie over het zoeken naar Id's in de Azure Portal: de Azure AD-Tenant-ID, domein naam of specifieke gebruikers object-ID van een organisatie. Sommige taken hebben deze informatie nodig."
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360068"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="db71e-104">Belang rijke Id's voor een gebruiker zoeken</span><span class="sxs-lookup"><span data-stu-id="db71e-104">Locate important IDs for a user</span></span>

<span data-ttu-id="db71e-105">In dit artikel wordt beschreven hoe u de [Azure Portal](https://portal.azure.com/) kunt gebruiken om de volgende informatie te vinden voor een gebruiker:</span><span class="sxs-lookup"><span data-stu-id="db71e-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="db71e-106">De Tenant-ID van het Microsoft Azure Active Directory (Azure AD) van de organisatie of het bedrijf van de gebruiker</span><span class="sxs-lookup"><span data-stu-id="db71e-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="db71e-107">De primaire domein naam van de organisatie of het bedrijf dat is gekoppeld aan de Azure AD-Tenant</span><span class="sxs-lookup"><span data-stu-id="db71e-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="db71e-108">De gebruikers object-ID</span><span class="sxs-lookup"><span data-stu-id="db71e-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="db71e-109">De Microsoft Azure AD Tenant-ID en primaire domein naam zoeken</span><span class="sxs-lookup"><span data-stu-id="db71e-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="db71e-110">Volg deze stappen om de Tenant-ID van Azure AD of de primaire domein naam binnen de Azure Portal te vinden.</span><span class="sxs-lookup"><span data-stu-id="db71e-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="db71e-111">(Als u een Tenant-ID wilt zoeken via een programma, raadpleegt u [Tenant-id zoeken met Power shell of cli](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span><span class="sxs-lookup"><span data-stu-id="db71e-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="db71e-112">De Tenant-ID kan verschillende namen in verschillende toepassingen of bronnen worden genoemd.</span><span class="sxs-lookup"><span data-stu-id="db71e-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="db71e-113">De Tenant-ID kan bijvoorbeeld worden aangeduid als de Directory-ID, de Azure Active Directory (Azure AD)-Tenant, micro soft-ID of voor bepaalde rapporten, zelfs het *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="db71e-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="db71e-114">Meld u aan bij de [Azure-portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="db71e-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="db71e-115">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="db71e-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

3. <span data-ttu-id="db71e-117">Er wordt een Azure Active Directory **overzichts** pagina weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="db71e-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="db71e-118">Als u de Tenant-ID van Azure AD of de naam van het primaire domein wilt zoeken, zoekt u naar het veld **Tenant-id** en het veld **primair domein** .</span><span class="sxs-lookup"><span data-stu-id="db71e-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="db71e-119">Deze velden worden weer gegeven in de sectie informatie over tenants.</span><span class="sxs-lookup"><span data-stu-id="db71e-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Geeft overzichts pagina weer met twee gemarkeerde velden, Tenant-ID en primaire domein naam.":::

4. <span data-ttu-id="db71e-121">U kunt de Tenant-ID in de Azure Portal op een paar andere manieren vinden.</span><span class="sxs-lookup"><span data-stu-id="db71e-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="db71e-122">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="db71e-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="db71e-123">Zoek vervolgens de sectie **beheren** in het menu en selecteer **Eigenschappen**.</span><span class="sxs-lookup"><span data-stu-id="db71e-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="db71e-124">Op de pagina eigenschappen wordt ook de bijbehorende Tenant-ID van de gebruiker weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="db71e-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Eigenschappen pagina met gemarkeerd Tenant-ID-veld weer geven.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="db71e-126">De gebruikers object-ID zoeken</span><span class="sxs-lookup"><span data-stu-id="db71e-126">Find the user object ID</span></span>

<span data-ttu-id="db71e-127">Het is niet altijd voldoende om de domein naam en Tenant-ID te zoeken.</span><span class="sxs-lookup"><span data-stu-id="db71e-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="db71e-128">Mogelijk moet u ook de specifieke object-ID vinden die aan een gebruiker is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="db71e-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="db71e-129">Volg deze stappen om de object-ID van een gebruiker te zoeken in de Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="db71e-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="db71e-130">Meld u aan bij de [Azure-portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="db71e-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="db71e-131">Selecteer **Azure Active Directory** in het menu.</span><span class="sxs-lookup"><span data-stu-id="db71e-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="db71e-132">Ga naar de sectie **beheren** in het menu en selecteer vervolgens **gebruikers**.</span><span class="sxs-lookup"><span data-stu-id="db71e-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Toont Azure Active Directory menu met gemarkeerde gebruikers opties.":::

4. <span data-ttu-id="db71e-134">Typ op de pagina gebruikers de naam van de gebruiker in het zoekvak.</span><span class="sxs-lookup"><span data-stu-id="db71e-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Toont de pagina gebruikers met het zoekvak om te zoeken naar een specifieke gebruiker.":::

5. <span data-ttu-id="db71e-136">Selecteer de naam van de gebruiker die wordt weer gegeven in de lijst.</span><span class="sxs-lookup"><span data-stu-id="db71e-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Gebruikers pagina weer geven waarin een rij voor de gezochte gebruiker wordt weer gegeven.":::

6. <span data-ttu-id="db71e-138">Zoek de sectie identiteit op de profiel pagina van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="db71e-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="db71e-139">Het veld object-ID wordt hier weer gegeven met de unieke object-ID van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="db71e-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Hiermee wordt de gebruikers profiel pagina met de identiteits sectie en één gemarkeerd veld voor de object-ID weer gegeven.":::

## <a name="next-steps"></a><span data-ttu-id="db71e-141">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="db71e-141">Next steps</span></span>

- [<span data-ttu-id="db71e-142">Uw Tenant-ID programmatisch vinden met Power shell of CLI</span><span class="sxs-lookup"><span data-stu-id="db71e-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="db71e-143">Meer informatie over gebruikers profielen in Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="db71e-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="db71e-144">Ontdek hoe partners klant gegevens kunnen zien of exporteren in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="db71e-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)
