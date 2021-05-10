---
title: Wanbetaling, fraude of misbruik beheren
description: Meer informatie over de verschillende risico's van onlinetransacties en de best practices voor het beheren en beperken van deze risico's in Partner Center.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: c3b7db95bbbd039f8328ddd2785579bb533197cc
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686293"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a><span data-ttu-id="50b02-103">Beheer van niet-betaling, fraude of misbruik in het partnercentrum</span><span class="sxs-lookup"><span data-stu-id="50b02-103">Managing non-payment, fraud, or misuse in Partner Center</span></span>

<span data-ttu-id="50b02-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="50b02-104">**Applies to**</span></span>

- <span data-ttu-id="50b02-105">Partnercentrum voor Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="50b02-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="50b02-106">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="50b02-106">**Appropriate roles**</span></span>

- <span data-ttu-id="50b02-107">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="50b02-107">Global admin</span></span>
- <span data-ttu-id="50b02-108">Beheerder van gebruikersbeheer</span><span class="sxs-lookup"><span data-stu-id="50b02-108">User management admin</span></span>
- <span data-ttu-id="50b02-109">Beheeragent</span><span class="sxs-lookup"><span data-stu-id="50b02-109">Admin agent</span></span>
- <span data-ttu-id="50b02-110">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="50b02-110">Billing admin</span></span>

<span data-ttu-id="50b02-111">U bent financieel verantwoordelijk voor frauduleuze aankopen door uw klanten en/of de niet-betaling van aangeschafte services.</span><span class="sxs-lookup"><span data-stu-id="50b02-111">You are financially responsible for fraudulent purchases by your customers and/or customers' non-payment of purchased services.</span></span> <span data-ttu-id="50b02-112">Daarom raden we u ten zeerste aan om maatregelen voor fraudepreventie *en detectierisicobeperking in te voeren.*</span><span class="sxs-lookup"><span data-stu-id="50b02-112">Therefore, *we strongly recommend that you put in place fraud prevention and detection risk mitigation controls*.</span></span>

<span data-ttu-id="50b02-113">Om frauduleuze activiteiten of misbruik te voorkomen en/of aan te pakken, is het belangrijk om inzicht te krijgen in mogelijke risico's en om beleidsregels en procedures te ontwikkelen die uw blootstelling kunnen verminderen.</span><span class="sxs-lookup"><span data-stu-id="50b02-113">To avoid and/or address fraudulent activity or misuse, it's important to understand potential risks and to develop policies and practices that can reduce your exposure.</span></span>

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a><span data-ttu-id="50b02-114">Afdwinging van beleid voor acceptabel gebruik door Microsoft</span><span class="sxs-lookup"><span data-stu-id="50b02-114">Enforcement of Microsoft Acceptable Use Policy</span></span>

<span data-ttu-id="50b02-115">Als Microsoft partner- of klantactiviteit detecteert die wordt bevestigd of vermoed dat het beleid voor acceptabel gebruik wordt schendt, nemen we afdwingingsstappen.</span><span class="sxs-lookup"><span data-stu-id="50b02-115">If Microsoft detects partner or customer activity that we confirm or suspect violates the Acceptable Use Policy, we will take enforcement steps.</span></span> <span data-ttu-id="50b02-116">De klant kan onmiddellijk worden opgeschort.</span><span class="sxs-lookup"><span data-stu-id="50b02-116">The customer could be immediately suspended.</span></span> <span data-ttu-id="50b02-117">U wordt op de hoogte gesteld van afdwingingsacties of uw aanvragen worden bijgewerkt door Microsoft.</span><span class="sxs-lookup"><span data-stu-id="50b02-117">You'll be notified of enforcement actions or updated on your requests by Microsoft.</span></span>

## <a name="abuse-of-service-risks"></a><span data-ttu-id="50b02-118">Misbruik van servicerisico's</span><span class="sxs-lookup"><span data-stu-id="50b02-118">Abuse of service risks</span></span>

<span data-ttu-id="50b02-119">**Misbruik van servicerisico's** betekent dat klanten die cloudservices gebruiken in strijd zijn met het beleid voor acceptabel gebruik van Microsoft.</span><span class="sxs-lookup"><span data-stu-id="50b02-119">**Abuse of service** risks means customers who use cloud services in violation of Microsoft's Acceptable Use Policy.</span></span>

### <a name="examples-of-abuse-of-service"></a><span data-ttu-id="50b02-120">Voorbeelden van misbruik van service</span><span class="sxs-lookup"><span data-stu-id="50b02-120">Examples of abuse of service</span></span>

<span data-ttu-id="50b02-121">Voorbeelden van deze schendingen van het acceptabele gebruiksbeleid van Microsoft zijn:</span><span class="sxs-lookup"><span data-stu-id="50b02-121">Examples of these violations of Microsoft's acceptable use policy can include:</span></span>

- <span data-ttu-id="50b02-122">Spamming</span><span class="sxs-lookup"><span data-stu-id="50b02-122">Spamming</span></span>
- <span data-ttu-id="50b02-123">Hacking</span><span class="sxs-lookup"><span data-stu-id="50b02-123">Hacking</span></span>
- <span data-ttu-id="50b02-124">DDoS-aanvallen (Distributed Denial of Service)</span><span class="sxs-lookup"><span data-stu-id="50b02-124">Distributed denial-of-service (DDoS) attacks</span></span>
- <span data-ttu-id="50b02-125">Bitcoin-mining</span><span class="sxs-lookup"><span data-stu-id="50b02-125">Bitcoin mining</span></span>
- <span data-ttu-id="50b02-126">Distributie van malware</span><span class="sxs-lookup"><span data-stu-id="50b02-126">Malware distribution</span></span>
- <span data-ttu-id="50b02-127">1000 abonnementen</span><span class="sxs-lookup"><span data-stu-id="50b02-127">Resale of pirated subscriptions</span></span>

## <a name="theft-of-service-risks"></a><span data-ttu-id="50b02-128">Diefstal van servicerisico's</span><span class="sxs-lookup"><span data-stu-id="50b02-128">Theft of service risks</span></span>

<span data-ttu-id="50b02-129">**Diefstal van** servicerisico's betekent dat klanten die niet van plan zijn te betalen voor verbruikte services.</span><span class="sxs-lookup"><span data-stu-id="50b02-129">**Theft of service** risks means customers who have no intention of paying for consumed services.</span></span> <span data-ttu-id="50b02-130">Deze diefstal kan betrekking hebben op het gebruik van gestolen betaalmiddelen, het verstrekken van valse factureringsgegevens en/of het standaardinstellingsaldo.</span><span class="sxs-lookup"><span data-stu-id="50b02-130">This theft may involve using stolen payment instruments, providing false billing information, and/or defaulting on outstanding balances.</span></span>

### <a name="examples-of-service-theft"></a><span data-ttu-id="50b02-131">Voorbeelden van servicediefstal</span><span class="sxs-lookup"><span data-stu-id="50b02-131">Examples of service theft</span></span>

<span data-ttu-id="50b02-132">Voorbeelden van deze online transactierisico's zijn:</span><span class="sxs-lookup"><span data-stu-id="50b02-132">Examples of these online transaction risks can include:</span></span>

- <span data-ttu-id="50b02-133">Transacties die niet persoonlijk plaatsvinden ('creditcard is niet aanwezig' transacties)</span><span class="sxs-lookup"><span data-stu-id="50b02-133">Transactions that don't occur in person ("credit card not present" transactions)</span></span>
- <span data-ttu-id="50b02-134">Onjuiste identiteiten</span><span class="sxs-lookup"><span data-stu-id="50b02-134">Misrepresented identities</span></span>
- <span data-ttu-id="50b02-135">Services die zijn ingericht en gebruikt voordat de eerste betaling wordt ontvangen</span><span class="sxs-lookup"><span data-stu-id="50b02-135">Services provisioned and used before initial payment is received</span></span>
- <span data-ttu-id="50b02-136">Opkomende markten en/of regio's met een hoog risico voor online fraude</span><span class="sxs-lookup"><span data-stu-id="50b02-136">Emerging markets and/or high-risk regions for online fraud</span></span>
- <span data-ttu-id="50b02-137">Het maken en kopen van een account automatiseren door kwaadde actoren</span><span class="sxs-lookup"><span data-stu-id="50b02-137">Automate account creation and purchasing by bad actors</span></span>

## <a name="managing-online-risk"></a><span data-ttu-id="50b02-138">Onlinerisico's beheren</span><span class="sxs-lookup"><span data-stu-id="50b02-138">Managing online risk</span></span>

<span data-ttu-id="50b02-139">U kunt de volgende aanbevelingen gebruiken om beleidsregels en procedures te ontwikkelen om uw blootstelling aan online transactierisico's in de levenscyclus van uw klantrelaties te verminderen.</span><span class="sxs-lookup"><span data-stu-id="50b02-139">You can use the following recommendations to help you develop policies and practices to reduce your exposure to online transaction risks in the lifecycle of your customer relationships.</span></span>

### <a name="onboarding-new-customers"></a><span data-ttu-id="50b02-140">Onboarding van nieuwe klanten</span><span class="sxs-lookup"><span data-stu-id="50b02-140">Onboarding new customers</span></span>

<span data-ttu-id="50b02-141">Suggesties voor het verminderen van onlinerisico's bij het onboarden van nieuwe klanten zijn onder andere:</span><span class="sxs-lookup"><span data-stu-id="50b02-141">Suggestions for reducing online risks when onboarding new customers include:</span></span>

- <span data-ttu-id="50b02-142">Stel waar mogelijk persoonlijke relaties met klanten tot stand (bijvoorbeeld telefonisch contact opnemen met klanten).</span><span class="sxs-lookup"><span data-stu-id="50b02-142">Establish personal relationships with customers when possible (for example, contacting customers by phone).</span></span>
- <span data-ttu-id="50b02-143">Controleer de referenties en achtergrond van klanten met behulp van betere methoden (zoals het gebruik van kredietbureaus of commerciële rapportinstanties).</span><span class="sxs-lookup"><span data-stu-id="50b02-143">Verify customers' credentials and background through better methods (such as using credit bureaus or business commercial report agencies).</span></span>
- <span data-ttu-id="50b02-144">Gebruik meervoudige verificatie (zoals sms-verificatie) tijdens de aanmelding om de blootstelling aan het maken en kopen van een roboticaaccount te minimaliseren.</span><span class="sxs-lookup"><span data-stu-id="50b02-144">Use multi-factor authentication (such as SMS verification) during sign-up to minimize exposure to robotic account creation and purchasing.</span></span>
- <span data-ttu-id="50b02-145">Identiteiten beheren en bijhouden met behulp van services (zoals digitale identiteitsservices).</span><span class="sxs-lookup"><span data-stu-id="50b02-145">Manage and track identities using services (such as digital identity services).</span></span>
- <span data-ttu-id="50b02-146">Evalueer de financiële sterkte van klanten via strenge systemen voor fraudedetectie van creditcards.</span><span class="sxs-lookup"><span data-stu-id="50b02-146">Assess customer financial strength through rigorous credit card fraud detection systems.</span></span>
- <span data-ttu-id="50b02-147">Stel een duidelijk verzamelingsbeleid in.</span><span class="sxs-lookup"><span data-stu-id="50b02-147">Establish a clear collections policy.</span></span> <span data-ttu-id="50b02-148">Details van uw verzamelingsproces en wanneer de toegang tot abonnementen wordt beïnvloed door niet-betaling.</span><span class="sxs-lookup"><span data-stu-id="50b02-148">Detail your collections process and when access to subscriptions will be impacted by non-payment.</span></span> <span data-ttu-id="50b02-149">(U kunt de toegang uitschakelen of de abonnementen van een [klant opzeggen voor](create-a-new-subscription.md#suspend-a-subscription) niet-betaling.)</span><span class="sxs-lookup"><span data-stu-id="50b02-149">(You can disable access or [suspend a customer's subscriptions](create-a-new-subscription.md#suspend-a-subscription) for non-payment.)</span></span>

### <a name="managing-customer-accounts"></a><span data-ttu-id="50b02-150">Klantaccounts beheren</span><span class="sxs-lookup"><span data-stu-id="50b02-150">Managing customer accounts</span></span>

<span data-ttu-id="50b02-151">Suggesties voor het beheren van klantaccounts na aankoop zijn onder andere:</span><span class="sxs-lookup"><span data-stu-id="50b02-151">Suggestions for managing customer accounts post-purchase include:</span></span>

- <span data-ttu-id="50b02-152">Implementeert een proces om snel Microsoft-meldingen te ontvangen, te beoordelen, te reageren en hierop te reageren.</span><span class="sxs-lookup"><span data-stu-id="50b02-152">Implement a process to quickly receive, review, act on, and respond to Microsoft notifications.</span></span>
- <span data-ttu-id="50b02-153">Werk samen met klanten om inzicht te krijgen in de zakelijke behoeften van hun cloudgebruik, terwijl de instellingen de juiste bewakingsdrempels instellen.</span><span class="sxs-lookup"><span data-stu-id="50b02-153">Work with customers to understand their cloud usage business needs while settings appropriate monitoring thresholds.</span></span> <span data-ttu-id="50b02-154">(U kunt bijvoorbeeld een [maandelijks Azure-uitgavenbudget instellen](set-an-azure-spending-budget-for-your-customers.md) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="50b02-154">(For example, you can [set a monthly Azure spending budget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center.</span></span> <span data-ttu-id="50b02-155">Met deze kennis kunt u het gebruik van klanten gedurende de maand bewaken en een melding ontvangen wanneer klanten dicht bij hun budget zijn.)</span><span class="sxs-lookup"><span data-stu-id="50b02-155">This understanding allows you to monitor customer usage during the month and be notified when customers are close to their budget.)</span></span>
- <span data-ttu-id="50b02-156">Controleer [regelmatig de activiteitenlogboeken van](activity-logs.md) klanten om fraude in een vroeg stadium te detecteren.</span><span class="sxs-lookup"><span data-stu-id="50b02-156">Monitor [customer activity logs](activity-logs.md) regularly to help detect fraud early.</span></span>
- <span data-ttu-id="50b02-157">Neem snel actie wanneer er verdachte activiteiten worden gedetecteerd.</span><span class="sxs-lookup"><span data-stu-id="50b02-157">Take quick action when suspicious activities are detected.</span></span>
- <span data-ttu-id="50b02-158">Voorkom dat klanten volledige beheerderstoegang tot abonnementen krijgen zonder eerst risicobeperkende maatregelen te implementeren.</span><span class="sxs-lookup"><span data-stu-id="50b02-158">Avoid giving customers full administrative access to subscriptions without first implementing risk mitigation controls.</span></span>

### <a name="managing-customer-billing"></a><span data-ttu-id="50b02-159">Klantfacturering beheren</span><span class="sxs-lookup"><span data-stu-id="50b02-159">Managing customer billing</span></span>

<span data-ttu-id="50b02-160">Suggesties voor het beheren van klantfacturering na aankoop zijn onder andere:</span><span class="sxs-lookup"><span data-stu-id="50b02-160">Suggestions for managing customer billing post-purchase include:</span></span>

- <span data-ttu-id="50b02-161">Vooruitbetaling aanvragen vóór initiële transacties en facturering.</span><span class="sxs-lookup"><span data-stu-id="50b02-161">Request prepayments prior to initial transactions and billing.</span></span>
- <span data-ttu-id="50b02-162">Accepteer geen betaalmiddelen met een hoog risico (zoals vooraf betaalde kaarten of kaarten met een opgeslagen waarde).</span><span class="sxs-lookup"><span data-stu-id="50b02-162">Don't accept high-risk payment instruments (such as pre-paid cards or stored-value cards).</span></span>
- <span data-ttu-id="50b02-163">Controleer betalingen van klanten en verouderde accounts.</span><span class="sxs-lookup"><span data-stu-id="50b02-163">Monitor customer payments and aging accounts receivables.</span></span> <span data-ttu-id="50b02-164">Gestandaardiseerde dunningsprocessen voor late betalingen of niet-betaling agressief afdwingen.</span><span class="sxs-lookup"><span data-stu-id="50b02-164">Aggressively enforce standardized dunning processes for late payments or non-payment.</span></span>

<span data-ttu-id="50b02-165">Zie de onlinehandleiding voor transactierisicobeheer voor gedetailleerdere strategieën voor het beperken van [onlinerisico's.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span><span class="sxs-lookup"><span data-stu-id="50b02-165">For more detailed strategies for mitigating online risk, see the [Online transaction risk management guide.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span></span>
