---
title: Gebruikers accounts maken en rollen toewijzen
description: Aan elke werk nemer moet een rol worden toegewezen voordat ze toegang krijgen tot het partner centrum. Meer informatie over het maken van gebruikers accounts, het toewijzen van rollen en het instellen van machtigingen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/13/2020
ms.locfileid: "92528664"
---
# <a name="create-user-accounts"></a><span data-ttu-id="13f0f-104">Gebruikers accounts maken</span><span class="sxs-lookup"><span data-stu-id="13f0f-104">Create user accounts</span></span>  

<span data-ttu-id="13f0f-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="13f0f-105">**Appropriate roles**</span></span>

- <span data-ttu-id="13f0f-106">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="13f0f-106">Account admin</span></span>
- <span data-ttu-id="13f0f-107">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="13f0f-107">Global admin</span></span>
- <span data-ttu-id="13f0f-108">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="13f0f-108">User management admin</span></span>

<span data-ttu-id="13f0f-109">Maak gebruikers accounts voor werk nemers die toegang nodig hebben tot het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="13f0f-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="13f0f-110">Deze taken moeten worden uitgevoerd door de beheerder voor gebruikers beheer, de account beheerder of de globale beheerder. De gebruiker die deze taken uitvoert, moet ook worden toegewezen aan de Azure Active Directory (AAD) rollen van gebruikers beheerder of globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="13f0f-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="13f0f-111">Zie [Administrator role permissions](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)(Engelstalig) in azure Active Directory voor meer informatie over Aad-rollen.</span><span class="sxs-lookup"><span data-stu-id="13f0f-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="13f0f-112">Een nieuwe gebruiker toevoegen</span><span class="sxs-lookup"><span data-stu-id="13f0f-112">Add a new user</span></span>

1. <span data-ttu-id="13f0f-113">Selecteer op het pictogram **instellingen** in de rechter bovenhoek van het partner centrum **account instellingen** en selecteer vervolgens **gebruikers beheer** .</span><span class="sxs-lookup"><span data-stu-id="13f0f-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management** .</span></span>

2. <span data-ttu-id="13f0f-114">Selecteer **Gebruiker toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="13f0f-114">Select **Add user** .</span></span>

3. <span data-ttu-id="13f0f-115">Voer de volledige naam en het unieke e-mail adres van de gebruiker in.</span><span class="sxs-lookup"><span data-stu-id="13f0f-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="13f0f-116">Selecteer het type agent en/of het type beheerder dat u wilt toewijzen aan de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="13f0f-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="13f0f-117">Toegang tot partner Center is op rollen gebaseerd, zodat u machtigingen kunt toewijzen om de weer gave van de gebruiker aan te passen, zodat alleen de functies worden weer gegeven die de gebruiker nodig heeft om specifieke taken uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="13f0f-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="13f0f-118">Als gebruikers een roltoewijzing willen, kunnen ze globale beheerders vinden om contact op te nemen door te gaan naar **gebruikers beheer** en filteren op globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="13f0f-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="13f0f-119">Selecteer **Toevoegen** om het gebruikersaccount te maken.</span><span class="sxs-lookup"><span data-stu-id="13f0f-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="13f0f-120">Bevestig de details van de gebruiker op de volgende pagina.</span><span class="sxs-lookup"><span data-stu-id="13f0f-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="13f0f-121">Noteer de aanmeldings gegevens voor de nieuwe gebruiker die op deze pagina worden weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="13f0f-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="13f0f-122">Zorg ervoor dat u deze informatie kopieert en naar de nieuwe gebruiker verzendt, omdat u deze later niet meer kunt openen.</span><span class="sxs-lookup"><span data-stu-id="13f0f-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="13f0f-123">De gebruiker moet zich bij het partner centrum aanmelden met de gebruikers naam en het tijdelijke wacht woord.</span><span class="sxs-lookup"><span data-stu-id="13f0f-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="13f0f-124">Wanneer de gebruiker zich voor de eerste keer aanmeldt bij het partner centrum, wordt u gevraagd om het wacht woord te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="13f0f-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="13f0f-125">Gebruikers rollen toewijzen</span><span class="sxs-lookup"><span data-stu-id="13f0f-125">Assign user roles</span></span>

<span data-ttu-id="13f0f-126">U moet een toegewezen rol hebben om in het partner centrum te kunnen werken.</span><span class="sxs-lookup"><span data-stu-id="13f0f-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="13f0f-127">Rollen omvatten momenteel Azure Active Directory Tenant rollen, functies van Cloud Solution Provider (CSP) en niet-AAD-bedrijfs rollen.</span><span class="sxs-lookup"><span data-stu-id="13f0f-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="13f0f-128">Een individueel bedrijf kan al deze rollen nodig hebben.</span><span class="sxs-lookup"><span data-stu-id="13f0f-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="13f0f-129">Personen moeten worden vermeld in uw Tenant om toegang te krijgen tot het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="13f0f-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="13f0f-130">Roltoewijzingen bieden extra toegang.</span><span class="sxs-lookup"><span data-stu-id="13f0f-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="13f0f-131">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="13f0f-131">Next steps</span></span>

- [<span data-ttu-id="13f0f-132">Gebruikers rollen en-machtigingen toewijzen aan werk nemers die moeten werken in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="13f0f-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
