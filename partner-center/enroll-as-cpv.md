---
title: Registreren als Configuratiescherm leverancier
description: Meer informatie over het registreren als een Configuratiescherm Vendor (CPV) in Partner Center zodat u CSP-partnersystemen beter kunt integreren met Partner Center API's.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147136"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="ab298-103">Registreren als een Configuratiescherm leverancier om CSP-partnersystemen te integreren met Partner Center API's</span><span class="sxs-lookup"><span data-stu-id="ab298-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="ab298-104">**Juiste rollen:** globale beheerder</span><span class="sxs-lookup"><span data-stu-id="ab298-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="ab298-105">Een Configuratiescherm Vendor (CPV) is een onafhankelijke softwareleverancier die toepassingen ontwikkelt voor gebruik door Cloud Solution Provider-partners (CSP) zodat ze hun systemen kunnen integreren met Partner Center API's.</span><span class="sxs-lookup"><span data-stu-id="ab298-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="ab298-106">Een Configuratiescherm is geen CSP-partner met directe toegang tot Partner Center dashboard of Partner Center API's.</span><span class="sxs-lookup"><span data-stu-id="ab298-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="ab298-107">Of u nu een huidige Configuratiescherm-leverancier (CPV) of een nieuwe CPV bent die wil samenwerken met Microsoft-partners, Microsoft vereist nu dat u zich registreert bij Partner Center om uw toepassingen te registreren en ondersteuning te Cloud Solution Provider-partners.</span><span class="sxs-lookup"><span data-stu-id="ab298-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="ab298-108">Als u een account wilt maken, kan een CPV-partner een bestaande CSP-partner-tenant of een bestaande CPV-tenant gebruiken of een nieuwe tenant maken als onderdeel van het onboardingproces.</span><span class="sxs-lookup"><span data-stu-id="ab298-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="ab298-109">Als de CPV-partner ervoor kiest om de bestaande CSP-tenant te gebruiken, moet deze afzonderlijke toepassingen voor meerdere tenants maken en deze registreren in Partner Center voor CPV-activiteiten.</span><span class="sxs-lookup"><span data-stu-id="ab298-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="ab298-110">Een toepassing kan niet worden geregistreerd als een CSP- en CPV-toepassing.</span><span class="sxs-lookup"><span data-stu-id="ab298-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="ab298-111">Nadat u zich hebt geregistreerd bij Partner Center en uw toepassingen hebt geregistreerd, hebt u toegang tot de Partner Center API's.</span><span class="sxs-lookup"><span data-stu-id="ab298-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="ab298-112">Neem contact op met Microsoft via Microsoft-ondersteuning aanvraag als u een sandbox-account nodig hebt.</span><span class="sxs-lookup"><span data-stu-id="ab298-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="ab298-113">Als u al een sandbox-account hebt, kunt u dit blijven gebruiken.</span><span class="sxs-lookup"><span data-stu-id="ab298-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="ab298-114">U hebt geen nieuwe sandbox nodig</span><span class="sxs-lookup"><span data-stu-id="ab298-114">You won't need a new sandbox</span></span>

<span data-ttu-id="ab298-115">De [Microsoft Configuratiescherm Vendor-overeenkomst controleren](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="ab298-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="ab298-116">Werken in Partner Center</span><span class="sxs-lookup"><span data-stu-id="ab298-116">Working in Partner Center</span></span>

<span data-ttu-id="ab298-117">Nadat u zich hebt geregistreerd bij Partner Center CPV-ervaring en de CPV-overeenkomst hebt geaccepteerd, kunt u het volgende doen:</span><span class="sxs-lookup"><span data-stu-id="ab298-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="ab298-118">Toepassingen met meerdere tenants beheren (toepassingen toevoegen aan Azure Portal registreren en de registratie van toepassingen in Partner Center).</span><span class="sxs-lookup"><span data-stu-id="ab298-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="ab298-119">CPV's moeten hun toepassingen registreren in Partner Center om te worden geautoriseerd voor Partner Center API's.</span><span class="sxs-lookup"><span data-stu-id="ab298-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="ab298-120">Als u alleen toepassingen Azure Portal toevoegt aan de Partner Center, worden CPV-toepassingen Partner Center geautoriseerd.</span><span class="sxs-lookup"><span data-stu-id="ab298-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="ab298-121">Uw CPV-profiel weergeven en beheren</span><span class="sxs-lookup"><span data-stu-id="ab298-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="ab298-122">Uw gebruikers weergeven en beheren die toegang nodig hebben tot CPV-mogelijkheden.</span><span class="sxs-lookup"><span data-stu-id="ab298-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="ab298-123">Globale beheerder is de enige rol die een CPV kan hebben.</span><span class="sxs-lookup"><span data-stu-id="ab298-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ab298-124">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="ab298-124">Next steps</span></span>

<span data-ttu-id="ab298-125">-[Extra tenants toevoegen aan uw Partner Center account](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="ab298-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>