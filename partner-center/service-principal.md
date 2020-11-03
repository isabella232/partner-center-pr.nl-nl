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
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2020
ms.locfileid: "92528153"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="d1c2f-104">Een Azure AD-toepassing (Service-Principal) toevoegen in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="d1c2f-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="d1c2f-105">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="d1c2f-105">**Applies to**</span></span>

- <span data-ttu-id="d1c2f-106">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="d1c2f-106">Partner Center</span></span>

<span data-ttu-id="d1c2f-107">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="d1c2f-107">**Appropriate roles**</span></span>

- <span data-ttu-id="d1c2f-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="d1c2f-108">Global admin</span></span>

<span data-ttu-id="d1c2f-109">In het Commercial Marketplace-programma in Partner Center kunt u nu een Azure AD-toepassing (Service-Principal) toevoegen als een gebruiker in uw partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="d1c2f-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="d1c2f-110">(U kunt dit eerder doen in uw Cloud Partner-portal, of CPP, account.</span><span class="sxs-lookup"><span data-stu-id="d1c2f-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="d1c2f-111">Nu u hebt gemigreerd naar het partner centrum, is het CPP-account alleen-lezen.)</span><span class="sxs-lookup"><span data-stu-id="d1c2f-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="d1c2f-112">Service-Principal is synoniem met Azure AD-toepassing.</span><span class="sxs-lookup"><span data-stu-id="d1c2f-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="d1c2f-113">Een Azure AD-toepassing toevoegen (Service-Principal)</span><span class="sxs-lookup"><span data-stu-id="d1c2f-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="d1c2f-114">Selecteer in het dash board van de partner centrum **instellingen** en selecteer vervolgens **instellingen voor ontwikkel aars** .</span><span class="sxs-lookup"><span data-stu-id="d1c2f-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings** .</span></span>

2. <span data-ttu-id="d1c2f-115">Selecteer **gebruikers** en selecteer vervolgens **Azure AD-toepassingen toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="d1c2f-115">Select **Users** and then select **Add Azure AD Applications** .</span></span>

3. <span data-ttu-id="d1c2f-116">Selecteer een bestaande Azure AD-toepassing of maak een nieuwe.</span><span class="sxs-lookup"><span data-stu-id="d1c2f-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="d1c2f-117">Als u een nieuwe Azure AD-toepassing maakt, neemt u de volgende informatie op:</span><span class="sxs-lookup"><span data-stu-id="d1c2f-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="d1c2f-118">**Antwoord-URL** : de URL waar gebruikers zich kunnen aanmelden om uw Azure AD-toepassing te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="d1c2f-118">**Reply URL** : The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="d1c2f-119">**App-ID-URI** : een logische id voor de Azure AD-toepassing die wordt gepresenteerd wanneer een eenmalige aanmelding wordt verzonden naar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d1c2f-119">**App ID URI** : A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="d1c2f-120">**Beveiligings rollen** : de rollen **beheerder** (dezelfde als de rol owner in cpp) en de **ontwikkelaar** (dezelfde als de rol Inzender in cpp) is van toepassing op het commerciële Marketplace-programma in partner centrum en ze kunnen worden gekoppeld aan deze Azure AD-toepassing.</span><span class="sxs-lookup"><span data-stu-id="d1c2f-120">**Security roles** : The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="d1c2f-121">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="d1c2f-121">Next steps</span></span>

- [<span data-ttu-id="d1c2f-122">Overzicht van de commerciële Marketplace in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="d1c2f-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)