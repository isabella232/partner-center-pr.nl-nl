---
title: Afdwinging van tegoedlimiet
ms.topic: how-to
ms.date: 05/11/2021
description: Meer informatie over uw tegoedlimiet en hoe deze wordt berekend. Bevat veelgestelde vragen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819379"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="da129-104">Afdwinging van tegoedlimieten (CLE)</span><span class="sxs-lookup"><span data-stu-id="da129-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="da129-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="da129-105">**Appropriate roles**</span></span>

- <span data-ttu-id="da129-106">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="da129-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="da129-107">Uw tegoedlimiet en hoe deze werkt</span><span class="sxs-lookup"><span data-stu-id="da129-107">Your credit limit and how it works</span></span>

<span data-ttu-id="da129-108">Uw tegoedlimiet is het maximumbedrag (in Amerikaanse dollars) dat u als partner kunt besteden aan het kopen van producten of abonnementen in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="da129-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="da129-109">Als u de tegoedlimiet overschrijdt, kunt u geen nieuwe aankopen doen totdat er voldoende betaling is gedaan.</span><span class="sxs-lookup"><span data-stu-id="da129-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="da129-110">Uw bestaande abonnementen blijven ononderbroken.</span><span class="sxs-lookup"><span data-stu-id="da129-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="da129-111">Tegoedlimieten zijn van toepassing op aanbiedingen in Azure-abonnement, Azure-reserveringen, Software, Marketplace, Azure 145 P, Office en Dynamics-producten.</span><span class="sxs-lookup"><span data-stu-id="da129-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="da129-112">Tegoedlimieten zijn niet van toepassing op verlengingen en doorlopend verbruik.</span><span class="sxs-lookup"><span data-stu-id="da129-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="da129-113">We wijzen uw tegoedlimiet toe op tenantniveau tijdens de onboardingperiode.</span><span class="sxs-lookup"><span data-stu-id="da129-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="da129-114">We baseren deze op uw geraamde omzet, aankoopprognoses en betalingsgeschiedenis.</span><span class="sxs-lookup"><span data-stu-id="da129-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="da129-115">Vervolgens gebruiken we de volgende formule om het beschikbare saldo te berekenen:</span><span class="sxs-lookup"><span data-stu-id="da129-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="da129-116">**[Tegoedlimiet – (binnenkomende aankoop + openstaande niet-betaalde facturen + niet-gefactureerde kosten – te veelbetaald)]**</span><span class="sxs-lookup"><span data-stu-id="da129-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="da129-117">Veelgestelde vragen</span><span class="sxs-lookup"><span data-stu-id="da129-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="da129-118">Is mijn tegoedlimiet ingesteld op tenant- of globaal niveau?</span><span class="sxs-lookup"><span data-stu-id="da129-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="da129-119">Het tenantniveau.</span><span class="sxs-lookup"><span data-stu-id="da129-119">The tenant level.</span></span> <span data-ttu-id="da129-120">Stel bijvoorbeeld dat u werkt vanuit de VS, Canada en Japan.</span><span class="sxs-lookup"><span data-stu-id="da129-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="da129-121">Als de Canadees tenant de tegoedlimiet bereikt, ontvangt die tenant een melding wanneer er wordt geprobeerd een aankoop te doen in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="da129-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="da129-122">De andere tenants worden niet beïnvloed.</span><span class="sxs-lookup"><span data-stu-id="da129-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="da129-123">Als ik mijn tegoedlimiet overschrijd, kan ik dan bestaande klanten en abonnementen blijven onderhouden met volledige toegang?</span><span class="sxs-lookup"><span data-stu-id="da129-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="da129-124">Ja.</span><span class="sxs-lookup"><span data-stu-id="da129-124">Yes.</span></span> <span data-ttu-id="da129-125">De bestaande abonnementen van uw klanten worden zonder onderbreking voortgezet.</span><span class="sxs-lookup"><span data-stu-id="da129-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="da129-126">U kunt echter geen nieuwe abonnementen voor uw klanten kopen.</span><span class="sxs-lookup"><span data-stu-id="da129-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="da129-127">Is CLE van toepassing op zowel directe factuurpartners als indirecte providers?</span><span class="sxs-lookup"><span data-stu-id="da129-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="da129-128">Ja, dit geldt voor beide.</span><span class="sxs-lookup"><span data-stu-id="da129-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="da129-129">Wanneer kan ik meer abonnementen kopen nadat ik mijn betaling heb gedaan om mijn account opnieuw in te stellen?</span><span class="sxs-lookup"><span data-stu-id="da129-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="da129-130">U moet de aankoop kunnen hervatten binnen 24 uur na uw betaling, ervan uitgaande dat Microsoft alle vereisten heeft ontvangen om door te gaan met het kredietcontroleproces.</span><span class="sxs-lookup"><span data-stu-id="da129-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="da129-131">Hoe kan ik mijn tegoedlimiet controleren?</span><span class="sxs-lookup"><span data-stu-id="da129-131">How can I check my credit limit?</span></span>

<span data-ttu-id="da129-132">Neem contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) op met om uw tegoedlimiet te bekijken en informatie te krijgen over recente aankopen.</span><span class="sxs-lookup"><span data-stu-id="da129-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="da129-133">Tellen facturen die in strijd zijn met de kredietlimiet mee?</span><span class="sxs-lookup"><span data-stu-id="da129-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="da129-134">Ja.</span><span class="sxs-lookup"><span data-stu-id="da129-134">Yes.</span></span> <span data-ttu-id="da129-135">U kunt echter contact opnemen met Microsoft op om [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) het probleem op te lossen.</span><span class="sxs-lookup"><span data-stu-id="da129-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="da129-136">Hoe snel hoort ik terug als ik schrijf naar ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="da129-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="da129-137">U moet binnen 24 uur een antwoord hebben.</span><span class="sxs-lookup"><span data-stu-id="da129-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="da129-138">Welke criteria gebruikt Microsoft voor het instellen van de tegoedlimiet van een partner?</span><span class="sxs-lookup"><span data-stu-id="da129-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="da129-139">We bepalen uw tegoedlimiet op basis van uw geraamde omzet, aankoopprowess en betalingsgeschiedenis.</span><span class="sxs-lookup"><span data-stu-id="da129-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="da129-140">Wordt de tegoedlimiet momenteel afgedwongen voor de New Commerce Experience?</span><span class="sxs-lookup"><span data-stu-id="da129-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="da129-141">Ja.</span><span class="sxs-lookup"><span data-stu-id="da129-141">Yes.</span></span> <span data-ttu-id="da129-142">Tegoedlimieten zijn van toepassing op alle CSP-programma's en -producten in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="da129-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="da129-143">Wie ontvangt de melding wanneer mijn organisatie de tegoedlimiet nadert?</span><span class="sxs-lookup"><span data-stu-id="da129-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="da129-144">De contactpersoon voor het financiële account van uw organisatie moet de melding ontvangen.</span><span class="sxs-lookup"><span data-stu-id="da129-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="da129-145">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="da129-145">Next steps</span></span>

<span data-ttu-id="da129-146">[Billing basics](./billing-basics.md) (Grondbeginselen van facturering)</span><span class="sxs-lookup"><span data-stu-id="da129-146">[Billing basics](./billing-basics.md)</span></span>
