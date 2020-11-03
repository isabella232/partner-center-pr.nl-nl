---
title: Azure Cost Management door Cloudyn voor Csp's
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het registreren van de Cloudyn-web-app en het gebruik van een geheime sleutel voor IT in het partner centrum, zodat u de app kunt gebruiken om het Azure-gebruik en de kosten van klanten bij te houden.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527512"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="96b53-103">Het Azure-gebruik en de kosten van klanten bijhouden met de Azure cost management-app voor CSP-partners</span><span class="sxs-lookup"><span data-stu-id="96b53-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="96b53-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="96b53-104">**Applies to**</span></span>

- <span data-ttu-id="96b53-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="96b53-105">Partner Center</span></span>
- <span data-ttu-id="96b53-106">Partners van Cloud Solution Provider-Program ma's</span><span class="sxs-lookup"><span data-stu-id="96b53-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="96b53-107">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="96b53-107">**Appropriate roles**</span></span>

- <span data-ttu-id="96b53-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="96b53-108">Global admin</span></span>
- <span data-ttu-id="96b53-109">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="96b53-109">Admin agent</span></span>

[<span data-ttu-id="96b53-110">Meer informatie over Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="96b53-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="96b53-111">Voordat u begint</span><span class="sxs-lookup"><span data-stu-id="96b53-111">Before you begin</span></span>
<span data-ttu-id="96b53-112">Zorg ervoor dat u voldoet aan de volgende vereisten voordat u Azure Cost Management kunt gebruiken:</span><span class="sxs-lookup"><span data-stu-id="96b53-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="96b53-113">U bent een partner in het Cloud Solution Provider-programma.</span><span class="sxs-lookup"><span data-stu-id="96b53-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="96b53-114">U hebt de mogelijkheid om een partner centrum API-Web-app te maken.</span><span class="sxs-lookup"><span data-stu-id="96b53-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="96b53-115">Overzicht</span><span class="sxs-lookup"><span data-stu-id="96b53-115">Overview</span></span>

<span data-ttu-id="96b53-116">Cloudyn is een web-app waarmee u kunt bijhouden en beheren hoeveel uw klanten Azure gebruiken en wat de kosten voor dat gebruik zijn.</span><span class="sxs-lookup"><span data-stu-id="96b53-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="96b53-117">U gebruikt dit via de partner centrum-API.</span><span class="sxs-lookup"><span data-stu-id="96b53-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="96b53-118">Uw web-app registreren in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="96b53-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="96b53-119">Wanneer u een Azure Active Directory Web-app registreert in het partner centrum, schakelt u de toegang tot de partner centrum-API in.</span><span class="sxs-lookup"><span data-stu-id="96b53-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="96b53-120">Meld u aan bij [het partner centrum](https://partnercenter.microsoft.com/pcv/dashboard/overview) met een [account voor globale beheerders of beheerders agenten](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="96b53-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="96b53-121">Selecteer in het **partner centrum** **account instellingen** &gt; **[app-beheer](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="96b53-121">From the **Partner Center** , select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span></span>
3.  <span data-ttu-id="96b53-122">Klik in de sectie **Web-app** op **nieuwe web-app toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="96b53-122">In the **Web App** section, click **Add new web app** .</span></span>
<br> <span data-ttu-id="96b53-123">**Opmerking** : als u eerder een web-app hebt gemaakt, kunt u stap 3 overs Laan.</span><span class="sxs-lookup"><span data-stu-id="96b53-123">**Note** : If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="96b53-124">Kopieer en sla de **Commerce ID-** GUID en de **App-ID-** GUID voor uw web-app op.</span><span class="sxs-lookup"><span data-stu-id="96b53-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="96b53-125">U hebt beide Id's nodig om de gratis proef versie van 30 dagen van de Azure cost management-app te kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="96b53-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="96b53-126">Een geheime sleutel toevoegen aan uw app</span><span class="sxs-lookup"><span data-stu-id="96b53-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="96b53-127">Selecteer in de vervolg keuzelijst naast de knop **sleutel toevoegen** een duur van 1 of 2 jaar.</span><span class="sxs-lookup"><span data-stu-id="96b53-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="96b53-128">Klik op **sleutel toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="96b53-128">Click **Add key** .</span></span> 
3. <span data-ttu-id="96b53-129">Kopieer de waarde van de geheime sleutel en sla deze op.</span><span class="sxs-lookup"><span data-stu-id="96b53-129">Copy and save the secret key value.</span></span> <span data-ttu-id="96b53-130">Dit hebt u nodig voor de gratis proef versie van 30 dagen.</span><span class="sxs-lookup"><span data-stu-id="96b53-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="96b53-131">De geheime sleutels van de toepassing zijn net als wacht woorden met langere verval datums.</span><span class="sxs-lookup"><span data-stu-id="96b53-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="96b53-132">Sla de sleutel waarde op een veilige locatie op voor toekomstig gebruik.</span><span class="sxs-lookup"><span data-stu-id="96b53-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="96b53-133">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="96b53-133">Next steps</span></span>
<span data-ttu-id="96b53-134">Start een [gratis proef versie van 30 dagen](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="96b53-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="96b53-135">U hebt de volgende gegevens nodig om de proef versie te starten:</span><span class="sxs-lookup"><span data-stu-id="96b53-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="96b53-136">Aanmeldings referenties Partner Center</span><span class="sxs-lookup"><span data-stu-id="96b53-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="96b53-137">Commerce ID-GUID</span><span class="sxs-lookup"><span data-stu-id="96b53-137">Commerce ID GUID</span></span>
- <span data-ttu-id="96b53-138">App-ID-GUID</span><span class="sxs-lookup"><span data-stu-id="96b53-138">App ID GUID</span></span>
- <span data-ttu-id="96b53-139">Waarde van geheime sleutel van toepassing</span><span class="sxs-lookup"><span data-stu-id="96b53-139">Application secret key value</span></span>
