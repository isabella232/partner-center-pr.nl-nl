---
title: Service-Principal van Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen van een service-principal aan uw Azure AD-Tenant. Dit betekent dat u een Azure AD-toepassing (Service-Principal) toevoegt in het partner centrum.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028465"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="04e88-104">Een Azure AD-toepassing (Service-Principal) toevoegen in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="04e88-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="04e88-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="04e88-105">**Appropriate roles**</span></span>

- <span data-ttu-id="04e88-106">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="04e88-106">Global admin</span></span>

<span data-ttu-id="04e88-107">In het Commercial Marketplace-programma in Partner Center kunt u nu een Azure AD-toepassing (Service-Principal) toevoegen als een gebruiker in uw partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="04e88-107">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="04e88-108">(U kunt dit eerder doen in uw Cloud Partner-portal, of CPP, account.</span><span class="sxs-lookup"><span data-stu-id="04e88-108">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="04e88-109">Nu u hebt gemigreerd naar het partner centrum, is het CPP-account alleen-lezen.)</span><span class="sxs-lookup"><span data-stu-id="04e88-109">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="04e88-110">Service-Principal is synoniem met Azure AD-toepassing.</span><span class="sxs-lookup"><span data-stu-id="04e88-110">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="04e88-111">Een Azure AD-toepassing toevoegen (Service-Principal)</span><span class="sxs-lookup"><span data-stu-id="04e88-111">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="04e88-112">Selecteer in het dash board van de partner centrum **instellingen** en selecteer vervolgens **instellingen voor ontwikkel aars**.</span><span class="sxs-lookup"><span data-stu-id="04e88-112">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="04e88-113">Selecteer **gebruikers** en selecteer vervolgens **Azure AD-toepassingen toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="04e88-113">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="04e88-114">Selecteer een bestaande Azure AD-toepassing of maak een nieuwe.</span><span class="sxs-lookup"><span data-stu-id="04e88-114">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="04e88-115">Als u een nieuwe Azure AD-toepassing maakt, neemt u de volgende informatie op:</span><span class="sxs-lookup"><span data-stu-id="04e88-115">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="04e88-116">**Antwoord-URL**: de URL waar gebruikers zich kunnen aanmelden om uw Azure AD-toepassing te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="04e88-116">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="04e88-117">**App-ID-URI**: een logische id voor de Azure AD-toepassing die wordt gepresenteerd wanneer een eenmalige aanmelding wordt verzonden naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="04e88-117">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="04e88-118">**Beveiligings rollen**: de rollen **beheerder** (dezelfde als de rol owner in cpp) en de **ontwikkelaar** (dezelfde als de rol Inzender in cpp) is van toepassing op het commerciële Marketplace-programma in partner centrum en ze kunnen worden gekoppeld aan deze Azure AD-toepassing.</span><span class="sxs-lookup"><span data-stu-id="04e88-118">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="04e88-119">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="04e88-119">Next steps</span></span>

- [<span data-ttu-id="04e88-120">Overzicht van de commerciële Marketplace in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="04e88-120">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)