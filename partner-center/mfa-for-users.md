---
title: Meervoudige verificatie instellen voor uw gebruikers
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het instellen van uw werk nemers met MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182372"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="0968e-103">Meervoudige verificatie instellen voor uw gebruikers</span><span class="sxs-lookup"><span data-stu-id="0968e-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="0968e-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="0968e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0968e-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="0968e-105">Global admin</span></span>

<span data-ttu-id="0968e-106">Grotere veiligheids maatregelen en beveiliging zijn onder de meest voorkomende prioriteiten.</span><span class="sxs-lookup"><span data-stu-id="0968e-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="0968e-107">We weten dat de beste verdediging voor komen en dat we alleen even sterk zijn als onze zwakste koppeling.</span><span class="sxs-lookup"><span data-stu-id="0968e-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="0968e-108">Daarom hebben we iedereen in ons ecosysteem nodig om te reageren en te zorgen dat de juiste beveiligings beveiligingen aanwezig zijn.</span><span class="sxs-lookup"><span data-stu-id="0968e-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="0968e-109">We raden u ten zeerste aan alle partners multi-factor Authentication (MFA) in te scha kelen voor hun gebruikers in hun partner Tenant.</span><span class="sxs-lookup"><span data-stu-id="0968e-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="0968e-110">Multi-factor Authentication voor uw gebruikers toevoegen</span><span class="sxs-lookup"><span data-stu-id="0968e-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="0968e-111">U moet de globale beheerder zijn voor uw bedrijf om deze taak te volt ooien.</span><span class="sxs-lookup"><span data-stu-id="0968e-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="0968e-112">Het is de eenvoudigste manier om MFA in te scha kelen voor uw gebruikers wanneer u deze toevoegt aan uw Azure AD-Tenant.</span><span class="sxs-lookup"><span data-stu-id="0968e-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="0968e-113">Meld u aan bij de [Azure Portal](https://portal.azure.com) en ga vervolgens naar **gebruikers beheer**.</span><span class="sxs-lookup"><span data-stu-id="0968e-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="0968e-114">Selecteer **multi-factor Authentication**.</span><span class="sxs-lookup"><span data-stu-id="0968e-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="0968e-115">Selecteer de gebruiker die u wilt inschakelen en selecteer **inschakelen**.</span><span class="sxs-lookup"><span data-stu-id="0968e-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="0968e-116">Hiermee wordt MFA ingeschakeld voor deze gebruiker.</span><span class="sxs-lookup"><span data-stu-id="0968e-116">This will enable MFA for this user.</span></span> <span data-ttu-id="0968e-117">Ingeschakeld betekent dat de gebruiker wordt gevraagd om de MFA-verificatie in te stellen wanneer deze zich voor de eerste keer aanmeldt.</span><span class="sxs-lookup"><span data-stu-id="0968e-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="0968e-118">Daarna wordt bij het aanmelden gevraagd om een code op te geven die naar hen wordt verzonden via een e-mail of SMS-bericht (afhankelijk van de instelling).</span><span class="sxs-lookup"><span data-stu-id="0968e-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Opgeven hoe moet worden gecontroleerd":::

>[!NOTE]
><span data-ttu-id="0968e-120">U kunt uw gebruikers **afdwingen** om MFA te gebruiken met behulp van dezelfde stappen als hierboven en vervolgens **afdwingen** te selecteren.</span><span class="sxs-lookup"><span data-stu-id="0968e-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="0968e-121">Voor meer informatie, Lees [toestaan per gebruiker Azure multi-factor Authentication om aanmeldings gebeurtenissen te beveiligen](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="0968e-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="0968e-122">Alle gebruikers worden **uitgeschakeld**.</span><span class="sxs-lookup"><span data-stu-id="0968e-122">All users start out **Disabled**.</span></span> <span data-ttu-id="0968e-123">Wanneer u gebruikers inschrijft in azure Multi-Factor Authentication per gebruiker, verandert de status in **ingeschakeld**.</span><span class="sxs-lookup"><span data-stu-id="0968e-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="0968e-124">Wanneer ingeschakelde gebruikers zich aanmelden en het registratie proces volt ooien, wordt de status ervan gewijzigd in **afgedwongen**.</span><span class="sxs-lookup"><span data-stu-id="0968e-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0968e-125">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="0968e-125">Next steps</span></span>

- [<span data-ttu-id="0968e-126">Rollen en machtigingen toewijzen aan gebruikers</span><span class="sxs-lookup"><span data-stu-id="0968e-126">Assign roles and permissions to users</span></span>](permissions-overview.md)