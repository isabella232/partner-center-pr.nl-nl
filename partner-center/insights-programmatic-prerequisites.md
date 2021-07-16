---
title: Vereisten voor programmatisch toegang tot analysegegevens
description: Vereisten voor programmatisch toegang tot analysegegevens
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376511"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="1c1ad-103">Vereisten voor programmatisch toegang tot analysegegevens</span><span class="sxs-lookup"><span data-stu-id="1c1ad-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="1c1ad-104">**Juiste rollen:** Globale beheerder | MPN-beheerder</span><span class="sxs-lookup"><span data-stu-id="1c1ad-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="1c1ad-105">Voordat u programmatisch toegang kunt krijgen tot analysegegevens van partnerinzichten, moet u voldoen aan de volgende vereisten.</span><span class="sxs-lookup"><span data-stu-id="1c1ad-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="1c1ad-106">MPN-programma-inschrijving</span><span class="sxs-lookup"><span data-stu-id="1c1ad-106">MPN Program enrollment</span></span>

<span data-ttu-id="1c1ad-107">Als u via een programma toegang wilt krijgen tot de analysegegevens van Partner Insights, moet u zijn ingeschreven bij het MPN-programma en een Partner Center hebben.</span><span class="sxs-lookup"><span data-stu-id="1c1ad-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="1c1ad-108">Zie Een [MPN-account maken in Partner Center](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="1c1ad-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="1c1ad-109">Een Azure Active Directory (AAD)-toepassing maken</span><span class="sxs-lookup"><span data-stu-id="1c1ad-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="1c1ad-110">Reguliere gebruikersreferenties kunnen niet worden gebruikt voor programmatische toegang tot Partner Insights Analytics-gegevens.</span><span class="sxs-lookup"><span data-stu-id="1c1ad-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="1c1ad-111">Een Azure Active Directory (AAD)-toepassing moet samen met een geheim (toepassing + gebruikerstoegang) worden gemaakt om toegang te krijgen tot de API's voor programmatische toegang.</span><span class="sxs-lookup"><span data-stu-id="1c1ad-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="1c1ad-112">Zie Quickstart: Een toepassing registreren bij de Microsoft identity platform voor meer informatie over het maken van een [AAD-toepassing en -Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app)   Machtiging is vereist voor toegang tot Microsoft Partner-API.</span><span class="sxs-lookup"><span data-stu-id="1c1ad-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="1c1ad-113">Zie Verificatie voor meer informatie over het toevoegen van [Partner-API - Partner](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="1c1ad-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="1c1ad-114">De rol Executive Report Viewer (ERV) toewijzen aan de gebruiker</span><span class="sxs-lookup"><span data-stu-id="1c1ad-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="1c1ad-115">Als u via een programma toegang wilt krijgen tot analytische gegevens van partnerinzichten, moet u Executive Report Viewer (ERV) hebben.</span><span class="sxs-lookup"><span data-stu-id="1c1ad-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="1c1ad-116">Zie Toegang op basis van rollen - Partner Center Insights voor meer informatie over het toewijzen van een [ERV-rol aan Partner Center](insights-roles.md)</span><span class="sxs-lookup"><span data-stu-id="1c1ad-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="1c1ad-117">Een AAD-token genereren</span><span class="sxs-lookup"><span data-stu-id="1c1ad-117">Generate an AAD token</span></span>

<span data-ttu-id="1c1ad-118">U moet een AAD-token genereren met behulp van de toepassings-id (client-id), het clientgeheim, uw gebruikers-id en het wachtwoord.   [Kijk hier voor](insights-programmatic-first-api-call.md#token-generation) de stappen voor het genereren van een AAD-token.</span><span class="sxs-lookup"><span data-stu-id="1c1ad-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="1c1ad-119">Het token is één uur geldig.</span><span class="sxs-lookup"><span data-stu-id="1c1ad-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1c1ad-120">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="1c1ad-120">Next steps</span></span>
[<span data-ttu-id="1c1ad-121">Programmatisch toegangsparadigma</span><span class="sxs-lookup"><span data-stu-id="1c1ad-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)