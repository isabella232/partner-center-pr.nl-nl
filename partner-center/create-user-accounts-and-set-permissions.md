---
title: Gebruikersaccounts maken en rollen toewijzen
description: Aan elke werknemer moet een rol worden toegewezen voordat deze toegang heeft tot Partner Center. Meer informatie over het maken van gebruikersaccounts, het toewijzen van rollen en het instellen van machtigingen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148139"
---
# <a name="create-user-accounts"></a><span data-ttu-id="a0827-104">Gebruikersaccounts maken</span><span class="sxs-lookup"><span data-stu-id="a0827-104">Create user accounts</span></span>  

<span data-ttu-id="a0827-105">**Juiste rollen:** Accountbeheerder | Globale beheerder | Beheerder van gebruikersbeheer</span><span class="sxs-lookup"><span data-stu-id="a0827-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="a0827-106">Maak gebruikersaccounts voor werknemers die toegang tot de Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a0827-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="a0827-107">Deze taken moeten worden uitgevoerd door de beheerder van het gebruikersbeheer, de accountbeheerder of de globale beheerder. Aan de gebruiker die deze taken uitvoert, moeten ook de AAD Azure Active Directory rollen Gebruikersbeheerder of Gebruikersaccount Globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="a0827-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="a0827-108">Zie Machtigingen voor beheerdersrollen in Azure Active Directory voor [meer informatie over AAD-Azure Active Directory.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)</span><span class="sxs-lookup"><span data-stu-id="a0827-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="a0827-109">Een nieuwe gebruiker toevoegen</span><span class="sxs-lookup"><span data-stu-id="a0827-109">Add a new user</span></span>

1. <span data-ttu-id="a0827-110">Selecteer in **het** pictogram Instellingen in de rechterboven Partner Center de optie **Accountinstellingen** en selecteer **vervolgens Gebruikersbeheer.**</span><span class="sxs-lookup"><span data-stu-id="a0827-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="a0827-111">Selecteer **Gebruiker toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="a0827-111">Select **Add user**.</span></span>

3. <span data-ttu-id="a0827-112">Voer de volledige naam en het unieke e-mailadres van de gebruiker in.</span><span class="sxs-lookup"><span data-stu-id="a0827-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="a0827-113">Selecteer het type agent en/of het type beheerder dat u aan de gebruiker wilt toewijzen.</span><span class="sxs-lookup"><span data-stu-id="a0827-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="a0827-114">Partner Center toegang is gebaseerd op rollen, zodat u machtigingen kunt toewijzen om de weergave van de gebruiker aan te passen, zodat alleen de functies worden weergeven die de gebruiker nodig heeft om specifieke taken uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="a0827-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="a0827-115">Als gebruikers een roltoewijzing willen, kunnen ze globale beheerders vinden om contact mee op te nemen door naar **Gebruikersbeheer** te gaan en te filteren op globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="a0827-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="a0827-116">Selecteer **Toevoegen** om het gebruikersaccount te maken.</span><span class="sxs-lookup"><span data-stu-id="a0827-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="a0827-117">Bevestig de details van de gebruiker op de volgende pagina.</span><span class="sxs-lookup"><span data-stu-id="a0827-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="a0827-118">Noteer de aanmeldingsgegevens van de nieuwe gebruiker die op deze pagina worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="a0827-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="a0827-119">Zorg ervoor dat u deze informatie kopieert en naar de nieuwe gebruiker verzendt, aangezien u deze later niet meer kunt openen.</span><span class="sxs-lookup"><span data-stu-id="a0827-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="a0827-120">De gebruiker moet zich aanmelden bij de Partner Center met zijn gebruikersnaam en tijdelijk wachtwoord.</span><span class="sxs-lookup"><span data-stu-id="a0827-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="a0827-121">Wanneer de gebruiker zich voor het eerst Partner Center, wordt de gebruiker gevraagd het wachtwoord te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="a0827-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="a0827-122">Gebruikersrollen toewijzen</span><span class="sxs-lookup"><span data-stu-id="a0827-122">Assign user roles</span></span>

<span data-ttu-id="a0827-123">Als u in de Partner Center, moet u een toegewezen rol hebben.</span><span class="sxs-lookup"><span data-stu-id="a0827-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="a0827-124">Rollen omvatten momenteel Azure Active Directory tenantrollen, Cloud Solution Provider (CSP)-rollen en niet-AAD-bedrijfsrollen.</span><span class="sxs-lookup"><span data-stu-id="a0827-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="a0827-125">Een individueel bedrijf kan al deze rollen nodig hebben.</span><span class="sxs-lookup"><span data-stu-id="a0827-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="a0827-126">Personen moeten worden vermeld in uw tenant om toegang te krijgen tot Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a0827-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="a0827-127">Roltoewijzingen bieden extra toegang.</span><span class="sxs-lookup"><span data-stu-id="a0827-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a0827-128">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="a0827-128">Next steps</span></span>

- [<span data-ttu-id="a0827-129">Gebruikersrollen en -machtigingen toewijzen aan werknemers die in een Partner Center</span><span class="sxs-lookup"><span data-stu-id="a0827-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
