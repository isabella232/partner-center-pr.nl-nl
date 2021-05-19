---
title: Meervoudige verificatie instellen voor uw gebruikers
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het instellen van uw werknemers met MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5173526d0f65623311d5cd3a1061e8b9e93e9bb9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151624"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="f887d-103">Meervoudige verificatie instellen voor uw gebruikers</span><span class="sxs-lookup"><span data-stu-id="f887d-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="f887d-104">**Juiste rollen:** globale beheerder</span><span class="sxs-lookup"><span data-stu-id="f887d-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="f887d-105">Betere privacybescherming en -beveiliging zijn een van onze belangrijkste prioriteiten.</span><span class="sxs-lookup"><span data-stu-id="f887d-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="f887d-106">We weten dat de beste verdediging preventie is en dat we alleen zo sterk zijn als onze zwakste koppeling.</span><span class="sxs-lookup"><span data-stu-id="f887d-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="f887d-107">Daarom hebben we iedereen in ons ecosysteem nodig om actie te ondernemen en ervoor te zorgen dat de juiste beveiligingsbescherming is gewaarborgd.</span><span class="sxs-lookup"><span data-stu-id="f887d-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="f887d-108">We raden alle partners ten zeerste aan multi-factor authentication (MFA) in te schakelen voor hun gebruikers in hun partner-tenant.</span><span class="sxs-lookup"><span data-stu-id="f887d-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="f887d-109">Meervoudige verificatie toevoegen voor uw gebruikers</span><span class="sxs-lookup"><span data-stu-id="f887d-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="f887d-110">U moet de globale beheerder voor uw bedrijf zijn om deze taak te voltooien.</span><span class="sxs-lookup"><span data-stu-id="f887d-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="f887d-111">Het is het gemakkelijkst om MFA in teschakelen voor uw gebruikers wanneer u ze toevoegt aan uw Azure AD-tenant.</span><span class="sxs-lookup"><span data-stu-id="f887d-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="f887d-112">Meld u aan [Azure Portal](https://portal.azure.com) en ga vervolgens naar **Gebruikersbeheer.**</span><span class="sxs-lookup"><span data-stu-id="f887d-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="f887d-113">Selecteer **Multi-Factor Authentication.**</span><span class="sxs-lookup"><span data-stu-id="f887d-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="f887d-114">Selecteer de gebruiker die u wilt inschakelen en selecteer vervolgens **Inschakelen.**</span><span class="sxs-lookup"><span data-stu-id="f887d-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="f887d-115">Hiermee wordt MFA ingeschakeld voor deze gebruiker.</span><span class="sxs-lookup"><span data-stu-id="f887d-115">This will enable MFA for this user.</span></span> <span data-ttu-id="f887d-116">Ingeschakeld betekent dat de gebruiker wordt gevraagd om de MFA-verificatie in te stellen wanneer deze zich voor de eerste keer aanmelden.</span><span class="sxs-lookup"><span data-stu-id="f887d-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="f887d-117">Daarna wordt ze bij het aanmelden gevraagd om een code op te geven die naar hen wordt verzonden via e-mail of sms-bericht (afhankelijk van de code die ze hebben ingesteld).</span><span class="sxs-lookup"><span data-stu-id="f887d-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Opgeven hoe u dit wilt controleren":::

>[!NOTE]
><span data-ttu-id="f887d-119">U kunt **afdwingen** dat gebruikers MFA gebruiken door dezelfde stappen te volgen als hierboven en Afdwingen **te selecteren.**</span><span class="sxs-lookup"><span data-stu-id="f887d-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="f887d-120">Lees Enable [per-user Azure Multi-Factor Authentication to secure sign-in events (Azure Multi-Factor Authentication per gebruiker](/azure/active-directory/authentication/howto-mfa-userstates)inschakelen om aanmeldingsgebeurtenissen te beveiligen) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f887d-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="f887d-121">Alle gebruikers starten **Uitgeschakeld.**</span><span class="sxs-lookup"><span data-stu-id="f887d-121">All users start out **Disabled**.</span></span> <span data-ttu-id="f887d-122">Wanneer u gebruikers per gebruiker inschrijft Azure Active Directory Multi-Factor Authentication, verandert hun status in **Ingeschakeld.**</span><span class="sxs-lookup"><span data-stu-id="f887d-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="f887d-123">Wanneer ingeschakelde gebruikers zich aanmelden en het registratieproces voltooien, verandert hun status in **Afgedwongen.**</span><span class="sxs-lookup"><span data-stu-id="f887d-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="f887d-124">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="f887d-124">Next steps</span></span>

- [<span data-ttu-id="f887d-125">Rollen en machtigingen toewijzen aan gebruikers</span><span class="sxs-lookup"><span data-stu-id="f887d-125">Assign roles and permissions to users</span></span>](permissions-overview.md)