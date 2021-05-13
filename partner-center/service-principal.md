---
title: Azure AD-service-principal
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ontdek hoe u een service-principal toevoegt aan uw Azure AD-tenant. Dit betekent dat u een Azure AD-toepassing (service-principal) toevoegt aan Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d12bb66574e6bcee60b2a1df1673dc9171fbee2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854924"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="f709e-104">Een Azure AD-toepassing (service-principal) toevoegen aan Partner Center</span><span class="sxs-lookup"><span data-stu-id="f709e-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="f709e-105">**Juiste rollen:** globale beheerder</span><span class="sxs-lookup"><span data-stu-id="f709e-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="f709e-106">In het commerciële Marketplace-programma in Partner Center kunt u nu een Azure AD-toepassing (service-principal) als gebruiker toevoegen aan uw Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="f709e-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="f709e-107">(U hebt dit eerder kunnen doen in uw Cloud Partner-portal of CPP-account.</span><span class="sxs-lookup"><span data-stu-id="f709e-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="f709e-108">Nu u bent gemigreerd naar Partner Center, is het CPP-account alleen-lezen.)</span><span class="sxs-lookup"><span data-stu-id="f709e-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="f709e-109">Service-principal is synoniem met de Azure AD-toepassing.</span><span class="sxs-lookup"><span data-stu-id="f709e-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="f709e-110">Een Azure AD-toepassing toevoegen (service-principal)</span><span class="sxs-lookup"><span data-stu-id="f709e-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="f709e-111">Selecteer in Partner Center dashboard **Instellingen** en selecteer vervolgens Instellingen voor **ontwikkelaars.**</span><span class="sxs-lookup"><span data-stu-id="f709e-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="f709e-112">Selecteer **Gebruikers** en selecteer vervolgens **Azure AD-toepassingen toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="f709e-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="f709e-113">Selecteer een bestaande Azure AD-toepassing of maak een nieuwe.</span><span class="sxs-lookup"><span data-stu-id="f709e-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="f709e-114">Als u een nieuwe Azure AD-toepassing maakt, moet u de volgende informatie opnemen:</span><span class="sxs-lookup"><span data-stu-id="f709e-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="f709e-115">**Antwoord-URL:** de URL waar gebruikers zich kunnen aanmelden om uw Azure AD-toepassing te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f709e-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="f709e-116">**App-id-URI:** een logische id voor de Azure AD-toepassing die wordt weergegeven wanneer deze een aanvraag voor een een aanmelding naar Azure AD verzendt.</span><span class="sxs-lookup"><span data-stu-id="f709e-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="f709e-117">**Beveiligingsrollen:** de rollen **Manager** (hetzelfde als de rol 'Eigenaar' in CPP) en Ontwikkelaars **(dezelfde** als de rol 'Inzender' in CPP) zijn van toepassing op het commerciële marketplace-programma in Partner Center en ze kunnen worden gekoppeld aan deze Azure AD-toepassing.</span><span class="sxs-lookup"><span data-stu-id="f709e-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="f709e-118">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="f709e-118">Next steps</span></span>

- [<span data-ttu-id="f709e-119">Overzicht van de commerciële marketplace in Partner Center</span><span class="sxs-lookup"><span data-stu-id="f709e-119">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)